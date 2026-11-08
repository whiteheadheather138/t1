代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://fp.zhonguo6118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://ms.zhonguo7118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://sc.zhonguo4118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ne.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://kp.zhonguo5118.cn

Go:   // 按 rune 判断长度后截断
来源：https://we.zhonguo8118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://dg.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://lc.zhonguo5118.cn

[E22] 字节长度与字符长度
来源：https://up.zhonguo6118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://as.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ts.zhonguo7118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://yx.zhonguo3118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://hd.zhonguo2118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://fi.zhonguo5118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://ke.zhonguo8118.cn

Ruby: s.bytesize;  s.length
来源：https://qu.zhonguo5118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://tx.zhonguo1118.cn

================================================================================
来源：https://xa.zhonguo5118.cn

F. 文件与目录
来源：https://tz.zhonguo2118.cn

================================================================================
来源：https://ga.zhonguo8118.cn

[F01] 读取整个文件
来源：https://sq.zhonguo2118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://fy.zhonguo2118.cn

PHP:  file_get_contents("a.txt");
来源：https://yi.zhonguo3118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://ku.zhonguo6118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://nf.zhonguo3118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ej.zhonguo6118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://vn.zhonguo7118.cn

Ruby: File.read("a.txt")
来源：https://em.zhonguo2118.cn

C#:   File.ReadAllText("a.txt");
来源：https://yv.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://fg.zhonguo4118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://qq.zhonguo8118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://iw.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://ve.zhonguo8118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://wa.zhonguo2118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://qg.zhonguo1118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://ow.zhonguo1118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://qd.zhonguo1118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ku.zhonguo3118.cn

[F03] 写入文件（覆盖）
来源：https://fa.zhonguo4118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://lq.zhonguo2118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://nf.zhonguo7118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://tv.zhonguo5118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://sv.zhonguo3118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://qp.zhonguo1118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ot.zhonguo2118.cn

Ruby: File.write("a.txt", "hi")
来源：https://kf.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://xh.zhonguo6118.cn

[F04] 追加写入文件
来源：https://zv.zhonguo8118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://te.zhonguo6118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://vb.zhonguo5118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://qy.zhonguo3118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://bx.zhonguo4118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://em.zhonguo6118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://lw.zhonguo7118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://wi.zhonguo4118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://td.zhonguo1118.cn

[F05] 判断文件或目录是否存在
来源：https://ad.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://fh.zhonguo5118.cn

PHP:  file_exists("a.txt");
来源：https://dw.zhonguo3118.cn

JS:   fs.existsSync("a.txt")
来源：https://ba.zhonguo3118.cn

TS:   fs.existsSync("a.txt")
来源：https://kc.zhonguo8118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://pl.zhonguo7118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://rh.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://hr.zhonguo8118.cn

C#:   File.Exists("a.txt")
来源：https://ia.zhonguo7118.cn

[F06] 删除文件
来源：https://dn.zhonguo5118.cn

Py:   os.remove("a.txt")
来源：https://mr.zhonguo4118.cn

PHP:  unlink("a.txt");
来源：https://id.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://uk.zhonguo8118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://ed.zhonguo6118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://jf.zhonguo6118.cn

Go:   os.Remove("a.txt")
来源：https://xm.zhonguo8118.cn

Ruby: File.delete("a.txt")
来源：https://ze.zhonguo7118.cn

C#:   File.Delete("a.txt");
来源：https://fg.zhonguo8118.cn

[F07] 创建目录（含多级）
来源：https://tj.zhonguo8118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://yi.zhonguo4118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://qg.zhonguo1118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ij.zhonguo4118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ex.zhonguo4118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://gi.zhonguo1118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://pn.zhonguo5118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://wo.zhonguo4118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://bc.zhonguo4118.cn

[F08] 遍历目录
来源：https://ma.zhonguo1118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://jx.zhonguo7118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://yu.zhonguo2118.cn

JS:   fs.readdirSync("dir")
来源：https://on.zhonguo3118.cn

TS:   fs.readdirSync("dir")
来源：https://lh.zhonguo8118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://la.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://tq.zhonguo2118.cn

Ruby: Dir.children("dir")
来源：https://qz.zhonguo1118.cn

C#:   Directory.GetFiles("dir")
来源：https://rb.zhonguo8118.cn

[F09] 获取文件大小
来源：https://vi.zhonguo6118.cn

Py:   os.path.getsize("a.txt")
来源：https://sy.zhonguo1118.cn

PHP:  filesize("a.txt");
来源：https://ql.zhonguo3118.cn

JS:   fs.statSync("a.txt").size
来源：https://kd.zhonguo6118.cn

TS:   fs.statSync("a.txt").size
来源：https://us.zhonguo3118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://zs.zhonguo6118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://oa.zhonguo6118.cn

Ruby: File.size("a.txt")
来源：https://zx.zhonguo1118.cn

C#:   new FileInfo("a.txt").Length
来源：https://sa.zhonguo8118.cn

[F10] 取文件扩展名 / 文件名
来源：https://nv.zhonguo5118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://lx.zhonguo6118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://ig.zhonguo2118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://xt.zhonguo8118.cn

TS:   path.extname("a.txt")
来源：https://fr.zhonguo2118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://yn.zhonguo3118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://uj.zhonguo4118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://or.zhonguo4118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://hn.zhonguo8118.cn

[F11] 复制与移动文件
来源：https://wh.zhonguo8118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://rj.zhonguo4118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ny.zhonguo4118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://og.zhonguo6118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://sv.zhonguo6118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://zi.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://yy.zhonguo8118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://tg.zhonguo3118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ro.zhonguo8118.cn

[F12] CSV 读写
来源：https://bv.zhonguo5118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ep.zhonguo5118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://mf.zhonguo6118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://yq.zhonguo8118.cn

TS:   // 同上
来源：https://fp.zhonguo3118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://kb.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://gl.zhonguo5118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://by.zhonguo8118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ex.zhonguo7118.cn

================================================================================
来源：https://lg.zhonguo7118.cn

G. 面向对象
来源：https://cv.zhonguo5118.cn

================================================================================
来源：https://xf.zhonguo1118.cn

[G01] 定义类
来源：https://vk.zhonguo2118.cn

Py:   class User: pass
来源：https://ox.zhonguo5118.cn

PHP:  class User {}
来源：https://hp.zhonguo6118.cn

JS:   class User {}
来源：https://fu.zhonguo8118.cn

TS:   class User { name: string = ""; }
来源：https://ij.zhonguo2118.cn

Java: class User {}
来源：https://qv.zhonguo3118.cn

Go:   type User struct { Name string }
来源：https://rd.zhonguo7118.cn

Ruby: class User; end
来源：https://qc.zhonguo3118.cn

C#:   class User {}
来源：https://lg.zhonguo8118.cn

[G02] 构造函数
来源：https://jj.zhonguo3118.cn

Py:   def __init__(self, name): self.name = name
来源：https://oi.zhonguo2118.cn

PHP:  public function __construct(public string $name) {}
来源：https://hy.zhonguo8118.cn

JS:   constructor(name) { this.name = name; }
来源：https://jf.zhonguo7118.cn

TS:   constructor(public name: string) {}
来源：https://xq.zhonguo1118.cn

Java: User(String name) { this.name = name; }
来源：https://el.zhonguo4118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://tl.zhonguo5118.cn

Ruby: def initialize(name); @name = name; end
来源：https://as.zhonguo5118.cn

C#:   public User(string name) { Name = name; }
来源：https://do.zhonguo7118.cn

[G03] 实例属性
来源：https://bt.zhonguo6118.cn

Py:   self.name = "x"
来源：https://yl.zhonguo4118.cn

PHP:  public string $name = "x";
来源：https://td.zhonguo6118.cn

JS:   this.name = "x";
来源：https://qu.zhonguo3118.cn

TS:   name: string = "x";
来源：https://iu.zhonguo1118.cn

Java: private String name;
来源：https://se.zhonguo2118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://hk.zhonguo7118.cn

Ruby: @name = "x"
来源：https://lf.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://fc.zhonguo2118.cn

[G04] 定义方法
来源：https://iv.zhonguo7118.cn

Py:   def greet(self): return self.name
来源：https://uy.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://hz.zhonguo1118.cn

JS:   greet() { return this.name; }
来源：https://dt.zhonguo2118.cn

TS:   greet(): string { return this.name; }
来源：https://bx.zhonguo3118.cn

Java: String greet() { return name; }
来源：https://yj.zhonguo5118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://dt.zhonguo3118.cn

Ruby: def greet; @name; end
来源：https://dj.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://om.zhonguo2118.cn

[G05] 继承
来源：https://ii.zhonguo2118.cn

Py:   class Admin(User): pass
来源：https://wi.zhonguo6118.cn

PHP:  class Admin extends User {}
来源：https://ls.zhonguo1118.cn

JS:   class Admin extends User {}
来源：https://ut.zhonguo8118.cn

TS:   class Admin extends User {}
来源：https://kl.zhonguo2118.cn

Java: class Admin extends User {}
来源：https://lr.zhonguo3118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://oz.zhonguo3118.cn

Ruby: class Admin < User; end
来源：https://xq.zhonguo1118.cn

C#:   class Admin : User {}
来源：https://sc.zhonguo3118.cn

[G06] 重写方法
来源：https://kv.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://yh.zhonguo5118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ig.zhonguo4118.cn

JS:   greet() { return "admin"; }
来源：https://zv.zhonguo3118.cn

TS:   greet(): string { return "admin"; }
来源：https://fw.zhonguo8118.cn

Java: @Override String greet() { return "admin"; }
来源：https://pj.zhonguo6118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://op.zhonguo1118.cn

Ruby: def greet; "admin"; end
来源：https://oi.zhonguo3118.cn

C#:   public override string Greet() => "admin";
来源：https://gt.zhonguo6118.cn

[G07] 调用父类方法
来源：https://aa.zhonguo6118.cn

Py:   super().greet()
来源：https://mg.zhonguo7118.cn

PHP:  parent::greet();
来源：https://bs.zhonguo2118.cn

JS:   super.greet();
来源：https://ry.zhonguo4118.cn

TS:   super.greet();
来源：https://zp.zhonguo2118.cn

Java: super.greet();
来源：https://ck.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://gz.zhonguo7118.cn

Ruby: super
来源：https://ki.zhonguo4118.cn

C#:   base.Greet();
来源：https://zw.zhonguo6118.cn

[G08] 静态方法与属性
来源：https://cw.zhonguo8118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://kv.zhonguo7118.cn

PHP:  public static function f() {}
来源：https://ej.zhonguo4118.cn

JS:   static f() {}
来源：https://rd.zhonguo7118.cn

TS:   static f(): void {}
来源：https://bo.zhonguo2118.cn

Java: static void f() {}
来源：https://on.zhonguo4118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://pf.zhonguo7118.cn

Ruby: def self.f; end
来源：https://kt.zhonguo5118.cn

C#:   public static void F() {}
来源：https://pg.zhonguo7118.cn

[G09] 接口 / 抽象类
来源：https://vg.zhonguo3118.cn

Py:   from abc import ABC, abstractmethod
来源：https://jz.zhonguo4118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://kx.zhonguo5118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://ft.zhonguo3118.cn

TS:   interface Shape { area(): number; }
来源：https://dl.zhonguo5118.cn

Java: interface Shape { double area(); }
来源：https://js.zhonguo2118.cn

Go:   type Shape interface { Area() float64 }
来源：https://ni.zhonguo6118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://wi.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://pn.zhonguo1118.cn

[G10] 访问控制
来源：https://bc.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://qh.zhonguo1118.cn

PHP:  public / protected / private
来源：https://to.zhonguo7118.cn

JS:   #private 字段；其余公开
来源：https://nk.zhonguo4118.cn

TS:   public / protected / private
来源：https://iu.zhonguo8118.cn

Java: public / protected / private / 默认包级
来源：https://je.zhonguo7118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://hu.zhonguo8118.cn

Ruby: public / protected / private
来源：https://mw.zhonguo4118.cn

C#:   public / protected / private / internal
来源：https://av.zhonguo6118.cn

[G11] getter / setter
来源：https://tm.zhonguo3118.cn

Py:   @property 与 @x.setter
来源：https://rk.zhonguo4118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://gf.zhonguo4118.cn

JS:   get name() { return this._name; }
来源：https://ec.zhonguo3118.cn

TS:   get name(): string { return this._name; }
来源：https://um.zhonguo4118.cn

Java: public String getName() { return name; }
来源：https://yr.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://jp.zhonguo4118.cn

Ruby: attr_accessor :name
来源：https://ty.zhonguo7118.cn

C#:   public string Name { get; set; }
来源：https://bz.zhonguo3118.cn

[G12] 对象转字符串
来源：https://yn.zhonguo2118.cn

Py:   def __str__(self): return self.name
来源：https://tx.zhonguo5118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ew.zhonguo2118.cn

JS:   toString() { return this.name; }
来源：https://uz.zhonguo3118.cn

TS:   toString(): string { return this.name; }
来源：https://gq.zhonguo1118.cn

Java: @Override public String toString() { return name; }
来源：https://ij.zhonguo7118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://gn.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://li.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://bh.zhonguo8118.cn

[G13] 判断对象类型
来源：https://qn.zhonguo3118.cn

Py:   isinstance(u, User)
来源：https://gk.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://zs.zhonguo4118.cn

JS:   u instanceof User
来源：https://cb.zhonguo1118.cn

TS:   u instanceof User
来源：https://mz.zhonguo4118.cn

Java: u instanceof User
来源：https://es.zhonguo4118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://hy.zhonguo4118.cn

Ruby: u.is_a?(User)
来源：https://cr.zhonguo1118.cn

C#:   u is User
来源：https://jw.zhonguo7118.cn

[G14] 数据类 / record
来源：https://ih.zhonguo2118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://jd.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://jb.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://eh.zhonguo7118.cn

TS:   type User = { name: string; age: number };
来源：https://dv.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://hq.zhonguo4118.cn

Go:   type User struct { Name string; Age int }
来源：https://ic.zhonguo7118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://uo.zhonguo2118.cn

C#:   record User(string Name, int Age);
来源：https://vi.zhonguo5118.cn

[G15] 枚举
来源：https://sn.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://pw.zhonguo8118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://nr.zhonguo1118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://wq.zhonguo6118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ot.zhonguo3118.cn

Java: enum Color { RED, GREEN }
来源：https://gz.zhonguo6118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://tv.zhonguo1118.cn

Ruby: Color = %i[red green].freeze
来源：https://sn.zhonguo5118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://jz.zhonguo6118.cn

[G16] 对象转数组 / 字典
来源：https://bt.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ar.zhonguo4118.cn

PHP:  get_object_vars($obj);
来源：https://gj.zhonguo6118.cn

JS:   Object.entries(obj)
来源：https://sl.zhonguo3118.cn

TS:   Object.entries(obj)
来源：https://qr.zhonguo7118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://tw.zhonguo5118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://po.zhonguo5118.cn

Ruby: obj.instance_variables
来源：https://dp.zhonguo3118.cn

C#:   // 用反射或 System.Text.Json
来源：https://eu.zhonguo8118.cn

================================================================================
来源：https://sq.zhonguo3118.cn

H. 异常与错误处理
来源：https://no.zhonguo6118.cn

================================================================================
来源：https://yb.zhonguo5118.cn

[H01] try / catch 基础
来源：https://kc.zhonguo2118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://tn.zhonguo4118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://ca.zhonguo3118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://jz.zhonguo2118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://hb.zhonguo3118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://jx.zhonguo1118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://vn.zhonguo7118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://uw.zhonguo1118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ot.zhonguo7118.cn

[H02] finally / ensure 收尾
来源：https://tb.zhonguo8118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://yn.zhonguo7118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://yv.zhonguo8118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://vu.zhonguo8118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://od.zhonguo4118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://bd.zhonguo3118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://yp.zhonguo4118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://fd.zhonguo1118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://nv.zhonguo4118.cn

[H03] 主动抛出异常
来源：https://lw.zhonguo1118.cn

Py:   raise ValueError("错误信息")
来源：https://dw.zhonguo8118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://kf.zhonguo3118.cn

JS:   throw new Error("错误信息");
来源：https://iw.zhonguo4118.cn


<!-- 参考信息 -->