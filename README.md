class Node{
  int data;
  Node next;

  Node(int data){
  this.data=data;
  this.next=null;
  }
}

class LinkedList{
  Node head;
  public void insert(int data){
    Node newNode = new Node(data);
    if(head == null){
       head = newNode;
       return;
       }
       Node last = head;
       while(last.next != null){
          last = last.next;
        }
        last.next = newNode;
    }

    public void display(){
      Node current = head;
      while(current != null){
      
