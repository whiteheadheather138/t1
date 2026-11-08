代发 wailian999

Go:   if s == "" {}
来源：https://sa.zhonguo6118.cn

Ruby: if s.empty?
来源：https://gi.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://qm.zhonguo1118.cn

[E21] 超长截断加省略号
来源：https://sm.zhonguo6118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://qa.zhonguo2118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://df.zhonguo2118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://yv.zhonguo4118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://qw.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ej.zhonguo3118.cn

Go:   // 按 rune 判断长度后截断
来源：https://xv.zhonguo4118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://ix.zhonguo8118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://yz.zhonguo6118.cn

[E22] 字节长度与字符长度
来源：https://xq.zhonguo5118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://cm.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ny.zhonguo4118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://vl.zhonguo8118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://si.zhonguo4118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://qv.zhonguo6118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://za.zhonguo8118.cn

Ruby: s.bytesize;  s.length
来源：https://al.zhonguo4118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://bo.zhonguo5118.cn

================================================================================
来源：https://zg.zhonguo3118.cn

F. 文件与目录
来源：https://lc.zhonguo1118.cn

================================================================================
来源：https://iv.zhonguo6118.cn

[F01] 读取整个文件
来源：https://hy.zhonguo7118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://tn.zhonguo8118.cn

PHP:  file_get_contents("a.txt");
来源：https://us.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://xg.zhonguo7118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://kv.zhonguo4118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://af.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://xf.zhonguo2118.cn

Ruby: File.read("a.txt")
来源：https://vz.zhonguo4118.cn

C#:   File.ReadAllText("a.txt");
来源：https://nl.zhonguo6118.cn

[F02] 逐行读取文件
来源：https://zh.zhonguo8118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ql.zhonguo6118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://dv.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://pc.zhonguo2118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://pi.zhonguo8118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://fb.zhonguo5118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://xx.zhonguo6118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ud.zhonguo5118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://rn.zhonguo5118.cn

[F03] 写入文件（覆盖）
来源：https://sp.zhonguo8118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://wb.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://ad.zhonguo2118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://hd.zhonguo3118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://il.zhonguo4118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://pa.zhonguo4118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ip.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://vz.zhonguo4118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://ph.zhonguo4118.cn

[F04] 追加写入文件
来源：https://qh.zhonguo7118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ov.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://tg.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://kd.zhonguo5118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ut.zhonguo3118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://xf.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://sq.zhonguo7118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ym.zhonguo1118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://kz.zhonguo1118.cn

[F05] 判断文件或目录是否存在
来源：https://wh.zhonguo1118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://zv.zhonguo5118.cn

PHP:  file_exists("a.txt");
来源：https://jj.zhonguo4118.cn

JS:   fs.existsSync("a.txt")
来源：https://vn.zhonguo7118.cn

TS:   fs.existsSync("a.txt")
来源：https://fe.zhonguo1118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://am.zhonguo6118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://yg.zhonguo3118.cn

Ruby: File.exist?("a.txt")
来源：https://vl.zhonguo5118.cn

C#:   File.Exists("a.txt")
来源：https://mx.zhonguo5118.cn

[F06] 删除文件
来源：https://dz.zhonguo2118.cn

Py:   os.remove("a.txt")
来源：https://mq.zhonguo2118.cn

PHP:  unlink("a.txt");
来源：https://go.zhonguo8118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://nw.zhonguo3118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://hy.zhonguo8118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://jv.zhonguo7118.cn

Go:   os.Remove("a.txt")
来源：https://ma.zhonguo1118.cn

Ruby: File.delete("a.txt")
来源：https://be.zhonguo3118.cn

C#:   File.Delete("a.txt");
来源：https://fs.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://gl.zhonguo6118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://bp.zhonguo5118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://pz.zhonguo7118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://zp.zhonguo5118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://fe.zhonguo5118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://xw.zhonguo4118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://ww.zhonguo5118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://va.zhonguo7118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://bh.zhonguo7118.cn

[F08] 遍历目录
来源：https://rj.zhonguo3118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://se.zhonguo3118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://kd.zhonguo2118.cn

JS:   fs.readdirSync("dir")
来源：https://zi.zhonguo4118.cn

TS:   fs.readdirSync("dir")
来源：https://et.zhonguo5118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://qk.zhonguo5118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://kh.zhonguo3118.cn

Ruby: Dir.children("dir")
来源：https://ui.zhonguo8118.cn

C#:   Directory.GetFiles("dir")
来源：https://cz.zhonguo1118.cn

[F09] 获取文件大小
来源：https://lg.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://vx.zhonguo2118.cn

PHP:  filesize("a.txt");
来源：https://nl.zhonguo8118.cn

JS:   fs.statSync("a.txt").size
来源：https://wf.zhonguo6118.cn

TS:   fs.statSync("a.txt").size
来源：https://sf.zhonguo6118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://by.zhonguo8118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://wd.zhonguo4118.cn

Ruby: File.size("a.txt")
来源：https://hn.zhonguo5118.cn

C#:   new FileInfo("a.txt").Length
来源：https://ga.zhonguo3118.cn

[F10] 取文件扩展名 / 文件名
来源：https://te.zhonguo6118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://wp.zhonguo4118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://db.zhonguo6118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://qk.zhonguo6118.cn

TS:   path.extname("a.txt")
来源：https://xt.zhonguo5118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://cz.zhonguo8118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://ge.zhonguo2118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://yy.zhonguo5118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://ne.zhonguo7118.cn

[F11] 复制与移动文件
来源：https://pw.zhonguo6118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://rz.zhonguo1118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://lr.zhonguo5118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://kz.zhonguo6118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://sf.zhonguo7118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://tf.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://nt.zhonguo6118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://vl.zhonguo7118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://id.zhonguo7118.cn

[F12] CSV 读写
来源：https://af.zhonguo3118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://vj.zhonguo8118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://ka.zhonguo8118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://hy.zhonguo7118.cn

TS:   // 同上
来源：https://lc.zhonguo8118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://id.zhonguo4118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://jm.zhonguo7118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://us.zhonguo2118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://pp.zhonguo2118.cn

================================================================================
来源：https://bl.zhonguo5118.cn

G. 面向对象
来源：https://cd.zhonguo7118.cn

================================================================================
来源：https://df.zhonguo6118.cn

[G01] 定义类
来源：https://ts.zhonguo2118.cn

Py:   class User: pass
来源：https://wh.zhonguo6118.cn

PHP:  class User {}
来源：https://oe.zhonguo2118.cn

JS:   class User {}
来源：https://vw.zhonguo4118.cn

TS:   class User { name: string = ""; }
来源：https://ax.zhonguo7118.cn

Java: class User {}
来源：https://wo.zhonguo4118.cn

Go:   type User struct { Name string }
来源：https://jr.zhonguo8118.cn

Ruby: class User; end
来源：https://tn.zhonguo7118.cn

C#:   class User {}
来源：https://zv.zhonguo7118.cn

[G02] 构造函数
来源：https://ux.zhonguo8118.cn

Py:   def __init__(self, name): self.name = name
来源：https://wq.zhonguo2118.cn

PHP:  public function __construct(public string $name) {}
来源：https://bd.zhonguo2118.cn

JS:   constructor(name) { this.name = name; }
来源：https://jf.zhonguo6118.cn

TS:   constructor(public name: string) {}
来源：https://fx.zhonguo6118.cn

Java: User(String name) { this.name = name; }
来源：https://ua.zhonguo7118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://yd.zhonguo5118.cn

Ruby: def initialize(name); @name = name; end
来源：https://eb.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://jq.zhonguo1118.cn

[G03] 实例属性
来源：https://ll.zhonguo1118.cn

Py:   self.name = "x"
来源：https://vr.zhonguo8118.cn

PHP:  public string $name = "x";
来源：https://sy.zhonguo8118.cn

JS:   this.name = "x";
来源：https://cn.zhonguo1118.cn

TS:   name: string = "x";
来源：https://sf.zhonguo7118.cn

Java: private String name;
来源：https://sw.zhonguo4118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://ha.zhonguo2118.cn

Ruby: @name = "x"
来源：https://nc.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://ef.zhonguo1118.cn

[G04] 定义方法
来源：https://wb.zhonguo4118.cn

Py:   def greet(self): return self.name
来源：https://bu.zhonguo1118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://km.zhonguo6118.cn

JS:   greet() { return this.name; }
来源：https://oj.zhonguo8118.cn

TS:   greet(): string { return this.name; }
来源：https://bm.zhonguo5118.cn

Java: String greet() { return name; }
来源：https://na.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://ik.zhonguo3118.cn

Ruby: def greet; @name; end
来源：https://dl.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://be.zhonguo7118.cn

[G05] 继承
来源：https://pi.zhonguo3118.cn

Py:   class Admin(User): pass
来源：https://pl.zhonguo1118.cn

PHP:  class Admin extends User {}
来源：https://ji.zhonguo2118.cn

JS:   class Admin extends User {}
来源：https://ec.zhonguo5118.cn

TS:   class Admin extends User {}
来源：https://ay.zhonguo6118.cn

Java: class Admin extends User {}
来源：https://is.zhonguo6118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://ka.zhonguo3118.cn

Ruby: class Admin < User; end
来源：https://vw.zhonguo7118.cn

C#:   class Admin : User {}
来源：https://gm.zhonguo5118.cn

[G06] 重写方法
来源：https://gd.zhonguo5118.cn

Py:   def greet(self): return "admin"
来源：https://pb.zhonguo2118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://zs.zhonguo6118.cn

JS:   greet() { return "admin"; }
来源：https://yw.zhonguo6118.cn

TS:   greet(): string { return "admin"; }
来源：https://ar.zhonguo7118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ru.zhonguo5118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://gd.zhonguo8118.cn

Ruby: def greet; "admin"; end
来源：https://sq.zhonguo5118.cn

C#:   public override string Greet() => "admin";
来源：https://aw.zhonguo3118.cn

[G07] 调用父类方法
来源：https://xf.zhonguo2118.cn

Py:   super().greet()
来源：https://kk.zhonguo2118.cn

PHP:  parent::greet();
来源：https://jx.zhonguo3118.cn

JS:   super.greet();
来源：https://dy.zhonguo4118.cn

TS:   super.greet();
来源：https://ea.zhonguo6118.cn

Java: super.greet();
来源：https://no.zhonguo1118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://zm.zhonguo1118.cn

Ruby: super
来源：https://on.zhonguo5118.cn

C#:   base.Greet();
来源：https://xw.zhonguo5118.cn

[G08] 静态方法与属性
来源：https://lr.zhonguo8118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://zx.zhonguo8118.cn

PHP:  public static function f() {}
来源：https://pe.zhonguo4118.cn

JS:   static f() {}
来源：https://vg.zhonguo6118.cn

TS:   static f(): void {}
来源：https://vn.zhonguo1118.cn

Java: static void f() {}
来源：https://qk.zhonguo2118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://jq.zhonguo3118.cn

Ruby: def self.f; end
来源：https://jh.zhonguo2118.cn

C#:   public static void F() {}
来源：https://zb.zhonguo1118.cn

[G09] 接口 / 抽象类
来源：https://qb.zhonguo2118.cn

Py:   from abc import ABC, abstractmethod
来源：https://xn.zhonguo6118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://ow.zhonguo8118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://lh.zhonguo4118.cn

TS:   interface Shape { area(): number; }
来源：https://id.zhonguo3118.cn

Java: interface Shape { double area(); }
来源：https://ec.zhonguo8118.cn

Go:   type Shape interface { Area() float64 }
来源：https://vu.zhonguo5118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://it.zhonguo6118.cn

C#:   interface IShape { double Area(); }
来源：https://vf.zhonguo4118.cn

[G10] 访问控制
来源：https://qu.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://wz.zhonguo6118.cn

PHP:  public / protected / private
来源：https://yw.zhonguo6118.cn

JS:   #private 字段；其余公开
来源：https://tc.zhonguo3118.cn

TS:   public / protected / private
来源：https://pz.zhonguo6118.cn

Java: public / protected / private / 默认包级
来源：https://aq.zhonguo8118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://pp.zhonguo8118.cn

Ruby: public / protected / private
来源：https://bw.zhonguo8118.cn

C#:   public / protected / private / internal
来源：https://at.zhonguo8118.cn

[G11] getter / setter
来源：https://tu.zhonguo3118.cn

Py:   @property 与 @x.setter
来源：https://bd.zhonguo5118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://gl.zhonguo2118.cn

JS:   get name() { return this._name; }
来源：https://oz.zhonguo7118.cn

TS:   get name(): string { return this._name; }
来源：https://vy.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://fl.zhonguo7118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://vl.zhonguo4118.cn

Ruby: attr_accessor :name
来源：https://sj.zhonguo3118.cn

C#:   public string Name { get; set; }
来源：https://tx.zhonguo8118.cn

[G12] 对象转字符串
来源：https://xp.zhonguo3118.cn

Py:   def __str__(self): return self.name
来源：https://pe.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://rw.zhonguo8118.cn

JS:   toString() { return this.name; }
来源：https://qk.zhonguo4118.cn

TS:   toString(): string { return this.name; }
来源：https://on.zhonguo2118.cn

Java: @Override public String toString() { return name; }
来源：https://cc.zhonguo3118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://wv.zhonguo1118.cn

Ruby: def to_s; @name; end
来源：https://la.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://av.zhonguo5118.cn

[G13] 判断对象类型
来源：https://ar.zhonguo4118.cn

Py:   isinstance(u, User)
来源：https://bx.zhonguo3118.cn

PHP:  $u instanceof User
来源：https://yh.zhonguo6118.cn

JS:   u instanceof User
来源：https://hd.zhonguo3118.cn

TS:   u instanceof User
来源：https://ze.zhonguo4118.cn

Java: u instanceof User
来源：https://kn.zhonguo6118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://vx.zhonguo7118.cn

Ruby: u.is_a?(User)
来源：https://zk.zhonguo3118.cn

C#:   u is User
来源：https://uo.zhonguo8118.cn

[G14] 数据类 / record
来源：https://qp.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://kz.zhonguo1118.cn

PHP:  // 用 readonly 属性模拟
来源：https://vd.zhonguo3118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://om.zhonguo3118.cn

TS:   type User = { name: string; age: number };
来源：https://wv.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://fw.zhonguo3118.cn

Go:   type User struct { Name string; Age int }
来源：https://kp.zhonguo3118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://rl.zhonguo2118.cn

C#:   record User(string Name, int Age);
来源：https://ha.zhonguo3118.cn

[G15] 枚举
来源：https://wa.zhonguo2118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://hk.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://lg.zhonguo5118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://fq.zhonguo7118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://oq.zhonguo2118.cn

Java: enum Color { RED, GREEN }
来源：https://zd.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://tt.zhonguo7118.cn

Ruby: Color = %i[red green].freeze
来源：https://oz.zhonguo8118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://uj.zhonguo3118.cn

[G16] 对象转数组 / 字典
来源：https://lo.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://bs.zhonguo2118.cn

PHP:  get_object_vars($obj);
来源：https://wb.zhonguo2118.cn

JS:   Object.entries(obj)
来源：https://ui.zhonguo5118.cn

TS:   Object.entries(obj)
来源：https://cw.zhonguo7118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://ys.zhonguo4118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://es.zhonguo4118.cn

Ruby: obj.instance_variables
来源：https://qt.zhonguo5118.cn

C#:   // 用反射或 System.Text.Json
来源：https://hm.zhonguo6118.cn

================================================================================
来源：https://qe.zhonguo1118.cn

H. 异常与错误处理
来源：https://ih.zhonguo6118.cn

================================================================================
来源：https://tm.zhonguo3118.cn

[H01] try / catch 基础
来源：https://xa.zhonguo8118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://lc.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://ig.zhonguo6118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://br.zhonguo1118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://jk.zhonguo6118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://ye.zhonguo6118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://gm.zhonguo6118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://lo.zhonguo5118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://uv.zhonguo4118.cn

[H02] finally / ensure 收尾
来源：https://ds.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://fc.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://hs.zhonguo7118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://eb.zhonguo4118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://jz.zhonguo7118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://dw.zhonguo2118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ae.zhonguo2118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://nr.zhonguo5118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://zb.zhonguo1118.cn


<!-- 参考信息 -->