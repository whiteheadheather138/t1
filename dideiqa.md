代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://dz.zhonguo3118.cn

Go:   // 按 rune 判断长度后截断
来源：https://pz.zhonguo5118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://sd.zhonguo1118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://hm.zhonguo3118.cn

[E22] 字节长度与字符长度
来源：https://gk.zhonguo4118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://at.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://rv.zhonguo1118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://dy.zhonguo6118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://ww.zhonguo4118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://rb.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://ab.zhonguo4118.cn

Ruby: s.bytesize;  s.length
来源：https://uq.zhonguo4118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://nl.zhonguo2118.cn

================================================================================
来源：https://yo.zhonguo8118.cn

F. 文件与目录
来源：https://uk.zhonguo8118.cn

================================================================================
来源：https://px.zhonguo5118.cn

[F01] 读取整个文件
来源：https://qk.zhonguo2118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://ri.zhonguo1118.cn

PHP:  file_get_contents("a.txt");
来源：https://fh.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://dt.zhonguo4118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://af.zhonguo6118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ds.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ge.zhonguo7118.cn

Ruby: File.read("a.txt")
来源：https://rg.zhonguo4118.cn

C#:   File.ReadAllText("a.txt");
来源：https://ju.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://kw.zhonguo6118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://wg.zhonguo3118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://xf.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://wi.zhonguo7118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://fk.zhonguo4118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://pu.zhonguo1118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://dh.zhonguo6118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://sw.zhonguo6118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ui.zhonguo4118.cn

[F03] 写入文件（覆盖）
来源：https://id.zhonguo8118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://ri.zhonguo5118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://xz.zhonguo7118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://qa.zhonguo1118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://wk.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://fe.zhonguo8118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://nh.zhonguo2118.cn

Ruby: File.write("a.txt", "hi")
来源：https://fs.zhonguo3118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://iy.zhonguo3118.cn

[F04] 追加写入文件
来源：https://jx.zhonguo2118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ax.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://pu.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://op.zhonguo1118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://bw.zhonguo6118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://vf.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://xk.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://cl.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://fn.zhonguo2118.cn

[F05] 判断文件或目录是否存在
来源：https://rp.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ls.zhonguo2118.cn

PHP:  file_exists("a.txt");
来源：https://ds.zhonguo5118.cn

JS:   fs.existsSync("a.txt")
来源：https://up.zhonguo7118.cn

TS:   fs.existsSync("a.txt")
来源：https://za.zhonguo8118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://gf.zhonguo3118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://zu.zhonguo6118.cn

Ruby: File.exist?("a.txt")
来源：https://pg.zhonguo6118.cn

C#:   File.Exists("a.txt")
来源：https://sx.zhonguo1118.cn

[F06] 删除文件
来源：https://jl.zhonguo5118.cn

Py:   os.remove("a.txt")
来源：https://oq.zhonguo5118.cn

PHP:  unlink("a.txt");
来源：https://uu.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://ke.zhonguo4118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://xp.zhonguo8118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://fq.zhonguo2118.cn

Go:   os.Remove("a.txt")
来源：https://cs.zhonguo3118.cn

Ruby: File.delete("a.txt")
来源：https://th.zhonguo2118.cn

C#:   File.Delete("a.txt");
来源：https://nj.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://ty.zhonguo5118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://sz.zhonguo4118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://sj.zhonguo1118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://dr.zhonguo2118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://cv.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://gy.zhonguo1118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://qz.zhonguo6118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://jv.zhonguo2118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://uv.zhonguo1118.cn

[F08] 遍历目录
来源：https://xr.zhonguo2118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://au.zhonguo3118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://wa.zhonguo1118.cn

JS:   fs.readdirSync("dir")
来源：https://ig.zhonguo8118.cn

TS:   fs.readdirSync("dir")
来源：https://ki.zhonguo7118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://ma.zhonguo7118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://kn.zhonguo5118.cn

Ruby: Dir.children("dir")
来源：https://bz.zhonguo5118.cn

C#:   Directory.GetFiles("dir")
来源：https://cq.zhonguo7118.cn

[F09] 获取文件大小
来源：https://db.zhonguo6118.cn

Py:   os.path.getsize("a.txt")
来源：https://ic.zhonguo3118.cn

PHP:  filesize("a.txt");
来源：https://zw.zhonguo2118.cn

JS:   fs.statSync("a.txt").size
来源：https://yj.zhonguo5118.cn

TS:   fs.statSync("a.txt").size
来源：https://vh.zhonguo7118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://ct.zhonguo1118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://nm.zhonguo6118.cn

Ruby: File.size("a.txt")
来源：https://br.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://ht.zhonguo8118.cn

[F10] 取文件扩展名 / 文件名
来源：https://sx.zhonguo1118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://ez.zhonguo3118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://mb.zhonguo1118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://kl.zhonguo4118.cn

TS:   path.extname("a.txt")
来源：https://sc.zhonguo1118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://wl.zhonguo4118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://wu.zhonguo6118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://ee.zhonguo1118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://ei.zhonguo4118.cn

[F11] 复制与移动文件
来源：https://bw.zhonguo5118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://ph.zhonguo3118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://wh.zhonguo8118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://sr.zhonguo8118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://qt.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://mz.zhonguo7118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ws.zhonguo6118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://cp.zhonguo8118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://yv.zhonguo4118.cn

[F12] CSV 读写
来源：https://rb.zhonguo2118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://lt.zhonguo6118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://iq.zhonguo7118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://tu.zhonguo7118.cn

TS:   // 同上
来源：https://bw.zhonguo2118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://oy.zhonguo8118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://rt.zhonguo7118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://yc.zhonguo7118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://mx.zhonguo8118.cn

================================================================================
来源：https://rm.zhonguo2118.cn

G. 面向对象
来源：https://pf.zhonguo1118.cn

================================================================================
来源：https://ta.zhonguo4118.cn

[G01] 定义类
来源：https://yx.zhonguo7118.cn

Py:   class User: pass
来源：https://ao.zhonguo8118.cn

PHP:  class User {}
来源：https://zb.zhonguo6118.cn

JS:   class User {}
来源：https://ba.zhonguo4118.cn

TS:   class User { name: string = ""; }
来源：https://jv.zhonguo3118.cn

Java: class User {}
来源：https://tv.zhonguo6118.cn

Go:   type User struct { Name string }
来源：https://ud.zhonguo8118.cn

Ruby: class User; end
来源：https://ky.zhonguo4118.cn

C#:   class User {}
来源：https://mi.zhonguo1118.cn

[G02] 构造函数
来源：https://xj.zhonguo7118.cn

Py:   def __init__(self, name): self.name = name
来源：https://db.zhonguo5118.cn

PHP:  public function __construct(public string $name) {}
来源：https://qi.zhonguo2118.cn

JS:   constructor(name) { this.name = name; }
来源：https://zn.zhonguo4118.cn

TS:   constructor(public name: string) {}
来源：https://zy.zhonguo5118.cn

Java: User(String name) { this.name = name; }
来源：https://se.zhonguo7118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://cy.zhonguo6118.cn

Ruby: def initialize(name); @name = name; end
来源：https://uz.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://ov.zhonguo5118.cn

[G03] 实例属性
来源：https://kw.zhonguo8118.cn

Py:   self.name = "x"
来源：https://xc.zhonguo3118.cn

PHP:  public string $name = "x";
来源：https://yo.zhonguo5118.cn

JS:   this.name = "x";
来源：https://cv.zhonguo2118.cn

TS:   name: string = "x";
来源：https://zt.zhonguo2118.cn

Java: private String name;
来源：https://dl.zhonguo6118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://wd.zhonguo5118.cn

Ruby: @name = "x"
来源：https://vw.zhonguo1118.cn

C#:   public string Name { get; set; } = "x";
来源：https://no.zhonguo4118.cn

[G04] 定义方法
来源：https://ik.zhonguo8118.cn

Py:   def greet(self): return self.name
来源：https://nk.zhonguo5118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://hn.zhonguo2118.cn

JS:   greet() { return this.name; }
来源：https://hz.zhonguo4118.cn

TS:   greet(): string { return this.name; }
来源：https://zx.zhonguo8118.cn

Java: String greet() { return name; }
来源：https://bs.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://me.zhonguo7118.cn

Ruby: def greet; @name; end
来源：https://km.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://ho.zhonguo8118.cn

[G05] 继承
来源：https://ws.zhonguo7118.cn

Py:   class Admin(User): pass
来源：https://ql.zhonguo3118.cn

PHP:  class Admin extends User {}
来源：https://nf.zhonguo7118.cn

JS:   class Admin extends User {}
来源：https://nv.zhonguo6118.cn

TS:   class Admin extends User {}
来源：https://tq.zhonguo7118.cn

Java: class Admin extends User {}
来源：https://us.zhonguo8118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://cv.zhonguo7118.cn

Ruby: class Admin < User; end
来源：https://yh.zhonguo6118.cn

C#:   class Admin : User {}
来源：https://ya.zhonguo1118.cn

[G06] 重写方法
来源：https://qc.zhonguo1118.cn

Py:   def greet(self): return "admin"
来源：https://hw.zhonguo5118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://yh.zhonguo8118.cn

JS:   greet() { return "admin"; }
来源：https://uh.zhonguo8118.cn

TS:   greet(): string { return "admin"; }
来源：https://rr.zhonguo4118.cn

Java: @Override String greet() { return "admin"; }
来源：https://an.zhonguo7118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://ux.zhonguo5118.cn

Ruby: def greet; "admin"; end
来源：https://bj.zhonguo2118.cn

C#:   public override string Greet() => "admin";
来源：https://ht.zhonguo2118.cn

[G07] 调用父类方法
来源：https://go.zhonguo5118.cn

Py:   super().greet()
来源：https://ef.zhonguo8118.cn

PHP:  parent::greet();
来源：https://gl.zhonguo5118.cn

JS:   super.greet();
来源：https://du.zhonguo7118.cn

TS:   super.greet();
来源：https://vf.zhonguo6118.cn

Java: super.greet();
来源：https://io.zhonguo5118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://ke.zhonguo5118.cn

Ruby: super
来源：https://js.zhonguo8118.cn

C#:   base.Greet();
来源：https://oj.zhonguo4118.cn

[G08] 静态方法与属性
来源：https://ga.zhonguo1118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://as.zhonguo5118.cn

PHP:  public static function f() {}
来源：https://vk.zhonguo7118.cn

JS:   static f() {}
来源：https://mi.zhonguo5118.cn

TS:   static f(): void {}
来源：https://nu.zhonguo2118.cn

Java: static void f() {}
来源：https://jm.zhonguo1118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://xe.zhonguo7118.cn

Ruby: def self.f; end
来源：https://sg.zhonguo7118.cn

C#:   public static void F() {}
来源：https://vb.zhonguo8118.cn

[G09] 接口 / 抽象类
来源：https://ta.zhonguo3118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ng.zhonguo8118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://ty.zhonguo5118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://bt.zhonguo2118.cn

TS:   interface Shape { area(): number; }
来源：https://hk.zhonguo6118.cn

Java: interface Shape { double area(); }
来源：https://pb.zhonguo7118.cn

Go:   type Shape interface { Area() float64 }
来源：https://cf.zhonguo6118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://yw.zhonguo1118.cn

C#:   interface IShape { double Area(); }
来源：https://jk.zhonguo1118.cn

[G10] 访问控制
来源：https://ds.zhonguo7118.cn

Py:   约定 _protected / __private（不强制）
来源：https://au.zhonguo4118.cn

PHP:  public / protected / private
来源：https://wv.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://wk.zhonguo6118.cn

TS:   public / protected / private
来源：https://bg.zhonguo8118.cn

Java: public / protected / private / 默认包级
来源：https://dk.zhonguo1118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://dy.zhonguo5118.cn

Ruby: public / protected / private
来源：https://vg.zhonguo8118.cn

C#:   public / protected / private / internal
来源：https://pk.zhonguo7118.cn

[G11] getter / setter
来源：https://bw.zhonguo6118.cn

Py:   @property 与 @x.setter
来源：https://so.zhonguo6118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://lq.zhonguo2118.cn

JS:   get name() { return this._name; }
来源：https://sb.zhonguo3118.cn

TS:   get name(): string { return this._name; }
来源：https://lx.zhonguo4118.cn

Java: public String getName() { return name; }
来源：https://wy.zhonguo6118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://yd.zhonguo1118.cn

Ruby: attr_accessor :name
来源：https://cb.zhonguo2118.cn

C#:   public string Name { get; set; }
来源：https://sj.zhonguo1118.cn

[G12] 对象转字符串
来源：https://pn.zhonguo2118.cn

Py:   def __str__(self): return self.name
来源：https://ox.zhonguo4118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://jo.zhonguo4118.cn

JS:   toString() { return this.name; }
来源：https://gq.zhonguo8118.cn

TS:   toString(): string { return this.name; }
来源：https://ep.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://ej.zhonguo7118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://pl.zhonguo3118.cn

Ruby: def to_s; @name; end
来源：https://ge.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://bm.zhonguo7118.cn

[G13] 判断对象类型
来源：https://ym.zhonguo2118.cn

Py:   isinstance(u, User)
来源：https://qd.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://ec.zhonguo3118.cn

JS:   u instanceof User
来源：https://tt.zhonguo6118.cn

TS:   u instanceof User
来源：https://ly.zhonguo1118.cn

Java: u instanceof User
来源：https://xx.zhonguo5118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://df.zhonguo5118.cn

Ruby: u.is_a?(User)
来源：https://ps.zhonguo3118.cn

C#:   u is User
来源：https://bb.zhonguo5118.cn

[G14] 数据类 / record
来源：https://oe.zhonguo2118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://qu.zhonguo2118.cn

PHP:  // 用 readonly 属性模拟
来源：https://pi.zhonguo5118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://io.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://ix.zhonguo1118.cn

Java: record User(String name, int age) {}
来源：https://wb.zhonguo8118.cn

Go:   type User struct { Name string; Age int }
来源：https://rq.zhonguo1118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://ih.zhonguo8118.cn

C#:   record User(string Name, int Age);
来源：https://jq.zhonguo4118.cn

[G15] 枚举
来源：https://id.zhonguo4118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://yn.zhonguo5118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://fm.zhonguo8118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://ew.zhonguo7118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://bt.zhonguo4118.cn

Java: enum Color { RED, GREEN }
来源：https://fr.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://ne.zhonguo3118.cn

Ruby: Color = %i[red green].freeze
来源：https://fg.zhonguo6118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://pw.zhonguo1118.cn

[G16] 对象转数组 / 字典
来源：https://ib.zhonguo1118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://zo.zhonguo7118.cn

PHP:  get_object_vars($obj);
来源：https://eh.zhonguo1118.cn

JS:   Object.entries(obj)
来源：https://ln.zhonguo7118.cn

TS:   Object.entries(obj)
来源：https://ae.zhonguo2118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://wk.zhonguo5118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://uj.zhonguo7118.cn

Ruby: obj.instance_variables
来源：https://wb.zhonguo1118.cn

C#:   // 用反射或 System.Text.Json
来源：https://ea.zhonguo7118.cn

================================================================================
来源：https://kq.zhonguo3118.cn

H. 异常与错误处理
来源：https://kp.zhonguo2118.cn

================================================================================
来源：https://eo.zhonguo4118.cn

[H01] try / catch 基础
来源：https://ez.zhonguo1118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://fw.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://io.zhonguo8118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://yg.zhonguo3118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://xh.zhonguo4118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://jf.zhonguo8118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://pm.zhonguo1118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ae.zhonguo4118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://si.zhonguo6118.cn

[H02] finally / ensure 收尾
来源：https://ch.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://kp.zhonguo8118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://qo.zhonguo3118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://ea.zhonguo5118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://jz.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ig.zhonguo2118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://tx.zhonguo3118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://gq.zhonguo8118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ki.zhonguo8118.cn

[H03] 主动抛出异常
来源：https://gd.zhonguo6118.cn

Py:   raise ValueError("错误信息")
来源：https://ks.zhonguo5118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ia.zhonguo7118.cn

JS:   throw new Error("错误信息");
来源：https://xb.zhonguo8118.cn

TS:   throw new Error("错误信息");
来源：https://xv.zhonguo2118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://rw.zhonguo4118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://vl.zhonguo4118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://fv.zhonguo8118.cn


<!-- 参考信息 -->