public static int median(Node<Integer> N)
 {
     Node<Integer> n = clone(N);
     int size = n.size();
     for (int i = 0; i < (size / 2); i++)
     {
         removeMax(n);
         removeMin(n);
     }
     return n.getValue();
 }

 public static void removeMax(Node<Integer> n)
 {
     Node<Integer> temp = n;
     int max = temp.getValue();
     temp = temp.getNext();
     Node<Integet> n1 = n;

     while (temp != null)
     {
         if (temp.getValue() > max)
         {
             max = temp.getValue();
         }
         temp = temp.getNext();
     }
     temp = n;
     while (temp != null)
     {
         if (temp.getValue() == max)
         {
             if (temp == n)
             {
                 temp = temp.getNext();
                 n.setNext(null);
                 n = temp;
                 return n;
             }
             else if (temp.getNext() != null)
             {
                 while (n1.getNext() != temp)
                 {
                     n1 = n1.getNext();
                 }
                 n1.setNext(temp.getNext());
                 temp.setNext(null);
                 return n;
             }
             else
             {
                 while (n1.getNext() != temp)
                 {
                     n1 = n1.getNext();
                 }
                 n1.setNext(null);
                 return n;
             }
         }
         temp = temp.getNext();

     }
 }

 public static void removeMin(Node<Integer> n)
 {
     Node<Integer> temp = n;
     int min = temp.getValue();
     temp = temp.getNext();
     Node<Integet> n1 = n;

     while (temp != null)
     {
         if (temp.getValue() < min)
         {
             min = temp.getValue();
         }
         temp = temp.getNext();
     }
     temp = n;
     while (temp != null)
     {
         if (temp.getValue() == min)
         {
             if (temp == n)
             {
                 temp = temp.getNext();
                 n.setNext(null);
                 n = temp;
                 return n;
             }
             else if (temp.getNext() != null)
             {
                 while (n1.getNext() != temp)
                 {
                     n1 = n1.getNext();
                 }
                 n1.setNext(temp.getNext());
                 temp.setNext(null);
                 return n;
             }
             else
             {
                 while (n1.getNext() != temp)
                 {
                     n1 = n1.getNext();
                 }
                 n1.setNext(null);
                 return n;
             }
         }
         temp = temp.getNext();

     }
 }

 public static int size(Node<Integer> n)
 {
     Node<Integer> clone = n;
     int count = 0;
     while (clone != null)
     {
         clone = clone.getNext();
         count++;
     }
     return count;}
public static int median(Queue<Integer> Q)
 {
     Queue<Integer> q = clone(Q);
     int size = q.size();
     for (int i = 0; i < (size / 2); i++)
     {
         removeMax(q);
         removeMin(q);
     }
     return q.remove();
 }

 public static void removeMax(Queue<Integer> q)
 {
     Queue<Integer> temp = new Queue<Integer>();
     int max = q.head();
     temp.insert(q.remove());

     while (!q.isEmpty())
     {
         if (q.head() > max)
         {
             max = q.head();
         }
         temp.insert(q.remove());
     }
     boolean flag = true;

     while (!temp.isEmpty())
     {
         if (temp.head() == max && flag == true)
         {
             flag = false;
             temp.remove();
         }
         else
         {
             q.insert(temp.remove());
         }
     }
 }

 public static void removeMin(Queue<Integer> q)
 {
     Queue<Integer> temp = new Queue<Integer>();
     int min = q.head();
     temp.insert(q.remove());

     while (!q.isEmpty())
     {
         if (q.head() < min)
         {
             min = q.head();
         }
         temp.insert(q.remove());
     }
     boolean flag = true;

     while (!temp.isEmpty())
     {
         if (temp.head() == min && flag == true)
         {
             flag = false;
             temp.remove();
         }
         else
         {
             q.insert(temp.remove());
         }
     }
 }

 public static int size(Queue<Integer> q)
 {
     Queue<Integer> clone = clone(q);
     int count = 0;
     while (!clone.isEmpty())
     {
         clone.remove();
         count++;
     }
     return count;
 }


