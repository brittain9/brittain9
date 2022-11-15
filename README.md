### Hi there 👋 I'm Alex!

---

    namespace Welcome
    {
        public class Person
        {
            public string m_UserName;
            public string m_Name;
            public int m_Age;
            public string m_School;
            public string m_Major;
            public string[]? m_Interests;

            public Person(string userName, string name, int age, string school, string major, string[]? interests)
            {
                m_UserName = userName;
                m_Name = name;
                m_Age = age;
                m_School = school;
                m_Major = major;
                m_Interests ??= interests;
            }

            public override string ToString()
            {
                string ret = $"Hello! My name is {m_Name}. I am a {m_Age} year old {m_Major} major at {m_School}.\n";
                if (m_Interests != null)
                {
                    ret += "\nMy interests include:\n";
                    foreach (var interest in m_Interests)
                    {
                        ret += $" - {interest}\n";
                    }
                }
                ret += "\nCheck out my website and feel free to contact me by email or Twitter.";
                return ret;
            }
        }

        public class Program
        {
            public static void Main()
            {
                Person A = new Person(
                    "brittain9", "Alexander Brittain", 21,
                    "University of Texas at Austin", "Management Information Systems",
                    (new string[]{"CSharp", ".NET", "Computer Science","Foodie"})
                );

                Console.WriteLine(A);
            }
        }
    }
