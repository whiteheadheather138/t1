代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://fz.zhonguo5118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://qp.zhonguo2118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://da.zhonguo1118.cn

Ruby: s.bytesize;  s.length
来源：https://uw.zhonguo5118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://rf.zhonguo6118.cn

================================================================================
来源：https://rk.zhonguo4118.cn

F. 文件与目录
来源：https://nt.zhonguo6118.cn

================================================================================
来源：https://ul.zhonguo8118.cn

[F01] 读取整个文件
来源：https://xv.zhonguo6118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://rc.zhonguo5118.cn

PHP:  file_get_contents("a.txt");
来源：https://ic.zhonguo3118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://pp.zhonguo4118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://jg.zhonguo6118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ai.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://hb.zhonguo6118.cn

Ruby: File.read("a.txt")
来源：https://qs.zhonguo4118.cn

C#:   File.ReadAllText("a.txt");
来源：https://rc.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://xs.zhonguo3118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://yj.zhonguo7118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://sr.zhonguo7118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://jv.zhonguo4118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://km.zhonguo1118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://aa.zhonguo7118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://jb.zhonguo5118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://fm.zhonguo3118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://nc.zhonguo8118.cn

[F03] 写入文件（覆盖）
来源：https://tq.zhonguo3118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://uu.zhonguo5118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://nz.zhonguo1118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://xo.zhonguo4118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://jw.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://mj.zhonguo1118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ib.zhonguo4118.cn

Ruby: File.write("a.txt", "hi")
来源：https://nx.zhonguo6118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://qk.zhonguo5118.cn

[F04] 追加写入文件
来源：https://pm.zhonguo5118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://fm.zhonguo2118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://dz.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://pa.zhonguo1118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://cq.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://sr.zhonguo1118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://ve.zhonguo2118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ot.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://tz.zhonguo5118.cn

[F05] 判断文件或目录是否存在
来源：https://qh.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://gx.zhonguo7118.cn

PHP:  file_exists("a.txt");
来源：https://lg.zhonguo2118.cn

JS:   fs.existsSync("a.txt")
来源：https://oh.zhonguo8118.cn

TS:   fs.existsSync("a.txt")
来源：https://dv.zhonguo1118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ct.zhonguo8118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ab.zhonguo5118.cn

Ruby: File.exist?("a.txt")
来源：https://ug.zhonguo5118.cn

C#:   File.Exists("a.txt")
来源：https://ll.zhonguo4118.cn

[F06] 删除文件
来源：https://wt.zhonguo8118.cn

Py:   os.remove("a.txt")
来源：https://ns.zhonguo1118.cn

PHP:  unlink("a.txt");
来源：https://kw.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://fs.zhonguo3118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://vf.zhonguo7118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://kv.zhonguo3118.cn

Go:   os.Remove("a.txt")
来源：https://sz.zhonguo1118.cn

Ruby: File.delete("a.txt")
来源：https://ti.zhonguo8118.cn

C#:   File.Delete("a.txt");
来源：https://yv.zhonguo7118.cn

[F07] 创建目录（含多级）
来源：https://tu.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://nf.zhonguo6118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://kn.zhonguo4118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ns.zhonguo4118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://sp.zhonguo4118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://xr.zhonguo7118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://cy.zhonguo5118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ax.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://ke.zhonguo6118.cn

[F08] 遍历目录
来源：https://gp.zhonguo6118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://fx.zhonguo2118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://aq.zhonguo5118.cn

JS:   fs.readdirSync("dir")
来源：https://br.zhonguo7118.cn

TS:   fs.readdirSync("dir")
来源：https://ju.zhonguo5118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://ly.zhonguo4118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://te.zhonguo3118.cn

Ruby: Dir.children("dir")
来源：https://bt.zhonguo1118.cn

C#:   Directory.GetFiles("dir")
来源：https://ox.zhonguo3118.cn

[F09] 获取文件大小
来源：https://xi.zhonguo7118.cn

Py:   os.path.getsize("a.txt")
来源：https://gm.zhonguo4118.cn

PHP:  filesize("a.txt");
来源：https://xc.zhonguo2118.cn

JS:   fs.statSync("a.txt").size
来源：https://jn.zhonguo5118.cn

TS:   fs.statSync("a.txt").size
来源：https://cm.zhonguo1118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://fa.zhonguo1118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://oj.zhonguo8118.cn

Ruby: File.size("a.txt")
来源：https://nx.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://xd.zhonguo6118.cn

[F10] 取文件扩展名 / 文件名
来源：https://ym.zhonguo3118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://hs.zhonguo1118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://aw.zhonguo1118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://vl.zhonguo6118.cn

TS:   path.extname("a.txt")
来源：https://kv.zhonguo4118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://nl.zhonguo4118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://gd.zhonguo6118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://af.zhonguo6118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://ah.zhonguo5118.cn

[F11] 复制与移动文件
来源：https://uz.zhonguo7118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://yt.zhonguo7118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://wb.zhonguo1118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://zi.zhonguo2118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ug.zhonguo8118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://fv.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://jz.zhonguo2118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://sp.zhonguo6118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ut.zhonguo1118.cn

[F12] CSV 读写
来源：https://fg.zhonguo6118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://qv.zhonguo2118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://iq.zhonguo6118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://kn.zhonguo2118.cn

TS:   // 同上
来源：https://ro.zhonguo2118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://fg.zhonguo3118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://pq.zhonguo3118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://co.zhonguo8118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://jk.zhonguo3118.cn

================================================================================
来源：https://im.zhonguo4118.cn

G. 面向对象
来源：https://wy.zhonguo2118.cn

================================================================================
来源：https://aa.zhonguo2118.cn

[G01] 定义类
来源：https://be.zhonguo2118.cn

Py:   class User: pass
来源：https://ml.zhonguo4118.cn

PHP:  class User {}
来源：https://ir.zhonguo2118.cn

JS:   class User {}
来源：https://wo.zhonguo7118.cn

TS:   class User { name: string = ""; }
来源：https://mg.zhonguo3118.cn

Java: class User {}
来源：https://uz.zhonguo7118.cn

Go:   type User struct { Name string }
来源：https://gx.zhonguo4118.cn

Ruby: class User; end
来源：https://uz.zhonguo8118.cn

C#:   class User {}
来源：https://du.zhonguo2118.cn

[G02] 构造函数
来源：https://dv.zhonguo6118.cn

Py:   def __init__(self, name): self.name = name
来源：https://si.zhonguo4118.cn

PHP:  public function __construct(public string $name) {}
来源：https://sn.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://gh.zhonguo4118.cn

TS:   constructor(public name: string) {}
来源：https://ku.zhonguo7118.cn

Java: User(String name) { this.name = name; }
来源：https://cj.zhonguo8118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://ph.zhonguo1118.cn

Ruby: def initialize(name); @name = name; end
来源：https://rs.zhonguo7118.cn

C#:   public User(string name) { Name = name; }
来源：https://ko.zhonguo6118.cn

[G03] 实例属性
来源：https://pw.zhonguo4118.cn

Py:   self.name = "x"
来源：https://lh.zhonguo3118.cn

PHP:  public string $name = "x";
来源：https://iw.zhonguo5118.cn

JS:   this.name = "x";
来源：https://pt.zhonguo2118.cn

TS:   name: string = "x";
来源：https://fs.zhonguo6118.cn

Java: private String name;
来源：https://bf.zhonguo3118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://cs.zhonguo4118.cn

Ruby: @name = "x"
来源：https://pk.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://bu.zhonguo3118.cn

[G04] 定义方法
来源：https://do.zhonguo8118.cn

Py:   def greet(self): return self.name
来源：https://sx.zhonguo5118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ks.zhonguo2118.cn

JS:   greet() { return this.name; }
来源：https://rk.zhonguo1118.cn

TS:   greet(): string { return this.name; }
来源：https://ej.zhonguo7118.cn

Java: String greet() { return name; }
来源：https://si.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://tu.zhonguo4118.cn

Ruby: def greet; @name; end
来源：https://ub.zhonguo6118.cn

C#:   public string Greet() => Name;
来源：https://fb.zhonguo8118.cn

[G05] 继承
来源：https://eq.zhonguo7118.cn

Py:   class Admin(User): pass
来源：https://jx.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://uk.zhonguo3118.cn

JS:   class Admin extends User {}
来源：https://ot.zhonguo5118.cn

TS:   class Admin extends User {}
来源：https://eg.zhonguo6118.cn

Java: class Admin extends User {}
来源：https://hr.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://ap.zhonguo4118.cn

Ruby: class Admin < User; end
来源：https://ls.zhonguo2118.cn

C#:   class Admin : User {}
来源：https://zs.zhonguo1118.cn

[G06] 重写方法
来源：https://tu.zhonguo7118.cn

Py:   def greet(self): return "admin"
来源：https://kf.zhonguo2118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://al.zhonguo1118.cn

JS:   greet() { return "admin"; }
来源：https://vk.zhonguo8118.cn

TS:   greet(): string { return "admin"; }
来源：https://hi.zhonguo2118.cn

Java: @Override String greet() { return "admin"; }
来源：https://xw.zhonguo6118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://jl.zhonguo4118.cn

Ruby: def greet; "admin"; end
来源：https://nt.zhonguo6118.cn

C#:   public override string Greet() => "admin";
来源：https://xs.zhonguo7118.cn

[G07] 调用父类方法
来源：https://ug.zhonguo2118.cn

Py:   super().greet()
来源：https://uv.zhonguo3118.cn

PHP:  parent::greet();
来源：https://ms.zhonguo8118.cn

JS:   super.greet();
来源：https://ua.zhonguo2118.cn

TS:   super.greet();
来源：https://em.zhonguo8118.cn

Java: super.greet();
来源：https://jr.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://fg.zhonguo7118.cn

Ruby: super
来源：https://ei.zhonguo4118.cn

C#:   base.Greet();
来源：https://zx.zhonguo7118.cn

[G08] 静态方法与属性
来源：https://ew.zhonguo3118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://wx.zhonguo7118.cn

PHP:  public static function f() {}
来源：https://mn.zhonguo1118.cn

JS:   static f() {}
来源：https://yc.zhonguo4118.cn

TS:   static f(): void {}
来源：https://ez.zhonguo4118.cn

Java: static void f() {}
来源：https://wb.zhonguo3118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://gp.zhonguo3118.cn

Ruby: def self.f; end
来源：https://uo.zhonguo2118.cn

C#:   public static void F() {}
来源：https://ck.zhonguo2118.cn

[G09] 接口 / 抽象类
来源：https://vx.zhonguo1118.cn

Py:   from abc import ABC, abstractmethod
来源：https://kn.zhonguo4118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://ad.zhonguo3118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://tv.zhonguo4118.cn

TS:   interface Shape { area(): number; }
来源：https://qi.zhonguo2118.cn

Java: interface Shape { double area(); }
来源：https://rm.zhonguo3118.cn

Go:   type Shape interface { Area() float64 }
来源：https://tq.zhonguo5118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://st.zhonguo7118.cn

C#:   interface IShape { double Area(); }
来源：https://hq.zhonguo6118.cn

[G10] 访问控制
来源：https://nu.zhonguo4118.cn

Py:   约定 _protected / __private（不强制）
来源：https://ux.zhonguo3118.cn

PHP:  public / protected / private
来源：https://uk.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://hk.zhonguo6118.cn

TS:   public / protected / private
来源：https://lc.zhonguo4118.cn

Java: public / protected / private / 默认包级
来源：https://el.zhonguo3118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://eo.zhonguo8118.cn

Ruby: public / protected / private
来源：https://pg.zhonguo6118.cn

C#:   public / protected / private / internal
来源：https://ma.zhonguo1118.cn

[G11] getter / setter
来源：https://iq.zhonguo7118.cn

Py:   @property 与 @x.setter
来源：https://ch.zhonguo1118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://mv.zhonguo1118.cn

JS:   get name() { return this._name; }
来源：https://ih.zhonguo4118.cn

TS:   get name(): string { return this._name; }
来源：https://uq.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://ul.zhonguo6118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://pg.zhonguo5118.cn

Ruby: attr_accessor :name
来源：https://ul.zhonguo4118.cn

C#:   public string Name { get; set; }
来源：https://sf.zhonguo7118.cn

[G12] 对象转字符串
来源：https://hm.zhonguo4118.cn

Py:   def __str__(self): return self.name
来源：https://pn.zhonguo4118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://om.zhonguo3118.cn

JS:   toString() { return this.name; }
来源：https://vj.zhonguo8118.cn

TS:   toString(): string { return this.name; }
来源：https://ue.zhonguo2118.cn

Java: @Override public String toString() { return name; }
来源：https://qo.zhonguo6118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://dq.zhonguo5118.cn

Ruby: def to_s; @name; end
来源：https://bd.zhonguo5118.cn

C#:   public override string ToString() => Name;
来源：https://cz.zhonguo1118.cn

[G13] 判断对象类型
来源：https://yu.zhonguo5118.cn

Py:   isinstance(u, User)
来源：https://hh.zhonguo4118.cn

PHP:  $u instanceof User
来源：https://ce.zhonguo4118.cn

JS:   u instanceof User
来源：https://ss.zhonguo8118.cn

TS:   u instanceof User
来源：https://ul.zhonguo4118.cn

Java: u instanceof User
来源：https://ss.zhonguo7118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://qr.zhonguo6118.cn

Ruby: u.is_a?(User)
来源：https://cs.zhonguo8118.cn

C#:   u is User
来源：https://mp.zhonguo4118.cn

[G14] 数据类 / record
来源：https://lw.zhonguo5118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://pf.zhonguo7118.cn

PHP:  // 用 readonly 属性模拟
来源：https://jd.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://hg.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://jt.zhonguo3118.cn

Java: record User(String name, int age) {}
来源：https://lx.zhonguo2118.cn

Go:   type User struct { Name string; Age int }
来源：https://mp.zhonguo7118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://ce.zhonguo3118.cn

C#:   record User(string Name, int Age);
来源：https://ni.zhonguo8118.cn

[G15] 枚举
来源：https://et.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ts.zhonguo3118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://rk.zhonguo1118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://tq.zhonguo1118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://pe.zhonguo1118.cn

Java: enum Color { RED, GREEN }
来源：https://pe.zhonguo2118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://cb.zhonguo3118.cn

Ruby: Color = %i[red green].freeze
来源：https://tb.zhonguo6118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://fh.zhonguo5118.cn

[G16] 对象转数组 / 字典
来源：https://zk.zhonguo5118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://hd.zhonguo2118.cn

PHP:  get_object_vars($obj);
来源：https://qm.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://os.zhonguo6118.cn

TS:   Object.entries(obj)
来源：https://kd.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://sd.zhonguo5118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://lq.zhonguo6118.cn

Ruby: obj.instance_variables
来源：https://bh.zhonguo1118.cn

C#:   // 用反射或 System.Text.Json
来源：https://sj.zhonguo7118.cn

================================================================================
来源：https://et.zhonguo4118.cn

H. 异常与错误处理
来源：https://iq.zhonguo2118.cn

================================================================================
来源：https://pk.zhonguo3118.cn

[H01] try / catch 基础
来源：https://vl.zhonguo4118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://yq.zhonguo7118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://hv.zhonguo4118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://um.zhonguo7118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://sm.zhonguo7118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://zj.zhonguo7118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://as.zhonguo7118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://rh.zhonguo7118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://im.zhonguo6118.cn

[H02] finally / ensure 收尾
来源：https://us.zhonguo5118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://yv.zhonguo5118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://sw.zhonguo2118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://lo.zhonguo1118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://vx.zhonguo6118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ev.zhonguo3118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://gb.zhonguo7118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://cs.zhonguo6118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://yj.zhonguo2118.cn

[H03] 主动抛出异常
来源：https://hz.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://wq.zhonguo7118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://sk.zhonguo5118.cn

JS:   throw new Error("错误信息");
来源：https://hv.zhonguo6118.cn

TS:   throw new Error("错误信息");
来源：https://zd.zhonguo6118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://rb.zhonguo5118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://xc.zhonguo5118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://yh.zhonguo2118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://zx.zhonguo7118.cn

[H04] 自定义异常类型
来源：https://rp.zhonguo2118.cn

Py:   class MyError(Exception): pass
来源：https://ih.zhonguo7118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://qq.zhonguo5118.cn

JS:   class MyError extends Error {}
来源：https://yj.zhonguo7118.cn

TS:   class MyError extends Error {}
来源：https://wi.zhonguo7118.cn

Java: class MyException extends RuntimeException {}
来源：https://sg.zhonguo8118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://py.zhonguo4118.cn


<!-- 参考信息 -->