# Creating_Portfoil_java
..java
how to use the recycler view in the main activity
RecyclerView menuRv;
    List<MenuItem> menuItems;
    MenuAdapter adapter;
    int selectedMenuPos = 0 ;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        getSupportActionBar().hide();

        // setup side menu
        setupSideMenu();

        // set the default fragment when activity launch
        setHomeFragment();

