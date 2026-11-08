代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://yw.zhonguo2118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://di.zhonguo8118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://rq.zhonguo3118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://cu.zhonguo4118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://sz.zhonguo1118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://oi.zhonguo5118.cn

[E16] 数字千分位
来源：https://ca.zhonguo8118.cn

Py:   f"{1234567:,}"
来源：https://fq.zhonguo4118.cn

PHP:  number_format(1234567);
来源：https://az.zhonguo7118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://el.zhonguo8118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://jj.zhonguo8118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://gj.zhonguo8118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://ww.zhonguo5118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://ws.zhonguo3118.cn

C#:   1234567.ToString("N0")
来源：https://fj.zhonguo3118.cn

[E17] 首字母大写
来源：https://bp.zhonguo1118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://fa.zhonguo7118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://my.zhonguo1118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://jr.zhonguo1118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ux.zhonguo3118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://sp.zhonguo5118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://an.zhonguo6118.cn

Ruby: s.capitalize
来源：https://np.zhonguo2118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://pu.zhonguo3118.cn

[E18] 模板占位符替换
来源：https://nc.zhonguo2118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://gz.zhonguo1118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://nb.zhonguo7118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://ko.zhonguo7118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://wd.zhonguo5118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://qf.zhonguo6118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://mk.zhonguo6118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://dy.zhonguo3118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://bq.zhonguo4118.cn

[E19] 多行文本按行拆分
来源：https://hv.zhonguo2118.cn

Py:   s.splitlines()
来源：https://su.zhonguo4118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://hg.zhonguo5118.cn

JS:   s.split(/\r?\n/)
来源：https://yt.zhonguo6118.cn

TS:   s.split(/\r?\n/)
来源：https://ye.zhonguo6118.cn

Java: s.lines().toList()
来源：https://cv.zhonguo5118.cn

Go:   strings.Split(s, "\n")
来源：https://nk.zhonguo3118.cn

Ruby: s.lines
来源：https://nr.zhonguo3118.cn

C#:   s.Split('\n')
来源：https://ts.zhonguo6118.cn

[E20] 判断字符串是否为空
来源：https://ve.zhonguo5118.cn

Py:   if not s:
来源：https://id.zhonguo4118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://qf.zhonguo4118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://cp.zhonguo8118.cn

TS:   if (s === "") {}
来源：https://xc.zhonguo1118.cn

Java: if (s.isEmpty()) {}
来源：https://bf.zhonguo1118.cn

Go:   if s == "" {}
来源：https://gd.zhonguo5118.cn

Ruby: if s.empty?
来源：https://ae.zhonguo8118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://ob.zhonguo5118.cn

[E21] 超长截断加省略号
来源：https://kg.zhonguo3118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://gx.zhonguo4118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://xc.zhonguo8118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://wm.zhonguo3118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://qt.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://kz.zhonguo2118.cn

Go:   // 按 rune 判断长度后截断
来源：https://og.zhonguo6118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://yg.zhonguo3118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://vm.zhonguo3118.cn

[E22] 字节长度与字符长度
来源：https://to.zhonguo6118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://mx.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://zg.zhonguo6118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://fv.zhonguo7118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://po.zhonguo6118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://qv.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://cl.zhonguo6118.cn

Ruby: s.bytesize;  s.length
来源：https://px.zhonguo1118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://zx.zhonguo7118.cn

================================================================================
来源：https://oa.zhonguo8118.cn

F. 文件与目录
来源：https://rr.zhonguo8118.cn

================================================================================
来源：https://qy.zhonguo3118.cn

[F01] 读取整个文件
来源：https://ha.zhonguo4118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://qg.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://le.zhonguo6118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://jl.zhonguo8118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://bk.zhonguo1118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ov.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://cw.zhonguo7118.cn

Ruby: File.read("a.txt")
来源：https://ui.zhonguo7118.cn

C#:   File.ReadAllText("a.txt");
来源：https://db.zhonguo4118.cn

[F02] 逐行读取文件
来源：https://im.zhonguo6118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ip.zhonguo5118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://hs.zhonguo7118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://vo.zhonguo1118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://rw.zhonguo8118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://nv.zhonguo5118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://js.zhonguo3118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://cj.zhonguo1118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://gm.zhonguo1118.cn

[F03] 写入文件（覆盖）
来源：https://fd.zhonguo6118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://yu.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://su.zhonguo5118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://od.zhonguo1118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ix.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://cj.zhonguo8118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://kk.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://cc.zhonguo2118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://eq.zhonguo4118.cn

[F04] 追加写入文件
来源：https://ig.zhonguo5118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://zx.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://ph.zhonguo6118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://mz.zhonguo7118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://bo.zhonguo3118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://lt.zhonguo8118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://gp.zhonguo7118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://rk.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://sq.zhonguo5118.cn

[F05] 判断文件或目录是否存在
来源：https://hd.zhonguo1118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ik.zhonguo4118.cn

PHP:  file_exists("a.txt");
来源：https://de.zhonguo8118.cn

JS:   fs.existsSync("a.txt")
来源：https://gj.zhonguo8118.cn

TS:   fs.existsSync("a.txt")
来源：https://sa.zhonguo1118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://qc.zhonguo3118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://hp.zhonguo3118.cn

Ruby: File.exist?("a.txt")
来源：https://vr.zhonguo8118.cn

C#:   File.Exists("a.txt")
来源：https://jg.zhonguo6118.cn

[F06] 删除文件
来源：https://lp.zhonguo5118.cn

Py:   os.remove("a.txt")
来源：https://mv.zhonguo3118.cn

PHP:  unlink("a.txt");
来源：https://cq.zhonguo5118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://av.zhonguo6118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://bs.zhonguo6118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://xi.zhonguo6118.cn

Go:   os.Remove("a.txt")
来源：https://as.zhonguo5118.cn

Ruby: File.delete("a.txt")
来源：https://kg.zhonguo1118.cn

C#:   File.Delete("a.txt");
来源：https://fw.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://lu.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://pv.zhonguo7118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://tw.zhonguo8118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://wd.zhonguo7118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://fv.zhonguo5118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://bt.zhonguo1118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://br.zhonguo4118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://rp.zhonguo8118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://ab.zhonguo1118.cn

[F08] 遍历目录
来源：https://ms.zhonguo7118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ja.zhonguo8118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://ie.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://zu.zhonguo5118.cn

TS:   fs.readdirSync("dir")
来源：https://zh.zhonguo4118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://bb.zhonguo1118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://sl.zhonguo3118.cn

Ruby: Dir.children("dir")
来源：https://vv.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://vk.zhonguo8118.cn

[F09] 获取文件大小
来源：https://uh.zhonguo4118.cn

Py:   os.path.getsize("a.txt")
来源：https://ua.zhonguo5118.cn

PHP:  filesize("a.txt");
来源：https://le.zhonguo1118.cn

JS:   fs.statSync("a.txt").size
来源：https://er.zhonguo1118.cn

TS:   fs.statSync("a.txt").size
来源：https://fd.zhonguo8118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://xu.zhonguo6118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://ds.zhonguo4118.cn

Ruby: File.size("a.txt")
来源：https://uv.zhonguo8118.cn

C#:   new FileInfo("a.txt").Length
来源：https://tt.zhonguo8118.cn

[F10] 取文件扩展名 / 文件名
来源：https://gz.zhonguo3118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://bw.zhonguo1118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://qc.zhonguo1118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://nc.zhonguo4118.cn

TS:   path.extname("a.txt")
来源：https://ds.zhonguo1118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://ft.zhonguo6118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://bg.zhonguo8118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://fk.zhonguo3118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://wb.zhonguo7118.cn

[F11] 复制与移动文件
来源：https://nq.zhonguo1118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://wi.zhonguo5118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://sf.zhonguo7118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ha.zhonguo5118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://pb.zhonguo6118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://sy.zhonguo3118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ti.zhonguo7118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://kh.zhonguo5118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://qe.zhonguo4118.cn

[F12] CSV 读写
来源：https://hj.zhonguo5118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://jm.zhonguo8118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://dg.zhonguo3118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://rx.zhonguo4118.cn

TS:   // 同上
来源：https://xy.zhonguo6118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://et.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://dq.zhonguo5118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://zm.zhonguo8118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://rp.zhonguo1118.cn

================================================================================
来源：https://wd.zhonguo2118.cn

G. 面向对象
来源：https://md.zhonguo5118.cn

================================================================================
来源：https://hk.zhonguo8118.cn

[G01] 定义类
来源：https://ti.zhonguo1118.cn

Py:   class User: pass
来源：https://mn.zhonguo2118.cn

PHP:  class User {}
来源：https://yc.zhonguo7118.cn

JS:   class User {}
来源：https://qa.zhonguo1118.cn

TS:   class User { name: string = ""; }
来源：https://cl.zhonguo8118.cn

Java: class User {}
来源：https://kk.zhonguo3118.cn

Go:   type User struct { Name string }
来源：https://pu.zhonguo4118.cn

Ruby: class User; end
来源：https://oh.zhonguo2118.cn

C#:   class User {}
来源：https://zb.zhonguo8118.cn

[G02] 构造函数
来源：https://ye.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://fb.zhonguo1118.cn

PHP:  public function __construct(public string $name) {}
来源：https://uu.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://vu.zhonguo2118.cn

TS:   constructor(public name: string) {}
来源：https://ps.zhonguo7118.cn

Java: User(String name) { this.name = name; }
来源：https://vd.zhonguo3118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://qg.zhonguo5118.cn

Ruby: def initialize(name); @name = name; end
来源：https://ze.zhonguo6118.cn

C#:   public User(string name) { Name = name; }
来源：https://qt.zhonguo5118.cn

[G03] 实例属性
来源：https://oi.zhonguo5118.cn

Py:   self.name = "x"
来源：https://io.zhonguo4118.cn

PHP:  public string $name = "x";
来源：https://dx.zhonguo1118.cn

JS:   this.name = "x";
来源：https://pp.zhonguo6118.cn

TS:   name: string = "x";
来源：https://pi.zhonguo2118.cn

Java: private String name;
来源：https://jh.zhonguo2118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://yo.zhonguo1118.cn

Ruby: @name = "x"
来源：https://za.zhonguo2118.cn

C#:   public string Name { get; set; } = "x";
来源：https://oc.zhonguo3118.cn

[G04] 定义方法
来源：https://qi.zhonguo1118.cn

Py:   def greet(self): return self.name
来源：https://ay.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://qz.zhonguo5118.cn

JS:   greet() { return this.name; }
来源：https://rd.zhonguo3118.cn

TS:   greet(): string { return this.name; }
来源：https://mt.zhonguo2118.cn

Java: String greet() { return name; }
来源：https://me.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://qf.zhonguo8118.cn

Ruby: def greet; @name; end
来源：https://op.zhonguo3118.cn

C#:   public string Greet() => Name;
来源：https://oj.zhonguo5118.cn

[G05] 继承
来源：https://yl.zhonguo8118.cn

Py:   class Admin(User): pass
来源：https://cy.zhonguo6118.cn

PHP:  class Admin extends User {}
来源：https://qa.zhonguo7118.cn

JS:   class Admin extends User {}
来源：https://ca.zhonguo5118.cn

TS:   class Admin extends User {}
来源：https://dp.zhonguo2118.cn

Java: class Admin extends User {}
来源：https://xy.zhonguo5118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://hg.zhonguo1118.cn

Ruby: class Admin < User; end
来源：https://jw.zhonguo2118.cn

C#:   class Admin : User {}
来源：https://km.zhonguo2118.cn

[G06] 重写方法
来源：https://tk.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://ep.zhonguo3118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://mi.zhonguo1118.cn

JS:   greet() { return "admin"; }
来源：https://ix.zhonguo3118.cn

TS:   greet(): string { return "admin"; }
来源：https://pa.zhonguo8118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ex.zhonguo8118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://sq.zhonguo5118.cn

Ruby: def greet; "admin"; end
来源：https://dc.zhonguo6118.cn

C#:   public override string Greet() => "admin";
来源：https://rp.zhonguo6118.cn

[G07] 调用父类方法
来源：https://ge.zhonguo5118.cn

Py:   super().greet()
来源：https://uu.zhonguo8118.cn

PHP:  parent::greet();
来源：https://tz.zhonguo8118.cn

JS:   super.greet();
来源：https://iz.zhonguo5118.cn

TS:   super.greet();
来源：https://zg.zhonguo8118.cn

Java: super.greet();
来源：https://ng.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://pi.zhonguo3118.cn

Ruby: super
来源：https://rk.zhonguo2118.cn

C#:   base.Greet();
来源：https://gt.zhonguo7118.cn

[G08] 静态方法与属性
来源：https://nc.zhonguo7118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://cm.zhonguo8118.cn

PHP:  public static function f() {}
来源：https://ay.zhonguo6118.cn

JS:   static f() {}
来源：https://nn.zhonguo8118.cn

TS:   static f(): void {}
来源：https://fj.zhonguo7118.cn

Java: static void f() {}
来源：https://ta.zhonguo3118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://za.zhonguo5118.cn

Ruby: def self.f; end
来源：https://aw.zhonguo8118.cn

C#:   public static void F() {}
来源：https://pb.zhonguo1118.cn

[G09] 接口 / 抽象类
来源：https://gu.zhonguo7118.cn

Py:   from abc import ABC, abstractmethod
来源：https://gp.zhonguo3118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://dx.zhonguo3118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://wz.zhonguo7118.cn

TS:   interface Shape { area(): number; }
来源：https://in.zhonguo5118.cn

Java: interface Shape { double area(); }
来源：https://yl.zhonguo2118.cn

Go:   type Shape interface { Area() float64 }
来源：https://jk.zhonguo1118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://ux.zhonguo4118.cn

C#:   interface IShape { double Area(); }
来源：https://nr.zhonguo8118.cn

[G10] 访问控制
来源：https://iw.zhonguo8118.cn

Py:   约定 _protected / __private（不强制）
来源：https://zh.zhonguo1118.cn

PHP:  public / protected / private
来源：https://cv.zhonguo7118.cn

JS:   #private 字段；其余公开
来源：https://ti.zhonguo2118.cn

TS:   public / protected / private
来源：https://yk.zhonguo5118.cn

Java: public / protected / private / 默认包级
来源：https://xv.zhonguo2118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://io.zhonguo6118.cn

Ruby: public / protected / private
来源：https://re.zhonguo4118.cn

C#:   public / protected / private / internal
来源：https://sm.zhonguo7118.cn

[G11] getter / setter
来源：https://xo.zhonguo7118.cn

Py:   @property 与 @x.setter
来源：https://ze.zhonguo1118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://hu.zhonguo4118.cn

JS:   get name() { return this._name; }
来源：https://rx.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://rm.zhonguo3118.cn

Java: public String getName() { return name; }
来源：https://os.zhonguo6118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ww.zhonguo5118.cn

Ruby: attr_accessor :name
来源：https://xj.zhonguo4118.cn

C#:   public string Name { get; set; }
来源：https://bi.zhonguo5118.cn

[G12] 对象转字符串
来源：https://zg.zhonguo1118.cn

Py:   def __str__(self): return self.name
来源：https://gw.zhonguo7118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://tm.zhonguo5118.cn

JS:   toString() { return this.name; }
来源：https://nx.zhonguo2118.cn

TS:   toString(): string { return this.name; }
来源：https://kd.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://el.zhonguo4118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://gb.zhonguo4118.cn

Ruby: def to_s; @name; end
来源：https://mv.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://ok.zhonguo2118.cn

[G13] 判断对象类型
来源：https://da.zhonguo6118.cn

Py:   isinstance(u, User)
来源：https://ck.zhonguo8118.cn

PHP:  $u instanceof User
来源：https://ge.zhonguo4118.cn

JS:   u instanceof User
来源：https://he.zhonguo3118.cn

TS:   u instanceof User
来源：https://yr.zhonguo6118.cn

Java: u instanceof User
来源：https://hk.zhonguo6118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://jb.zhonguo6118.cn

Ruby: u.is_a?(User)
来源：https://ae.zhonguo2118.cn

C#:   u is User
来源：https://gv.zhonguo6118.cn


<!-- 参考信息 -->