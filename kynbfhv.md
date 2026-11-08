代发 wailian999

JS:   [...s].reverse().join("")
来源：https://mz.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://ag.zhonguo4118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://vr.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://zb.zhonguo7118.cn

Ruby: s.reverse
来源：https://rw.zhonguo5118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://lw.zhonguo7118.cn

[E12] 统计某字符出现次数
来源：https://fg.zhonguo5118.cn

Py:   s.count("a")
来源：https://gk.zhonguo1118.cn

PHP:  substr_count($s, "a");
来源：https://bo.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://ss.zhonguo8118.cn

TS:   s.split("a").length - 1
来源：https://mi.zhonguo7118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://gl.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://rl.zhonguo4118.cn

Ruby: s.count("a")
来源：https://pe.zhonguo4118.cn

C#:   s.Count(c => c == 'a')
来源：https://rv.zhonguo8118.cn

[E13] 逐字符遍历
来源：https://st.zhonguo8118.cn

Py:   for ch in s: print(ch)
来源：https://yu.zhonguo3118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://qu.zhonguo2118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://ub.zhonguo4118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ca.zhonguo1118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://xh.zhonguo8118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://so.zhonguo4118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://nu.zhonguo4118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://nv.zhonguo4118.cn

[E14] URL 编码与 Base64
来源：https://ww.zhonguo7118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://vu.zhonguo1118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://in.zhonguo5118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://jn.zhonguo3118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://xq.zhonguo1118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://ay.zhonguo2118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://vl.zhonguo7118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://wi.zhonguo2118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://qi.zhonguo2118.cn

[E15] HTML 转义 / 反转义
来源：https://uu.zhonguo7118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://cj.zhonguo3118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://ka.zhonguo7118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://om.zhonguo2118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://gh.zhonguo4118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://nx.zhonguo3118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://bn.zhonguo1118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://iz.zhonguo7118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://uv.zhonguo3118.cn

[E16] 数字千分位
来源：https://jd.zhonguo1118.cn

Py:   f"{1234567:,}"
来源：https://nm.zhonguo1118.cn

PHP:  number_format(1234567);
来源：https://lg.zhonguo5118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://qv.zhonguo3118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://rb.zhonguo3118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://gr.zhonguo2118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://yy.zhonguo3118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://xo.zhonguo4118.cn

C#:   1234567.ToString("N0")
来源：https://xx.zhonguo7118.cn

[E17] 首字母大写
来源：https://yd.zhonguo6118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://ux.zhonguo2118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://gq.zhonguo4118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://mp.zhonguo8118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://dg.zhonguo3118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://bk.zhonguo8118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://rv.zhonguo3118.cn

Ruby: s.capitalize
来源：https://dp.zhonguo8118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://gj.zhonguo3118.cn

[E18] 模板占位符替换
来源：https://vz.zhonguo2118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://pf.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://uc.zhonguo3118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://he.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://jt.zhonguo7118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://oh.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://zs.zhonguo8118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://rg.zhonguo7118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://zt.zhonguo5118.cn

[E19] 多行文本按行拆分
来源：https://lf.zhonguo6118.cn

Py:   s.splitlines()
来源：https://wh.zhonguo4118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://ak.zhonguo2118.cn

JS:   s.split(/\r?\n/)
来源：https://kn.zhonguo6118.cn

TS:   s.split(/\r?\n/)
来源：https://mb.zhonguo8118.cn

Java: s.lines().toList()
来源：https://ud.zhonguo6118.cn

Go:   strings.Split(s, "\n")
来源：https://em.zhonguo2118.cn

Ruby: s.lines
来源：https://xw.zhonguo4118.cn

C#:   s.Split('\n')
来源：https://rb.zhonguo4118.cn

[E20] 判断字符串是否为空
来源：https://kz.zhonguo8118.cn

Py:   if not s:
来源：https://ry.zhonguo8118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://fe.zhonguo3118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://dd.zhonguo2118.cn

TS:   if (s === "") {}
来源：https://cg.zhonguo4118.cn

Java: if (s.isEmpty()) {}
来源：https://id.zhonguo1118.cn

Go:   if s == "" {}
来源：https://yc.zhonguo1118.cn

Ruby: if s.empty?
来源：https://ye.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://wp.zhonguo7118.cn

[E21] 超长截断加省略号
来源：https://gt.zhonguo4118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://ev.zhonguo6118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://vl.zhonguo8118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ar.zhonguo4118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://cv.zhonguo5118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://bz.zhonguo4118.cn

Go:   // 按 rune 判断长度后截断
来源：https://fr.zhonguo4118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://mg.zhonguo8118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://ps.zhonguo7118.cn

[E22] 字节长度与字符长度
来源：https://ce.zhonguo5118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://ra.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://is.zhonguo8118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://qj.zhonguo6118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://eb.zhonguo1118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://dr.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://hf.zhonguo5118.cn

Ruby: s.bytesize;  s.length
来源：https://ga.zhonguo2118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://ik.zhonguo2118.cn

================================================================================
来源：https://qh.zhonguo2118.cn

F. 文件与目录
来源：https://ug.zhonguo6118.cn

================================================================================
来源：https://st.zhonguo6118.cn

[F01] 读取整个文件
来源：https://ey.zhonguo5118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://vu.zhonguo3118.cn

PHP:  file_get_contents("a.txt");
来源：https://vf.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://yp.zhonguo7118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://wx.zhonguo1118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://qd.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://rz.zhonguo7118.cn

Ruby: File.read("a.txt")
来源：https://zb.zhonguo1118.cn

C#:   File.ReadAllText("a.txt");
来源：https://do.zhonguo6118.cn

[F02] 逐行读取文件
来源：https://ht.zhonguo1118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://tr.zhonguo1118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://qx.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://zb.zhonguo5118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://tk.zhonguo7118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://kp.zhonguo7118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://jd.zhonguo2118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://se.zhonguo6118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ah.zhonguo8118.cn

[F03] 写入文件（覆盖）
来源：https://us.zhonguo8118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://pv.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://pf.zhonguo4118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://qe.zhonguo7118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://xu.zhonguo6118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://cz.zhonguo3118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://kt.zhonguo6118.cn

Ruby: File.write("a.txt", "hi")
来源：https://hf.zhonguo8118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://xr.zhonguo5118.cn

[F04] 追加写入文件
来源：https://aj.zhonguo1118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://fb.zhonguo5118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://vn.zhonguo6118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://oo.zhonguo7118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://hz.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://wr.zhonguo6118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://le.zhonguo3118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://kb.zhonguo3118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://gy.zhonguo3118.cn

[F05] 判断文件或目录是否存在
来源：https://kb.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://vu.zhonguo6118.cn

PHP:  file_exists("a.txt");
来源：https://xn.zhonguo6118.cn

JS:   fs.existsSync("a.txt")
来源：https://cm.zhonguo8118.cn

TS:   fs.existsSync("a.txt")
来源：https://zk.zhonguo5118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://fs.zhonguo8118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ue.zhonguo2118.cn

Ruby: File.exist?("a.txt")
来源：https://ht.zhonguo7118.cn

C#:   File.Exists("a.txt")
来源：https://on.zhonguo4118.cn

[F06] 删除文件
来源：https://tt.zhonguo7118.cn

Py:   os.remove("a.txt")
来源：https://xv.zhonguo8118.cn

PHP:  unlink("a.txt");
来源：https://zu.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://zz.zhonguo6118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://ep.zhonguo4118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://df.zhonguo6118.cn

Go:   os.Remove("a.txt")
来源：https://he.zhonguo2118.cn

Ruby: File.delete("a.txt")
来源：https://cf.zhonguo1118.cn

C#:   File.Delete("a.txt");
来源：https://tl.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://zm.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://zw.zhonguo6118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://ho.zhonguo4118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://kg.zhonguo5118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://lm.zhonguo1118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://eh.zhonguo8118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://wm.zhonguo2118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://as.zhonguo6118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://jp.zhonguo2118.cn

[F08] 遍历目录
来源：https://lw.zhonguo7118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ob.zhonguo7118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://io.zhonguo5118.cn

JS:   fs.readdirSync("dir")
来源：https://eo.zhonguo6118.cn

TS:   fs.readdirSync("dir")
来源：https://eb.zhonguo7118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://kh.zhonguo6118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://dq.zhonguo6118.cn

Ruby: Dir.children("dir")
来源：https://wk.zhonguo1118.cn

C#:   Directory.GetFiles("dir")
来源：https://wa.zhonguo6118.cn

[F09] 获取文件大小
来源：https://ft.zhonguo2118.cn

Py:   os.path.getsize("a.txt")
来源：https://jt.zhonguo5118.cn

PHP:  filesize("a.txt");
来源：https://hr.zhonguo3118.cn

JS:   fs.statSync("a.txt").size
来源：https://vx.zhonguo5118.cn

TS:   fs.statSync("a.txt").size
来源：https://ho.zhonguo3118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://ez.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://eb.zhonguo5118.cn

Ruby: File.size("a.txt")
来源：https://jt.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://py.zhonguo5118.cn

[F10] 取文件扩展名 / 文件名
来源：https://fd.zhonguo5118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://os.zhonguo7118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://lg.zhonguo6118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://sr.zhonguo5118.cn

TS:   path.extname("a.txt")
来源：https://bl.zhonguo3118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://qu.zhonguo1118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://eb.zhonguo1118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://qw.zhonguo3118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://az.zhonguo8118.cn

[F11] 复制与移动文件
来源：https://jv.zhonguo6118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://wc.zhonguo8118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://xj.zhonguo3118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://qi.zhonguo5118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://tv.zhonguo7118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://xe.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://lg.zhonguo1118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://rd.zhonguo2118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://pe.zhonguo3118.cn

[F12] CSV 读写
来源：https://lr.zhonguo2118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://vd.zhonguo5118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://gu.zhonguo1118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://zf.zhonguo7118.cn

TS:   // 同上
来源：https://xy.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://ni.zhonguo6118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://ga.zhonguo5118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://nk.zhonguo4118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://rx.zhonguo5118.cn

================================================================================
来源：https://kt.zhonguo1118.cn

G. 面向对象
来源：https://uo.zhonguo7118.cn

================================================================================
来源：https://nh.zhonguo7118.cn

[G01] 定义类
来源：https://iz.zhonguo4118.cn

Py:   class User: pass
来源：https://xa.zhonguo5118.cn

PHP:  class User {}
来源：https://cx.zhonguo8118.cn

JS:   class User {}
来源：https://bh.zhonguo5118.cn

TS:   class User { name: string = ""; }
来源：https://if.zhonguo5118.cn

Java: class User {}
来源：https://wo.zhonguo7118.cn

Go:   type User struct { Name string }
来源：https://ai.zhonguo3118.cn

Ruby: class User; end
来源：https://ac.zhonguo6118.cn

C#:   class User {}
来源：https://wt.zhonguo4118.cn

[G02] 构造函数
来源：https://nh.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://bm.zhonguo4118.cn

PHP:  public function __construct(public string $name) {}
来源：https://xa.zhonguo5118.cn

JS:   constructor(name) { this.name = name; }
来源：https://nv.zhonguo8118.cn

TS:   constructor(public name: string) {}
来源：https://ov.zhonguo5118.cn

Java: User(String name) { this.name = name; }
来源：https://mj.zhonguo4118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://xk.zhonguo8118.cn

Ruby: def initialize(name); @name = name; end
来源：https://kw.zhonguo2118.cn

C#:   public User(string name) { Name = name; }
来源：https://lb.zhonguo4118.cn

[G03] 实例属性
来源：https://mm.zhonguo5118.cn

Py:   self.name = "x"
来源：https://ef.zhonguo5118.cn

PHP:  public string $name = "x";
来源：https://we.zhonguo8118.cn

JS:   this.name = "x";
来源：https://yl.zhonguo5118.cn

TS:   name: string = "x";
来源：https://nm.zhonguo8118.cn

Java: private String name;
来源：https://pl.zhonguo4118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://rf.zhonguo7118.cn

Ruby: @name = "x"
来源：https://dz.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://hg.zhonguo2118.cn

[G04] 定义方法
来源：https://ju.zhonguo7118.cn

Py:   def greet(self): return self.name
来源：https://uc.zhonguo4118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ru.zhonguo7118.cn

JS:   greet() { return this.name; }
来源：https://ca.zhonguo1118.cn

TS:   greet(): string { return this.name; }
来源：https://wi.zhonguo8118.cn

Java: String greet() { return name; }
来源：https://zv.zhonguo4118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://ox.zhonguo5118.cn

Ruby: def greet; @name; end
来源：https://gk.zhonguo8118.cn

C#:   public string Greet() => Name;
来源：https://jd.zhonguo3118.cn

[G05] 继承
来源：https://ua.zhonguo3118.cn

Py:   class Admin(User): pass
来源：https://zw.zhonguo5118.cn

PHP:  class Admin extends User {}
来源：https://do.zhonguo3118.cn

JS:   class Admin extends User {}
来源：https://rv.zhonguo2118.cn

TS:   class Admin extends User {}
来源：https://ky.zhonguo2118.cn

Java: class Admin extends User {}
来源：https://zb.zhonguo2118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://zh.zhonguo2118.cn

Ruby: class Admin < User; end
来源：https://oe.zhonguo6118.cn

C#:   class Admin : User {}
来源：https://uf.zhonguo4118.cn

[G06] 重写方法
来源：https://ln.zhonguo6118.cn

Py:   def greet(self): return "admin"
来源：https://ls.zhonguo5118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://gz.zhonguo8118.cn

JS:   greet() { return "admin"; }
来源：https://uj.zhonguo7118.cn

TS:   greet(): string { return "admin"; }
来源：https://xy.zhonguo6118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ga.zhonguo5118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://vo.zhonguo5118.cn

Ruby: def greet; "admin"; end
来源：https://aw.zhonguo7118.cn

C#:   public override string Greet() => "admin";
来源：https://xc.zhonguo5118.cn

[G07] 调用父类方法
来源：https://eu.zhonguo8118.cn

Py:   super().greet()
来源：https://sm.zhonguo1118.cn

PHP:  parent::greet();
来源：https://dy.zhonguo2118.cn

JS:   super.greet();
来源：https://eg.zhonguo7118.cn

TS:   super.greet();
来源：https://rj.zhonguo4118.cn

Java: super.greet();
来源：https://ee.zhonguo6118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://dy.zhonguo2118.cn

Ruby: super
来源：https://vj.zhonguo8118.cn

C#:   base.Greet();
来源：https://mh.zhonguo8118.cn

[G08] 静态方法与属性
来源：https://kb.zhonguo8118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://cq.zhonguo6118.cn

PHP:  public static function f() {}
来源：https://bm.zhonguo3118.cn

JS:   static f() {}
来源：https://ea.zhonguo7118.cn

TS:   static f(): void {}
来源：https://sd.zhonguo8118.cn

Java: static void f() {}
来源：https://au.zhonguo6118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://aq.zhonguo7118.cn

Ruby: def self.f; end
来源：https://vu.zhonguo4118.cn

C#:   public static void F() {}
来源：https://mn.zhonguo6118.cn

[G09] 接口 / 抽象类
来源：https://pw.zhonguo6118.cn

Py:   from abc import ABC, abstractmethod
来源：https://vb.zhonguo2118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://oy.zhonguo1118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://fx.zhonguo4118.cn

TS:   interface Shape { area(): number; }
来源：https://vp.zhonguo4118.cn

Java: interface Shape { double area(); }
来源：https://co.zhonguo1118.cn

Go:   type Shape interface { Area() float64 }
来源：https://lt.zhonguo6118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://mm.zhonguo4118.cn

C#:   interface IShape { double Area(); }
来源：https://rw.zhonguo3118.cn


<!-- 参考信息 -->