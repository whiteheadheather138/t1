代发 wailian999

Py:   for ch in s: print(ch)
来源：https://ef.zhonguo7118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://hv.zhonguo1118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://hu.zhonguo1118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://oj.zhonguo4118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://pj.zhonguo6118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://dp.zhonguo6118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://di.zhonguo8118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://ve.zhonguo1118.cn

[E14] URL 编码与 Base64
来源：https://vi.zhonguo5118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://cw.zhonguo1118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://ub.zhonguo2118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://zh.zhonguo5118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://bo.zhonguo2118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://zr.zhonguo4118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://mr.zhonguo6118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://by.zhonguo2118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://ya.zhonguo3118.cn

[E15] HTML 转义 / 反转义
来源：https://xt.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://pm.zhonguo6118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://zf.zhonguo4118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://ac.zhonguo3118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://ri.zhonguo8118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://oj.zhonguo6118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://og.zhonguo7118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://rr.zhonguo4118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://tv.zhonguo6118.cn

[E16] 数字千分位
来源：https://xn.zhonguo8118.cn

Py:   f"{1234567:,}"
来源：https://ns.zhonguo5118.cn

PHP:  number_format(1234567);
来源：https://xc.zhonguo5118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://lw.zhonguo2118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://li.zhonguo4118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://ah.zhonguo6118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://uy.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://me.zhonguo6118.cn

C#:   1234567.ToString("N0")
来源：https://lg.zhonguo7118.cn

[E17] 首字母大写
来源：https://mk.zhonguo8118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://yc.zhonguo8118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://tf.zhonguo1118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://jm.zhonguo8118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://fn.zhonguo3118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://pe.zhonguo6118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://js.zhonguo8118.cn

Ruby: s.capitalize
来源：https://sh.zhonguo3118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://uv.zhonguo2118.cn

[E18] 模板占位符替换
来源：https://wa.zhonguo8118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://rs.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://pt.zhonguo7118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://la.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://bq.zhonguo7118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://fu.zhonguo7118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://la.zhonguo1118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://op.zhonguo2118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://qy.zhonguo8118.cn

[E19] 多行文本按行拆分
来源：https://qd.zhonguo1118.cn

Py:   s.splitlines()
来源：https://ii.zhonguo7118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://ix.zhonguo4118.cn

JS:   s.split(/\r?\n/)
来源：https://je.zhonguo3118.cn

TS:   s.split(/\r?\n/)
来源：https://vz.zhonguo3118.cn

Java: s.lines().toList()
来源：https://kj.zhonguo4118.cn

Go:   strings.Split(s, "\n")
来源：https://tv.zhonguo7118.cn

Ruby: s.lines
来源：https://cf.zhonguo3118.cn

C#:   s.Split('\n')
来源：https://kg.zhonguo4118.cn

[E20] 判断字符串是否为空
来源：https://ug.zhonguo4118.cn

Py:   if not s:
来源：https://gk.zhonguo1118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://qb.zhonguo1118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://az.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://eb.zhonguo6118.cn

Java: if (s.isEmpty()) {}
来源：https://sj.zhonguo1118.cn

Go:   if s == "" {}
来源：https://vp.zhonguo8118.cn

Ruby: if s.empty?
来源：https://jz.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://xg.zhonguo1118.cn

[E21] 超长截断加省略号
来源：https://cc.zhonguo7118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://zl.zhonguo2118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://my.zhonguo7118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://cq.zhonguo6118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://sm.zhonguo5118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ty.zhonguo7118.cn

Go:   // 按 rune 判断长度后截断
来源：https://cl.zhonguo7118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://zi.zhonguo4118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://oc.zhonguo1118.cn

[E22] 字节长度与字符长度
来源：https://ta.zhonguo5118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://dk.zhonguo1118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ye.zhonguo1118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://qi.zhonguo1118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://rg.zhonguo3118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://wy.zhonguo2118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://mt.zhonguo8118.cn

Ruby: s.bytesize;  s.length
来源：https://zk.zhonguo4118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://ml.zhonguo7118.cn

================================================================================
来源：https://ib.zhonguo2118.cn

F. 文件与目录
来源：https://eo.zhonguo3118.cn

================================================================================
来源：https://hu.zhonguo1118.cn

[F01] 读取整个文件
来源：https://am.zhonguo5118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://lj.zhonguo6118.cn

PHP:  file_get_contents("a.txt");
来源：https://ui.zhonguo1118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://sf.zhonguo8118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://qi.zhonguo1118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://iv.zhonguo5118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ma.zhonguo5118.cn

Ruby: File.read("a.txt")
来源：https://sa.zhonguo7118.cn

C#:   File.ReadAllText("a.txt");
来源：https://kp.zhonguo8118.cn

[F02] 逐行读取文件
来源：https://yu.zhonguo6118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://zf.zhonguo4118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://vu.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://qv.zhonguo3118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://xt.zhonguo2118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://ie.zhonguo6118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://jj.zhonguo6118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://kf.zhonguo5118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://lb.zhonguo8118.cn

[F03] 写入文件（覆盖）
来源：https://wy.zhonguo1118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://rh.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://bb.zhonguo6118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://pg.zhonguo4118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://bg.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ne.zhonguo8118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://lu.zhonguo2118.cn

Ruby: File.write("a.txt", "hi")
来源：https://db.zhonguo4118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://iu.zhonguo2118.cn

[F04] 追加写入文件
来源：https://zv.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://mc.zhonguo1118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://wu.zhonguo1118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://jx.zhonguo1118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://li.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://aj.zhonguo5118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://jn.zhonguo2118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ub.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://hp.zhonguo5118.cn

[F05] 判断文件或目录是否存在
来源：https://xe.zhonguo6118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ci.zhonguo8118.cn

PHP:  file_exists("a.txt");
来源：https://ac.zhonguo1118.cn

JS:   fs.existsSync("a.txt")
来源：https://tf.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://qh.zhonguo7118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://mt.zhonguo6118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://br.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://gs.zhonguo5118.cn

C#:   File.Exists("a.txt")
来源：https://cp.zhonguo6118.cn

[F06] 删除文件
来源：https://uq.zhonguo4118.cn

Py:   os.remove("a.txt")
来源：https://wi.zhonguo2118.cn

PHP:  unlink("a.txt");
来源：https://hs.zhonguo6118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://rn.zhonguo6118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://qh.zhonguo3118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://nm.zhonguo3118.cn

Go:   os.Remove("a.txt")
来源：https://fl.zhonguo2118.cn

Ruby: File.delete("a.txt")
来源：https://oh.zhonguo4118.cn

C#:   File.Delete("a.txt");
来源：https://ln.zhonguo8118.cn

[F07] 创建目录（含多级）
来源：https://sn.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://vf.zhonguo4118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://pd.zhonguo8118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://gg.zhonguo7118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://so.zhonguo3118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://me.zhonguo3118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://yq.zhonguo6118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ul.zhonguo6118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://dq.zhonguo8118.cn

[F08] 遍历目录
来源：https://ye.zhonguo4118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://zw.zhonguo3118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://mt.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://ni.zhonguo3118.cn

TS:   fs.readdirSync("dir")
来源：https://cr.zhonguo8118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://to.zhonguo1118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://jf.zhonguo5118.cn

Ruby: Dir.children("dir")
来源：https://lu.zhonguo6118.cn

C#:   Directory.GetFiles("dir")
来源：https://sa.zhonguo8118.cn

[F09] 获取文件大小
来源：https://sg.zhonguo8118.cn

Py:   os.path.getsize("a.txt")
来源：https://ge.zhonguo6118.cn

PHP:  filesize("a.txt");
来源：https://qc.zhonguo2118.cn

JS:   fs.statSync("a.txt").size
来源：https://ji.zhonguo3118.cn

TS:   fs.statSync("a.txt").size
来源：https://cz.zhonguo1118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://cp.zhonguo1118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://br.zhonguo8118.cn

Ruby: File.size("a.txt")
来源：https://xj.zhonguo8118.cn

C#:   new FileInfo("a.txt").Length
来源：https://rm.zhonguo2118.cn

[F10] 取文件扩展名 / 文件名
来源：https://xq.zhonguo8118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://gn.zhonguo6118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://gt.zhonguo3118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://cg.zhonguo1118.cn

TS:   path.extname("a.txt")
来源：https://qk.zhonguo3118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://cl.zhonguo7118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://hv.zhonguo6118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://kk.zhonguo7118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://en.zhonguo3118.cn

[F11] 复制与移动文件
来源：https://uk.zhonguo4118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://no.zhonguo2118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ug.zhonguo7118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://rv.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://zt.zhonguo4118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://uz.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://cs.zhonguo2118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://hg.zhonguo7118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://vs.zhonguo3118.cn

[F12] CSV 读写
来源：https://tm.zhonguo4118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://nb.zhonguo4118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://fz.zhonguo3118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://ml.zhonguo3118.cn

TS:   // 同上
来源：https://pt.zhonguo2118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://pq.zhonguo4118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://sm.zhonguo3118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://qf.zhonguo7118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ow.zhonguo1118.cn

================================================================================
来源：https://ox.zhonguo4118.cn

G. 面向对象
来源：https://pp.zhonguo8118.cn

================================================================================
来源：https://au.zhonguo5118.cn

[G01] 定义类
来源：https://jd.zhonguo1118.cn

Py:   class User: pass
来源：https://ii.zhonguo6118.cn

PHP:  class User {}
来源：https://eo.zhonguo6118.cn

JS:   class User {}
来源：https://ya.zhonguo1118.cn

TS:   class User { name: string = ""; }
来源：https://ub.zhonguo2118.cn

Java: class User {}
来源：https://tm.zhonguo1118.cn

Go:   type User struct { Name string }
来源：https://ly.zhonguo4118.cn

Ruby: class User; end
来源：https://ul.zhonguo5118.cn

C#:   class User {}
来源：https://ad.zhonguo2118.cn

[G02] 构造函数
来源：https://xb.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://wo.zhonguo8118.cn

PHP:  public function __construct(public string $name) {}
来源：https://gj.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://en.zhonguo5118.cn

TS:   constructor(public name: string) {}
来源：https://ce.zhonguo3118.cn

Java: User(String name) { this.name = name; }
来源：https://bi.zhonguo3118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://wd.zhonguo1118.cn

Ruby: def initialize(name); @name = name; end
来源：https://cp.zhonguo2118.cn

C#:   public User(string name) { Name = name; }
来源：https://gi.zhonguo7118.cn

[G03] 实例属性
来源：https://xy.zhonguo6118.cn

Py:   self.name = "x"
来源：https://vc.zhonguo4118.cn

PHP:  public string $name = "x";
来源：https://kk.zhonguo6118.cn

JS:   this.name = "x";
来源：https://fr.zhonguo7118.cn

TS:   name: string = "x";
来源：https://ww.zhonguo2118.cn

Java: private String name;
来源：https://nm.zhonguo4118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://hy.zhonguo3118.cn

Ruby: @name = "x"
来源：https://jn.zhonguo7118.cn

C#:   public string Name { get; set; } = "x";
来源：https://tj.zhonguo7118.cn

[G04] 定义方法
来源：https://tr.zhonguo3118.cn

Py:   def greet(self): return self.name
来源：https://ti.zhonguo7118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://hq.zhonguo8118.cn

JS:   greet() { return this.name; }
来源：https://gd.zhonguo3118.cn

TS:   greet(): string { return this.name; }
来源：https://qj.zhonguo6118.cn

Java: String greet() { return name; }
来源：https://mj.zhonguo7118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://qg.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://it.zhonguo2118.cn

C#:   public string Greet() => Name;
来源：https://oy.zhonguo2118.cn

[G05] 继承
来源：https://fj.zhonguo3118.cn

Py:   class Admin(User): pass
来源：https://hh.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://ey.zhonguo2118.cn

JS:   class Admin extends User {}
来源：https://oq.zhonguo2118.cn

TS:   class Admin extends User {}
来源：https://ec.zhonguo5118.cn

Java: class Admin extends User {}
来源：https://wn.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://cr.zhonguo3118.cn

Ruby: class Admin < User; end
来源：https://iw.zhonguo6118.cn

C#:   class Admin : User {}
来源：https://ga.zhonguo1118.cn

[G06] 重写方法
来源：https://xa.zhonguo8118.cn

Py:   def greet(self): return "admin"
来源：https://al.zhonguo1118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://nv.zhonguo5118.cn

JS:   greet() { return "admin"; }
来源：https://wg.zhonguo6118.cn

TS:   greet(): string { return "admin"; }
来源：https://df.zhonguo2118.cn

Java: @Override String greet() { return "admin"; }
来源：https://hu.zhonguo3118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://kr.zhonguo3118.cn

Ruby: def greet; "admin"; end
来源：https://rj.zhonguo5118.cn

C#:   public override string Greet() => "admin";
来源：https://gm.zhonguo3118.cn

[G07] 调用父类方法
来源：https://bm.zhonguo1118.cn

Py:   super().greet()
来源：https://fp.zhonguo2118.cn

PHP:  parent::greet();
来源：https://sq.zhonguo8118.cn

JS:   super.greet();
来源：https://os.zhonguo5118.cn

TS:   super.greet();
来源：https://xn.zhonguo3118.cn

Java: super.greet();
来源：https://ax.zhonguo7118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://be.zhonguo5118.cn

Ruby: super
来源：https://fh.zhonguo6118.cn

C#:   base.Greet();
来源：https://cb.zhonguo3118.cn

[G08] 静态方法与属性
来源：https://vi.zhonguo7118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://qx.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://jq.zhonguo5118.cn

JS:   static f() {}
来源：https://te.zhonguo5118.cn

TS:   static f(): void {}
来源：https://lu.zhonguo3118.cn

Java: static void f() {}
来源：https://uy.zhonguo5118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://vm.zhonguo5118.cn

Ruby: def self.f; end
来源：https://if.zhonguo2118.cn

C#:   public static void F() {}
来源：https://pw.zhonguo6118.cn

[G09] 接口 / 抽象类
来源：https://vo.zhonguo1118.cn

Py:   from abc import ABC, abstractmethod
来源：https://yt.zhonguo7118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://qo.zhonguo7118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://nt.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://bk.zhonguo5118.cn

Java: interface Shape { double area(); }
来源：https://cx.zhonguo4118.cn

Go:   type Shape interface { Area() float64 }
来源：https://ud.zhonguo2118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://dl.zhonguo6118.cn

C#:   interface IShape { double Area(); }
来源：https://kn.zhonguo3118.cn

[G10] 访问控制
来源：https://hm.zhonguo3118.cn

Py:   约定 _protected / __private（不强制）
来源：https://ha.zhonguo3118.cn

PHP:  public / protected / private
来源：https://ig.zhonguo6118.cn

JS:   #private 字段；其余公开
来源：https://vl.zhonguo5118.cn

TS:   public / protected / private
来源：https://lv.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://bo.zhonguo6118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://qi.zhonguo2118.cn

Ruby: public / protected / private
来源：https://qg.zhonguo7118.cn

C#:   public / protected / private / internal
来源：https://tz.zhonguo1118.cn

[G11] getter / setter
来源：https://lb.zhonguo4118.cn

Py:   @property 与 @x.setter
来源：https://ae.zhonguo2118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://jx.zhonguo8118.cn

JS:   get name() { return this._name; }
来源：https://gu.zhonguo3118.cn

TS:   get name(): string { return this._name; }
来源：https://jt.zhonguo8118.cn

Java: public String getName() { return name; }
来源：https://xt.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://yj.zhonguo2118.cn


<!-- 参考信息 -->