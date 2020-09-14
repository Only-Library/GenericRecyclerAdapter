# GenericRecyclerAdapter

The main purpose of this repo to reduce creating **RecyclerAdapter** and **ViewHolder** to display data on view and one listener
```
BaseAdapter<AndroidVersion> adapter = new BaseAdapter<>(R.layout.item_android_version);
        binding.recyclerView.setLayoutManager(new LinearLayoutManager(this));
        binding.recyclerView.addItemDecoration(new DividerItemDecoration(this, DividerItemDecoration.VERTICAL));
        binding.recyclerView.setAdapter(adapter);
        adapter.setList(getList());
        adapter.setActionListener(position ->
                Toast.makeText(this
                        , ((AndroidVersion) adapter.getItemAtPosition(position)).getName()
                        , Toast.LENGTH_SHORT).show());
```

## Reference 
https://proandroiddev.com/using-a-generic-recyclerview-adapter-for-all-the-lists-in-your-android-application-6724501a9d
