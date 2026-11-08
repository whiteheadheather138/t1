代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://yg.zhonguo7118.cn

[E15] HTML 转义 / 反转义
来源：https://xn.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://gy.zhonguo7118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://ye.zhonguo5118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://pn.zhonguo7118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://nn.zhonguo3118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://gi.zhonguo2118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://ym.zhonguo1118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://nd.zhonguo3118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://hs.zhonguo6118.cn

[E16] 数字千分位
来源：https://do.zhonguo6118.cn

Py:   f"{1234567:,}"
来源：https://pb.zhonguo2118.cn

PHP:  number_format(1234567);
来源：https://ri.zhonguo2118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://ro.zhonguo4118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://jc.zhonguo1118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://tt.zhonguo2118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://in.zhonguo4118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://tc.zhonguo7118.cn

C#:   1234567.ToString("N0")
来源：https://gs.zhonguo4118.cn

[E17] 首字母大写
来源：https://od.zhonguo6118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://fi.zhonguo6118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://qw.zhonguo5118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://yk.zhonguo4118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://uu.zhonguo5118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://df.zhonguo6118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://lh.zhonguo5118.cn

Ruby: s.capitalize
来源：https://lp.zhonguo2118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://ee.zhonguo8118.cn

[E18] 模板占位符替换
来源：https://we.zhonguo6118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://mm.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://cr.zhonguo2118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://mp.zhonguo2118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://kk.zhonguo1118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://kd.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://dn.zhonguo8118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://xz.zhonguo6118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://sb.zhonguo1118.cn

[E19] 多行文本按行拆分
来源：https://nk.zhonguo1118.cn

Py:   s.splitlines()
来源：https://rg.zhonguo3118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://cs.zhonguo7118.cn

JS:   s.split(/\r?\n/)
来源：https://qj.zhonguo2118.cn

TS:   s.split(/\r?\n/)
来源：https://vt.zhonguo3118.cn

Java: s.lines().toList()
来源：https://ub.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://ny.zhonguo3118.cn

Ruby: s.lines
来源：https://ue.zhonguo8118.cn

C#:   s.Split('\n')
来源：https://tl.zhonguo5118.cn

[E20] 判断字符串是否为空
来源：https://na.zhonguo2118.cn

Py:   if not s:
来源：https://od.zhonguo6118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://bc.zhonguo3118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://qx.zhonguo4118.cn

TS:   if (s === "") {}
来源：https://cp.zhonguo1118.cn

Java: if (s.isEmpty()) {}
来源：https://du.zhonguo7118.cn

Go:   if s == "" {}
来源：https://ks.zhonguo4118.cn

Ruby: if s.empty?
来源：https://du.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://lt.zhonguo3118.cn

[E21] 超长截断加省略号
来源：https://rk.zhonguo7118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://dp.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://ut.zhonguo6118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ss.zhonguo5118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://oy.zhonguo6118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://qp.zhonguo5118.cn

Go:   // 按 rune 判断长度后截断
来源：https://hc.zhonguo3118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://xd.zhonguo7118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://tu.zhonguo6118.cn

[E22] 字节长度与字符长度
来源：https://ls.zhonguo1118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://fu.zhonguo6118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://vf.zhonguo4118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://mv.zhonguo8118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://mt.zhonguo2118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://ki.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://fx.zhonguo8118.cn

Ruby: s.bytesize;  s.length
来源：https://fx.zhonguo8118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://qv.zhonguo4118.cn

================================================================================
来源：https://ls.zhonguo7118.cn

F. 文件与目录
来源：https://wr.zhonguo5118.cn

================================================================================
来源：https://md.zhonguo2118.cn

[F01] 读取整个文件
来源：https://ke.zhonguo2118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://yo.zhonguo6118.cn

PHP:  file_get_contents("a.txt");
来源：https://fg.zhonguo7118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://nb.zhonguo7118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://ee.zhonguo7118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://sh.zhonguo7118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://qy.zhonguo5118.cn

Ruby: File.read("a.txt")
来源：https://ql.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://hi.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://nd.zhonguo2118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://gj.zhonguo8118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://ad.zhonguo3118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://bg.zhonguo6118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://po.zhonguo1118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://lt.zhonguo4118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://wu.zhonguo6118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://cn.zhonguo4118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://al.zhonguo4118.cn

[F03] 写入文件（覆盖）
来源：https://dm.zhonguo7118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://je.zhonguo7118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://yt.zhonguo4118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://vs.zhonguo5118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://rk.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://at.zhonguo3118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://qv.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://kz.zhonguo2118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://bd.zhonguo2118.cn

[F04] 追加写入文件
来源：https://vr.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://mo.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://vc.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ia.zhonguo6118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://rj.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://aw.zhonguo7118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://td.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://hg.zhonguo7118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://eg.zhonguo8118.cn

[F05] 判断文件或目录是否存在
来源：https://uk.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://lv.zhonguo2118.cn

PHP:  file_exists("a.txt");
来源：https://qr.zhonguo7118.cn

JS:   fs.existsSync("a.txt")
来源：https://ki.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://et.zhonguo6118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://cv.zhonguo4118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://qx.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://zq.zhonguo2118.cn

C#:   File.Exists("a.txt")
来源：https://mz.zhonguo7118.cn

[F06] 删除文件
来源：https://gt.zhonguo5118.cn

Py:   os.remove("a.txt")
来源：https://lk.zhonguo3118.cn

PHP:  unlink("a.txt");
来源：https://rf.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://es.zhonguo6118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://sq.zhonguo4118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://xv.zhonguo3118.cn

Go:   os.Remove("a.txt")
来源：https://sm.zhonguo4118.cn

Ruby: File.delete("a.txt")
来源：https://hb.zhonguo6118.cn

C#:   File.Delete("a.txt");
来源：https://bk.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://jh.zhonguo7118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://nx.zhonguo6118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://lr.zhonguo4118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://qs.zhonguo3118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ze.zhonguo3118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://yc.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://dr.zhonguo4118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://zf.zhonguo2118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://mg.zhonguo8118.cn

[F08] 遍历目录
来源：https://rm.zhonguo2118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://fi.zhonguo4118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://ez.zhonguo3118.cn

JS:   fs.readdirSync("dir")
来源：https://tm.zhonguo4118.cn

TS:   fs.readdirSync("dir")
来源：https://ms.zhonguo7118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://mj.zhonguo5118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://gi.zhonguo6118.cn

Ruby: Dir.children("dir")
来源：https://ls.zhonguo7118.cn

C#:   Directory.GetFiles("dir")
来源：https://qd.zhonguo8118.cn

[F09] 获取文件大小
来源：https://zk.zhonguo6118.cn

Py:   os.path.getsize("a.txt")
来源：https://fv.zhonguo3118.cn

PHP:  filesize("a.txt");
来源：https://ao.zhonguo2118.cn

JS:   fs.statSync("a.txt").size
来源：https://ee.zhonguo4118.cn

TS:   fs.statSync("a.txt").size
来源：https://wj.zhonguo6118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://un.zhonguo4118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://on.zhonguo8118.cn

Ruby: File.size("a.txt")
来源：https://bm.zhonguo8118.cn

C#:   new FileInfo("a.txt").Length
来源：https://sm.zhonguo7118.cn

[F10] 取文件扩展名 / 文件名
来源：https://ve.zhonguo3118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://tq.zhonguo5118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://vv.zhonguo5118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://zg.zhonguo4118.cn

TS:   path.extname("a.txt")
来源：https://vp.zhonguo4118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://er.zhonguo2118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://ve.zhonguo8118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://fu.zhonguo8118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://jh.zhonguo8118.cn

[F11] 复制与移动文件
来源：https://uv.zhonguo5118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://lj.zhonguo2118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ot.zhonguo6118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://af.zhonguo4118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://fn.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://uf.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://jy.zhonguo2118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://sy.zhonguo1118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://cv.zhonguo8118.cn

[F12] CSV 读写
来源：https://hm.zhonguo4118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://nx.zhonguo3118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://pc.zhonguo1118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://bx.zhonguo4118.cn

TS:   // 同上
来源：https://er.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://nd.zhonguo5118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://gb.zhonguo8118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://nc.zhonguo3118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://yu.zhonguo6118.cn

================================================================================
来源：https://pz.zhonguo8118.cn

G. 面向对象
来源：https://oq.zhonguo7118.cn

================================================================================
来源：https://mw.zhonguo4118.cn

[G01] 定义类
来源：https://yw.zhonguo8118.cn

Py:   class User: pass
来源：https://xb.zhonguo3118.cn

PHP:  class User {}
来源：https://wz.zhonguo6118.cn

JS:   class User {}
来源：https://kv.zhonguo5118.cn

TS:   class User { name: string = ""; }
来源：https://dp.zhonguo3118.cn

Java: class User {}
来源：https://nu.zhonguo2118.cn

Go:   type User struct { Name string }
来源：https://mu.zhonguo6118.cn

Ruby: class User; end
来源：https://ao.zhonguo8118.cn

C#:   class User {}
来源：https://ly.zhonguo1118.cn

[G02] 构造函数
来源：https://rn.zhonguo8118.cn

Py:   def __init__(self, name): self.name = name
来源：https://hw.zhonguo3118.cn

PHP:  public function __construct(public string $name) {}
来源：https://hl.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://yc.zhonguo4118.cn

TS:   constructor(public name: string) {}
来源：https://ok.zhonguo1118.cn

Java: User(String name) { this.name = name; }
来源：https://yn.zhonguo3118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://fh.zhonguo3118.cn

Ruby: def initialize(name); @name = name; end
来源：https://yc.zhonguo8118.cn

C#:   public User(string name) { Name = name; }
来源：https://kz.zhonguo3118.cn

[G03] 实例属性
来源：https://hf.zhonguo7118.cn

Py:   self.name = "x"
来源：https://pz.zhonguo1118.cn

PHP:  public string $name = "x";
来源：https://rw.zhonguo6118.cn

JS:   this.name = "x";
来源：https://mi.zhonguo1118.cn

TS:   name: string = "x";
来源：https://ck.zhonguo4118.cn

Java: private String name;
来源：https://hd.zhonguo3118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://kq.zhonguo1118.cn

Ruby: @name = "x"
来源：https://na.zhonguo8118.cn

C#:   public string Name { get; set; } = "x";
来源：https://yl.zhonguo2118.cn

[G04] 定义方法
来源：https://pr.zhonguo8118.cn

Py:   def greet(self): return self.name
来源：https://be.zhonguo4118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://uy.zhonguo1118.cn

JS:   greet() { return this.name; }
来源：https://cf.zhonguo2118.cn

TS:   greet(): string { return this.name; }
来源：https://vn.zhonguo6118.cn

Java: String greet() { return name; }
来源：https://hi.zhonguo5118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://kn.zhonguo6118.cn

Ruby: def greet; @name; end
来源：https://nn.zhonguo7118.cn

C#:   public string Greet() => Name;
来源：https://ut.zhonguo5118.cn

[G05] 继承
来源：https://sr.zhonguo2118.cn

Py:   class Admin(User): pass
来源：https://vf.zhonguo6118.cn

PHP:  class Admin extends User {}
来源：https://dy.zhonguo3118.cn

JS:   class Admin extends User {}
来源：https://xd.zhonguo7118.cn

TS:   class Admin extends User {}
来源：https://py.zhonguo1118.cn

Java: class Admin extends User {}
来源：https://xe.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://kp.zhonguo6118.cn

Ruby: class Admin < User; end
来源：https://ma.zhonguo1118.cn

C#:   class Admin : User {}
来源：https://gj.zhonguo6118.cn

[G06] 重写方法
来源：https://uv.zhonguo8118.cn

Py:   def greet(self): return "admin"
来源：https://vh.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://do.zhonguo6118.cn

JS:   greet() { return "admin"; }
来源：https://dh.zhonguo1118.cn

TS:   greet(): string { return "admin"; }
来源：https://lc.zhonguo3118.cn

Java: @Override String greet() { return "admin"; }
来源：https://gl.zhonguo5118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://ke.zhonguo8118.cn

Ruby: def greet; "admin"; end
来源：https://nf.zhonguo4118.cn

C#:   public override string Greet() => "admin";
来源：https://kz.zhonguo3118.cn

[G07] 调用父类方法
来源：https://ts.zhonguo2118.cn

Py:   super().greet()
来源：https://qw.zhonguo5118.cn

PHP:  parent::greet();
来源：https://zq.zhonguo1118.cn

JS:   super.greet();
来源：https://ol.zhonguo3118.cn

TS:   super.greet();
来源：https://oy.zhonguo3118.cn

Java: super.greet();
来源：https://nv.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://we.zhonguo7118.cn

Ruby: super
来源：https://vf.zhonguo6118.cn

C#:   base.Greet();
来源：https://ly.zhonguo2118.cn

[G08] 静态方法与属性
来源：https://kq.zhonguo3118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://nt.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://tm.zhonguo2118.cn

JS:   static f() {}
来源：https://eh.zhonguo5118.cn

TS:   static f(): void {}
来源：https://mq.zhonguo8118.cn

Java: static void f() {}
来源：https://oo.zhonguo4118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://ge.zhonguo3118.cn

Ruby: def self.f; end
来源：https://wd.zhonguo6118.cn

C#:   public static void F() {}
来源：https://nd.zhonguo4118.cn

[G09] 接口 / 抽象类
来源：https://kc.zhonguo1118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ti.zhonguo4118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://vi.zhonguo4118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://kf.zhonguo7118.cn

TS:   interface Shape { area(): number; }
来源：https://yy.zhonguo6118.cn

Java: interface Shape { double area(); }
来源：https://rr.zhonguo7118.cn

Go:   type Shape interface { Area() float64 }
来源：https://id.zhonguo3118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://as.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://et.zhonguo4118.cn

[G10] 访问控制
来源：https://il.zhonguo8118.cn

Py:   约定 _protected / __private（不强制）
来源：https://nm.zhonguo1118.cn

PHP:  public / protected / private
来源：https://ep.zhonguo3118.cn

JS:   #private 字段；其余公开
来源：https://ld.zhonguo6118.cn

TS:   public / protected / private
来源：https://qt.zhonguo3118.cn

Java: public / protected / private / 默认包级
来源：https://dg.zhonguo8118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://hk.zhonguo7118.cn

Ruby: public / protected / private
来源：https://vw.zhonguo8118.cn

C#:   public / protected / private / internal
来源：https://ft.zhonguo4118.cn

[G11] getter / setter
来源：https://rr.zhonguo2118.cn

Py:   @property 与 @x.setter
来源：https://el.zhonguo1118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://mk.zhonguo8118.cn

JS:   get name() { return this._name; }
来源：https://ge.zhonguo5118.cn

TS:   get name(): string { return this._name; }
来源：https://uz.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://bf.zhonguo1118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://jn.zhonguo5118.cn

Ruby: attr_accessor :name
来源：https://tq.zhonguo3118.cn

C#:   public string Name { get; set; }
来源：https://nd.zhonguo7118.cn

[G12] 对象转字符串
来源：https://or.zhonguo8118.cn

Py:   def __str__(self): return self.name
来源：https://jx.zhonguo4118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ya.zhonguo4118.cn

JS:   toString() { return this.name; }
来源：https://ro.zhonguo7118.cn

TS:   toString(): string { return this.name; }
来源：https://dm.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://jd.zhonguo3118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://xt.zhonguo3118.cn

Ruby: def to_s; @name; end
来源：https://dy.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://hs.zhonguo6118.cn

[G13] 判断对象类型
来源：https://hm.zhonguo3118.cn

Py:   isinstance(u, User)
来源：https://el.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://zm.zhonguo3118.cn

JS:   u instanceof User
来源：https://di.zhonguo1118.cn

TS:   u instanceof User
来源：https://ya.zhonguo8118.cn


<!-- 参考信息 -->