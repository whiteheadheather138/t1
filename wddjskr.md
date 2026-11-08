代发 wailian999

[E10] 左侧补零 / 定长填充
来源：https://sx.zhonguo4118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ls.zhonguo4118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://vm.zhonguo4118.cn

JS:   "7".padStart(3, "0")
来源：https://ja.zhonguo4118.cn

TS:   "7".padStart(3, "0")
来源：https://sw.zhonguo2118.cn

Java: String.format("%03d", 7)
来源：https://en.zhonguo8118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://oa.zhonguo6118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://xl.zhonguo8118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://lf.zhonguo6118.cn

[E11] 反转字符串
来源：https://ag.zhonguo7118.cn

Py:   s[::-1]
来源：https://wb.zhonguo1118.cn

PHP:  strrev($s);
来源：https://wf.zhonguo1118.cn

JS:   [...s].reverse().join("")
来源：https://pj.zhonguo4118.cn

TS:   [...s].reverse().join("")
来源：https://it.zhonguo4118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://lk.zhonguo8118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://ux.zhonguo3118.cn

Ruby: s.reverse
来源：https://er.zhonguo7118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://un.zhonguo2118.cn

[E12] 统计某字符出现次数
来源：https://bh.zhonguo7118.cn

Py:   s.count("a")
来源：https://vw.zhonguo2118.cn

PHP:  substr_count($s, "a");
来源：https://ct.zhonguo1118.cn

JS:   s.split("a").length - 1
来源：https://hu.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://eu.zhonguo7118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://sc.zhonguo8118.cn

Go:   strings.Count(s, "a")
来源：https://nx.zhonguo3118.cn

Ruby: s.count("a")
来源：https://sn.zhonguo6118.cn

C#:   s.Count(c => c == 'a')
来源：https://yo.zhonguo7118.cn

[E13] 逐字符遍历
来源：https://pj.zhonguo6118.cn

Py:   for ch in s: print(ch)
来源：https://bl.zhonguo3118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://tq.zhonguo4118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://mh.zhonguo5118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://wl.zhonguo7118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://um.zhonguo1118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://cn.zhonguo7118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://pk.zhonguo3118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://uo.zhonguo7118.cn

[E14] URL 编码与 Base64
来源：https://lt.zhonguo2118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://yp.zhonguo3118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://ao.zhonguo1118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://xr.zhonguo7118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://cr.zhonguo4118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://aj.zhonguo4118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://rs.zhonguo2118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://os.zhonguo2118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://xn.zhonguo2118.cn

[E15] HTML 转义 / 反转义
来源：https://ao.zhonguo5118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://qz.zhonguo6118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://ts.zhonguo6118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://sb.zhonguo6118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://gu.zhonguo4118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://ss.zhonguo6118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://ru.zhonguo8118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://pv.zhonguo5118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://zp.zhonguo1118.cn

[E16] 数字千分位
来源：https://nk.zhonguo1118.cn

Py:   f"{1234567:,}"
来源：https://yp.zhonguo7118.cn

PHP:  number_format(1234567);
来源：https://um.zhonguo6118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://jb.zhonguo6118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://bc.zhonguo6118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://ji.zhonguo2118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://qq.zhonguo2118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://fc.zhonguo8118.cn

C#:   1234567.ToString("N0")
来源：https://lk.zhonguo2118.cn

[E17] 首字母大写
来源：https://jw.zhonguo3118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://mx.zhonguo2118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://yc.zhonguo3118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://rk.zhonguo3118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://az.zhonguo4118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://kx.zhonguo8118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://ah.zhonguo5118.cn

Ruby: s.capitalize
来源：https://kt.zhonguo1118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://ao.zhonguo5118.cn

[E18] 模板占位符替换
来源：https://mr.zhonguo3118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ko.zhonguo5118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://kw.zhonguo8118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://oq.zhonguo3118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://po.zhonguo2118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://uh.zhonguo1118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://hi.zhonguo5118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://hl.zhonguo8118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://ro.zhonguo6118.cn

[E19] 多行文本按行拆分
来源：https://uy.zhonguo2118.cn

Py:   s.splitlines()
来源：https://uq.zhonguo2118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://zq.zhonguo4118.cn

JS:   s.split(/\r?\n/)
来源：https://kc.zhonguo8118.cn

TS:   s.split(/\r?\n/)
来源：https://la.zhonguo7118.cn

Java: s.lines().toList()
来源：https://lp.zhonguo5118.cn

Go:   strings.Split(s, "\n")
来源：https://ie.zhonguo1118.cn

Ruby: s.lines
来源：https://rx.zhonguo4118.cn

C#:   s.Split('\n')
来源：https://fk.zhonguo8118.cn

[E20] 判断字符串是否为空
来源：https://ck.zhonguo7118.cn

Py:   if not s:
来源：https://cy.zhonguo2118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://rb.zhonguo8118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://jj.zhonguo1118.cn

TS:   if (s === "") {}
来源：https://of.zhonguo8118.cn

Java: if (s.isEmpty()) {}
来源：https://ps.zhonguo2118.cn

Go:   if s == "" {}
来源：https://nd.zhonguo1118.cn

Ruby: if s.empty?
来源：https://bc.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://kg.zhonguo5118.cn

[E21] 超长截断加省略号
来源：https://nt.zhonguo3118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://uf.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://wx.zhonguo8118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ax.zhonguo7118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://zm.zhonguo6118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://nn.zhonguo8118.cn

Go:   // 按 rune 判断长度后截断
来源：https://lz.zhonguo7118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://er.zhonguo3118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://er.zhonguo7118.cn

[E22] 字节长度与字符长度
来源：https://wh.zhonguo4118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://tb.zhonguo8118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://bi.zhonguo2118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://ku.zhonguo4118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://jl.zhonguo2118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://id.zhonguo7118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://xo.zhonguo5118.cn

Ruby: s.bytesize;  s.length
来源：https://ro.zhonguo8118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://nm.zhonguo1118.cn

================================================================================
来源：https://mz.zhonguo1118.cn

F. 文件与目录
来源：https://qf.zhonguo5118.cn

================================================================================
来源：https://ul.zhonguo1118.cn

[F01] 读取整个文件
来源：https://dd.zhonguo8118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://ue.zhonguo7118.cn

PHP:  file_get_contents("a.txt");
来源：https://yi.zhonguo5118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://qn.zhonguo8118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://ns.zhonguo8118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://bf.zhonguo4118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ko.zhonguo2118.cn

Ruby: File.read("a.txt")
来源：https://fy.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://ni.zhonguo6118.cn

[F02] 逐行读取文件
来源：https://eu.zhonguo2118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://mk.zhonguo5118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://ec.zhonguo3118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://cj.zhonguo3118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://vt.zhonguo3118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://ll.zhonguo3118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://or.zhonguo7118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://uj.zhonguo5118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ru.zhonguo6118.cn

[F03] 写入文件（覆盖）
来源：https://vt.zhonguo3118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://rt.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://if.zhonguo6118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://qs.zhonguo1118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ws.zhonguo6118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://sx.zhonguo6118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://gt.zhonguo4118.cn

Ruby: File.write("a.txt", "hi")
来源：https://sn.zhonguo5118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://qc.zhonguo3118.cn

[F04] 追加写入文件
来源：https://cv.zhonguo1118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://oz.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://is.zhonguo3118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://kh.zhonguo2118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://oo.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://gh.zhonguo2118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://fl.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://zq.zhonguo7118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://fl.zhonguo6118.cn

[F05] 判断文件或目录是否存在
来源：https://po.zhonguo2118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ov.zhonguo2118.cn

PHP:  file_exists("a.txt");
来源：https://sn.zhonguo8118.cn

JS:   fs.existsSync("a.txt")
来源：https://sm.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://ze.zhonguo7118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://rl.zhonguo8118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://kg.zhonguo7118.cn

Ruby: File.exist?("a.txt")
来源：https://fb.zhonguo1118.cn

C#:   File.Exists("a.txt")
来源：https://ha.zhonguo8118.cn

[F06] 删除文件
来源：https://wq.zhonguo3118.cn

Py:   os.remove("a.txt")
来源：https://zl.zhonguo2118.cn

PHP:  unlink("a.txt");
来源：https://gg.zhonguo8118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://zc.zhonguo4118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://qn.zhonguo5118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://hl.zhonguo5118.cn

Go:   os.Remove("a.txt")
来源：https://mn.zhonguo3118.cn

Ruby: File.delete("a.txt")
来源：https://en.zhonguo5118.cn

C#:   File.Delete("a.txt");
来源：https://ip.zhonguo3118.cn

[F07] 创建目录（含多级）
来源：https://uw.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://mo.zhonguo1118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://hf.zhonguo8118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://re.zhonguo3118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://vu.zhonguo7118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://ok.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://gu.zhonguo6118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://it.zhonguo8118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://xb.zhonguo1118.cn

[F08] 遍历目录
来源：https://hd.zhonguo7118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://oo.zhonguo3118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://no.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://ai.zhonguo4118.cn

TS:   fs.readdirSync("dir")
来源：https://wa.zhonguo6118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://ii.zhonguo6118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://rc.zhonguo6118.cn

Ruby: Dir.children("dir")
来源：https://hg.zhonguo7118.cn

C#:   Directory.GetFiles("dir")
来源：https://vh.zhonguo6118.cn

[F09] 获取文件大小
来源：https://du.zhonguo1118.cn

Py:   os.path.getsize("a.txt")
来源：https://lp.zhonguo3118.cn

PHP:  filesize("a.txt");
来源：https://yh.zhonguo2118.cn

JS:   fs.statSync("a.txt").size
来源：https://ov.zhonguo7118.cn

TS:   fs.statSync("a.txt").size
来源：https://ml.zhonguo1118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://jp.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://ms.zhonguo2118.cn

Ruby: File.size("a.txt")
来源：https://xz.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://bj.zhonguo2118.cn

[F10] 取文件扩展名 / 文件名
来源：https://md.zhonguo1118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://uu.zhonguo8118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://po.zhonguo6118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://dk.zhonguo7118.cn

TS:   path.extname("a.txt")
来源：https://uh.zhonguo8118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://mw.zhonguo6118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://et.zhonguo7118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://ke.zhonguo2118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://hl.zhonguo5118.cn

[F11] 复制与移动文件
来源：https://dd.zhonguo2118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://dy.zhonguo7118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://qc.zhonguo5118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://rs.zhonguo1118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ba.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://xs.zhonguo5118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ft.zhonguo1118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://mx.zhonguo4118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ro.zhonguo6118.cn

[F12] CSV 读写
来源：https://fy.zhonguo1118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://sx.zhonguo1118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://lr.zhonguo6118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://hx.zhonguo6118.cn

TS:   // 同上
来源：https://iv.zhonguo3118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://eb.zhonguo5118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://us.zhonguo7118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://ss.zhonguo4118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ol.zhonguo8118.cn

================================================================================
来源：https://st.zhonguo1118.cn

G. 面向对象
来源：https://bk.zhonguo1118.cn

================================================================================
来源：https://xc.zhonguo1118.cn

[G01] 定义类
来源：https://qp.zhonguo2118.cn

Py:   class User: pass
来源：https://uh.zhonguo2118.cn

PHP:  class User {}
来源：https://ay.zhonguo8118.cn

JS:   class User {}
来源：https://ns.zhonguo8118.cn

TS:   class User { name: string = ""; }
来源：https://qf.zhonguo7118.cn

Java: class User {}
来源：https://ai.zhonguo7118.cn

Go:   type User struct { Name string }
来源：https://fx.zhonguo2118.cn

Ruby: class User; end
来源：https://ca.zhonguo6118.cn

C#:   class User {}
来源：https://bf.zhonguo7118.cn

[G02] 构造函数
来源：https://sm.zhonguo3118.cn

Py:   def __init__(self, name): self.name = name
来源：https://jd.zhonguo2118.cn

PHP:  public function __construct(public string $name) {}
来源：https://ml.zhonguo2118.cn

JS:   constructor(name) { this.name = name; }
来源：https://lj.zhonguo7118.cn

TS:   constructor(public name: string) {}
来源：https://hv.zhonguo2118.cn

Java: User(String name) { this.name = name; }
来源：https://bm.zhonguo5118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://lq.zhonguo2118.cn

Ruby: def initialize(name); @name = name; end
来源：https://rc.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://nj.zhonguo6118.cn

[G03] 实例属性
来源：https://ax.zhonguo4118.cn

Py:   self.name = "x"
来源：https://nm.zhonguo6118.cn

PHP:  public string $name = "x";
来源：https://lh.zhonguo1118.cn

JS:   this.name = "x";
来源：https://ty.zhonguo4118.cn

TS:   name: string = "x";
来源：https://ne.zhonguo8118.cn

Java: private String name;
来源：https://hc.zhonguo7118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://br.zhonguo5118.cn

Ruby: @name = "x"
来源：https://kn.zhonguo3118.cn

C#:   public string Name { get; set; } = "x";
来源：https://no.zhonguo6118.cn

[G04] 定义方法
来源：https://vp.zhonguo3118.cn

Py:   def greet(self): return self.name
来源：https://uk.zhonguo1118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ml.zhonguo6118.cn

JS:   greet() { return this.name; }
来源：https://xv.zhonguo7118.cn

TS:   greet(): string { return this.name; }
来源：https://bg.zhonguo7118.cn

Java: String greet() { return name; }
来源：https://dt.zhonguo5118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://ya.zhonguo3118.cn

Ruby: def greet; @name; end
来源：https://ix.zhonguo4118.cn

C#:   public string Greet() => Name;
来源：https://vm.zhonguo3118.cn

[G05] 继承
来源：https://lb.zhonguo6118.cn

Py:   class Admin(User): pass
来源：https://qs.zhonguo8118.cn

PHP:  class Admin extends User {}
来源：https://wo.zhonguo5118.cn

JS:   class Admin extends User {}
来源：https://sa.zhonguo7118.cn

TS:   class Admin extends User {}
来源：https://ej.zhonguo4118.cn

Java: class Admin extends User {}
来源：https://aw.zhonguo8118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://em.zhonguo6118.cn

Ruby: class Admin < User; end
来源：https://fk.zhonguo2118.cn

C#:   class Admin : User {}
来源：https://qo.zhonguo4118.cn

[G06] 重写方法
来源：https://gv.zhonguo2118.cn

Py:   def greet(self): return "admin"
来源：https://ii.zhonguo3118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://yn.zhonguo8118.cn

JS:   greet() { return "admin"; }
来源：https://vg.zhonguo8118.cn

TS:   greet(): string { return "admin"; }
来源：https://so.zhonguo2118.cn

Java: @Override String greet() { return "admin"; }
来源：https://qj.zhonguo8118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://fs.zhonguo6118.cn

Ruby: def greet; "admin"; end
来源：https://rs.zhonguo3118.cn

C#:   public override string Greet() => "admin";
来源：https://om.zhonguo6118.cn

[G07] 调用父类方法
来源：https://sq.zhonguo6118.cn

Py:   super().greet()
来源：https://df.zhonguo1118.cn

PHP:  parent::greet();
来源：https://qr.zhonguo7118.cn

JS:   super.greet();
来源：https://hp.zhonguo6118.cn

TS:   super.greet();
来源：https://mj.zhonguo7118.cn

Java: super.greet();
来源：https://pd.zhonguo8118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://sk.zhonguo2118.cn

Ruby: super
来源：https://ot.zhonguo7118.cn

C#:   base.Greet();
来源：https://nn.zhonguo1118.cn

[G08] 静态方法与属性
来源：https://kp.zhonguo1118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://lm.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://wo.zhonguo4118.cn

JS:   static f() {}
来源：https://nr.zhonguo3118.cn

TS:   static f(): void {}
来源：https://lw.zhonguo7118.cn

Java: static void f() {}
来源：https://ut.zhonguo1118.cn


<!-- 参考信息 -->