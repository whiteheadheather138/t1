代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://rk.zhonguo3118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://yf.zhonguo4118.cn

C#:   1234567.ToString("N0")
来源：https://do.zhonguo2118.cn

[E17] 首字母大写
来源：https://eq.zhonguo8118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://gj.zhonguo4118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://pv.zhonguo1118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://be.zhonguo6118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://vn.zhonguo1118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://vs.zhonguo5118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://st.zhonguo4118.cn

Ruby: s.capitalize
来源：https://kz.zhonguo2118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://mj.zhonguo7118.cn

[E18] 模板占位符替换
来源：https://op.zhonguo5118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://pg.zhonguo8118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://lt.zhonguo5118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://kq.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://by.zhonguo8118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://dp.zhonguo7118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://um.zhonguo8118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://ha.zhonguo5118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://yv.zhonguo8118.cn

[E19] 多行文本按行拆分
来源：https://cm.zhonguo2118.cn

Py:   s.splitlines()
来源：https://pt.zhonguo6118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://rz.zhonguo5118.cn

JS:   s.split(/\r?\n/)
来源：https://li.zhonguo2118.cn

TS:   s.split(/\r?\n/)
来源：https://ur.zhonguo2118.cn

Java: s.lines().toList()
来源：https://ts.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://te.zhonguo8118.cn

Ruby: s.lines
来源：https://zg.zhonguo7118.cn

C#:   s.Split('\n')
来源：https://zf.zhonguo8118.cn

[E20] 判断字符串是否为空
来源：https://ph.zhonguo4118.cn

Py:   if not s:
来源：https://vb.zhonguo4118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://ha.zhonguo3118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ig.zhonguo3118.cn

TS:   if (s === "") {}
来源：https://zm.zhonguo5118.cn

Java: if (s.isEmpty()) {}
来源：https://mh.zhonguo6118.cn

Go:   if s == "" {}
来源：https://ih.zhonguo1118.cn

Ruby: if s.empty?
来源：https://jf.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://ci.zhonguo2118.cn

[E21] 超长截断加省略号
来源：https://fw.zhonguo4118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://gg.zhonguo5118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://mz.zhonguo2118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ws.zhonguo2118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://rb.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://hg.zhonguo7118.cn

Go:   // 按 rune 判断长度后截断
来源：https://pr.zhonguo2118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://tm.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://vs.zhonguo1118.cn

[E22] 字节长度与字符长度
来源：https://bi.zhonguo8118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://lu.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://xt.zhonguo1118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://xf.zhonguo2118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://mh.zhonguo4118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://va.zhonguo7118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://lg.zhonguo3118.cn

Ruby: s.bytesize;  s.length
来源：https://yf.zhonguo6118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://qf.zhonguo5118.cn

================================================================================
来源：https://mw.zhonguo3118.cn

F. 文件与目录
来源：https://ik.zhonguo5118.cn

================================================================================
来源：https://ve.zhonguo2118.cn

[F01] 读取整个文件
来源：https://np.zhonguo7118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://sf.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://ta.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://ef.zhonguo6118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://at.zhonguo5118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://cp.zhonguo1118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://hd.zhonguo6118.cn

Ruby: File.read("a.txt")
来源：https://is.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://wt.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://ru.zhonguo8118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://po.zhonguo1118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://om.zhonguo3118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://pd.zhonguo3118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://fp.zhonguo7118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://sx.zhonguo7118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://lk.zhonguo4118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://dx.zhonguo4118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://nb.zhonguo5118.cn

[F03] 写入文件（覆盖）
来源：https://dt.zhonguo8118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://et.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://mj.zhonguo4118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://vm.zhonguo2118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://hx.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://jb.zhonguo7118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ij.zhonguo2118.cn

Ruby: File.write("a.txt", "hi")
来源：https://sm.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://im.zhonguo3118.cn

[F04] 追加写入文件
来源：https://my.zhonguo6118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ce.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://pv.zhonguo5118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://sl.zhonguo2118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://zm.zhonguo6118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://oq.zhonguo8118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://gb.zhonguo1118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://vr.zhonguo3118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://ym.zhonguo3118.cn

[F05] 判断文件或目录是否存在
来源：https://ip.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://fj.zhonguo6118.cn

PHP:  file_exists("a.txt");
来源：https://iv.zhonguo5118.cn

JS:   fs.existsSync("a.txt")
来源：https://di.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://jk.zhonguo6118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://au.zhonguo8118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://tn.zhonguo6118.cn

Ruby: File.exist?("a.txt")
来源：https://nm.zhonguo8118.cn

C#:   File.Exists("a.txt")
来源：https://tu.zhonguo8118.cn

[F06] 删除文件
来源：https://yu.zhonguo6118.cn

Py:   os.remove("a.txt")
来源：https://la.zhonguo6118.cn

PHP:  unlink("a.txt");
来源：https://xw.zhonguo5118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://pt.zhonguo1118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://ri.zhonguo8118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://lg.zhonguo4118.cn

Go:   os.Remove("a.txt")
来源：https://jg.zhonguo6118.cn

Ruby: File.delete("a.txt")
来源：https://kv.zhonguo2118.cn

C#:   File.Delete("a.txt");
来源：https://df.zhonguo3118.cn

[F07] 创建目录（含多级）
来源：https://wp.zhonguo2118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://an.zhonguo1118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://fg.zhonguo2118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://pw.zhonguo6118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://gh.zhonguo6118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://kf.zhonguo8118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://eb.zhonguo8118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://rp.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://ty.zhonguo7118.cn

[F08] 遍历目录
来源：https://yj.zhonguo1118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://kj.zhonguo6118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://oj.zhonguo7118.cn

JS:   fs.readdirSync("dir")
来源：https://nh.zhonguo4118.cn

TS:   fs.readdirSync("dir")
来源：https://sx.zhonguo3118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://in.zhonguo5118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://oy.zhonguo2118.cn

Ruby: Dir.children("dir")
来源：https://hb.zhonguo8118.cn

C#:   Directory.GetFiles("dir")
来源：https://iu.zhonguo2118.cn

[F09] 获取文件大小
来源：https://rw.zhonguo4118.cn

Py:   os.path.getsize("a.txt")
来源：https://rw.zhonguo7118.cn

PHP:  filesize("a.txt");
来源：https://px.zhonguo7118.cn

JS:   fs.statSync("a.txt").size
来源：https://tb.zhonguo7118.cn

TS:   fs.statSync("a.txt").size
来源：https://sd.zhonguo3118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://nk.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://hy.zhonguo7118.cn

Ruby: File.size("a.txt")
来源：https://zu.zhonguo8118.cn

C#:   new FileInfo("a.txt").Length
来源：https://ni.zhonguo1118.cn

[F10] 取文件扩展名 / 文件名
来源：https://th.zhonguo8118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://qt.zhonguo5118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://jf.zhonguo6118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://nc.zhonguo7118.cn

TS:   path.extname("a.txt")
来源：https://ng.zhonguo5118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://wg.zhonguo6118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://wg.zhonguo3118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://gm.zhonguo1118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://jf.zhonguo6118.cn

[F11] 复制与移动文件
来源：https://ac.zhonguo8118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://cm.zhonguo3118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://rc.zhonguo8118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://kn.zhonguo2118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://nd.zhonguo4118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://qt.zhonguo5118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://yx.zhonguo6118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://jt.zhonguo1118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ph.zhonguo4118.cn

[F12] CSV 读写
来源：https://gk.zhonguo6118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ad.zhonguo3118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://uo.zhonguo6118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://ih.zhonguo2118.cn

TS:   // 同上
来源：https://lt.zhonguo4118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://bl.zhonguo6118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://lz.zhonguo4118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://pj.zhonguo6118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://yj.zhonguo2118.cn

================================================================================
来源：https://tu.zhonguo8118.cn

G. 面向对象
来源：https://wv.zhonguo6118.cn

================================================================================
来源：https://by.zhonguo7118.cn

[G01] 定义类
来源：https://jt.zhonguo7118.cn

Py:   class User: pass
来源：https://ib.zhonguo1118.cn

PHP:  class User {}
来源：https://lw.zhonguo7118.cn

JS:   class User {}
来源：https://ig.zhonguo5118.cn

TS:   class User { name: string = ""; }
来源：https://uf.zhonguo1118.cn

Java: class User {}
来源：https://uh.zhonguo6118.cn

Go:   type User struct { Name string }
来源：https://hh.zhonguo4118.cn

Ruby: class User; end
来源：https://su.zhonguo2118.cn

C#:   class User {}
来源：https://hb.zhonguo3118.cn

[G02] 构造函数
来源：https://gb.zhonguo4118.cn

Py:   def __init__(self, name): self.name = name
来源：https://qo.zhonguo4118.cn

PHP:  public function __construct(public string $name) {}
来源：https://xr.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://av.zhonguo3118.cn

TS:   constructor(public name: string) {}
来源：https://vb.zhonguo6118.cn

Java: User(String name) { this.name = name; }
来源：https://es.zhonguo3118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://kl.zhonguo7118.cn

Ruby: def initialize(name); @name = name; end
来源：https://iq.zhonguo5118.cn

C#:   public User(string name) { Name = name; }
来源：https://im.zhonguo4118.cn

[G03] 实例属性
来源：https://jj.zhonguo7118.cn

Py:   self.name = "x"
来源：https://np.zhonguo5118.cn

PHP:  public string $name = "x";
来源：https://mb.zhonguo3118.cn

JS:   this.name = "x";
来源：https://xx.zhonguo3118.cn

TS:   name: string = "x";
来源：https://eh.zhonguo7118.cn

Java: private String name;
来源：https://km.zhonguo3118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://uw.zhonguo6118.cn

Ruby: @name = "x"
来源：https://fj.zhonguo1118.cn

C#:   public string Name { get; set; } = "x";
来源：https://ya.zhonguo4118.cn

[G04] 定义方法
来源：https://tv.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://yz.zhonguo5118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ba.zhonguo3118.cn

JS:   greet() { return this.name; }
来源：https://il.zhonguo5118.cn

TS:   greet(): string { return this.name; }
来源：https://ck.zhonguo6118.cn

Java: String greet() { return name; }
来源：https://mk.zhonguo6118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://dg.zhonguo6118.cn

Ruby: def greet; @name; end
来源：https://pe.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://or.zhonguo7118.cn

[G05] 继承
来源：https://sl.zhonguo4118.cn

Py:   class Admin(User): pass
来源：https://gc.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://ja.zhonguo8118.cn

JS:   class Admin extends User {}
来源：https://eh.zhonguo6118.cn

TS:   class Admin extends User {}
来源：https://yo.zhonguo6118.cn

Java: class Admin extends User {}
来源：https://kz.zhonguo3118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://re.zhonguo3118.cn

Ruby: class Admin < User; end
来源：https://fi.zhonguo4118.cn

C#:   class Admin : User {}
来源：https://bw.zhonguo3118.cn

[G06] 重写方法
来源：https://if.zhonguo5118.cn

Py:   def greet(self): return "admin"
来源：https://py.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ai.zhonguo3118.cn

JS:   greet() { return "admin"; }
来源：https://hv.zhonguo1118.cn

TS:   greet(): string { return "admin"; }
来源：https://zv.zhonguo1118.cn

Java: @Override String greet() { return "admin"; }
来源：https://wu.zhonguo1118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://ez.zhonguo4118.cn

Ruby: def greet; "admin"; end
来源：https://aa.zhonguo3118.cn

C#:   public override string Greet() => "admin";
来源：https://yl.zhonguo7118.cn

[G07] 调用父类方法
来源：https://qs.zhonguo7118.cn

Py:   super().greet()
来源：https://qd.zhonguo8118.cn

PHP:  parent::greet();
来源：https://ez.zhonguo7118.cn

JS:   super.greet();
来源：https://dr.zhonguo8118.cn

TS:   super.greet();
来源：https://bu.zhonguo1118.cn

Java: super.greet();
来源：https://st.zhonguo1118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://vy.zhonguo1118.cn

Ruby: super
来源：https://qd.zhonguo2118.cn

C#:   base.Greet();
来源：https://ed.zhonguo2118.cn

[G08] 静态方法与属性
来源：https://ft.zhonguo1118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://kx.zhonguo3118.cn

PHP:  public static function f() {}
来源：https://zu.zhonguo5118.cn

JS:   static f() {}
来源：https://tt.zhonguo3118.cn

TS:   static f(): void {}
来源：https://fm.zhonguo6118.cn

Java: static void f() {}
来源：https://ll.zhonguo1118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://ho.zhonguo7118.cn

Ruby: def self.f; end
来源：https://ql.zhonguo3118.cn

C#:   public static void F() {}
来源：https://sn.zhonguo4118.cn

[G09] 接口 / 抽象类
来源：https://jk.zhonguo4118.cn

Py:   from abc import ABC, abstractmethod
来源：https://py.zhonguo6118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://yf.zhonguo1118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://sc.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://wv.zhonguo3118.cn

Java: interface Shape { double area(); }
来源：https://fq.zhonguo4118.cn

Go:   type Shape interface { Area() float64 }
来源：https://hf.zhonguo8118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://wk.zhonguo2118.cn

C#:   interface IShape { double Area(); }
来源：https://ck.zhonguo6118.cn

[G10] 访问控制
来源：https://zh.zhonguo4118.cn

Py:   约定 _protected / __private（不强制）
来源：https://pe.zhonguo5118.cn

PHP:  public / protected / private
来源：https://wh.zhonguo6118.cn

JS:   #private 字段；其余公开
来源：https://pq.zhonguo7118.cn

TS:   public / protected / private
来源：https://xt.zhonguo4118.cn

Java: public / protected / private / 默认包级
来源：https://ew.zhonguo6118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://an.zhonguo2118.cn

Ruby: public / protected / private
来源：https://su.zhonguo3118.cn

C#:   public / protected / private / internal
来源：https://mi.zhonguo2118.cn

[G11] getter / setter
来源：https://nc.zhonguo3118.cn

Py:   @property 与 @x.setter
来源：https://mb.zhonguo6118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://wy.zhonguo8118.cn

JS:   get name() { return this._name; }
来源：https://dn.zhonguo8118.cn

TS:   get name(): string { return this._name; }
来源：https://wn.zhonguo6118.cn

Java: public String getName() { return name; }
来源：https://bi.zhonguo1118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ai.zhonguo6118.cn

Ruby: attr_accessor :name
来源：https://oe.zhonguo6118.cn

C#:   public string Name { get; set; }
来源：https://xx.zhonguo4118.cn

[G12] 对象转字符串
来源：https://zw.zhonguo1118.cn

Py:   def __str__(self): return self.name
来源：https://mr.zhonguo2118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://gk.zhonguo5118.cn

JS:   toString() { return this.name; }
来源：https://ma.zhonguo3118.cn

TS:   toString(): string { return this.name; }
来源：https://hg.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://tw.zhonguo2118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://ul.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://tr.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://tc.zhonguo4118.cn

[G13] 判断对象类型
来源：https://iz.zhonguo2118.cn

Py:   isinstance(u, User)
来源：https://ho.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://rn.zhonguo2118.cn

JS:   u instanceof User
来源：https://ie.zhonguo3118.cn

TS:   u instanceof User
来源：https://mz.zhonguo5118.cn

Java: u instanceof User
来源：https://kx.zhonguo3118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://wu.zhonguo2118.cn

Ruby: u.is_a?(User)
来源：https://lv.zhonguo1118.cn

C#:   u is User
来源：https://cf.zhonguo1118.cn

[G14] 数据类 / record
来源：https://am.zhonguo5118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://zt.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://ot.zhonguo7118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://jx.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://yd.zhonguo8118.cn

Java: record User(String name, int age) {}
来源：https://sa.zhonguo7118.cn

Go:   type User struct { Name string; Age int }
来源：https://uv.zhonguo2118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://mz.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://uz.zhonguo4118.cn

[G15] 枚举
来源：https://rz.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ah.zhonguo5118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://eu.zhonguo8118.cn


<!-- 参考信息 -->