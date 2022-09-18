- 👋 Hi, I’m @harshit00001
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
harshit00001/harshit00001 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->



		System.out.println("Enter 5 Student Marks: ");
		Scanner in =new Scanner(System.in);
		Student stud1=new Student("Harsh",1,22,in.nextInt());
		Student stud2=new Student("Aaddya",2,22,in.nextInt());
		Student stud3=new Student("Abhay",3,21,in.nextInt());
		Student stud4=new Student("Chetan",4,22,in.nextInt());
		Student stud5=new Student("Debayan",5,22,in.nextInt());
    
    private String Name;
		private int Roll_no;
		private int Age;
		private int Marks;
		public Student(String Name,int Roll_no,int Age,int Marks) 
		{
			this.Name=Name;
			this.Roll_no=Roll_no;
			this.Age=Age;
			this.Marks=Marks;
			if (Marks<30)
			{
				System.out.println("Name: " + Name + "\nRollNo: " + Roll_no + "\nage: " + Age+ "\nMarks: " + Marks + " ,Marks Less than 30 Cannot be accepted");
			}
			else
			{
				System.out.println("Name: " + Name + "\nRollNo: " + Roll_no + "\nage: " + Age+ "\nMarks: " + Marks +" ,Marks Acceptable ");
			}
		}
		
		public String getName() {
			return Name;
		}

		public void setName(String name) {
			Name = name;
		}

		public int getRoll_no() {
			return Roll_no;
		}

		public void setRoll_no(int roll_no) {
			Roll_no = roll_no;
		}

		public int getAge() {
			return Age;
		}

		public void setAge(int age) {
			Age = age;
		}

		public int getMarks() {
			return Marks;
		}

		public void setMarks(int marks) {
			Marks = marks;
		}
