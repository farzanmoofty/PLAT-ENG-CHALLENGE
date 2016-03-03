# PLAT-ENG-CHALLENGE
1. Coding task: Need to finish this coding task in 2 hours.

please implement an immutable queue with the following api:
	Scala Version:
	trait Queue[T] {
	  def isEmpty: Boolean
	  def enQueue(t: T): Queue[T]
	  def deQueue(t: T): Queue[T]
	  def head: Option[T]
	}
	object Queue {
	  def empty[T]: Queue[T] = ???
	}

	Java Version:
	public interface Queue[T] {
	    public Queue<T> enQueue(T t);
	    public Queue<T> deQueue(T t);
	    public T head();
	    public boolean isEmpty();
	}

2. Design Question: Design A Google Analytic like Backend System.
We need to provide Google Analytic like services to our customers. Pls provide a high level solution design for the backend system. Feel free to choose any open source tools as you want.

The system needs to:
1) handle large write volume: Billions write events per day.
2) handle large read/query volume: Millions merchants want to get insight about their business. Read/Query patterns are time-series related metrics. 
3) metrics need to be available to customers with at most one hour delay.
4) run with minimum downtime.
5) have the ability to reprocess historical data in case of bugs in the processing logic.
