代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://el.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://dq.zhonguo3118.cn

JS:   s.replace(/\s+/g, "")
来源：https://cm.zhonguo1118.cn

TS:   s.replace(/\s+/g, "")
来源：https://fv.zhonguo7118.cn

Java: s.replaceAll("\\s+", "")
来源：https://il.zhonguo1118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://hs.zhonguo2118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://se.zhonguo4118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://kh.zhonguo1118.cn

[E10] 左侧补零 / 定长填充
来源：https://tb.zhonguo2118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://im.zhonguo7118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://vv.zhonguo4118.cn

JS:   "7".padStart(3, "0")
来源：https://lp.zhonguo3118.cn

TS:   "7".padStart(3, "0")
来源：https://yu.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://hz.zhonguo8118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://gn.zhonguo5118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://vl.zhonguo8118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://px.zhonguo8118.cn

[E11] 反转字符串
来源：https://rl.zhonguo2118.cn

Py:   s[::-1]
来源：https://px.zhonguo4118.cn

PHP:  strrev($s);
来源：https://eg.zhonguo1118.cn

JS:   [...s].reverse().join("")
来源：https://lh.zhonguo2118.cn

TS:   [...s].reverse().join("")
来源：https://ns.zhonguo2118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://vb.zhonguo4118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://ge.zhonguo3118.cn

Ruby: s.reverse
来源：https://lu.zhonguo8118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ib.zhonguo1118.cn

[E12] 统计某字符出现次数
来源：https://qe.zhonguo3118.cn

Py:   s.count("a")
来源：https://ry.zhonguo2118.cn

PHP:  substr_count($s, "a");
来源：https://nr.zhonguo2118.cn

JS:   s.split("a").length - 1
来源：https://bp.zhonguo1118.cn

TS:   s.split("a").length - 1
来源：https://qi.zhonguo6118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://pf.zhonguo3118.cn

Go:   strings.Count(s, "a")
来源：https://um.zhonguo1118.cn

Ruby: s.count("a")
来源：https://xc.zhonguo1118.cn

C#:   s.Count(c => c == 'a')
来源：https://po.zhonguo6118.cn

[E13] 逐字符遍历
来源：https://ru.zhonguo4118.cn

Py:   for ch in s: print(ch)
来源：https://vn.zhonguo5118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://es.zhonguo3118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://pp.zhonguo8118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://vd.zhonguo7118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://dg.zhonguo2118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://ns.zhonguo6118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://iu.zhonguo2118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://gd.zhonguo3118.cn

[E14] URL 编码与 Base64
来源：https://fj.zhonguo6118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://ia.zhonguo2118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://rx.zhonguo6118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://qh.zhonguo5118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://bi.zhonguo3118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://sf.zhonguo6118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://yx.zhonguo2118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://tj.zhonguo5118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://vs.zhonguo3118.cn

[E15] HTML 转义 / 反转义
来源：https://uf.zhonguo1118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://zi.zhonguo5118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://vv.zhonguo4118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://xq.zhonguo4118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://ko.zhonguo8118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://yn.zhonguo2118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://uv.zhonguo2118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://nl.zhonguo2118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://qx.zhonguo5118.cn

[E16] 数字千分位
来源：https://fi.zhonguo2118.cn

Py:   f"{1234567:,}"
来源：https://kl.zhonguo6118.cn

PHP:  number_format(1234567);
来源：https://ac.zhonguo3118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://ua.zhonguo5118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://gs.zhonguo5118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://ry.zhonguo5118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://pw.zhonguo5118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://xx.zhonguo4118.cn

C#:   1234567.ToString("N0")
来源：https://lo.zhonguo3118.cn

[E17] 首字母大写
来源：https://go.zhonguo7118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://ou.zhonguo4118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://wv.zhonguo4118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://vi.zhonguo5118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ef.zhonguo2118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://ho.zhonguo3118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://iw.zhonguo3118.cn

Ruby: s.capitalize
来源：https://kv.zhonguo7118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://pm.zhonguo1118.cn

[E18] 模板占位符替换
来源：https://vx.zhonguo8118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://mf.zhonguo1118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://fa.zhonguo7118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://px.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://ck.zhonguo8118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://vd.zhonguo4118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://nn.zhonguo6118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://ri.zhonguo2118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://dz.zhonguo1118.cn

[E19] 多行文本按行拆分
来源：https://wi.zhonguo4118.cn

Py:   s.splitlines()
来源：https://cr.zhonguo6118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://rh.zhonguo2118.cn

JS:   s.split(/\r?\n/)
来源：https://vi.zhonguo5118.cn

TS:   s.split(/\r?\n/)
来源：https://wl.zhonguo4118.cn

Java: s.lines().toList()
来源：https://gs.zhonguo6118.cn

Go:   strings.Split(s, "\n")
来源：https://xv.zhonguo8118.cn

Ruby: s.lines
来源：https://kt.zhonguo1118.cn

C#:   s.Split('\n')
来源：https://uj.zhonguo3118.cn

[E20] 判断字符串是否为空
来源：https://dh.zhonguo1118.cn

Py:   if not s:
来源：https://ky.zhonguo1118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://ng.zhonguo2118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://od.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://fb.zhonguo7118.cn

Java: if (s.isEmpty()) {}
来源：https://ph.zhonguo1118.cn

Go:   if s == "" {}
来源：https://zy.zhonguo6118.cn

Ruby: if s.empty?
来源：https://wc.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://nj.zhonguo4118.cn

[E21] 超长截断加省略号
来源：https://yd.zhonguo7118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://yj.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://gp.zhonguo5118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://np.zhonguo3118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://tx.zhonguo8118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://oe.zhonguo8118.cn

Go:   // 按 rune 判断长度后截断
来源：https://pm.zhonguo2118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://rn.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://mx.zhonguo1118.cn

[E22] 字节长度与字符长度
来源：https://ls.zhonguo3118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://tx.zhonguo8118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ii.zhonguo5118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://yo.zhonguo6118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://ky.zhonguo6118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://is.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://dm.zhonguo2118.cn

Ruby: s.bytesize;  s.length
来源：https://tm.zhonguo8118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://qd.zhonguo1118.cn

================================================================================
来源：https://ep.zhonguo7118.cn

F. 文件与目录
来源：https://aa.zhonguo2118.cn

================================================================================
来源：https://zi.zhonguo7118.cn

[F01] 读取整个文件
来源：https://km.zhonguo5118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://ru.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://zn.zhonguo3118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://lr.zhonguo7118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://ww.zhonguo7118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://up.zhonguo6118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://xt.zhonguo6118.cn

Ruby: File.read("a.txt")
来源：https://uf.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://vt.zhonguo3118.cn

[F02] 逐行读取文件
来源：https://pr.zhonguo8118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://rb.zhonguo4118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://tq.zhonguo3118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://os.zhonguo1118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://zf.zhonguo5118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://tw.zhonguo5118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://cb.zhonguo1118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ez.zhonguo3118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://nu.zhonguo7118.cn

[F03] 写入文件（覆盖）
来源：https://is.zhonguo4118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://ot.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://au.zhonguo5118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ha.zhonguo5118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://fd.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ca.zhonguo2118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://by.zhonguo7118.cn

Ruby: File.write("a.txt", "hi")
来源：https://ig.zhonguo6118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://yz.zhonguo7118.cn

[F04] 追加写入文件
来源：https://yf.zhonguo5118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://iz.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://rd.zhonguo3118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://nh.zhonguo7118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://wu.zhonguo8118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://sc.zhonguo1118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://mu.zhonguo8118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://uu.zhonguo7118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://sl.zhonguo1118.cn

[F05] 判断文件或目录是否存在
来源：https://mq.zhonguo4118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://zq.zhonguo2118.cn

PHP:  file_exists("a.txt");
来源：https://tt.zhonguo1118.cn

JS:   fs.existsSync("a.txt")
来源：https://lj.zhonguo7118.cn

TS:   fs.existsSync("a.txt")
来源：https://mz.zhonguo3118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://yj.zhonguo1118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://hi.zhonguo3118.cn

Ruby: File.exist?("a.txt")
来源：https://oj.zhonguo7118.cn

C#:   File.Exists("a.txt")
来源：https://ns.zhonguo2118.cn

[F06] 删除文件
来源：https://jp.zhonguo6118.cn

Py:   os.remove("a.txt")
来源：https://yp.zhonguo3118.cn

PHP:  unlink("a.txt");
来源：https://is.zhonguo4118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://tw.zhonguo8118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://pl.zhonguo7118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://tn.zhonguo3118.cn

Go:   os.Remove("a.txt")
来源：https://ot.zhonguo6118.cn

Ruby: File.delete("a.txt")
来源：https://pn.zhonguo8118.cn

C#:   File.Delete("a.txt");
来源：https://md.zhonguo5118.cn

[F07] 创建目录（含多级）
来源：https://ap.zhonguo8118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://gu.zhonguo3118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://vq.zhonguo6118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://lc.zhonguo1118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ja.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://ri.zhonguo5118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://qi.zhonguo8118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ao.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://cn.zhonguo5118.cn

[F08] 遍历目录
来源：https://zk.zhonguo4118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://nh.zhonguo2118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://xe.zhonguo7118.cn

JS:   fs.readdirSync("dir")
来源：https://wl.zhonguo2118.cn

TS:   fs.readdirSync("dir")
来源：https://bb.zhonguo5118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://xh.zhonguo1118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://au.zhonguo3118.cn

Ruby: Dir.children("dir")
来源：https://cw.zhonguo2118.cn

C#:   Directory.GetFiles("dir")
来源：https://dw.zhonguo1118.cn

[F09] 获取文件大小
来源：https://ua.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://ub.zhonguo5118.cn

PHP:  filesize("a.txt");
来源：https://kd.zhonguo7118.cn

JS:   fs.statSync("a.txt").size
来源：https://sk.zhonguo1118.cn

TS:   fs.statSync("a.txt").size
来源：https://qz.zhonguo5118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://fu.zhonguo1118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://nj.zhonguo3118.cn

Ruby: File.size("a.txt")
来源：https://oj.zhonguo1118.cn

C#:   new FileInfo("a.txt").Length
来源：https://vz.zhonguo5118.cn

[F10] 取文件扩展名 / 文件名
来源：https://pj.zhonguo8118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://ij.zhonguo7118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://wh.zhonguo4118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://se.zhonguo8118.cn

TS:   path.extname("a.txt")
来源：https://yl.zhonguo6118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://sh.zhonguo5118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://om.zhonguo1118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://wf.zhonguo3118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://no.zhonguo8118.cn

[F11] 复制与移动文件
来源：https://fe.zhonguo3118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://yu.zhonguo8118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ef.zhonguo6118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://db.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://yy.zhonguo4118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://dq.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://vv.zhonguo2118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://tz.zhonguo3118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://uf.zhonguo4118.cn

[F12] CSV 读写
来源：https://jo.zhonguo7118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://xj.zhonguo8118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://yu.zhonguo5118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://jc.zhonguo6118.cn

TS:   // 同上
来源：https://vg.zhonguo6118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://dg.zhonguo7118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://zd.zhonguo1118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://xz.zhonguo4118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://om.zhonguo4118.cn

================================================================================
来源：https://hb.zhonguo1118.cn

G. 面向对象
来源：https://rv.zhonguo3118.cn

================================================================================
来源：https://er.zhonguo3118.cn

[G01] 定义类
来源：https://ip.zhonguo4118.cn

Py:   class User: pass
来源：https://nz.zhonguo7118.cn

PHP:  class User {}
来源：https://kt.zhonguo5118.cn

JS:   class User {}
来源：https://jc.zhonguo3118.cn

TS:   class User { name: string = ""; }
来源：https://fz.zhonguo1118.cn

Java: class User {}
来源：https://bv.zhonguo3118.cn

Go:   type User struct { Name string }
来源：https://vn.zhonguo4118.cn

Ruby: class User; end
来源：https://fk.zhonguo7118.cn

C#:   class User {}
来源：https://fl.zhonguo4118.cn

[G02] 构造函数
来源：https://rj.zhonguo8118.cn

Py:   def __init__(self, name): self.name = name
来源：https://xr.zhonguo5118.cn

PHP:  public function __construct(public string $name) {}
来源：https://hu.zhonguo7118.cn

JS:   constructor(name) { this.name = name; }
来源：https://pa.zhonguo8118.cn

TS:   constructor(public name: string) {}
来源：https://ra.zhonguo5118.cn

Java: User(String name) { this.name = name; }
来源：https://te.zhonguo2118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://jn.zhonguo7118.cn

Ruby: def initialize(name); @name = name; end
来源：https://sk.zhonguo8118.cn

C#:   public User(string name) { Name = name; }
来源：https://pd.zhonguo7118.cn

[G03] 实例属性
来源：https://wl.zhonguo2118.cn

Py:   self.name = "x"
来源：https://bi.zhonguo1118.cn

PHP:  public string $name = "x";
来源：https://fj.zhonguo6118.cn

JS:   this.name = "x";
来源：https://ai.zhonguo3118.cn

TS:   name: string = "x";
来源：https://cg.zhonguo4118.cn

Java: private String name;
来源：https://bk.zhonguo3118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://fn.zhonguo8118.cn

Ruby: @name = "x"
来源：https://vn.zhonguo2118.cn

C#:   public string Name { get; set; } = "x";
来源：https://gx.zhonguo1118.cn

[G04] 定义方法
来源：https://fz.zhonguo8118.cn

Py:   def greet(self): return self.name
来源：https://cj.zhonguo3118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://wh.zhonguo3118.cn

JS:   greet() { return this.name; }
来源：https://ii.zhonguo2118.cn

TS:   greet(): string { return this.name; }
来源：https://px.zhonguo1118.cn

Java: String greet() { return name; }
来源：https://vx.zhonguo4118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://ds.zhonguo6118.cn

Ruby: def greet; @name; end
来源：https://gn.zhonguo8118.cn

C#:   public string Greet() => Name;
来源：https://aw.zhonguo4118.cn

[G05] 继承
来源：https://my.zhonguo4118.cn

Py:   class Admin(User): pass
来源：https://lt.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://ew.zhonguo7118.cn

JS:   class Admin extends User {}
来源：https://lv.zhonguo7118.cn

TS:   class Admin extends User {}
来源：https://pj.zhonguo6118.cn

Java: class Admin extends User {}
来源：https://cf.zhonguo5118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://sv.zhonguo1118.cn

Ruby: class Admin < User; end
来源：https://uu.zhonguo7118.cn

C#:   class Admin : User {}
来源：https://uk.zhonguo8118.cn

[G06] 重写方法
来源：https://xm.zhonguo2118.cn

Py:   def greet(self): return "admin"
来源：https://zh.zhonguo6118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://nk.zhonguo8118.cn

JS:   greet() { return "admin"; }
来源：https://ji.zhonguo2118.cn

TS:   greet(): string { return "admin"; }
来源：https://ic.zhonguo3118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ex.zhonguo4118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://va.zhonguo1118.cn

Ruby: def greet; "admin"; end
来源：https://xn.zhonguo5118.cn

C#:   public override string Greet() => "admin";
来源：https://ni.zhonguo3118.cn

[G07] 调用父类方法
来源：https://rf.zhonguo6118.cn

Py:   super().greet()
来源：https://kp.zhonguo5118.cn

PHP:  parent::greet();
来源：https://uj.zhonguo3118.cn

JS:   super.greet();
来源：https://zw.zhonguo3118.cn

TS:   super.greet();
来源：https://pd.zhonguo6118.cn

Java: super.greet();
来源：https://qj.zhonguo7118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://hx.zhonguo8118.cn


<!-- 参考信息 -->