代发 wailian999

JS:   s.split(/\r?\n/)
来源：https://ri.zhonguo2118.cn

TS:   s.split(/\r?\n/)
来源：https://hy.zhonguo8118.cn

Java: s.lines().toList()
来源：https://ni.zhonguo6118.cn

Go:   strings.Split(s, "\n")
来源：https://cf.zhonguo1118.cn

Ruby: s.lines
来源：https://pm.zhonguo3118.cn

C#:   s.Split('\n')
来源：https://yh.zhonguo7118.cn

[E20] 判断字符串是否为空
来源：https://bd.zhonguo5118.cn

Py:   if not s:
来源：https://ez.zhonguo3118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://pi.zhonguo6118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://nn.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://dd.zhonguo6118.cn

Java: if (s.isEmpty()) {}
来源：https://lo.zhonguo4118.cn

Go:   if s == "" {}
来源：https://ly.zhonguo8118.cn

Ruby: if s.empty?
来源：https://uf.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://bt.zhonguo2118.cn

[E21] 超长截断加省略号
来源：https://be.zhonguo4118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://ci.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://il.zhonguo6118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ij.zhonguo2118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://xx.zhonguo8118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ve.zhonguo7118.cn

Go:   // 按 rune 判断长度后截断
来源：https://nb.zhonguo6118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://sr.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://tb.zhonguo6118.cn

[E22] 字节长度与字符长度
来源：https://yf.zhonguo8118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://fw.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ax.zhonguo7118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://vq.zhonguo1118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://nm.zhonguo4118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://lm.zhonguo3118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://xd.zhonguo6118.cn

Ruby: s.bytesize;  s.length
来源：https://cc.zhonguo2118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://xo.zhonguo3118.cn

================================================================================
来源：https://yi.zhonguo6118.cn

F. 文件与目录
来源：https://oh.zhonguo2118.cn

================================================================================
来源：https://jp.zhonguo8118.cn

[F01] 读取整个文件
来源：https://ln.zhonguo1118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://xh.zhonguo5118.cn

PHP:  file_get_contents("a.txt");
来源：https://xf.zhonguo1118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://bc.zhonguo3118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://in.zhonguo5118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://gh.zhonguo7118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://yp.zhonguo7118.cn

Ruby: File.read("a.txt")
来源：https://bf.zhonguo3118.cn

C#:   File.ReadAllText("a.txt");
来源：https://fy.zhonguo1118.cn

[F02] 逐行读取文件
来源：https://sw.zhonguo1118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://bp.zhonguo2118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://ne.zhonguo3118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://mh.zhonguo4118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://en.zhonguo4118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://yi.zhonguo1118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://id.zhonguo7118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ex.zhonguo6118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ud.zhonguo6118.cn

[F03] 写入文件（覆盖）
来源：https://io.zhonguo7118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://sl.zhonguo8118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://bs.zhonguo6118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ka.zhonguo2118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://wd.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://wg.zhonguo5118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://gf.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://uz.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://dn.zhonguo3118.cn

[F04] 追加写入文件
来源：https://vk.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://yf.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://je.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://mn.zhonguo4118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://kk.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://cg.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://au.zhonguo2118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ds.zhonguo3118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://ge.zhonguo2118.cn

[F05] 判断文件或目录是否存在
来源：https://oq.zhonguo6118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://tn.zhonguo5118.cn

PHP:  file_exists("a.txt");
来源：https://bv.zhonguo3118.cn

JS:   fs.existsSync("a.txt")
来源：https://nw.zhonguo1118.cn

TS:   fs.existsSync("a.txt")
来源：https://ft.zhonguo4118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://wy.zhonguo8118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://jd.zhonguo6118.cn

Ruby: File.exist?("a.txt")
来源：https://em.zhonguo3118.cn

C#:   File.Exists("a.txt")
来源：https://ix.zhonguo8118.cn

[F06] 删除文件
来源：https://hu.zhonguo3118.cn

Py:   os.remove("a.txt")
来源：https://wv.zhonguo5118.cn

PHP:  unlink("a.txt");
来源：https://fh.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://ca.zhonguo1118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://cq.zhonguo2118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://lc.zhonguo2118.cn

Go:   os.Remove("a.txt")
来源：https://pk.zhonguo7118.cn

Ruby: File.delete("a.txt")
来源：https://oo.zhonguo6118.cn

C#:   File.Delete("a.txt");
来源：https://ry.zhonguo5118.cn

[F07] 创建目录（含多级）
来源：https://vg.zhonguo2118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://nx.zhonguo4118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://oi.zhonguo4118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://fg.zhonguo4118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://hw.zhonguo1118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://rt.zhonguo6118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://eg.zhonguo1118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://tc.zhonguo5118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://mq.zhonguo5118.cn

[F08] 遍历目录
来源：https://st.zhonguo6118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://aq.zhonguo1118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://au.zhonguo7118.cn

JS:   fs.readdirSync("dir")
来源：https://bd.zhonguo7118.cn

TS:   fs.readdirSync("dir")
来源：https://hy.zhonguo4118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://hk.zhonguo8118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://ob.zhonguo4118.cn

Ruby: Dir.children("dir")
来源：https://tf.zhonguo2118.cn

C#:   Directory.GetFiles("dir")
来源：https://gz.zhonguo8118.cn

[F09] 获取文件大小
来源：https://hm.zhonguo1118.cn

Py:   os.path.getsize("a.txt")
来源：https://xl.zhonguo1118.cn

PHP:  filesize("a.txt");
来源：https://fo.zhonguo3118.cn

JS:   fs.statSync("a.txt").size
来源：https://rd.zhonguo6118.cn

TS:   fs.statSync("a.txt").size
来源：https://os.zhonguo4118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://dr.zhonguo3118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://sn.zhonguo8118.cn

Ruby: File.size("a.txt")
来源：https://ye.zhonguo3118.cn

C#:   new FileInfo("a.txt").Length
来源：https://my.zhonguo8118.cn

[F10] 取文件扩展名 / 文件名
来源：https://dn.zhonguo7118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://uq.zhonguo5118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://wm.zhonguo3118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://vm.zhonguo2118.cn

TS:   path.extname("a.txt")
来源：https://pf.zhonguo3118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://mk.zhonguo1118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://ec.zhonguo1118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://nt.zhonguo3118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://qk.zhonguo2118.cn

[F11] 复制与移动文件
来源：https://gd.zhonguo6118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://rx.zhonguo6118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://vg.zhonguo7118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://rw.zhonguo5118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://vq.zhonguo2118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://aj.zhonguo7118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://pm.zhonguo8118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://fp.zhonguo1118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ir.zhonguo8118.cn

[F12] CSV 读写
来源：https://io.zhonguo8118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://gl.zhonguo6118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://zn.zhonguo2118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://lf.zhonguo3118.cn

TS:   // 同上
来源：https://yw.zhonguo8118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://an.zhonguo6118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://un.zhonguo5118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://gx.zhonguo5118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://qf.zhonguo8118.cn

================================================================================
来源：https://lz.zhonguo4118.cn

G. 面向对象
来源：https://ei.zhonguo7118.cn

================================================================================
来源：https://gi.zhonguo3118.cn

[G01] 定义类
来源：https://jm.zhonguo4118.cn

Py:   class User: pass
来源：https://fg.zhonguo3118.cn

PHP:  class User {}
来源：https://ik.zhonguo2118.cn

JS:   class User {}
来源：https://dv.zhonguo6118.cn

TS:   class User { name: string = ""; }
来源：https://pk.zhonguo6118.cn

Java: class User {}
来源：https://vy.zhonguo1118.cn

Go:   type User struct { Name string }
来源：https://hn.zhonguo3118.cn

Ruby: class User; end
来源：https://sc.zhonguo7118.cn

C#:   class User {}
来源：https://ak.zhonguo5118.cn

[G02] 构造函数
来源：https://au.zhonguo8118.cn

Py:   def __init__(self, name): self.name = name
来源：https://ww.zhonguo3118.cn

PHP:  public function __construct(public string $name) {}
来源：https://de.zhonguo5118.cn

JS:   constructor(name) { this.name = name; }
来源：https://xd.zhonguo5118.cn

TS:   constructor(public name: string) {}
来源：https://sb.zhonguo2118.cn

Java: User(String name) { this.name = name; }
来源：https://kf.zhonguo4118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://fx.zhonguo6118.cn

Ruby: def initialize(name); @name = name; end
来源：https://jf.zhonguo2118.cn

C#:   public User(string name) { Name = name; }
来源：https://ib.zhonguo5118.cn

[G03] 实例属性
来源：https://at.zhonguo3118.cn

Py:   self.name = "x"
来源：https://il.zhonguo1118.cn

PHP:  public string $name = "x";
来源：https://xi.zhonguo6118.cn

JS:   this.name = "x";
来源：https://lt.zhonguo1118.cn

TS:   name: string = "x";
来源：https://bw.zhonguo8118.cn

Java: private String name;
来源：https://pe.zhonguo2118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://ah.zhonguo8118.cn

Ruby: @name = "x"
来源：https://sm.zhonguo2118.cn

C#:   public string Name { get; set; } = "x";
来源：https://jl.zhonguo2118.cn

[G04] 定义方法
来源：https://sx.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://dd.zhonguo6118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://vk.zhonguo4118.cn

JS:   greet() { return this.name; }
来源：https://xy.zhonguo3118.cn

TS:   greet(): string { return this.name; }
来源：https://gd.zhonguo6118.cn

Java: String greet() { return name; }
来源：https://dw.zhonguo1118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://jx.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://my.zhonguo8118.cn

C#:   public string Greet() => Name;
来源：https://oe.zhonguo5118.cn

[G05] 继承
来源：https://em.zhonguo2118.cn

Py:   class Admin(User): pass
来源：https://eb.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://vz.zhonguo8118.cn

JS:   class Admin extends User {}
来源：https://th.zhonguo6118.cn

TS:   class Admin extends User {}
来源：https://hf.zhonguo4118.cn

Java: class Admin extends User {}
来源：https://ev.zhonguo1118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://oc.zhonguo8118.cn

Ruby: class Admin < User; end
来源：https://pr.zhonguo4118.cn

C#:   class Admin : User {}
来源：https://fn.zhonguo5118.cn

[G06] 重写方法
来源：https://cf.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://ig.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://fh.zhonguo7118.cn

JS:   greet() { return "admin"; }
来源：https://uq.zhonguo5118.cn

TS:   greet(): string { return "admin"; }
来源：https://yx.zhonguo2118.cn

Java: @Override String greet() { return "admin"; }
来源：https://lu.zhonguo8118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://vw.zhonguo4118.cn

Ruby: def greet; "admin"; end
来源：https://br.zhonguo3118.cn

C#:   public override string Greet() => "admin";
来源：https://wx.zhonguo3118.cn

[G07] 调用父类方法
来源：https://rv.zhonguo1118.cn

Py:   super().greet()
来源：https://qe.zhonguo6118.cn

PHP:  parent::greet();
来源：https://mm.zhonguo5118.cn

JS:   super.greet();
来源：https://ai.zhonguo8118.cn

TS:   super.greet();
来源：https://eu.zhonguo5118.cn

Java: super.greet();
来源：https://ms.zhonguo7118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://ex.zhonguo5118.cn

Ruby: super
来源：https://ko.zhonguo5118.cn

C#:   base.Greet();
来源：https://rh.zhonguo2118.cn

[G08] 静态方法与属性
来源：https://mn.zhonguo5118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://ov.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://jk.zhonguo4118.cn

JS:   static f() {}
来源：https://zm.zhonguo3118.cn

TS:   static f(): void {}
来源：https://hv.zhonguo2118.cn

Java: static void f() {}
来源：https://ik.zhonguo5118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://wa.zhonguo5118.cn

Ruby: def self.f; end
来源：https://ki.zhonguo4118.cn

C#:   public static void F() {}
来源：https://vh.zhonguo2118.cn

[G09] 接口 / 抽象类
来源：https://gb.zhonguo8118.cn

Py:   from abc import ABC, abstractmethod
来源：https://bz.zhonguo7118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://fz.zhonguo7118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://gx.zhonguo4118.cn

TS:   interface Shape { area(): number; }
来源：https://lp.zhonguo5118.cn

Java: interface Shape { double area(); }
来源：https://fr.zhonguo3118.cn

Go:   type Shape interface { Area() float64 }
来源：https://sc.zhonguo6118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://uk.zhonguo6118.cn

C#:   interface IShape { double Area(); }
来源：https://ff.zhonguo7118.cn

[G10] 访问控制
来源：https://mq.zhonguo5118.cn

Py:   约定 _protected / __private（不强制）
来源：https://iv.zhonguo3118.cn

PHP:  public / protected / private
来源：https://cg.zhonguo8118.cn

JS:   #private 字段；其余公开
来源：https://ev.zhonguo2118.cn

TS:   public / protected / private
来源：https://pp.zhonguo8118.cn

Java: public / protected / private / 默认包级
来源：https://fd.zhonguo4118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://hd.zhonguo2118.cn

Ruby: public / protected / private
来源：https://jf.zhonguo1118.cn

C#:   public / protected / private / internal
来源：https://cm.zhonguo5118.cn

[G11] getter / setter
来源：https://dm.zhonguo6118.cn

Py:   @property 与 @x.setter
来源：https://xv.zhonguo8118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://wy.zhonguo5118.cn

JS:   get name() { return this._name; }
来源：https://nm.zhonguo3118.cn

TS:   get name(): string { return this._name; }
来源：https://zc.zhonguo5118.cn

Java: public String getName() { return name; }
来源：https://ib.zhonguo4118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ue.zhonguo6118.cn

Ruby: attr_accessor :name
来源：https://lw.zhonguo5118.cn

C#:   public string Name { get; set; }
来源：https://tr.zhonguo1118.cn

[G12] 对象转字符串
来源：https://ob.zhonguo8118.cn

Py:   def __str__(self): return self.name
来源：https://ct.zhonguo8118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://qn.zhonguo8118.cn

JS:   toString() { return this.name; }
来源：https://cr.zhonguo2118.cn

TS:   toString(): string { return this.name; }
来源：https://bu.zhonguo5118.cn

Java: @Override public String toString() { return name; }
来源：https://ss.zhonguo7118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://nx.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://gg.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://bt.zhonguo6118.cn

[G13] 判断对象类型
来源：https://as.zhonguo8118.cn

Py:   isinstance(u, User)
来源：https://ge.zhonguo1118.cn

PHP:  $u instanceof User
来源：https://bq.zhonguo2118.cn

JS:   u instanceof User
来源：https://eg.zhonguo3118.cn

TS:   u instanceof User
来源：https://pk.zhonguo4118.cn

Java: u instanceof User
来源：https://mp.zhonguo4118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://di.zhonguo4118.cn

Ruby: u.is_a?(User)
来源：https://qo.zhonguo6118.cn

C#:   u is User
来源：https://bj.zhonguo8118.cn

[G14] 数据类 / record
来源：https://mw.zhonguo5118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://tt.zhonguo5118.cn

PHP:  // 用 readonly 属性模拟
来源：https://sb.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://mt.zhonguo6118.cn

TS:   type User = { name: string; age: number };
来源：https://iw.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://bd.zhonguo5118.cn

Go:   type User struct { Name string; Age int }
来源：https://fw.zhonguo1118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://rj.zhonguo2118.cn

C#:   record User(string Name, int Age);
来源：https://mh.zhonguo4118.cn

[G15] 枚举
来源：https://mf.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://no.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://np.zhonguo8118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://yy.zhonguo6118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://xl.zhonguo6118.cn

Java: enum Color { RED, GREEN }
来源：https://ju.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://hv.zhonguo2118.cn

Ruby: Color = %i[red green].freeze
来源：https://ip.zhonguo7118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://nz.zhonguo4118.cn

[G16] 对象转数组 / 字典
来源：https://rq.zhonguo1118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ni.zhonguo4118.cn

PHP:  get_object_vars($obj);
来源：https://zh.zhonguo7118.cn

JS:   Object.entries(obj)
来源：https://kk.zhonguo4118.cn

TS:   Object.entries(obj)
来源：https://he.zhonguo7118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://jx.zhonguo1118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://sj.zhonguo6118.cn

Ruby: obj.instance_variables
来源：https://uk.zhonguo7118.cn

C#:   // 用反射或 System.Text.Json
来源：https://xo.zhonguo6118.cn

================================================================================
来源：https://jo.zhonguo3118.cn

H. 异常与错误处理
来源：https://bq.zhonguo5118.cn

================================================================================
来源：https://pf.zhonguo1118.cn

[H01] try / catch 基础
来源：https://le.zhonguo7118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://og.zhonguo2118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://or.zhonguo2118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://mq.zhonguo6118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://bz.zhonguo1118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://wu.zhonguo3118.cn


<!-- 参考信息 -->