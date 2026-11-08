代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：https://xd.zhonguo4118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://gj.zhonguo1118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://bl.zhonguo5118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://dq.zhonguo5118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://vy.zhonguo6118.cn

[E19] 多行文本按行拆分
来源：https://kp.zhonguo1118.cn

Py:   s.splitlines()
来源：https://kn.zhonguo3118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://xs.zhonguo2118.cn

JS:   s.split(/\r?\n/)
来源：https://na.zhonguo5118.cn

TS:   s.split(/\r?\n/)
来源：https://zj.zhonguo3118.cn

Java: s.lines().toList()
来源：https://lm.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://bg.zhonguo6118.cn

Ruby: s.lines
来源：https://do.zhonguo8118.cn

C#:   s.Split('\n')
来源：https://wi.zhonguo5118.cn

[E20] 判断字符串是否为空
来源：https://zb.zhonguo2118.cn

Py:   if not s:
来源：https://ip.zhonguo8118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://sd.zhonguo5118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://sb.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://lu.zhonguo8118.cn

Java: if (s.isEmpty()) {}
来源：https://dm.zhonguo2118.cn

Go:   if s == "" {}
来源：https://nb.zhonguo6118.cn

Ruby: if s.empty?
来源：https://vv.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://vp.zhonguo2118.cn

[E21] 超长截断加省略号
来源：https://yi.zhonguo2118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://vw.zhonguo7118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://ct.zhonguo1118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://qh.zhonguo6118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ov.zhonguo1118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://cb.zhonguo7118.cn

Go:   // 按 rune 判断长度后截断
来源：https://qn.zhonguo8118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://ds.zhonguo5118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://xa.zhonguo2118.cn

[E22] 字节长度与字符长度
来源：https://ba.zhonguo4118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://yh.zhonguo8118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ep.zhonguo2118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://eq.zhonguo5118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://xc.zhonguo8118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://yq.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://pc.zhonguo1118.cn

Ruby: s.bytesize;  s.length
来源：https://xw.zhonguo6118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://mz.zhonguo6118.cn

================================================================================
来源：https://rx.zhonguo8118.cn

F. 文件与目录
来源：https://yb.zhonguo2118.cn

================================================================================
来源：https://zz.zhonguo4118.cn

[F01] 读取整个文件
来源：https://lb.zhonguo4118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://vq.zhonguo5118.cn

PHP:  file_get_contents("a.txt");
来源：https://gb.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://io.zhonguo8118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://of.zhonguo1118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://zj.zhonguo5118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://tl.zhonguo4118.cn

Ruby: File.read("a.txt")
来源：https://uq.zhonguo7118.cn

C#:   File.ReadAllText("a.txt");
来源：https://dj.zhonguo3118.cn

[F02] 逐行读取文件
来源：https://ix.zhonguo2118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ly.zhonguo1118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://yc.zhonguo1118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://eu.zhonguo8118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://xv.zhonguo3118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://px.zhonguo6118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://pb.zhonguo2118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://yw.zhonguo8118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://dh.zhonguo4118.cn

[F03] 写入文件（覆盖）
来源：https://wf.zhonguo8118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://qx.zhonguo2118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://bf.zhonguo6118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://fd.zhonguo8118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ma.zhonguo3118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://qy.zhonguo5118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ws.zhonguo4118.cn

Ruby: File.write("a.txt", "hi")
来源：https://yj.zhonguo4118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://cv.zhonguo4118.cn

[F04] 追加写入文件
来源：https://xb.zhonguo6118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://xu.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://mb.zhonguo5118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://tb.zhonguo4118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://pi.zhonguo4118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://jj.zhonguo3118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://jw.zhonguo3118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://fd.zhonguo4118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://ey.zhonguo8118.cn

[F05] 判断文件或目录是否存在
来源：https://wi.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://bs.zhonguo8118.cn

PHP:  file_exists("a.txt");
来源：https://ns.zhonguo2118.cn

JS:   fs.existsSync("a.txt")
来源：https://lj.zhonguo8118.cn

TS:   fs.existsSync("a.txt")
来源：https://ys.zhonguo1118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://rw.zhonguo3118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://vr.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://yb.zhonguo6118.cn

C#:   File.Exists("a.txt")
来源：https://lg.zhonguo7118.cn

[F06] 删除文件
来源：https://kv.zhonguo4118.cn

Py:   os.remove("a.txt")
来源：https://am.zhonguo1118.cn

PHP:  unlink("a.txt");
来源：https://wc.zhonguo6118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://kh.zhonguo5118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://bd.zhonguo6118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://rw.zhonguo4118.cn

Go:   os.Remove("a.txt")
来源：https://mu.zhonguo8118.cn

Ruby: File.delete("a.txt")
来源：https://eg.zhonguo7118.cn

C#:   File.Delete("a.txt");
来源：https://fa.zhonguo5118.cn

[F07] 创建目录（含多级）
来源：https://cw.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://fo.zhonguo3118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://ld.zhonguo8118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://rf.zhonguo5118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://uy.zhonguo3118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://tl.zhonguo5118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://lw.zhonguo2118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://wl.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://pe.zhonguo2118.cn

[F08] 遍历目录
来源：https://rr.zhonguo2118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://cs.zhonguo7118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://pa.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://mn.zhonguo6118.cn

TS:   fs.readdirSync("dir")
来源：https://tf.zhonguo3118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://bf.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://aj.zhonguo2118.cn

Ruby: Dir.children("dir")
来源：https://he.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://tk.zhonguo7118.cn

[F09] 获取文件大小
来源：https://xh.zhonguo8118.cn

Py:   os.path.getsize("a.txt")
来源：https://ct.zhonguo1118.cn

PHP:  filesize("a.txt");
来源：https://of.zhonguo8118.cn

JS:   fs.statSync("a.txt").size
来源：https://yv.zhonguo7118.cn

TS:   fs.statSync("a.txt").size
来源：https://bu.zhonguo6118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://po.zhonguo8118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://yr.zhonguo3118.cn

Ruby: File.size("a.txt")
来源：https://fk.zhonguo5118.cn

C#:   new FileInfo("a.txt").Length
来源：https://me.zhonguo7118.cn

[F10] 取文件扩展名 / 文件名
来源：https://xk.zhonguo8118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://cl.zhonguo7118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://we.zhonguo4118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://px.zhonguo5118.cn

TS:   path.extname("a.txt")
来源：https://ae.zhonguo2118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://bz.zhonguo1118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://ao.zhonguo3118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://tb.zhonguo2118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://uw.zhonguo6118.cn

[F11] 复制与移动文件
来源：https://ls.zhonguo8118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://ph.zhonguo5118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://pq.zhonguo3118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://gq.zhonguo2118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://rq.zhonguo5118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://pl.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://zg.zhonguo7118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://mz.zhonguo6118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://np.zhonguo8118.cn

[F12] CSV 读写
来源：https://gy.zhonguo6118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://lv.zhonguo4118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://rc.zhonguo4118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://yq.zhonguo4118.cn

TS:   // 同上
来源：https://gk.zhonguo8118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://jy.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://fg.zhonguo5118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://yw.zhonguo3118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://db.zhonguo5118.cn

================================================================================
来源：https://cl.zhonguo7118.cn

G. 面向对象
来源：https://is.zhonguo5118.cn

================================================================================
来源：https://kk.zhonguo3118.cn

[G01] 定义类
来源：https://on.zhonguo2118.cn

Py:   class User: pass
来源：https://wd.zhonguo3118.cn

PHP:  class User {}
来源：https://bx.zhonguo1118.cn

JS:   class User {}
来源：https://rg.zhonguo8118.cn

TS:   class User { name: string = ""; }
来源：https://bz.zhonguo5118.cn

Java: class User {}
来源：https://hv.zhonguo8118.cn

Go:   type User struct { Name string }
来源：https://po.zhonguo5118.cn

Ruby: class User; end
来源：https://pi.zhonguo1118.cn

C#:   class User {}
来源：https://lk.zhonguo8118.cn

[G02] 构造函数
来源：https://lu.zhonguo6118.cn

Py:   def __init__(self, name): self.name = name
来源：https://xp.zhonguo6118.cn

PHP:  public function __construct(public string $name) {}
来源：https://dg.zhonguo2118.cn

JS:   constructor(name) { this.name = name; }
来源：https://lu.zhonguo4118.cn

TS:   constructor(public name: string) {}
来源：https://si.zhonguo1118.cn

Java: User(String name) { this.name = name; }
来源：https://ib.zhonguo8118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://og.zhonguo3118.cn

Ruby: def initialize(name); @name = name; end
来源：https://xo.zhonguo8118.cn

C#:   public User(string name) { Name = name; }
来源：https://qn.zhonguo5118.cn

[G03] 实例属性
来源：https://bx.zhonguo2118.cn

Py:   self.name = "x"
来源：https://kv.zhonguo6118.cn

PHP:  public string $name = "x";
来源：https://sv.zhonguo8118.cn

JS:   this.name = "x";
来源：https://vy.zhonguo8118.cn

TS:   name: string = "x";
来源：https://ds.zhonguo5118.cn

Java: private String name;
来源：https://xj.zhonguo6118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://lr.zhonguo3118.cn

Ruby: @name = "x"
来源：https://st.zhonguo5118.cn

C#:   public string Name { get; set; } = "x";
来源：https://zt.zhonguo2118.cn

[G04] 定义方法
来源：https://nj.zhonguo6118.cn

Py:   def greet(self): return self.name
来源：https://up.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://xe.zhonguo8118.cn

JS:   greet() { return this.name; }
来源：https://yz.zhonguo5118.cn

TS:   greet(): string { return this.name; }
来源：https://wh.zhonguo1118.cn

Java: String greet() { return name; }
来源：https://wd.zhonguo5118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://qq.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://go.zhonguo5118.cn

C#:   public string Greet() => Name;
来源：https://pc.zhonguo1118.cn

[G05] 继承
来源：https://wu.zhonguo8118.cn

Py:   class Admin(User): pass
来源：https://yc.zhonguo1118.cn

PHP:  class Admin extends User {}
来源：https://pz.zhonguo2118.cn

JS:   class Admin extends User {}
来源：https://kn.zhonguo4118.cn

TS:   class Admin extends User {}
来源：https://rn.zhonguo1118.cn

Java: class Admin extends User {}
来源：https://kr.zhonguo4118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://fd.zhonguo8118.cn

Ruby: class Admin < User; end
来源：https://vc.zhonguo5118.cn

C#:   class Admin : User {}
来源：https://zv.zhonguo7118.cn

[G06] 重写方法
来源：https://ub.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://jl.zhonguo8118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://qe.zhonguo4118.cn

JS:   greet() { return "admin"; }
来源：https://ab.zhonguo2118.cn

TS:   greet(): string { return "admin"; }
来源：https://cx.zhonguo5118.cn

Java: @Override String greet() { return "admin"; }
来源：https://go.zhonguo2118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://re.zhonguo1118.cn

Ruby: def greet; "admin"; end
来源：https://xl.zhonguo6118.cn

C#:   public override string Greet() => "admin";
来源：https://gi.zhonguo5118.cn

[G07] 调用父类方法
来源：https://xg.zhonguo6118.cn

Py:   super().greet()
来源：https://iq.zhonguo3118.cn

PHP:  parent::greet();
来源：https://fy.zhonguo8118.cn

JS:   super.greet();
来源：https://mm.zhonguo7118.cn

TS:   super.greet();
来源：https://gp.zhonguo1118.cn

Java: super.greet();
来源：https://ch.zhonguo6118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://xy.zhonguo3118.cn

Ruby: super
来源：https://sl.zhonguo2118.cn

C#:   base.Greet();
来源：https://ap.zhonguo2118.cn

[G08] 静态方法与属性
来源：https://wd.zhonguo2118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://bn.zhonguo1118.cn

PHP:  public static function f() {}
来源：https://aa.zhonguo6118.cn

JS:   static f() {}
来源：https://sj.zhonguo1118.cn

TS:   static f(): void {}
来源：https://ww.zhonguo1118.cn

Java: static void f() {}
来源：https://lk.zhonguo5118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://he.zhonguo3118.cn

Ruby: def self.f; end
来源：https://lc.zhonguo3118.cn

C#:   public static void F() {}
来源：https://rt.zhonguo1118.cn

[G09] 接口 / 抽象类
来源：https://km.zhonguo8118.cn

Py:   from abc import ABC, abstractmethod
来源：https://jn.zhonguo4118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://va.zhonguo2118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://nj.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://bi.zhonguo8118.cn

Java: interface Shape { double area(); }
来源：https://wa.zhonguo6118.cn

Go:   type Shape interface { Area() float64 }
来源：https://qb.zhonguo4118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://sn.zhonguo8118.cn

C#:   interface IShape { double Area(); }
来源：https://zs.zhonguo6118.cn

[G10] 访问控制
来源：https://wk.zhonguo3118.cn

Py:   约定 _protected / __private（不强制）
来源：https://wh.zhonguo5118.cn

PHP:  public / protected / private
来源：https://rl.zhonguo3118.cn

JS:   #private 字段；其余公开
来源：https://uz.zhonguo7118.cn

TS:   public / protected / private
来源：https://pg.zhonguo5118.cn

Java: public / protected / private / 默认包级
来源：https://hb.zhonguo4118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://hq.zhonguo6118.cn

Ruby: public / protected / private
来源：https://zy.zhonguo3118.cn

C#:   public / protected / private / internal
来源：https://bk.zhonguo8118.cn

[G11] getter / setter
来源：https://va.zhonguo8118.cn

Py:   @property 与 @x.setter
来源：https://jw.zhonguo8118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://fp.zhonguo4118.cn

JS:   get name() { return this._name; }
来源：https://mu.zhonguo6118.cn

TS:   get name(): string { return this._name; }
来源：https://pf.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://fv.zhonguo5118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ju.zhonguo5118.cn

Ruby: attr_accessor :name
来源：https://hf.zhonguo7118.cn

C#:   public string Name { get; set; }
来源：https://ft.zhonguo3118.cn

[G12] 对象转字符串
来源：https://tc.zhonguo7118.cn

Py:   def __str__(self): return self.name
来源：https://zi.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ef.zhonguo8118.cn

JS:   toString() { return this.name; }
来源：https://gs.zhonguo2118.cn

TS:   toString(): string { return this.name; }
来源：https://wx.zhonguo8118.cn

Java: @Override public String toString() { return name; }
来源：https://vb.zhonguo3118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://vr.zhonguo4118.cn

Ruby: def to_s; @name; end
来源：https://nt.zhonguo1118.cn

C#:   public override string ToString() => Name;
来源：https://dv.zhonguo8118.cn

[G13] 判断对象类型
来源：https://me.zhonguo5118.cn

Py:   isinstance(u, User)
来源：https://rm.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://ze.zhonguo3118.cn

JS:   u instanceof User
来源：https://xz.zhonguo7118.cn

TS:   u instanceof User
来源：https://gl.zhonguo8118.cn

Java: u instanceof User
来源：https://sy.zhonguo8118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://mq.zhonguo6118.cn

Ruby: u.is_a?(User)
来源：https://zd.zhonguo3118.cn

C#:   u is User
来源：https://cc.zhonguo7118.cn

[G14] 数据类 / record
来源：https://tl.zhonguo8118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://md.zhonguo7118.cn

PHP:  // 用 readonly 属性模拟
来源：https://ah.zhonguo4118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ta.zhonguo3118.cn

TS:   type User = { name: string; age: number };
来源：https://mx.zhonguo8118.cn

Java: record User(String name, int age) {}
来源：https://px.zhonguo1118.cn

Go:   type User struct { Name string; Age int }
来源：https://op.zhonguo5118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://gt.zhonguo3118.cn

C#:   record User(string Name, int Age);
来源：https://hb.zhonguo5118.cn

[G15] 枚举
来源：https://ji.zhonguo8118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://pp.zhonguo5118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://mv.zhonguo2118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://bm.zhonguo4118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://xh.zhonguo6118.cn

Java: enum Color { RED, GREEN }
来源：https://dy.zhonguo4118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://cu.zhonguo7118.cn

Ruby: Color = %i[red green].freeze
来源：https://tt.zhonguo4118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://nr.zhonguo6118.cn

[G16] 对象转数组 / 字典
来源：https://rs.zhonguo3118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ae.zhonguo4118.cn

PHP:  get_object_vars($obj);
来源：https://jf.zhonguo5118.cn

JS:   Object.entries(obj)
来源：https://xr.zhonguo4118.cn

TS:   Object.entries(obj)
来源：https://sz.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://bg.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://oz.zhonguo4118.cn

Ruby: obj.instance_variables
来源：https://bn.zhonguo8118.cn

C#:   // 用反射或 System.Text.Json
来源：https://uu.zhonguo1118.cn

================================================================================
来源：https://zy.zhonguo8118.cn


<!-- 参考信息 -->