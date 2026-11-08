代发 wailian999

JS:   s.split(/\r?\n/)
来源：https://fj.zhonguo8118.cn

TS:   s.split(/\r?\n/)
来源：https://su.zhonguo1118.cn

Java: s.lines().toList()
来源：https://iz.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://ak.zhonguo1118.cn

Ruby: s.lines
来源：https://oz.zhonguo2118.cn

C#:   s.Split('\n')
来源：https://ld.zhonguo1118.cn

[E20] 判断字符串是否为空
来源：https://pn.zhonguo4118.cn

Py:   if not s:
来源：https://gu.zhonguo3118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://jh.zhonguo3118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ah.zhonguo1118.cn

TS:   if (s === "") {}
来源：https://pw.zhonguo2118.cn

Java: if (s.isEmpty()) {}
来源：https://fj.zhonguo1118.cn

Go:   if s == "" {}
来源：https://nj.zhonguo4118.cn

Ruby: if s.empty?
来源：https://jj.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://xp.zhonguo3118.cn

[E21] 超长截断加省略号
来源：https://bb.zhonguo1118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://ag.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://fl.zhonguo1118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://jr.zhonguo5118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://jx.zhonguo5118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://uv.zhonguo4118.cn

Go:   // 按 rune 判断长度后截断
来源：https://pi.zhonguo6118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://hp.zhonguo8118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://ys.zhonguo5118.cn

[E22] 字节长度与字符长度
来源：https://iv.zhonguo2118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://ym.zhonguo8118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ic.zhonguo3118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://yf.zhonguo2118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://fc.zhonguo8118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://rg.zhonguo5118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://ss.zhonguo7118.cn

Ruby: s.bytesize;  s.length
来源：https://hi.zhonguo6118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://zq.zhonguo4118.cn

================================================================================
来源：https://fi.zhonguo2118.cn

F. 文件与目录
来源：https://ya.zhonguo6118.cn

================================================================================
来源：https://co.zhonguo7118.cn

[F01] 读取整个文件
来源：https://us.zhonguo2118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://ic.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://iz.zhonguo7118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://dt.zhonguo5118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://wm.zhonguo4118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ar.zhonguo6118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://xg.zhonguo4118.cn

Ruby: File.read("a.txt")
来源：https://fb.zhonguo6118.cn

C#:   File.ReadAllText("a.txt");
来源：https://vd.zhonguo6118.cn

[F02] 逐行读取文件
来源：https://tt.zhonguo6118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://wd.zhonguo8118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://gl.zhonguo2118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://qf.zhonguo4118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://kw.zhonguo2118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://zg.zhonguo7118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://fz.zhonguo6118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://bq.zhonguo2118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://om.zhonguo1118.cn

[F03] 写入文件（覆盖）
来源：https://bz.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://va.zhonguo1118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://kx.zhonguo1118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://hh.zhonguo3118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://dm.zhonguo4118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://qa.zhonguo7118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ew.zhonguo5118.cn

Ruby: File.write("a.txt", "hi")
来源：https://dt.zhonguo5118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://ab.zhonguo4118.cn

[F04] 追加写入文件
来源：https://sa.zhonguo4118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://pq.zhonguo6118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://po.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://al.zhonguo8118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://zp.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://ba.zhonguo7118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://xt.zhonguo7118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://qu.zhonguo7118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://dh.zhonguo8118.cn

[F05] 判断文件或目录是否存在
来源：https://lu.zhonguo5118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ap.zhonguo1118.cn

PHP:  file_exists("a.txt");
来源：https://xj.zhonguo7118.cn

JS:   fs.existsSync("a.txt")
来源：https://vy.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://zf.zhonguo6118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://vs.zhonguo4118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://wk.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://vm.zhonguo1118.cn

C#:   File.Exists("a.txt")
来源：https://ku.zhonguo4118.cn

[F06] 删除文件
来源：https://hh.zhonguo4118.cn

Py:   os.remove("a.txt")
来源：https://uh.zhonguo8118.cn

PHP:  unlink("a.txt");
来源：https://yw.zhonguo7118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://on.zhonguo2118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://hr.zhonguo3118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://zr.zhonguo5118.cn

Go:   os.Remove("a.txt")
来源：https://oq.zhonguo3118.cn

Ruby: File.delete("a.txt")
来源：https://mi.zhonguo2118.cn

C#:   File.Delete("a.txt");
来源：https://wq.zhonguo8118.cn

[F07] 创建目录（含多级）
来源：https://fc.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://ww.zhonguo2118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://pr.zhonguo6118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://vh.zhonguo1118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://zh.zhonguo4118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://ww.zhonguo6118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://vf.zhonguo3118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://gd.zhonguo8118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://bw.zhonguo5118.cn

[F08] 遍历目录
来源：https://xu.zhonguo1118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ed.zhonguo6118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://uk.zhonguo3118.cn

JS:   fs.readdirSync("dir")
来源：https://qw.zhonguo6118.cn

TS:   fs.readdirSync("dir")
来源：https://vs.zhonguo3118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://bu.zhonguo2118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://xh.zhonguo1118.cn

Ruby: Dir.children("dir")
来源：https://gh.zhonguo1118.cn

C#:   Directory.GetFiles("dir")
来源：https://gt.zhonguo1118.cn

[F09] 获取文件大小
来源：https://ja.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://gl.zhonguo8118.cn

PHP:  filesize("a.txt");
来源：https://pv.zhonguo2118.cn

JS:   fs.statSync("a.txt").size
来源：https://lt.zhonguo6118.cn

TS:   fs.statSync("a.txt").size
来源：https://df.zhonguo2118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://uq.zhonguo4118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://cs.zhonguo3118.cn

Ruby: File.size("a.txt")
来源：https://ps.zhonguo6118.cn

C#:   new FileInfo("a.txt").Length
来源：https://nx.zhonguo8118.cn

[F10] 取文件扩展名 / 文件名
来源：https://nb.zhonguo8118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://en.zhonguo2118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://hb.zhonguo8118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://fd.zhonguo5118.cn

TS:   path.extname("a.txt")
来源：https://hx.zhonguo6118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://vm.zhonguo8118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://ic.zhonguo5118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://bh.zhonguo8118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://zj.zhonguo7118.cn

[F11] 复制与移动文件
来源：https://hy.zhonguo8118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://st.zhonguo3118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ie.zhonguo5118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://hn.zhonguo8118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://rr.zhonguo4118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://io.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ia.zhonguo5118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://cs.zhonguo8118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://nu.zhonguo7118.cn

[F12] CSV 读写
来源：https://tv.zhonguo8118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://xh.zhonguo1118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://jk.zhonguo2118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://kj.zhonguo5118.cn

TS:   // 同上
来源：https://gm.zhonguo4118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://dq.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://ti.zhonguo1118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://ix.zhonguo1118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://uv.zhonguo5118.cn

================================================================================
来源：https://fe.zhonguo1118.cn

G. 面向对象
来源：https://pd.zhonguo6118.cn

================================================================================
来源：https://jz.zhonguo4118.cn

[G01] 定义类
来源：https://sn.zhonguo8118.cn

Py:   class User: pass
来源：https://ll.zhonguo6118.cn

PHP:  class User {}
来源：https://vc.zhonguo2118.cn

JS:   class User {}
来源：https://jl.zhonguo5118.cn

TS:   class User { name: string = ""; }
来源：https://xt.zhonguo2118.cn

Java: class User {}
来源：https://gt.zhonguo3118.cn

Go:   type User struct { Name string }
来源：https://pg.zhonguo7118.cn

Ruby: class User; end
来源：https://kb.zhonguo7118.cn

C#:   class User {}
来源：https://fv.zhonguo2118.cn

[G02] 构造函数
来源：https://sp.zhonguo7118.cn

Py:   def __init__(self, name): self.name = name
来源：https://hr.zhonguo6118.cn

PHP:  public function __construct(public string $name) {}
来源：https://ag.zhonguo6118.cn

JS:   constructor(name) { this.name = name; }
来源：https://be.zhonguo7118.cn

TS:   constructor(public name: string) {}
来源：https://rm.zhonguo4118.cn

Java: User(String name) { this.name = name; }
来源：https://kc.zhonguo7118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://ut.zhonguo3118.cn

Ruby: def initialize(name); @name = name; end
来源：https://xo.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://qn.zhonguo1118.cn

[G03] 实例属性
来源：https://bv.zhonguo3118.cn

Py:   self.name = "x"
来源：https://gp.zhonguo5118.cn

PHP:  public string $name = "x";
来源：https://mu.zhonguo6118.cn

JS:   this.name = "x";
来源：https://ne.zhonguo6118.cn

TS:   name: string = "x";
来源：https://ac.zhonguo7118.cn

Java: private String name;
来源：https://mg.zhonguo8118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://ib.zhonguo7118.cn

Ruby: @name = "x"
来源：https://db.zhonguo8118.cn

C#:   public string Name { get; set; } = "x";
来源：https://nr.zhonguo6118.cn

[G04] 定义方法
来源：https://ex.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://lr.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://nh.zhonguo5118.cn

JS:   greet() { return this.name; }
来源：https://hn.zhonguo1118.cn

TS:   greet(): string { return this.name; }
来源：https://qr.zhonguo6118.cn

Java: String greet() { return name; }
来源：https://wb.zhonguo4118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://te.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://qw.zhonguo8118.cn

C#:   public string Greet() => Name;
来源：https://zb.zhonguo6118.cn

[G05] 继承
来源：https://ud.zhonguo1118.cn

Py:   class Admin(User): pass
来源：https://le.zhonguo5118.cn

PHP:  class Admin extends User {}
来源：https://wt.zhonguo6118.cn

JS:   class Admin extends User {}
来源：https://on.zhonguo5118.cn

TS:   class Admin extends User {}
来源：https://br.zhonguo4118.cn

Java: class Admin extends User {}
来源：https://mp.zhonguo2118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://vu.zhonguo7118.cn

Ruby: class Admin < User; end
来源：https://iz.zhonguo7118.cn

C#:   class Admin : User {}
来源：https://tp.zhonguo4118.cn

[G06] 重写方法
来源：https://cp.zhonguo2118.cn

Py:   def greet(self): return "admin"
来源：https://hg.zhonguo5118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ex.zhonguo3118.cn

JS:   greet() { return "admin"; }
来源：https://ma.zhonguo3118.cn

TS:   greet(): string { return "admin"; }
来源：https://ps.zhonguo5118.cn

Java: @Override String greet() { return "admin"; }
来源：https://zo.zhonguo8118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://ky.zhonguo2118.cn

Ruby: def greet; "admin"; end
来源：https://fw.zhonguo5118.cn

C#:   public override string Greet() => "admin";
来源：https://lo.zhonguo3118.cn

[G07] 调用父类方法
来源：https://yd.zhonguo2118.cn

Py:   super().greet()
来源：https://ah.zhonguo6118.cn

PHP:  parent::greet();
来源：https://df.zhonguo6118.cn

JS:   super.greet();
来源：https://yl.zhonguo5118.cn

TS:   super.greet();
来源：https://ry.zhonguo6118.cn

Java: super.greet();
来源：https://rg.zhonguo3118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://gb.zhonguo6118.cn

Ruby: super
来源：https://eo.zhonguo1118.cn

C#:   base.Greet();
来源：https://mx.zhonguo8118.cn

[G08] 静态方法与属性
来源：https://cp.zhonguo8118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://co.zhonguo8118.cn

PHP:  public static function f() {}
来源：https://ls.zhonguo7118.cn

JS:   static f() {}
来源：https://lc.zhonguo4118.cn

TS:   static f(): void {}
来源：https://qq.zhonguo1118.cn

Java: static void f() {}
来源：https://bn.zhonguo2118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://ci.zhonguo5118.cn

Ruby: def self.f; end
来源：https://kl.zhonguo4118.cn

C#:   public static void F() {}
来源：https://tk.zhonguo7118.cn

[G09] 接口 / 抽象类
来源：https://ne.zhonguo2118.cn

Py:   from abc import ABC, abstractmethod
来源：https://gv.zhonguo1118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://za.zhonguo8118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://dy.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://dx.zhonguo2118.cn

Java: interface Shape { double area(); }
来源：https://qz.zhonguo7118.cn

Go:   type Shape interface { Area() float64 }
来源：https://ba.zhonguo4118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://sp.zhonguo8118.cn

C#:   interface IShape { double Area(); }
来源：https://ee.zhonguo4118.cn

[G10] 访问控制
来源：https://ec.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://jp.zhonguo8118.cn

PHP:  public / protected / private
来源：https://qs.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://kv.zhonguo8118.cn

TS:   public / protected / private
来源：https://hd.zhonguo6118.cn

Java: public / protected / private / 默认包级
来源：https://eg.zhonguo3118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://gf.zhonguo6118.cn

Ruby: public / protected / private
来源：https://er.zhonguo5118.cn

C#:   public / protected / private / internal
来源：https://jp.zhonguo6118.cn

[G11] getter / setter
来源：https://fi.zhonguo1118.cn

Py:   @property 与 @x.setter
来源：https://fc.zhonguo6118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://vb.zhonguo7118.cn

JS:   get name() { return this._name; }
来源：https://wd.zhonguo6118.cn

TS:   get name(): string { return this._name; }
来源：https://ez.zhonguo6118.cn

Java: public String getName() { return name; }
来源：https://co.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://rh.zhonguo2118.cn

Ruby: attr_accessor :name
来源：https://ts.zhonguo1118.cn

C#:   public string Name { get; set; }
来源：https://wh.zhonguo6118.cn

[G12] 对象转字符串
来源：https://di.zhonguo2118.cn

Py:   def __str__(self): return self.name
来源：https://ii.zhonguo7118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://uw.zhonguo6118.cn

JS:   toString() { return this.name; }
来源：https://bf.zhonguo5118.cn

TS:   toString(): string { return this.name; }
来源：https://ox.zhonguo7118.cn

Java: @Override public String toString() { return name; }
来源：https://bh.zhonguo7118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://gv.zhonguo1118.cn

Ruby: def to_s; @name; end
来源：https://xg.zhonguo7118.cn

C#:   public override string ToString() => Name;
来源：https://ft.zhonguo3118.cn

[G13] 判断对象类型
来源：https://ju.zhonguo4118.cn

Py:   isinstance(u, User)
来源：https://ht.zhonguo7118.cn

PHP:  $u instanceof User
来源：https://fb.zhonguo1118.cn

JS:   u instanceof User
来源：https://je.zhonguo4118.cn

TS:   u instanceof User
来源：https://if.zhonguo1118.cn

Java: u instanceof User
来源：https://wo.zhonguo5118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://xl.zhonguo4118.cn

Ruby: u.is_a?(User)
来源：https://ne.zhonguo8118.cn

C#:   u is User
来源：https://cb.zhonguo4118.cn

[G14] 数据类 / record
来源：https://jc.zhonguo8118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://mf.zhonguo7118.cn

PHP:  // 用 readonly 属性模拟
来源：https://rc.zhonguo7118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ti.zhonguo4118.cn

TS:   type User = { name: string; age: number };
来源：https://fb.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://rj.zhonguo3118.cn

Go:   type User struct { Name string; Age int }
来源：https://pk.zhonguo5118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://ya.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://sv.zhonguo6118.cn

[G15] 枚举
来源：https://ig.zhonguo1118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ll.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://fa.zhonguo4118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://uc.zhonguo8118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ip.zhonguo3118.cn

Java: enum Color { RED, GREEN }
来源：https://et.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://fq.zhonguo1118.cn

Ruby: Color = %i[red green].freeze
来源：https://sg.zhonguo1118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://au.zhonguo2118.cn

[G16] 对象转数组 / 字典
来源：https://tg.zhonguo5118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://rx.zhonguo6118.cn

PHP:  get_object_vars($obj);
来源：https://zf.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://po.zhonguo3118.cn

TS:   Object.entries(obj)
来源：https://bi.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://oj.zhonguo8118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://sz.zhonguo7118.cn

Ruby: obj.instance_variables
来源：https://bj.zhonguo1118.cn

C#:   // 用反射或 System.Text.Json
来源：https://al.zhonguo8118.cn

================================================================================
来源：https://tc.zhonguo6118.cn

H. 异常与错误处理
来源：https://rl.zhonguo8118.cn

================================================================================
来源：https://gy.zhonguo2118.cn

[H01] try / catch 基础
来源：https://dz.zhonguo5118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://uh.zhonguo7118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://vj.zhonguo8118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://ao.zhonguo4118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://sz.zhonguo7118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://kb.zhonguo5118.cn


<!-- 参考信息 -->