代发 wailian999

PHP:  number_format(1234567);
来源：https://mq.zhonguo2118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://mo.zhonguo2118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://dr.zhonguo2118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://ea.zhonguo7118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://pf.zhonguo8118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://wl.zhonguo4118.cn

C#:   1234567.ToString("N0")
来源：https://uj.zhonguo5118.cn

[E17] 首字母大写
来源：https://wa.zhonguo2118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://pe.zhonguo5118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://hc.zhonguo8118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://lz.zhonguo6118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ar.zhonguo4118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://zd.zhonguo7118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://mu.zhonguo2118.cn

Ruby: s.capitalize
来源：https://ez.zhonguo8118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://ej.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://bz.zhonguo1118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://jd.zhonguo5118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://cc.zhonguo3118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://ut.zhonguo7118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://jn.zhonguo3118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://ck.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://hn.zhonguo8118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://wj.zhonguo2118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://cm.zhonguo6118.cn

[E19] 多行文本按行拆分
来源：https://le.zhonguo1118.cn

Py:   s.splitlines()
来源：https://vs.zhonguo1118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://pm.zhonguo6118.cn

JS:   s.split(/\r?\n/)
来源：https://fy.zhonguo5118.cn

TS:   s.split(/\r?\n/)
来源：https://cz.zhonguo8118.cn

Java: s.lines().toList()
来源：https://wc.zhonguo6118.cn

Go:   strings.Split(s, "\n")
来源：https://ut.zhonguo7118.cn

Ruby: s.lines
来源：https://cq.zhonguo3118.cn

C#:   s.Split('\n')
来源：https://eh.zhonguo1118.cn

[E20] 判断字符串是否为空
来源：https://em.zhonguo3118.cn

Py:   if not s:
来源：https://io.zhonguo4118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://zk.zhonguo4118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ga.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://js.zhonguo5118.cn

Java: if (s.isEmpty()) {}
来源：https://xl.zhonguo8118.cn

Go:   if s == "" {}
来源：https://ql.zhonguo8118.cn

Ruby: if s.empty?
来源：https://ry.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://xc.zhonguo3118.cn

[E21] 超长截断加省略号
来源：https://ox.zhonguo7118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://oj.zhonguo3118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://qf.zhonguo1118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://us.zhonguo2118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://na.zhonguo4118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://la.zhonguo1118.cn

Go:   // 按 rune 判断长度后截断
来源：https://qv.zhonguo1118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://jg.zhonguo8118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://tg.zhonguo7118.cn

[E22] 字节长度与字符长度
来源：https://yz.zhonguo4118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://pu.zhonguo2118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://rm.zhonguo4118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://rt.zhonguo5118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://uo.zhonguo8118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://qx.zhonguo8118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://in.zhonguo7118.cn

Ruby: s.bytesize;  s.length
来源：https://ao.zhonguo6118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://ta.zhonguo2118.cn

================================================================================
来源：https://xb.zhonguo6118.cn

F. 文件与目录
来源：https://dv.zhonguo6118.cn

================================================================================
来源：https://ok.zhonguo7118.cn

[F01] 读取整个文件
来源：https://bu.zhonguo3118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://ll.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://pd.zhonguo6118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://fx.zhonguo8118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://ke.zhonguo6118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://yc.zhonguo3118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://py.zhonguo3118.cn

Ruby: File.read("a.txt")
来源：https://ye.zhonguo4118.cn

C#:   File.ReadAllText("a.txt");
来源：https://mm.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://ij.zhonguo3118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://yp.zhonguo1118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://vz.zhonguo2118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://zg.zhonguo8118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://ff.zhonguo3118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://ed.zhonguo6118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://mn.zhonguo8118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://nc.zhonguo8118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://jd.zhonguo4118.cn

[F03] 写入文件（覆盖）
来源：https://bl.zhonguo3118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://vx.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://yy.zhonguo5118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://er.zhonguo4118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ij.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://cr.zhonguo7118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://jy.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://cu.zhonguo2118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://nd.zhonguo8118.cn

[F04] 追加写入文件
来源：https://rl.zhonguo4118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ll.zhonguo7118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://nw.zhonguo4118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://kw.zhonguo2118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://bd.zhonguo2118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://av.zhonguo7118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://tj.zhonguo1118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://fl.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://bg.zhonguo8118.cn

[F05] 判断文件或目录是否存在
来源：https://kq.zhonguo5118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ei.zhonguo3118.cn

PHP:  file_exists("a.txt");
来源：https://hr.zhonguo3118.cn

JS:   fs.existsSync("a.txt")
来源：https://us.zhonguo3118.cn

TS:   fs.existsSync("a.txt")
来源：https://le.zhonguo3118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://it.zhonguo3118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://eo.zhonguo3118.cn

Ruby: File.exist?("a.txt")
来源：https://lq.zhonguo2118.cn

C#:   File.Exists("a.txt")
来源：https://it.zhonguo4118.cn

[F06] 删除文件
来源：https://wi.zhonguo2118.cn

Py:   os.remove("a.txt")
来源：https://ku.zhonguo5118.cn

PHP:  unlink("a.txt");
来源：https://df.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://bb.zhonguo3118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://us.zhonguo3118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://fm.zhonguo2118.cn

Go:   os.Remove("a.txt")
来源：https://cu.zhonguo1118.cn

Ruby: File.delete("a.txt")
来源：https://dp.zhonguo6118.cn

C#:   File.Delete("a.txt");
来源：https://ro.zhonguo1118.cn

[F07] 创建目录（含多级）
来源：https://ct.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://vd.zhonguo8118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://ht.zhonguo4118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ws.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://km.zhonguo3118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://fp.zhonguo6118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://fb.zhonguo3118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://sc.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://sa.zhonguo7118.cn

[F08] 遍历目录
来源：https://nz.zhonguo8118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://rz.zhonguo4118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://yq.zhonguo3118.cn

JS:   fs.readdirSync("dir")
来源：https://pm.zhonguo1118.cn

TS:   fs.readdirSync("dir")
来源：https://rd.zhonguo3118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://qh.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://au.zhonguo8118.cn

Ruby: Dir.children("dir")
来源：https://kj.zhonguo7118.cn

C#:   Directory.GetFiles("dir")
来源：https://kk.zhonguo4118.cn

[F09] 获取文件大小
来源：https://uh.zhonguo7118.cn

Py:   os.path.getsize("a.txt")
来源：https://rk.zhonguo4118.cn

PHP:  filesize("a.txt");
来源：https://ph.zhonguo8118.cn

JS:   fs.statSync("a.txt").size
来源：https://yv.zhonguo2118.cn

TS:   fs.statSync("a.txt").size
来源：https://yc.zhonguo5118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://zj.zhonguo6118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://yr.zhonguo1118.cn

Ruby: File.size("a.txt")
来源：https://yu.zhonguo4118.cn

C#:   new FileInfo("a.txt").Length
来源：https://li.zhonguo1118.cn

[F10] 取文件扩展名 / 文件名
来源：https://ia.zhonguo7118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://fc.zhonguo6118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://ml.zhonguo2118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://xx.zhonguo4118.cn

TS:   path.extname("a.txt")
来源：https://cr.zhonguo8118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://ef.zhonguo4118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://tt.zhonguo4118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://th.zhonguo2118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://so.zhonguo8118.cn

[F11] 复制与移动文件
来源：https://ai.zhonguo1118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://rt.zhonguo6118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://jo.zhonguo1118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://dc.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://dy.zhonguo4118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://qz.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://qh.zhonguo3118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://ic.zhonguo1118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://vm.zhonguo3118.cn

[F12] CSV 读写
来源：https://is.zhonguo5118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ts.zhonguo6118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://rn.zhonguo1118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://cq.zhonguo6118.cn

TS:   // 同上
来源：https://lw.zhonguo8118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://xq.zhonguo8118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://nc.zhonguo2118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://sk.zhonguo7118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://cc.zhonguo1118.cn

================================================================================
来源：https://du.zhonguo8118.cn

G. 面向对象
来源：https://sa.zhonguo4118.cn

================================================================================
来源：https://ei.zhonguo5118.cn

[G01] 定义类
来源：https://yw.zhonguo7118.cn

Py:   class User: pass
来源：https://kw.zhonguo5118.cn

PHP:  class User {}
来源：https://wt.zhonguo4118.cn

JS:   class User {}
来源：https://ld.zhonguo6118.cn

TS:   class User { name: string = ""; }
来源：https://bn.zhonguo1118.cn

Java: class User {}
来源：https://nm.zhonguo1118.cn

Go:   type User struct { Name string }
来源：https://xz.zhonguo4118.cn

Ruby: class User; end
来源：https://xj.zhonguo8118.cn

C#:   class User {}
来源：https://uo.zhonguo3118.cn

[G02] 构造函数
来源：https://ih.zhonguo4118.cn

Py:   def __init__(self, name): self.name = name
来源：https://do.zhonguo1118.cn

PHP:  public function __construct(public string $name) {}
来源：https://xq.zhonguo7118.cn

JS:   constructor(name) { this.name = name; }
来源：https://ql.zhonguo3118.cn

TS:   constructor(public name: string) {}
来源：https://so.zhonguo2118.cn

Java: User(String name) { this.name = name; }
来源：https://cl.zhonguo7118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://el.zhonguo4118.cn

Ruby: def initialize(name); @name = name; end
来源：https://oi.zhonguo6118.cn

C#:   public User(string name) { Name = name; }
来源：https://rb.zhonguo1118.cn

[G03] 实例属性
来源：https://bk.zhonguo4118.cn

Py:   self.name = "x"
来源：https://cx.zhonguo4118.cn

PHP:  public string $name = "x";
来源：https://no.zhonguo7118.cn

JS:   this.name = "x";
来源：https://pb.zhonguo7118.cn

TS:   name: string = "x";
来源：https://pq.zhonguo2118.cn

Java: private String name;
来源：https://rc.zhonguo5118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://be.zhonguo6118.cn

Ruby: @name = "x"
来源：https://cu.zhonguo1118.cn

C#:   public string Name { get; set; } = "x";
来源：https://xl.zhonguo5118.cn

[G04] 定义方法
来源：https://oi.zhonguo6118.cn

Py:   def greet(self): return self.name
来源：https://nd.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ji.zhonguo5118.cn

JS:   greet() { return this.name; }
来源：https://hv.zhonguo8118.cn

TS:   greet(): string { return this.name; }
来源：https://dz.zhonguo7118.cn

Java: String greet() { return name; }
来源：https://as.zhonguo2118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://mk.zhonguo8118.cn

Ruby: def greet; @name; end
来源：https://pp.zhonguo2118.cn

C#:   public string Greet() => Name;
来源：https://xa.zhonguo4118.cn

[G05] 继承
来源：https://jm.zhonguo3118.cn

Py:   class Admin(User): pass
来源：https://ft.zhonguo3118.cn

PHP:  class Admin extends User {}
来源：https://sf.zhonguo8118.cn

JS:   class Admin extends User {}
来源：https://sk.zhonguo4118.cn

TS:   class Admin extends User {}
来源：https://gj.zhonguo3118.cn

Java: class Admin extends User {}
来源：https://wb.zhonguo4118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://tl.zhonguo1118.cn

Ruby: class Admin < User; end
来源：https://hm.zhonguo6118.cn

C#:   class Admin : User {}
来源：https://yg.zhonguo7118.cn

[G06] 重写方法
来源：https://hl.zhonguo5118.cn

Py:   def greet(self): return "admin"
来源：https://ir.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://zv.zhonguo1118.cn

JS:   greet() { return "admin"; }
来源：https://ax.zhonguo6118.cn

TS:   greet(): string { return "admin"; }
来源：https://np.zhonguo4118.cn

Java: @Override String greet() { return "admin"; }
来源：https://bq.zhonguo1118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://jv.zhonguo3118.cn

Ruby: def greet; "admin"; end
来源：https://hh.zhonguo5118.cn

C#:   public override string Greet() => "admin";
来源：https://zs.zhonguo6118.cn

[G07] 调用父类方法
来源：https://jq.zhonguo5118.cn

Py:   super().greet()
来源：https://fv.zhonguo1118.cn

PHP:  parent::greet();
来源：https://kp.zhonguo1118.cn

JS:   super.greet();
来源：https://iv.zhonguo8118.cn

TS:   super.greet();
来源：https://ma.zhonguo2118.cn

Java: super.greet();
来源：https://dt.zhonguo8118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://fi.zhonguo4118.cn

Ruby: super
来源：https://ru.zhonguo8118.cn

C#:   base.Greet();
来源：https://ns.zhonguo1118.cn

[G08] 静态方法与属性
来源：https://pa.zhonguo1118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://ir.zhonguo5118.cn

PHP:  public static function f() {}
来源：https://pg.zhonguo5118.cn

JS:   static f() {}
来源：https://rg.zhonguo3118.cn

TS:   static f(): void {}
来源：https://up.zhonguo3118.cn

Java: static void f() {}
来源：https://mq.zhonguo1118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://lu.zhonguo3118.cn

Ruby: def self.f; end
来源：https://jt.zhonguo2118.cn

C#:   public static void F() {}
来源：https://zj.zhonguo3118.cn

[G09] 接口 / 抽象类
来源：https://ra.zhonguo1118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ke.zhonguo8118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://ay.zhonguo2118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://af.zhonguo1118.cn

TS:   interface Shape { area(): number; }
来源：https://pn.zhonguo8118.cn

Java: interface Shape { double area(); }
来源：https://hx.zhonguo7118.cn

Go:   type Shape interface { Area() float64 }
来源：https://kk.zhonguo2118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://md.zhonguo3118.cn

C#:   interface IShape { double Area(); }
来源：https://xq.zhonguo2118.cn

[G10] 访问控制
来源：https://fq.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://zi.zhonguo1118.cn

PHP:  public / protected / private
来源：https://wl.zhonguo8118.cn

JS:   #private 字段；其余公开
来源：https://vs.zhonguo5118.cn

TS:   public / protected / private
来源：https://eb.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://kp.zhonguo5118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://ob.zhonguo2118.cn

Ruby: public / protected / private
来源：https://et.zhonguo1118.cn

C#:   public / protected / private / internal
来源：https://uf.zhonguo2118.cn

[G11] getter / setter
来源：https://xs.zhonguo5118.cn

Py:   @property 与 @x.setter
来源：https://aj.zhonguo8118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://wo.zhonguo2118.cn

JS:   get name() { return this._name; }
来源：https://ul.zhonguo7118.cn

TS:   get name(): string { return this._name; }
来源：https://jf.zhonguo5118.cn

Java: public String getName() { return name; }
来源：https://vu.zhonguo3118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://cf.zhonguo1118.cn

Ruby: attr_accessor :name
来源：https://cw.zhonguo6118.cn

C#:   public string Name { get; set; }
来源：https://fx.zhonguo4118.cn

[G12] 对象转字符串
来源：https://tz.zhonguo2118.cn

Py:   def __str__(self): return self.name
来源：https://it.zhonguo8118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://hq.zhonguo3118.cn

JS:   toString() { return this.name; }
来源：https://hn.zhonguo8118.cn

TS:   toString(): string { return this.name; }
来源：https://mk.zhonguo4118.cn

Java: @Override public String toString() { return name; }
来源：https://ud.zhonguo1118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://fj.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://fw.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://eo.zhonguo5118.cn

[G13] 判断对象类型
来源：https://ta.zhonguo2118.cn

Py:   isinstance(u, User)
来源：https://vq.zhonguo2118.cn

PHP:  $u instanceof User
来源：https://bi.zhonguo7118.cn

JS:   u instanceof User
来源：https://ak.zhonguo4118.cn

TS:   u instanceof User
来源：https://mh.zhonguo5118.cn

Java: u instanceof User
来源：https://wp.zhonguo3118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://gf.zhonguo7118.cn

Ruby: u.is_a?(User)
来源：https://gk.zhonguo3118.cn

C#:   u is User
来源：https://pf.zhonguo4118.cn

[G14] 数据类 / record
来源：https://qf.zhonguo5118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://ex.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://uk.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://rr.zhonguo7118.cn

TS:   type User = { name: string; age: number };
来源：https://zo.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://ih.zhonguo4118.cn

Go:   type User struct { Name string; Age int }
来源：https://hh.zhonguo8118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://oh.zhonguo3118.cn


<!-- 参考信息 -->