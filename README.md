# lengthoflinkedlist
package LinkedList;

public class lenghoflinkedlist  {
    public static int length(Node head){
        int count=0;
        while(head!=null){
            count++;
            head=head.next;
        }
        return count;
    }

    public static class Node{
        int data; //value
        Node next; // address of next node
        Node(int data){
            this.data=data;
        }
    }
    public static void main(String[] args) {
        Node a =new Node(5);
        //System.out.println(a.next);//null
        Node b =new Node(3);
        Node c =new Node(9);
        Node d =new Node(8);
        Node e =new Node(4);
        /* 5-3-9-8-4 */
        a.next=b;// 5 is connected with 3
        b.next=c;
        c.next=d;
        d.next=e;
        System.out.println(length(a));




    }
}
