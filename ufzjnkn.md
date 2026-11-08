代发 wailian999

TS:   "7".padStart(3, "0")
来源：https://qi.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://gv.zhonguo7118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://bb.zhonguo2118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://ub.zhonguo3118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://to.zhonguo7118.cn

[E11] 反转字符串
来源：https://jp.zhonguo1118.cn

Py:   s[::-1]
来源：https://gr.zhonguo2118.cn

PHP:  strrev($s);
来源：https://nz.zhonguo7118.cn

JS:   [...s].reverse().join("")
来源：https://lh.zhonguo7118.cn

TS:   [...s].reverse().join("")
来源：https://ax.zhonguo5118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://bc.zhonguo7118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://pc.zhonguo6118.cn

Ruby: s.reverse
来源：https://cn.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://cz.zhonguo3118.cn

[E12] 统计某字符出现次数
来源：https://ke.zhonguo5118.cn

Py:   s.count("a")
来源：https://am.zhonguo2118.cn

PHP:  substr_count($s, "a");
来源：https://qf.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://ey.zhonguo6118.cn

TS:   s.split("a").length - 1
来源：https://yg.zhonguo2118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://vg.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://ay.zhonguo6118.cn

Ruby: s.count("a")
来源：https://kk.zhonguo7118.cn

C#:   s.Count(c => c == 'a')
来源：https://me.zhonguo5118.cn

[E13] 逐字符遍历
来源：https://yw.zhonguo5118.cn

Py:   for ch in s: print(ch)
来源：https://jn.zhonguo5118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://ph.zhonguo5118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://sa.zhonguo7118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ki.zhonguo3118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://za.zhonguo5118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://ey.zhonguo3118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://dv.zhonguo8118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://qt.zhonguo3118.cn

[E14] URL 编码与 Base64
来源：https://bw.zhonguo8118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://si.zhonguo4118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://nq.zhonguo5118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://zb.zhonguo7118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://bf.zhonguo2118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://hy.zhonguo2118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://kx.zhonguo6118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://gh.zhonguo8118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://ba.zhonguo1118.cn

[E15] HTML 转义 / 反转义
来源：https://vp.zhonguo3118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://za.zhonguo5118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://dx.zhonguo4118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://lc.zhonguo5118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://ux.zhonguo7118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://se.zhonguo2118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://kh.zhonguo5118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://xa.zhonguo6118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://ex.zhonguo7118.cn

[E16] 数字千分位
来源：https://qq.zhonguo4118.cn

Py:   f"{1234567:,}"
来源：https://qd.zhonguo7118.cn

PHP:  number_format(1234567);
来源：https://bn.zhonguo6118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://wb.zhonguo6118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://ne.zhonguo6118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://zo.zhonguo1118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://lv.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://rh.zhonguo6118.cn

C#:   1234567.ToString("N0")
来源：https://jh.zhonguo8118.cn

[E17] 首字母大写
来源：https://ui.zhonguo5118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://wj.zhonguo2118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://sq.zhonguo2118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://qc.zhonguo2118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://lc.zhonguo4118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://vb.zhonguo1118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://vt.zhonguo7118.cn

Ruby: s.capitalize
来源：https://fu.zhonguo8118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://tc.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://gr.zhonguo7118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://fo.zhonguo2118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://np.zhonguo1118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://il.zhonguo7118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://cu.zhonguo3118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://qp.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://xi.zhonguo6118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://np.zhonguo7118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://es.zhonguo1118.cn

[E19] 多行文本按行拆分
来源：https://cp.zhonguo1118.cn

Py:   s.splitlines()
来源：https://tu.zhonguo2118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://nq.zhonguo4118.cn

JS:   s.split(/\r?\n/)
来源：https://xs.zhonguo8118.cn

TS:   s.split(/\r?\n/)
来源：https://ea.zhonguo2118.cn

Java: s.lines().toList()
来源：https://bb.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://mo.zhonguo8118.cn

Ruby: s.lines
来源：https://vk.zhonguo5118.cn

C#:   s.Split('\n')
来源：https://mo.zhonguo3118.cn

[E20] 判断字符串是否为空
来源：https://hz.zhonguo6118.cn

Py:   if not s:
来源：https://cz.zhonguo8118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://jm.zhonguo7118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ac.zhonguo7118.cn

TS:   if (s === "") {}
来源：https://rh.zhonguo7118.cn

Java: if (s.isEmpty()) {}
来源：https://pu.zhonguo7118.cn

Go:   if s == "" {}
来源：https://ev.zhonguo1118.cn

Ruby: if s.empty?
来源：https://bo.zhonguo1118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://ki.zhonguo3118.cn

[E21] 超长截断加省略号
来源：https://uz.zhonguo3118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://ug.zhonguo7118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://sf.zhonguo6118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://mi.zhonguo2118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://or.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ii.zhonguo7118.cn

Go:   // 按 rune 判断长度后截断
来源：https://xn.zhonguo2118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://bg.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://kx.zhonguo4118.cn

[E22] 字节长度与字符长度
来源：https://vr.zhonguo3118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://ht.zhonguo2118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ki.zhonguo6118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://ni.zhonguo6118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://fk.zhonguo7118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://zt.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://tv.zhonguo6118.cn

Ruby: s.bytesize;  s.length
来源：https://mm.zhonguo8118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://iw.zhonguo4118.cn

================================================================================
来源：https://os.zhonguo3118.cn

F. 文件与目录
来源：https://id.zhonguo5118.cn

================================================================================
来源：https://px.zhonguo2118.cn

[F01] 读取整个文件
来源：https://pl.zhonguo8118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://xd.zhonguo2118.cn

PHP:  file_get_contents("a.txt");
来源：https://wz.zhonguo2118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://ml.zhonguo3118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://xf.zhonguo2118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://dr.zhonguo5118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://zk.zhonguo3118.cn

Ruby: File.read("a.txt")
来源：https://gm.zhonguo5118.cn

C#:   File.ReadAllText("a.txt");
来源：https://hl.zhonguo7118.cn

[F02] 逐行读取文件
来源：https://fm.zhonguo1118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://fc.zhonguo1118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://oe.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://fm.zhonguo3118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://fu.zhonguo3118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://sx.zhonguo3118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://gx.zhonguo2118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ro.zhonguo3118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://tq.zhonguo3118.cn

[F03] 写入文件（覆盖）
来源：https://dg.zhonguo6118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://nm.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://wv.zhonguo3118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://jt.zhonguo7118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://tn.zhonguo4118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://xm.zhonguo4118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://dk.zhonguo6118.cn

Ruby: File.write("a.txt", "hi")
来源：https://dn.zhonguo7118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://hi.zhonguo8118.cn

[F04] 追加写入文件
来源：https://bm.zhonguo6118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://dw.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://tj.zhonguo4118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ld.zhonguo7118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ba.zhonguo6118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://qc.zhonguo6118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://ri.zhonguo5118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ry.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://rr.zhonguo7118.cn

[F05] 判断文件或目录是否存在
来源：https://jo.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://jg.zhonguo5118.cn

PHP:  file_exists("a.txt");
来源：https://tr.zhonguo8118.cn

JS:   fs.existsSync("a.txt")
来源：https://ku.zhonguo4118.cn

TS:   fs.existsSync("a.txt")
来源：https://wy.zhonguo5118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ga.zhonguo2118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://mo.zhonguo1118.cn

Ruby: File.exist?("a.txt")
来源：https://pc.zhonguo4118.cn

C#:   File.Exists("a.txt")
来源：https://oh.zhonguo2118.cn

[F06] 删除文件
来源：https://mr.zhonguo4118.cn

Py:   os.remove("a.txt")
来源：https://gn.zhonguo1118.cn

PHP:  unlink("a.txt");
来源：https://wv.zhonguo6118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://cn.zhonguo2118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://tq.zhonguo8118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://mt.zhonguo3118.cn

Go:   os.Remove("a.txt")
来源：https://go.zhonguo3118.cn

Ruby: File.delete("a.txt")
来源：https://qq.zhonguo6118.cn

C#:   File.Delete("a.txt");
来源：https://pz.zhonguo6118.cn

[F07] 创建目录（含多级）
来源：https://un.zhonguo7118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://vj.zhonguo2118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://xl.zhonguo5118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://cu.zhonguo5118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://pv.zhonguo6118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://sv.zhonguo6118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://bx.zhonguo2118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://py.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://ue.zhonguo6118.cn

[F08] 遍历目录
来源：https://if.zhonguo5118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ph.zhonguo7118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://uo.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://vx.zhonguo4118.cn

TS:   fs.readdirSync("dir")
来源：https://rx.zhonguo1118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://ge.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://on.zhonguo7118.cn

Ruby: Dir.children("dir")
来源：https://bs.zhonguo5118.cn

C#:   Directory.GetFiles("dir")
来源：https://st.zhonguo8118.cn

[F09] 获取文件大小
来源：https://le.zhonguo8118.cn

Py:   os.path.getsize("a.txt")
来源：https://wa.zhonguo1118.cn

PHP:  filesize("a.txt");
来源：https://am.zhonguo8118.cn

JS:   fs.statSync("a.txt").size
来源：https://kz.zhonguo3118.cn

TS:   fs.statSync("a.txt").size
来源：https://we.zhonguo5118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://xb.zhonguo5118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://ux.zhonguo3118.cn

Ruby: File.size("a.txt")
来源：https://hk.zhonguo3118.cn

C#:   new FileInfo("a.txt").Length
来源：https://dl.zhonguo7118.cn

[F10] 取文件扩展名 / 文件名
来源：https://wz.zhonguo1118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://xy.zhonguo8118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://zd.zhonguo6118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://xr.zhonguo7118.cn

TS:   path.extname("a.txt")
来源：https://rs.zhonguo8118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://tt.zhonguo2118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://hr.zhonguo1118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://cw.zhonguo4118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://aa.zhonguo8118.cn

[F11] 复制与移动文件
来源：https://tq.zhonguo7118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://qd.zhonguo5118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://qk.zhonguo6118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://kc.zhonguo2118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://uo.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://ub.zhonguo5118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://nr.zhonguo4118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://dv.zhonguo8118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://yl.zhonguo8118.cn

[F12] CSV 读写
来源：https://wb.zhonguo3118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ai.zhonguo7118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://da.zhonguo4118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://xd.zhonguo8118.cn

TS:   // 同上
来源：https://ux.zhonguo2118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://mt.zhonguo7118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://yz.zhonguo4118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://jw.zhonguo8118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ua.zhonguo3118.cn

================================================================================
来源：https://hw.zhonguo8118.cn

G. 面向对象
来源：https://gp.zhonguo5118.cn

================================================================================
来源：https://vd.zhonguo7118.cn

[G01] 定义类
来源：https://sf.zhonguo7118.cn

Py:   class User: pass
来源：https://ak.zhonguo6118.cn

PHP:  class User {}
来源：https://tj.zhonguo8118.cn

JS:   class User {}
来源：https://ox.zhonguo7118.cn

TS:   class User { name: string = ""; }
来源：https://zz.zhonguo3118.cn

Java: class User {}
来源：https://lq.zhonguo2118.cn

Go:   type User struct { Name string }
来源：https://de.zhonguo2118.cn

Ruby: class User; end
来源：https://of.zhonguo8118.cn

C#:   class User {}
来源：https://df.zhonguo6118.cn

[G02] 构造函数
来源：https://nl.zhonguo3118.cn

Py:   def __init__(self, name): self.name = name
来源：https://cj.zhonguo3118.cn

PHP:  public function __construct(public string $name) {}
来源：https://kh.zhonguo1118.cn

JS:   constructor(name) { this.name = name; }
来源：https://aw.zhonguo3118.cn

TS:   constructor(public name: string) {}
来源：https://be.zhonguo8118.cn

Java: User(String name) { this.name = name; }
来源：https://zp.zhonguo6118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://ej.zhonguo4118.cn

Ruby: def initialize(name); @name = name; end
来源：https://yk.zhonguo3118.cn

C#:   public User(string name) { Name = name; }
来源：https://jb.zhonguo7118.cn

[G03] 实例属性
来源：https://ac.zhonguo5118.cn

Py:   self.name = "x"
来源：https://sf.zhonguo4118.cn

PHP:  public string $name = "x";
来源：https://hr.zhonguo8118.cn

JS:   this.name = "x";
来源：https://ap.zhonguo5118.cn

TS:   name: string = "x";
来源：https://lt.zhonguo5118.cn

Java: private String name;
来源：https://vt.zhonguo4118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://mv.zhonguo3118.cn

Ruby: @name = "x"
来源：https://ml.zhonguo5118.cn

C#:   public string Name { get; set; } = "x";
来源：https://ve.zhonguo1118.cn

[G04] 定义方法
来源：https://zs.zhonguo1118.cn

Py:   def greet(self): return self.name
来源：https://ym.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://fq.zhonguo6118.cn

JS:   greet() { return this.name; }
来源：https://ox.zhonguo6118.cn

TS:   greet(): string { return this.name; }
来源：https://zf.zhonguo7118.cn

Java: String greet() { return name; }
来源：https://vi.zhonguo7118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://bp.zhonguo4118.cn

Ruby: def greet; @name; end
来源：https://gx.zhonguo5118.cn

C#:   public string Greet() => Name;
来源：https://hd.zhonguo2118.cn

[G05] 继承
来源：https://sb.zhonguo2118.cn

Py:   class Admin(User): pass
来源：https://it.zhonguo7118.cn

PHP:  class Admin extends User {}
来源：https://cn.zhonguo8118.cn

JS:   class Admin extends User {}
来源：https://cn.zhonguo3118.cn

TS:   class Admin extends User {}
来源：https://xf.zhonguo1118.cn

Java: class Admin extends User {}
来源：https://ap.zhonguo6118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://xb.zhonguo2118.cn

Ruby: class Admin < User; end
来源：https://um.zhonguo4118.cn

C#:   class Admin : User {}
来源：https://tf.zhonguo2118.cn

[G06] 重写方法
来源：https://yb.zhonguo5118.cn

Py:   def greet(self): return "admin"
来源：https://jg.zhonguo2118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://pg.zhonguo2118.cn

JS:   greet() { return "admin"; }
来源：https://ja.zhonguo1118.cn

TS:   greet(): string { return "admin"; }
来源：https://gv.zhonguo3118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ik.zhonguo7118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://lf.zhonguo2118.cn

Ruby: def greet; "admin"; end
来源：https://ax.zhonguo2118.cn

C#:   public override string Greet() => "admin";
来源：https://mp.zhonguo3118.cn

[G07] 调用父类方法
来源：https://sr.zhonguo5118.cn

Py:   super().greet()
来源：https://ps.zhonguo2118.cn

PHP:  parent::greet();
来源：https://aj.zhonguo8118.cn

JS:   super.greet();
来源：https://mz.zhonguo7118.cn

TS:   super.greet();
来源：https://un.zhonguo4118.cn

Java: super.greet();
来源：https://bq.zhonguo5118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://zp.zhonguo3118.cn

Ruby: super
来源：https://wr.zhonguo5118.cn

C#:   base.Greet();
来源：https://at.zhonguo1118.cn

[G08] 静态方法与属性
来源：https://dh.zhonguo2118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://kc.zhonguo6118.cn

PHP:  public static function f() {}
来源：https://wn.zhonguo5118.cn

JS:   static f() {}
来源：https://ea.zhonguo8118.cn

TS:   static f(): void {}
来源：https://xv.zhonguo3118.cn

Java: static void f() {}
来源：https://ji.zhonguo1118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://jx.zhonguo1118.cn

Ruby: def self.f; end
来源：https://rm.zhonguo1118.cn

C#:   public static void F() {}
来源：https://is.zhonguo1118.cn

[G09] 接口 / 抽象类
来源：https://em.zhonguo5118.cn


<!-- 参考信息 -->