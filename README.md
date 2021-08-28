# datastructure
SinglylinkedList insertion
package com.arun;

public class SinglylinkedList {
	 
	Node head;
	static class Node {
		int data;
		Node next=null;
		
	

	 Node(int data) {
		 
		 this.data=data;
		
		
	}
	}
	 void display()
	 {
		 Node current=head;
		 while(current!=null)
		 {
			 System.out.print(current.data+" ");
			 current=current.next;
			 
		 }
		 System.out.print("null");
	 }	 
	 

	public static void main(String[] args) {

SinglylinkedList sll=new SinglylinkedList();

sll.head=new Node(10);
Node first=new Node(9);

Node second=new Node(8);
Node third=new Node(7);
sll.head.next=first;
first.next=second;
second.next=third;
sll.display();

	}

}
