# Stack-implimentation


 public class Stack
 {
    public int arr[];
    int top;
    int size;
     Stack()
    {
        this.size=100;
        top=-1;
        
        arr=new int[this.size];
    }
  /*  Stack(int size)
    {
        this.size=size;
        top=-1;
        arr=new int[this.size];
    }*/
    public void push(int v)
    {
        arr[++top]=v;
    }
    public int pop()
    {
        return arr[top--];
    }
    public boolean isempty()
    {
        return top==-1;
    }
    public int peek()
    {
        return arr[top];
    }



    public static void main(String[] args)
    {
        Stack ob=new Stack();
        int v=1;
       
     ob.push(v);
      
      
 System.out.println(ob.peek());
    }
    
}   

