代发 wailian999

TS:   s.replaceAll("a", "b")
来源：https://fm.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://cz.zhonguo6118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ki.zhonguo4118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://lx.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://bu.zhonguo1118.cn

[E07] 按分隔符拆分
来源：https://yl.zhonguo7118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://kr.zhonguo1118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://za.zhonguo1118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://vx.zhonguo5118.cn

TS:   s.split(",")
来源：https://vr.zhonguo5118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://ru.zhonguo2118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ix.zhonguo2118.cn

Ruby: s.split(",");  s.split
来源：https://yb.zhonguo7118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://mv.zhonguo3118.cn

[E08] 数组按分隔符合并
来源：https://es.zhonguo6118.cn

Py:   ",".join(items)
来源：https://je.zhonguo8118.cn

PHP:  implode(",", $items);
来源：https://qe.zhonguo2118.cn

JS:   items.join(",")
来源：https://nr.zhonguo1118.cn

TS:   items.join(",")
来源：https://de.zhonguo4118.cn

Java: String.join(",", items)
来源：https://ls.zhonguo8118.cn

Go:   strings.Join(items, ",")
来源：https://fl.zhonguo4118.cn

Ruby: items.join(",")
来源：https://qw.zhonguo1118.cn

C#:   string.Join(",", items)
来源：https://wg.zhonguo4118.cn

[E09] 去除所有空白字符
来源：https://pz.zhonguo3118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://sq.zhonguo1118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://bi.zhonguo5118.cn

JS:   s.replace(/\s+/g, "")
来源：https://eh.zhonguo7118.cn

TS:   s.replace(/\s+/g, "")
来源：https://by.zhonguo4118.cn

Java: s.replaceAll("\\s+", "")
来源：https://na.zhonguo3118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://yx.zhonguo8118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://cp.zhonguo2118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://ww.zhonguo5118.cn

[E10] 左侧补零 / 定长填充
来源：https://ss.zhonguo4118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://es.zhonguo8118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://pe.zhonguo2118.cn

JS:   "7".padStart(3, "0")
来源：https://wz.zhonguo3118.cn

TS:   "7".padStart(3, "0")
来源：https://qh.zhonguo1118.cn

Java: String.format("%03d", 7)
来源：https://vl.zhonguo7118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://dw.zhonguo8118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://qg.zhonguo3118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://gp.zhonguo2118.cn

[E11] 反转字符串
来源：https://dv.zhonguo1118.cn

Py:   s[::-1]
来源：https://mi.zhonguo3118.cn

PHP:  strrev($s);
来源：https://aq.zhonguo5118.cn

JS:   [...s].reverse().join("")
来源：https://ar.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://te.zhonguo8118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://rm.zhonguo4118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://se.zhonguo8118.cn

Ruby: s.reverse
来源：https://pa.zhonguo3118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://jf.zhonguo7118.cn

[E12] 统计某字符出现次数
来源：https://ep.zhonguo7118.cn

Py:   s.count("a")
来源：https://me.zhonguo2118.cn

PHP:  substr_count($s, "a");
来源：https://qn.zhonguo1118.cn

JS:   s.split("a").length - 1
来源：https://gd.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://uj.zhonguo7118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://kd.zhonguo5118.cn

Go:   strings.Count(s, "a")
来源：https://gy.zhonguo4118.cn

Ruby: s.count("a")
来源：https://ca.zhonguo2118.cn

C#:   s.Count(c => c == 'a')
来源：https://ko.zhonguo6118.cn

[E13] 逐字符遍历
来源：https://do.zhonguo3118.cn

Py:   for ch in s: print(ch)
来源：https://er.zhonguo5118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://ic.zhonguo6118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://jn.zhonguo2118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://oa.zhonguo2118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://ll.zhonguo3118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://th.zhonguo7118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://gp.zhonguo6118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://cf.zhonguo6118.cn

[E14] URL 编码与 Base64
来源：https://eo.zhonguo8118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://gh.zhonguo6118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://vv.zhonguo1118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://so.zhonguo7118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://ch.zhonguo8118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://ih.zhonguo5118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://xl.zhonguo5118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://ox.zhonguo7118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://vq.zhonguo5118.cn

[E15] HTML 转义 / 反转义
来源：https://js.zhonguo1118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://wk.zhonguo1118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://oj.zhonguo6118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://es.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://ey.zhonguo3118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://ui.zhonguo6118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://zu.zhonguo8118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://wh.zhonguo1118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://wf.zhonguo7118.cn

[E16] 数字千分位
来源：https://qr.zhonguo3118.cn

Py:   f"{1234567:,}"
来源：https://uh.zhonguo3118.cn

PHP:  number_format(1234567);
来源：https://jt.zhonguo3118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://eg.zhonguo2118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://aq.zhonguo5118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://to.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://ha.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://uq.zhonguo2118.cn

C#:   1234567.ToString("N0")
来源：https://yl.zhonguo3118.cn

[E17] 首字母大写
来源：https://il.zhonguo6118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://ym.zhonguo5118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://nc.zhonguo5118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://te.zhonguo6118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://aa.zhonguo4118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://tt.zhonguo7118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://wt.zhonguo2118.cn

Ruby: s.capitalize
来源：https://um.zhonguo4118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://xw.zhonguo1118.cn

[E18] 模板占位符替换
来源：https://bj.zhonguo4118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ey.zhonguo8118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://yv.zhonguo1118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://lu.zhonguo8118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://mk.zhonguo1118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://ke.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://so.zhonguo3118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://tq.zhonguo3118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://ax.zhonguo5118.cn

[E19] 多行文本按行拆分
来源：https://vi.zhonguo3118.cn

Py:   s.splitlines()
来源：https://za.zhonguo6118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://hm.zhonguo2118.cn

JS:   s.split(/\r?\n/)
来源：https://mz.zhonguo7118.cn

TS:   s.split(/\r?\n/)
来源：https://pr.zhonguo5118.cn

Java: s.lines().toList()
来源：https://pw.zhonguo3118.cn

Go:   strings.Split(s, "\n")
来源：https://rj.zhonguo5118.cn

Ruby: s.lines
来源：https://hl.zhonguo7118.cn

C#:   s.Split('\n')
来源：https://zb.zhonguo4118.cn

[E20] 判断字符串是否为空
来源：https://br.zhonguo1118.cn

Py:   if not s:
来源：https://zv.zhonguo1118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://cj.zhonguo5118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://mw.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://pd.zhonguo8118.cn

Java: if (s.isEmpty()) {}
来源：https://kg.zhonguo7118.cn

Go:   if s == "" {}
来源：https://ju.zhonguo6118.cn

Ruby: if s.empty?
来源：https://cq.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://px.zhonguo5118.cn

[E21] 超长截断加省略号
来源：https://xt.zhonguo1118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://jp.zhonguo3118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://fu.zhonguo6118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://zi.zhonguo2118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://sp.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://qb.zhonguo1118.cn

Go:   // 按 rune 判断长度后截断
来源：https://rb.zhonguo3118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://pb.zhonguo8118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://jt.zhonguo6118.cn

[E22] 字节长度与字符长度
来源：https://yr.zhonguo1118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://sg.zhonguo5118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://qg.zhonguo2118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://nv.zhonguo7118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://zb.zhonguo3118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://ql.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://uq.zhonguo4118.cn

Ruby: s.bytesize;  s.length
来源：https://mk.zhonguo3118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://rc.zhonguo4118.cn

================================================================================
来源：https://wg.zhonguo3118.cn

F. 文件与目录
来源：https://dn.zhonguo6118.cn

================================================================================
来源：https://pj.zhonguo4118.cn

[F01] 读取整个文件
来源：https://gs.zhonguo8118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://hm.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://jv.zhonguo6118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://nn.zhonguo6118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://hp.zhonguo1118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://wp.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://tt.zhonguo7118.cn

Ruby: File.read("a.txt")
来源：https://bm.zhonguo6118.cn

C#:   File.ReadAllText("a.txt");
来源：https://jf.zhonguo3118.cn

[F02] 逐行读取文件
来源：https://or.zhonguo8118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ti.zhonguo8118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://ui.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://dd.zhonguo2118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://ag.zhonguo3118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://is.zhonguo6118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://ml.zhonguo4118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://lv.zhonguo2118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://lu.zhonguo2118.cn

[F03] 写入文件（覆盖）
来源：https://ba.zhonguo1118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://wd.zhonguo5118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://nw.zhonguo6118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://bd.zhonguo3118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ak.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://td.zhonguo1118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://kq.zhonguo1118.cn

Ruby: File.write("a.txt", "hi")
来源：https://zs.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://ed.zhonguo2118.cn

[F04] 追加写入文件
来源：https://el.zhonguo8118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://jk.zhonguo1118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://nw.zhonguo3118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://es.zhonguo2118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://as.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://lf.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://gy.zhonguo2118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://wv.zhonguo2118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://mh.zhonguo4118.cn

[F05] 判断文件或目录是否存在
来源：https://fy.zhonguo5118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://yh.zhonguo3118.cn

PHP:  file_exists("a.txt");
来源：https://gl.zhonguo2118.cn

JS:   fs.existsSync("a.txt")
来源：https://dw.zhonguo7118.cn

TS:   fs.existsSync("a.txt")
来源：https://uo.zhonguo2118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://wa.zhonguo2118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://tk.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://sg.zhonguo3118.cn

C#:   File.Exists("a.txt")
来源：https://xt.zhonguo3118.cn

[F06] 删除文件
来源：https://hm.zhonguo3118.cn

Py:   os.remove("a.txt")
来源：https://pq.zhonguo8118.cn

PHP:  unlink("a.txt");
来源：https://sg.zhonguo6118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://pw.zhonguo7118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://tu.zhonguo2118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://ky.zhonguo8118.cn

Go:   os.Remove("a.txt")
来源：https://qr.zhonguo7118.cn

Ruby: File.delete("a.txt")
来源：https://nw.zhonguo5118.cn

C#:   File.Delete("a.txt");
来源：https://xu.zhonguo7118.cn

[F07] 创建目录（含多级）
来源：https://wb.zhonguo5118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://qx.zhonguo6118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://nq.zhonguo4118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://le.zhonguo7118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://qi.zhonguo7118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://os.zhonguo1118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://hk.zhonguo2118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://xk.zhonguo7118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://hi.zhonguo4118.cn

[F08] 遍历目录
来源：https://af.zhonguo5118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://sk.zhonguo7118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://nl.zhonguo4118.cn

JS:   fs.readdirSync("dir")
来源：https://iz.zhonguo1118.cn

TS:   fs.readdirSync("dir")
来源：https://xx.zhonguo1118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://dk.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://bg.zhonguo1118.cn

Ruby: Dir.children("dir")
来源：https://rc.zhonguo5118.cn

C#:   Directory.GetFiles("dir")
来源：https://yb.zhonguo4118.cn

[F09] 获取文件大小
来源：https://nq.zhonguo8118.cn

Py:   os.path.getsize("a.txt")
来源：https://rw.zhonguo6118.cn

PHP:  filesize("a.txt");
来源：https://cg.zhonguo6118.cn

JS:   fs.statSync("a.txt").size
来源：https://ip.zhonguo3118.cn

TS:   fs.statSync("a.txt").size
来源：https://gq.zhonguo6118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://wr.zhonguo8118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://ax.zhonguo2118.cn

Ruby: File.size("a.txt")
来源：https://dg.zhonguo1118.cn

C#:   new FileInfo("a.txt").Length
来源：https://bg.zhonguo8118.cn

[F10] 取文件扩展名 / 文件名
来源：https://ad.zhonguo5118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://vn.zhonguo1118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://jq.zhonguo5118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://sa.zhonguo4118.cn

TS:   path.extname("a.txt")
来源：https://oh.zhonguo2118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://mh.zhonguo5118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://pm.zhonguo3118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://to.zhonguo3118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://ro.zhonguo8118.cn

[F11] 复制与移动文件
来源：https://ia.zhonguo7118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://lr.zhonguo8118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ak.zhonguo5118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://cj.zhonguo6118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://fw.zhonguo8118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://yt.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ts.zhonguo5118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://ke.zhonguo7118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://fw.zhonguo1118.cn

[F12] CSV 读写
来源：https://me.zhonguo1118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ex.zhonguo7118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://go.zhonguo7118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://gd.zhonguo8118.cn

TS:   // 同上
来源：https://jc.zhonguo5118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://zk.zhonguo5118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://sv.zhonguo7118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://yu.zhonguo7118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://sa.zhonguo8118.cn

================================================================================
来源：https://yc.zhonguo1118.cn

G. 面向对象
来源：https://or.zhonguo8118.cn

================================================================================
来源：https://gg.zhonguo6118.cn

[G01] 定义类
来源：https://tm.zhonguo5118.cn

Py:   class User: pass
来源：https://hf.zhonguo8118.cn

PHP:  class User {}
来源：https://zq.zhonguo4118.cn

JS:   class User {}
来源：https://hy.zhonguo3118.cn

TS:   class User { name: string = ""; }
来源：https://dn.zhonguo1118.cn

Java: class User {}
来源：https://an.zhonguo1118.cn

Go:   type User struct { Name string }
来源：https://cl.zhonguo8118.cn

Ruby: class User; end
来源：https://pp.zhonguo8118.cn

C#:   class User {}
来源：https://ys.zhonguo7118.cn

[G02] 构造函数
来源：https://vd.zhonguo1118.cn

Py:   def __init__(self, name): self.name = name
来源：https://nh.zhonguo8118.cn

PHP:  public function __construct(public string $name) {}
来源：https://uh.zhonguo7118.cn

JS:   constructor(name) { this.name = name; }
来源：https://xg.zhonguo5118.cn

TS:   constructor(public name: string) {}
来源：https://oz.zhonguo8118.cn

Java: User(String name) { this.name = name; }
来源：https://cv.zhonguo4118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://of.zhonguo5118.cn

Ruby: def initialize(name); @name = name; end
来源：https://cs.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://un.zhonguo1118.cn

[G03] 实例属性
来源：https://zq.zhonguo5118.cn

Py:   self.name = "x"
来源：https://la.zhonguo7118.cn

PHP:  public string $name = "x";
来源：https://cb.zhonguo1118.cn

JS:   this.name = "x";
来源：https://hj.zhonguo3118.cn

TS:   name: string = "x";
来源：https://uw.zhonguo6118.cn

Java: private String name;
来源：https://xt.zhonguo8118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://nv.zhonguo8118.cn

Ruby: @name = "x"
来源：https://or.zhonguo1118.cn

C#:   public string Name { get; set; } = "x";
来源：https://sk.zhonguo7118.cn

[G04] 定义方法
来源：https://uw.zhonguo6118.cn

Py:   def greet(self): return self.name
来源：https://oc.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://cm.zhonguo1118.cn

JS:   greet() { return this.name; }
来源：https://rm.zhonguo2118.cn

TS:   greet(): string { return this.name; }
来源：https://fb.zhonguo7118.cn

Java: String greet() { return name; }
来源：https://xf.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://wk.zhonguo7118.cn

Ruby: def greet; @name; end
来源：https://ao.zhonguo6118.cn

C#:   public string Greet() => Name;
来源：https://rv.zhonguo5118.cn

[G05] 继承
来源：https://ph.zhonguo6118.cn


<!-- 参考信息 -->