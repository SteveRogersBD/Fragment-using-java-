<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fragment Transaction</title>
</head>
<body>
  <p>Create fragments</p>
  <p>Keep an empty ViewGroup inside the layout where I want the fragment to be shown</p>
  <p>Give it an ID</p>
  <p>Use transaction to add, remove, substitute a fragment</p>
  <p>Use the following code:</p>
  <pre><code>FirstFragment firstFragment = new FirstFragment();
FragmentTransaction transaction = getSupportFragmentManager().beginTransaction();
transaction.replace(R.id.linear,firstFragment); // destination, target fragment
transaction.commit();</code></pre>
</body>
