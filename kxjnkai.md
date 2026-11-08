代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ed.zhonguo3118.cn

Go:   // 按 rune 判断长度后截断
来源：https://zh.zhonguo8118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://hz.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://gx.zhonguo5118.cn

[E22] 字节长度与字符长度
来源：https://ro.zhonguo2118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://vn.zhonguo5118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://wd.zhonguo7118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://al.zhonguo2118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://xl.zhonguo6118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://jc.zhonguo2118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://jt.zhonguo1118.cn

Ruby: s.bytesize;  s.length
来源：https://gd.zhonguo7118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://pr.zhonguo5118.cn

================================================================================
来源：https://bf.zhonguo6118.cn

F. 文件与目录
来源：https://ci.zhonguo8118.cn

================================================================================
来源：https://be.zhonguo8118.cn

[F01] 读取整个文件
来源：https://vr.zhonguo2118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://py.zhonguo2118.cn

PHP:  file_get_contents("a.txt");
来源：https://nd.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://md.zhonguo5118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://ti.zhonguo6118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://dd.zhonguo7118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ch.zhonguo7118.cn

Ruby: File.read("a.txt")
来源：https://qr.zhonguo5118.cn

C#:   File.ReadAllText("a.txt");
来源：https://sk.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://dy.zhonguo5118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://zz.zhonguo6118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://zu.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://ky.zhonguo3118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://im.zhonguo6118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://sa.zhonguo2118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://fg.zhonguo1118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://je.zhonguo3118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ag.zhonguo1118.cn

[F03] 写入文件（覆盖）
来源：https://cr.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://cq.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://wm.zhonguo6118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://bv.zhonguo2118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://cl.zhonguo2118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ut.zhonguo5118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://tv.zhonguo8118.cn

Ruby: File.write("a.txt", "hi")
来源：https://yo.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://li.zhonguo3118.cn

[F04] 追加写入文件
来源：https://gc.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ep.zhonguo6118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://ab.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://lm.zhonguo8118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ka.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://tl.zhonguo5118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://wm.zhonguo8118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ag.zhonguo5118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://sp.zhonguo2118.cn

[F05] 判断文件或目录是否存在
来源：https://tu.zhonguo7118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://mt.zhonguo1118.cn

PHP:  file_exists("a.txt");
来源：https://po.zhonguo7118.cn

JS:   fs.existsSync("a.txt")
来源：https://mo.zhonguo1118.cn

TS:   fs.existsSync("a.txt")
来源：https://ao.zhonguo5118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ad.zhonguo1118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://zz.zhonguo7118.cn

Ruby: File.exist?("a.txt")
来源：https://nq.zhonguo7118.cn

C#:   File.Exists("a.txt")
来源：https://bn.zhonguo6118.cn

[F06] 删除文件
来源：https://qa.zhonguo1118.cn

Py:   os.remove("a.txt")
来源：https://rd.zhonguo2118.cn

PHP:  unlink("a.txt");
来源：https://wc.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://lv.zhonguo1118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://yh.zhonguo7118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://kg.zhonguo3118.cn

Go:   os.Remove("a.txt")
来源：https://xa.zhonguo4118.cn

Ruby: File.delete("a.txt")
来源：https://fv.zhonguo3118.cn

C#:   File.Delete("a.txt");
来源：https://qw.zhonguo6118.cn

[F07] 创建目录（含多级）
来源：https://bu.zhonguo7118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://xt.zhonguo8118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://nw.zhonguo8118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://az.zhonguo3118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://vz.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://xm.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://by.zhonguo6118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://fu.zhonguo1118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://xy.zhonguo4118.cn

[F08] 遍历目录
来源：https://dd.zhonguo8118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://jh.zhonguo1118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://ts.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://kz.zhonguo6118.cn

TS:   fs.readdirSync("dir")
来源：https://hd.zhonguo7118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://cn.zhonguo5118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://im.zhonguo1118.cn

Ruby: Dir.children("dir")
来源：https://ro.zhonguo4118.cn

C#:   Directory.GetFiles("dir")
来源：https://aj.zhonguo2118.cn

[F09] 获取文件大小
来源：https://ao.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://jl.zhonguo1118.cn

PHP:  filesize("a.txt");
来源：https://to.zhonguo5118.cn

JS:   fs.statSync("a.txt").size
来源：https://nf.zhonguo7118.cn

TS:   fs.statSync("a.txt").size
来源：https://jh.zhonguo6118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://us.zhonguo6118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://dw.zhonguo1118.cn

Ruby: File.size("a.txt")
来源：https://ww.zhonguo6118.cn

C#:   new FileInfo("a.txt").Length
来源：https://dm.zhonguo5118.cn

[F10] 取文件扩展名 / 文件名
来源：https://iy.zhonguo2118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://jf.zhonguo4118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://ds.zhonguo5118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://km.zhonguo8118.cn

TS:   path.extname("a.txt")
来源：https://ed.zhonguo1118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://kb.zhonguo8118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://cq.zhonguo4118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://jn.zhonguo1118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://di.zhonguo4118.cn

[F11] 复制与移动文件
来源：https://iu.zhonguo5118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://mk.zhonguo7118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://dx.zhonguo8118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ud.zhonguo7118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://oz.zhonguo8118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://rf.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://el.zhonguo1118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://el.zhonguo2118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ho.zhonguo1118.cn

[F12] CSV 读写
来源：https://yh.zhonguo6118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://qq.zhonguo7118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://zv.zhonguo1118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://gm.zhonguo7118.cn

TS:   // 同上
来源：https://of.zhonguo1118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://bb.zhonguo6118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://iu.zhonguo7118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://zp.zhonguo2118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://we.zhonguo6118.cn

================================================================================
来源：https://yu.zhonguo4118.cn

G. 面向对象
来源：https://fk.zhonguo3118.cn

================================================================================
来源：https://yl.zhonguo7118.cn

[G01] 定义类
来源：https://pc.zhonguo8118.cn

Py:   class User: pass
来源：https://of.zhonguo4118.cn

PHP:  class User {}
来源：https://ck.zhonguo1118.cn

JS:   class User {}
来源：https://pw.zhonguo2118.cn

TS:   class User { name: string = ""; }
来源：https://ti.zhonguo4118.cn

Java: class User {}
来源：https://ws.zhonguo2118.cn

Go:   type User struct { Name string }
来源：https://nk.zhonguo5118.cn

Ruby: class User; end
来源：https://ej.zhonguo5118.cn

C#:   class User {}
来源：https://dq.zhonguo6118.cn

[G02] 构造函数
来源：https://lv.zhonguo4118.cn

Py:   def __init__(self, name): self.name = name
来源：https://hg.zhonguo2118.cn

PHP:  public function __construct(public string $name) {}
来源：https://rw.zhonguo3118.cn

JS:   constructor(name) { this.name = name; }
来源：https://so.zhonguo2118.cn

TS:   constructor(public name: string) {}
来源：https://cu.zhonguo1118.cn

Java: User(String name) { this.name = name; }
来源：https://iq.zhonguo3118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://wv.zhonguo2118.cn

Ruby: def initialize(name); @name = name; end
来源：https://qv.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://zf.zhonguo7118.cn

[G03] 实例属性
来源：https://ju.zhonguo4118.cn

Py:   self.name = "x"
来源：https://jp.zhonguo5118.cn

PHP:  public string $name = "x";
来源：https://ry.zhonguo1118.cn

JS:   this.name = "x";
来源：https://up.zhonguo5118.cn

TS:   name: string = "x";
来源：https://pl.zhonguo5118.cn

Java: private String name;
来源：https://la.zhonguo2118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://ms.zhonguo3118.cn

Ruby: @name = "x"
来源：https://tl.zhonguo5118.cn

C#:   public string Name { get; set; } = "x";
来源：https://td.zhonguo6118.cn

[G04] 定义方法
来源：https://qo.zhonguo1118.cn

Py:   def greet(self): return self.name
来源：https://iz.zhonguo5118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://wo.zhonguo6118.cn

JS:   greet() { return this.name; }
来源：https://qs.zhonguo3118.cn

TS:   greet(): string { return this.name; }
来源：https://cb.zhonguo8118.cn

Java: String greet() { return name; }
来源：https://dp.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://vh.zhonguo8118.cn

Ruby: def greet; @name; end
来源：https://nf.zhonguo8118.cn

C#:   public string Greet() => Name;
来源：https://rg.zhonguo1118.cn

[G05] 继承
来源：https://jv.zhonguo4118.cn

Py:   class Admin(User): pass
来源：https://yb.zhonguo8118.cn

PHP:  class Admin extends User {}
来源：https://sm.zhonguo4118.cn

JS:   class Admin extends User {}
来源：https://re.zhonguo5118.cn

TS:   class Admin extends User {}
来源：https://bh.zhonguo5118.cn

Java: class Admin extends User {}
来源：https://qc.zhonguo3118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://da.zhonguo1118.cn

Ruby: class Admin < User; end
来源：https://rb.zhonguo6118.cn

C#:   class Admin : User {}
来源：https://hw.zhonguo5118.cn

[G06] 重写方法
来源：https://ci.zhonguo8118.cn

Py:   def greet(self): return "admin"
来源：https://bo.zhonguo3118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://hm.zhonguo6118.cn

JS:   greet() { return "admin"; }
来源：https://rr.zhonguo7118.cn

TS:   greet(): string { return "admin"; }
来源：https://hn.zhonguo2118.cn

Java: @Override String greet() { return "admin"; }
来源：https://kj.zhonguo6118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://tl.zhonguo1118.cn

Ruby: def greet; "admin"; end
来源：https://xr.zhonguo4118.cn

C#:   public override string Greet() => "admin";
来源：https://sq.zhonguo3118.cn

[G07] 调用父类方法
来源：https://sd.zhonguo4118.cn

Py:   super().greet()
来源：https://wn.zhonguo4118.cn

PHP:  parent::greet();
来源：https://me.zhonguo2118.cn

JS:   super.greet();
来源：https://pn.zhonguo4118.cn

TS:   super.greet();
来源：https://ie.zhonguo8118.cn

Java: super.greet();
来源：https://gy.zhonguo7118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://di.zhonguo3118.cn

Ruby: super
来源：https://vq.zhonguo8118.cn

C#:   base.Greet();
来源：https://uv.zhonguo7118.cn

[G08] 静态方法与属性
来源：https://xm.zhonguo8118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://ej.zhonguo4118.cn

PHP:  public static function f() {}
来源：https://ut.zhonguo1118.cn

JS:   static f() {}
来源：https://ni.zhonguo8118.cn

TS:   static f(): void {}
来源：https://to.zhonguo3118.cn

Java: static void f() {}
来源：https://jc.zhonguo4118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://jv.zhonguo3118.cn

Ruby: def self.f; end
来源：https://lp.zhonguo5118.cn

C#:   public static void F() {}
来源：https://xv.zhonguo2118.cn

[G09] 接口 / 抽象类
来源：https://ec.zhonguo3118.cn

Py:   from abc import ABC, abstractmethod
来源：https://dj.zhonguo1118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://et.zhonguo2118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://kq.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://ri.zhonguo1118.cn

Java: interface Shape { double area(); }
来源：https://pn.zhonguo4118.cn

Go:   type Shape interface { Area() float64 }
来源：https://zf.zhonguo3118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://kg.zhonguo4118.cn

C#:   interface IShape { double Area(); }
来源：https://sy.zhonguo8118.cn

[G10] 访问控制
来源：https://xm.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://op.zhonguo3118.cn

PHP:  public / protected / private
来源：https://lj.zhonguo2118.cn

JS:   #private 字段；其余公开
来源：https://ae.zhonguo4118.cn

TS:   public / protected / private
来源：https://jl.zhonguo3118.cn

Java: public / protected / private / 默认包级
来源：https://lc.zhonguo2118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://pc.zhonguo4118.cn

Ruby: public / protected / private
来源：https://zf.zhonguo3118.cn

C#:   public / protected / private / internal
来源：https://vw.zhonguo3118.cn

[G11] getter / setter
来源：https://vw.zhonguo4118.cn

Py:   @property 与 @x.setter
来源：https://hf.zhonguo4118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://mw.zhonguo1118.cn

JS:   get name() { return this._name; }
来源：https://cj.zhonguo4118.cn

TS:   get name(): string { return this._name; }
来源：https://eo.zhonguo4118.cn

Java: public String getName() { return name; }
来源：https://an.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ki.zhonguo2118.cn

Ruby: attr_accessor :name
来源：https://nt.zhonguo6118.cn

C#:   public string Name { get; set; }
来源：https://ck.zhonguo1118.cn

[G12] 对象转字符串
来源：https://fk.zhonguo3118.cn

Py:   def __str__(self): return self.name
来源：https://pm.zhonguo6118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://mc.zhonguo8118.cn

JS:   toString() { return this.name; }
来源：https://bm.zhonguo3118.cn

TS:   toString(): string { return this.name; }
来源：https://tg.zhonguo8118.cn

Java: @Override public String toString() { return name; }
来源：https://qa.zhonguo4118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://mm.zhonguo4118.cn

Ruby: def to_s; @name; end
来源：https://qd.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://jg.zhonguo8118.cn

[G13] 判断对象类型
来源：https://wn.zhonguo2118.cn

Py:   isinstance(u, User)
来源：https://ao.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://gg.zhonguo4118.cn

JS:   u instanceof User
来源：https://hx.zhonguo5118.cn

TS:   u instanceof User
来源：https://qf.zhonguo5118.cn

Java: u instanceof User
来源：https://un.zhonguo7118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ap.zhonguo8118.cn

Ruby: u.is_a?(User)
来源：https://kg.zhonguo4118.cn

C#:   u is User
来源：https://xz.zhonguo6118.cn

[G14] 数据类 / record
来源：https://gw.zhonguo8118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://mt.zhonguo1118.cn

PHP:  // 用 readonly 属性模拟
来源：https://mw.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://zf.zhonguo2118.cn

TS:   type User = { name: string; age: number };
来源：https://ls.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://lu.zhonguo3118.cn

Go:   type User struct { Name string; Age int }
来源：https://gs.zhonguo2118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://iy.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://hw.zhonguo6118.cn

[G15] 枚举
来源：https://cf.zhonguo2118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://qc.zhonguo2118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ny.zhonguo8118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://yo.zhonguo6118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://fb.zhonguo1118.cn

Java: enum Color { RED, GREEN }
来源：https://eu.zhonguo3118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://xq.zhonguo6118.cn

Ruby: Color = %i[red green].freeze
来源：https://li.zhonguo2118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://kn.zhonguo2118.cn

[G16] 对象转数组 / 字典
来源：https://op.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://at.zhonguo8118.cn

PHP:  get_object_vars($obj);
来源：https://gz.zhonguo6118.cn

JS:   Object.entries(obj)
来源：https://wi.zhonguo8118.cn

TS:   Object.entries(obj)
来源：https://ls.zhonguo2118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://es.zhonguo3118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://zs.zhonguo3118.cn

Ruby: obj.instance_variables
来源：https://jr.zhonguo4118.cn

C#:   // 用反射或 System.Text.Json
来源：https://zo.zhonguo6118.cn

================================================================================
来源：https://gk.zhonguo4118.cn

H. 异常与错误处理
来源：https://dl.zhonguo1118.cn

================================================================================
来源：https://bw.zhonguo2118.cn

[H01] try / catch 基础
来源：https://zt.zhonguo3118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://cp.zhonguo2118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://gi.zhonguo2118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://fr.zhonguo5118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://if.zhonguo4118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://tt.zhonguo3118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://kj.zhonguo8118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://tb.zhonguo7118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://id.zhonguo5118.cn

[H02] finally / ensure 收尾
来源：https://up.zhonguo3118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://en.zhonguo5118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://qi.zhonguo6118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://kf.zhonguo8118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://kh.zhonguo5118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://yf.zhonguo2118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://gc.zhonguo3118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://su.zhonguo8118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://af.zhonguo8118.cn

[H03] 主动抛出异常
来源：https://rw.zhonguo2118.cn

Py:   raise ValueError("错误信息")
来源：https://sr.zhonguo4118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://xb.zhonguo2118.cn

JS:   throw new Error("错误信息");
来源：https://th.zhonguo1118.cn

TS:   throw new Error("错误信息");
来源：https://hk.zhonguo7118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://gm.zhonguo4118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ap.zhonguo8118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://cg.zhonguo1118.cn


<!-- 参考信息 -->