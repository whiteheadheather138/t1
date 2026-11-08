代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://xi.zhonguo2118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://ok.zhonguo8118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://bh.zhonguo1118.cn

Ruby: s.bytesize;  s.length
来源：https://ox.zhonguo2118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://mt.zhonguo6118.cn

================================================================================
来源：https://eg.zhonguo8118.cn

F. 文件与目录
来源：https://qz.zhonguo3118.cn

================================================================================
来源：https://os.zhonguo8118.cn

[F01] 读取整个文件
来源：https://so.zhonguo1118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://xe.zhonguo1118.cn

PHP:  file_get_contents("a.txt");
来源：https://oi.zhonguo7118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://aw.zhonguo5118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://ly.zhonguo2118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://tz.zhonguo4118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://mi.zhonguo6118.cn

Ruby: File.read("a.txt")
来源：https://mo.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://ag.zhonguo2118.cn

[F02] 逐行读取文件
来源：https://pv.zhonguo7118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ab.zhonguo5118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://oj.zhonguo1118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://eu.zhonguo1118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://rs.zhonguo7118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://jm.zhonguo4118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://ci.zhonguo4118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://tk.zhonguo8118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ms.zhonguo3118.cn

[F03] 写入文件（覆盖）
来源：https://tn.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://ao.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://zb.zhonguo4118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://rw.zhonguo1118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://pz.zhonguo8118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://vm.zhonguo2118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://cs.zhonguo8118.cn

Ruby: File.write("a.txt", "hi")
来源：https://gp.zhonguo8118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://xk.zhonguo2118.cn

[F04] 追加写入文件
来源：https://dl.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ws.zhonguo5118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://dl.zhonguo3118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ot.zhonguo5118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://sj.zhonguo6118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://sg.zhonguo7118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://rr.zhonguo6118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://cz.zhonguo2118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://pu.zhonguo1118.cn

[F05] 判断文件或目录是否存在
来源：https://yr.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ok.zhonguo4118.cn

PHP:  file_exists("a.txt");
来源：https://hz.zhonguo2118.cn

JS:   fs.existsSync("a.txt")
来源：https://ck.zhonguo5118.cn

TS:   fs.existsSync("a.txt")
来源：https://sv.zhonguo6118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://vy.zhonguo2118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ni.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://gz.zhonguo1118.cn

C#:   File.Exists("a.txt")
来源：https://pr.zhonguo6118.cn

[F06] 删除文件
来源：https://bl.zhonguo5118.cn

Py:   os.remove("a.txt")
来源：https://fj.zhonguo2118.cn

PHP:  unlink("a.txt");
来源：https://mn.zhonguo8118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://dd.zhonguo5118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://af.zhonguo8118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://gg.zhonguo7118.cn

Go:   os.Remove("a.txt")
来源：https://vd.zhonguo6118.cn

Ruby: File.delete("a.txt")
来源：https://jb.zhonguo2118.cn

C#:   File.Delete("a.txt");
来源：https://lp.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://ng.zhonguo6118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://ul.zhonguo3118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://xk.zhonguo7118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://jm.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://wf.zhonguo5118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://to.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://ip.zhonguo4118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ae.zhonguo6118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://oo.zhonguo6118.cn

[F08] 遍历目录
来源：https://kz.zhonguo3118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ri.zhonguo6118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://uf.zhonguo7118.cn

JS:   fs.readdirSync("dir")
来源：https://re.zhonguo1118.cn

TS:   fs.readdirSync("dir")
来源：https://lp.zhonguo7118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://lt.zhonguo6118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://xm.zhonguo8118.cn

Ruby: Dir.children("dir")
来源：https://oh.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://uv.zhonguo7118.cn

[F09] 获取文件大小
来源：https://ev.zhonguo6118.cn

Py:   os.path.getsize("a.txt")
来源：https://fc.zhonguo8118.cn

PHP:  filesize("a.txt");
来源：https://rm.zhonguo4118.cn

JS:   fs.statSync("a.txt").size
来源：https://aa.zhonguo2118.cn

TS:   fs.statSync("a.txt").size
来源：https://xw.zhonguo8118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://tu.zhonguo3118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://tp.zhonguo1118.cn

Ruby: File.size("a.txt")
来源：https://py.zhonguo1118.cn

C#:   new FileInfo("a.txt").Length
来源：https://pb.zhonguo3118.cn

[F10] 取文件扩展名 / 文件名
来源：https://hc.zhonguo3118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://xv.zhonguo7118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://hv.zhonguo4118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://nq.zhonguo7118.cn

TS:   path.extname("a.txt")
来源：https://yu.zhonguo2118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://uo.zhonguo6118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://tb.zhonguo4118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://pi.zhonguo5118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://zt.zhonguo7118.cn

[F11] 复制与移动文件
来源：https://sy.zhonguo8118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://nv.zhonguo1118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://tb.zhonguo4118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://oe.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://dl.zhonguo5118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://zw.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ar.zhonguo5118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://bf.zhonguo6118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://wh.zhonguo5118.cn

[F12] CSV 读写
来源：https://pa.zhonguo1118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://eu.zhonguo5118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://jg.zhonguo3118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://wz.zhonguo4118.cn

TS:   // 同上
来源：https://ht.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://aw.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://wo.zhonguo4118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://we.zhonguo4118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://le.zhonguo8118.cn

================================================================================
来源：https://fm.zhonguo5118.cn

G. 面向对象
来源：https://pf.zhonguo3118.cn

================================================================================
来源：https://hi.zhonguo5118.cn

[G01] 定义类
来源：https://hg.zhonguo4118.cn

Py:   class User: pass
来源：https://ct.zhonguo2118.cn

PHP:  class User {}
来源：https://lo.zhonguo8118.cn

JS:   class User {}
来源：https://by.zhonguo3118.cn

TS:   class User { name: string = ""; }
来源：https://dk.zhonguo1118.cn

Java: class User {}
来源：https://zq.zhonguo2118.cn

Go:   type User struct { Name string }
来源：https://fe.zhonguo4118.cn

Ruby: class User; end
来源：https://wm.zhonguo8118.cn

C#:   class User {}
来源：https://jm.zhonguo6118.cn

[G02] 构造函数
来源：https://ih.zhonguo4118.cn

Py:   def __init__(self, name): self.name = name
来源：https://ps.zhonguo2118.cn

PHP:  public function __construct(public string $name) {}
来源：https://yd.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://qr.zhonguo6118.cn

TS:   constructor(public name: string) {}
来源：https://vr.zhonguo6118.cn

Java: User(String name) { this.name = name; }
来源：https://ke.zhonguo8118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://td.zhonguo5118.cn

Ruby: def initialize(name); @name = name; end
来源：https://hp.zhonguo1118.cn

C#:   public User(string name) { Name = name; }
来源：https://oe.zhonguo4118.cn

[G03] 实例属性
来源：https://er.zhonguo4118.cn

Py:   self.name = "x"
来源：https://dv.zhonguo8118.cn

PHP:  public string $name = "x";
来源：https://rg.zhonguo4118.cn

JS:   this.name = "x";
来源：https://al.zhonguo2118.cn

TS:   name: string = "x";
来源：https://lw.zhonguo7118.cn

Java: private String name;
来源：https://ha.zhonguo8118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://fd.zhonguo5118.cn

Ruby: @name = "x"
来源：https://ay.zhonguo8118.cn

C#:   public string Name { get; set; } = "x";
来源：https://pw.zhonguo1118.cn

[G04] 定义方法
来源：https://vt.zhonguo2118.cn

Py:   def greet(self): return self.name
来源：https://jn.zhonguo4118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://du.zhonguo4118.cn

JS:   greet() { return this.name; }
来源：https://nc.zhonguo4118.cn

TS:   greet(): string { return this.name; }
来源：https://ae.zhonguo5118.cn

Java: String greet() { return name; }
来源：https://oh.zhonguo4118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://qk.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://ib.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://mr.zhonguo6118.cn

[G05] 继承
来源：https://hb.zhonguo8118.cn

Py:   class Admin(User): pass
来源：https://et.zhonguo3118.cn

PHP:  class Admin extends User {}
来源：https://ll.zhonguo5118.cn

JS:   class Admin extends User {}
来源：https://py.zhonguo2118.cn

TS:   class Admin extends User {}
来源：https://sz.zhonguo6118.cn

Java: class Admin extends User {}
来源：https://nv.zhonguo8118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://ab.zhonguo8118.cn

Ruby: class Admin < User; end
来源：https://oq.zhonguo1118.cn

C#:   class Admin : User {}
来源：https://lo.zhonguo3118.cn

[G06] 重写方法
来源：https://ge.zhonguo1118.cn

Py:   def greet(self): return "admin"
来源：https://qm.zhonguo6118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://hi.zhonguo5118.cn

JS:   greet() { return "admin"; }
来源：https://en.zhonguo6118.cn

TS:   greet(): string { return "admin"; }
来源：https://po.zhonguo2118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ay.zhonguo1118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://nz.zhonguo1118.cn

Ruby: def greet; "admin"; end
来源：https://fe.zhonguo2118.cn

C#:   public override string Greet() => "admin";
来源：https://so.zhonguo5118.cn

[G07] 调用父类方法
来源：https://rm.zhonguo6118.cn

Py:   super().greet()
来源：https://wf.zhonguo4118.cn

PHP:  parent::greet();
来源：https://sd.zhonguo3118.cn

JS:   super.greet();
来源：https://eb.zhonguo2118.cn

TS:   super.greet();
来源：https://dx.zhonguo8118.cn

Java: super.greet();
来源：https://oc.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://ej.zhonguo2118.cn

Ruby: super
来源：https://of.zhonguo5118.cn

C#:   base.Greet();
来源：https://ns.zhonguo2118.cn

[G08] 静态方法与属性
来源：https://pf.zhonguo1118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://hq.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://ki.zhonguo6118.cn

JS:   static f() {}
来源：https://hv.zhonguo2118.cn

TS:   static f(): void {}
来源：https://cn.zhonguo4118.cn

Java: static void f() {}
来源：https://sx.zhonguo8118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://da.zhonguo2118.cn

Ruby: def self.f; end
来源：https://vn.zhonguo7118.cn

C#:   public static void F() {}
来源：https://dk.zhonguo4118.cn

[G09] 接口 / 抽象类
来源：https://kc.zhonguo8118.cn

Py:   from abc import ABC, abstractmethod
来源：https://fy.zhonguo5118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://mc.zhonguo1118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://ww.zhonguo3118.cn

TS:   interface Shape { area(): number; }
来源：https://vq.zhonguo3118.cn

Java: interface Shape { double area(); }
来源：https://me.zhonguo1118.cn

Go:   type Shape interface { Area() float64 }
来源：https://vh.zhonguo3118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://pe.zhonguo1118.cn

C#:   interface IShape { double Area(); }
来源：https://kx.zhonguo5118.cn

[G10] 访问控制
来源：https://ni.zhonguo7118.cn

Py:   约定 _protected / __private（不强制）
来源：https://qx.zhonguo4118.cn

PHP:  public / protected / private
来源：https://to.zhonguo2118.cn

JS:   #private 字段；其余公开
来源：https://bg.zhonguo8118.cn

TS:   public / protected / private
来源：https://es.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://te.zhonguo1118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://ir.zhonguo5118.cn

Ruby: public / protected / private
来源：https://la.zhonguo4118.cn

C#:   public / protected / private / internal
来源：https://tn.zhonguo6118.cn

[G11] getter / setter
来源：https://mt.zhonguo4118.cn

Py:   @property 与 @x.setter
来源：https://cv.zhonguo8118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://ta.zhonguo5118.cn

JS:   get name() { return this._name; }
来源：https://wb.zhonguo5118.cn

TS:   get name(): string { return this._name; }
来源：https://fd.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://pu.zhonguo3118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://mx.zhonguo2118.cn

Ruby: attr_accessor :name
来源：https://gk.zhonguo3118.cn

C#:   public string Name { get; set; }
来源：https://uy.zhonguo7118.cn

[G12] 对象转字符串
来源：https://zu.zhonguo6118.cn

Py:   def __str__(self): return self.name
来源：https://bz.zhonguo7118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ma.zhonguo7118.cn

JS:   toString() { return this.name; }
来源：https://nf.zhonguo1118.cn

TS:   toString(): string { return this.name; }
来源：https://nk.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://ih.zhonguo4118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://nd.zhonguo3118.cn

Ruby: def to_s; @name; end
来源：https://lq.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://gk.zhonguo5118.cn

[G13] 判断对象类型
来源：https://gj.zhonguo2118.cn

Py:   isinstance(u, User)
来源：https://mc.zhonguo8118.cn

PHP:  $u instanceof User
来源：https://vx.zhonguo1118.cn

JS:   u instanceof User
来源：https://hy.zhonguo6118.cn

TS:   u instanceof User
来源：https://vn.zhonguo8118.cn

Java: u instanceof User
来源：https://zw.zhonguo3118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://qb.zhonguo3118.cn

Ruby: u.is_a?(User)
来源：https://di.zhonguo7118.cn

C#:   u is User
来源：https://bt.zhonguo6118.cn

[G14] 数据类 / record
来源：https://ki.zhonguo7118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://nd.zhonguo2118.cn

PHP:  // 用 readonly 属性模拟
来源：https://ui.zhonguo8118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://wu.zhonguo4118.cn

TS:   type User = { name: string; age: number };
来源：https://hp.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://ri.zhonguo7118.cn

Go:   type User struct { Name string; Age int }
来源：https://uh.zhonguo2118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://dk.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://ms.zhonguo7118.cn

[G15] 枚举
来源：https://sd.zhonguo1118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://np.zhonguo2118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ym.zhonguo3118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://yh.zhonguo2118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://rs.zhonguo1118.cn

Java: enum Color { RED, GREEN }
来源：https://uc.zhonguo3118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://al.zhonguo2118.cn

Ruby: Color = %i[red green].freeze
来源：https://pe.zhonguo4118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ke.zhonguo2118.cn

[G16] 对象转数组 / 字典
来源：https://rt.zhonguo8118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://qc.zhonguo6118.cn

PHP:  get_object_vars($obj);
来源：https://qn.zhonguo8118.cn

JS:   Object.entries(obj)
来源：https://ob.zhonguo6118.cn

TS:   Object.entries(obj)
来源：https://ef.zhonguo2118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://gv.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://vw.zhonguo8118.cn

Ruby: obj.instance_variables
来源：https://hp.zhonguo8118.cn

C#:   // 用反射或 System.Text.Json
来源：https://aj.zhonguo3118.cn

================================================================================
来源：https://cz.zhonguo1118.cn

H. 异常与错误处理
来源：https://px.zhonguo2118.cn

================================================================================
来源：https://qe.zhonguo4118.cn

[H01] try / catch 基础
来源：https://sb.zhonguo5118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://tr.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://dj.zhonguo6118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://xp.zhonguo4118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://zm.zhonguo3118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://ig.zhonguo4118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://vv.zhonguo5118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://of.zhonguo8118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://zr.zhonguo8118.cn

[H02] finally / ensure 收尾
来源：https://xh.zhonguo3118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://ce.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://us.zhonguo8118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://bd.zhonguo7118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://gr.zhonguo4118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ql.zhonguo1118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://qo.zhonguo5118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://sz.zhonguo3118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://fh.zhonguo2118.cn

[H03] 主动抛出异常
来源：https://rs.zhonguo4118.cn

Py:   raise ValueError("错误信息")
来源：https://vj.zhonguo4118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://nt.zhonguo1118.cn

JS:   throw new Error("错误信息");
来源：https://rc.zhonguo4118.cn

TS:   throw new Error("错误信息");
来源：https://ue.zhonguo6118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://it.zhonguo6118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ul.zhonguo4118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://dl.zhonguo4118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://cg.zhonguo3118.cn

[H04] 自定义异常类型
来源：https://se.zhonguo1118.cn

Py:   class MyError(Exception): pass
来源：https://sr.zhonguo3118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://ro.zhonguo7118.cn

JS:   class MyError extends Error {}
来源：https://lu.zhonguo4118.cn

TS:   class MyError extends Error {}
来源：https://pt.zhonguo2118.cn

Java: class MyException extends RuntimeException {}
来源：https://ov.zhonguo7118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://uz.zhonguo1118.cn


<!-- 参考信息 -->