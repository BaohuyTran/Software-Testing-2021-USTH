# Excercise 7.2.2.8
---

```java
import java.util.Collections;
import java.util.Comparator;
import java.util.List;
import java.util.LinkedList;
import java.util.Iterator;


public class PathList {
	protected List<Path> pr;

	public PathList() {
		pr = new LinkedList<Path>();
	}

	public PathList(List<Node> _nodes) {
		pr = new LinkedList<Path>();
		initNodes(_nodes);
	}

	public void initNodes(List<Node> _nodeList) {
		Path p;
		for(int i = 0; i < _nodeList.size(); i++) {
			Node node = _nodeList.get(i);
			p = new Path(node);
			pr.add(p);
		}
	}

	public Iterator<Path> iterator() {
		return pr.iterator();
	}

	public void add(Path _p) {
		pr.add(_p);
	}

	public int size() {
		return pr.size();
	}

	public String toString() {
		Collections.sort(pr, new Comparator<Path>() {
			public int compare(Path _s1, Path _s2) {
				if(_s1.len() == _s2.len()) {
					int len = _s1.len();
					for(int i = 0; i < len; i++) {
						if(_s1.GetNode(i).GetNodeNumber() != _s2.GetNode(i).GetNodeNumber()) {
							return(_s1.GetNode(i).GetNodeNumber() - _s2.GetNode(i).GetNodeNumber());
						}
					}
					return 0;
				}
				else	
					return _s1.len() - _s2.len();
			}
		});

		Path p;
		String res = "";
		for(int i = 0; i < pr.size(); i++) {
			p = pr.get(i);
			res += p + " ";
		}
		return res;
	}
} 
```