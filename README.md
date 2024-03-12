
  <H1>Fragment Transaction</H1>

  <p>Create fragments</p>
  <p>Keep an empty ViewGroup inside the layout where I want the fragment to be shown</p>
  <p>Give it an ID</p>
  <p>Use transaction to add, remove, substitute a fragment</p>
  <p>Use the following code:</p>
  <pre><code>FirstFragment firstFragment = new FirstFragment();
FragmentTransaction transaction = getSupportFragmentManager().beginTransaction();
transaction.replace(R.id.linear,firstFragment); // destination, target fragment
transaction.commit();</code></pre>
<h2>If you want to move from one fragment to a different activity in that case you have to use intent. </h2>
<br>Use the following code. <br>
Intent intent = new Intent(getContext(), MainActivity2.class);<br>
startActivity(intent);<br>
//Since we don't know in which activity this fragment can be therefore, instead of <br>
//using MainActivity.this we use getContext(); <br>


