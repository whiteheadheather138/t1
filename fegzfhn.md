代发 wailian999

================================================================================
来源：https://qr.zhonguo6118.cn

E. 字符串处理
来源：https://ty.zhonguo4118.cn

================================================================================
来源：https://ia.zhonguo7118.cn

[E01] 拼接字符串
来源：https://vt.zhonguo8118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://bi.zhonguo7118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://kx.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://gx.zhonguo4118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://sz.zhonguo3118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://qo.zhonguo5118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://mt.zhonguo2118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://nu.zhonguo5118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://uk.zhonguo6118.cn

[E02] 重复字符串
来源：https://xt.zhonguo7118.cn

Py:   "ab" * 3
来源：https://ns.zhonguo7118.cn

PHP:  str_repeat("ab", 3);
来源：https://dl.zhonguo2118.cn

JS:   "ab".repeat(3)
来源：https://as.zhonguo8118.cn

TS:   "ab".repeat(3)
来源：https://wv.zhonguo4118.cn

Java: "ab".repeat(3)
来源：https://gp.zhonguo6118.cn

Go:   strings.Repeat("ab", 3)
来源：https://mj.zhonguo7118.cn

Ruby: "ab" * 3
来源：https://eb.zhonguo4118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://kl.zhonguo1118.cn

[E03] 截取子串
来源：https://se.zhonguo8118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://dv.zhonguo2118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://jc.zhonguo3118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://pe.zhonguo1118.cn

TS:   s.slice(1, 4)
来源：https://gb.zhonguo4118.cn

Java: s.substring(1, 4)
来源：https://en.zhonguo4118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://fs.zhonguo1118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://se.zhonguo6118.cn

C#:   s.Substring(1, 3)
来源：https://ze.zhonguo8118.cn

[E04] 查找子串位置
来源：https://dx.zhonguo6118.cn

Py:   s.find("x");  s.index("x")
来源：https://ee.zhonguo6118.cn

PHP:  strpos($s, "x");
来源：https://cg.zhonguo1118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://yb.zhonguo4118.cn

TS:   s.indexOf("x")
来源：https://tp.zhonguo2118.cn

Java: s.indexOf("x")
来源：https://sy.zhonguo4118.cn

Go:   strings.Index(s, "x")
来源：https://jh.zhonguo3118.cn

Ruby: s.index("x")
来源：https://ws.zhonguo5118.cn

C#:   s.IndexOf("x")
来源：https://by.zhonguo6118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://zq.zhonguo3118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://rz.zhonguo6118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://zx.zhonguo7118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://xf.zhonguo6118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://af.zhonguo6118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ls.zhonguo8118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://ny.zhonguo2118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://uj.zhonguo7118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://te.zhonguo5118.cn

[E06] 替换子串
来源：https://fn.zhonguo3118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://ie.zhonguo7118.cn

PHP:  str_replace("a", "b", $s);
来源：https://te.zhonguo2118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://ii.zhonguo2118.cn

TS:   s.replaceAll("a", "b")
来源：https://dm.zhonguo8118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://nm.zhonguo5118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://nw.zhonguo3118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://sy.zhonguo6118.cn

C#:   s.Replace("a", "b")
来源：https://to.zhonguo2118.cn

[E07] 按分隔符拆分
来源：https://zz.zhonguo1118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://xv.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://xr.zhonguo5118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://fs.zhonguo6118.cn

TS:   s.split(",")
来源：https://ds.zhonguo8118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://yw.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ey.zhonguo7118.cn

Ruby: s.split(",");  s.split
来源：https://pd.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://bb.zhonguo7118.cn

[E08] 数组按分隔符合并
来源：https://sh.zhonguo8118.cn

Py:   ",".join(items)
来源：https://km.zhonguo6118.cn

PHP:  implode(",", $items);
来源：https://pl.zhonguo8118.cn

JS:   items.join(",")
来源：https://vi.zhonguo4118.cn

TS:   items.join(",")
来源：https://wq.zhonguo2118.cn

Java: String.join(",", items)
来源：https://bj.zhonguo2118.cn

Go:   strings.Join(items, ",")
来源：https://yi.zhonguo3118.cn

Ruby: items.join(",")
来源：https://fp.zhonguo1118.cn

C#:   string.Join(",", items)
来源：https://xs.zhonguo3118.cn

[E09] 去除所有空白字符
来源：https://ya.zhonguo3118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://rj.zhonguo5118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://im.zhonguo2118.cn

JS:   s.replace(/\s+/g, "")
来源：https://fg.zhonguo4118.cn

TS:   s.replace(/\s+/g, "")
来源：https://xk.zhonguo2118.cn

Java: s.replaceAll("\\s+", "")
来源：https://vq.zhonguo3118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://gu.zhonguo1118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://cl.zhonguo8118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://sz.zhonguo1118.cn

[E10] 左侧补零 / 定长填充
来源：https://wb.zhonguo6118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://wu.zhonguo3118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://vu.zhonguo3118.cn

JS:   "7".padStart(3, "0")
来源：https://vn.zhonguo1118.cn

TS:   "7".padStart(3, "0")
来源：https://wf.zhonguo3118.cn

Java: String.format("%03d", 7)
来源：https://jj.zhonguo3118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://lz.zhonguo5118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://sd.zhonguo5118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://rv.zhonguo2118.cn

[E11] 反转字符串
来源：https://ca.zhonguo4118.cn

Py:   s[::-1]
来源：https://zf.zhonguo8118.cn

PHP:  strrev($s);
来源：https://xz.zhonguo2118.cn

JS:   [...s].reverse().join("")
来源：https://uh.zhonguo3118.cn

TS:   [...s].reverse().join("")
来源：https://fc.zhonguo8118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://kn.zhonguo8118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://hb.zhonguo5118.cn

Ruby: s.reverse
来源：https://ub.zhonguo2118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://xc.zhonguo6118.cn

[E12] 统计某字符出现次数
来源：https://cr.zhonguo4118.cn

Py:   s.count("a")
来源：https://qt.zhonguo2118.cn

PHP:  substr_count($s, "a");
来源：https://pd.zhonguo2118.cn

JS:   s.split("a").length - 1
来源：https://uv.zhonguo1118.cn

TS:   s.split("a").length - 1
来源：https://nr.zhonguo4118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://lx.zhonguo4118.cn

Go:   strings.Count(s, "a")
来源：https://yv.zhonguo4118.cn

Ruby: s.count("a")
来源：https://gg.zhonguo8118.cn

C#:   s.Count(c => c == 'a')
来源：https://jg.zhonguo4118.cn

[E13] 逐字符遍历
来源：https://fo.zhonguo6118.cn

Py:   for ch in s: print(ch)
来源：https://dy.zhonguo8118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://mt.zhonguo3118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://dz.zhonguo6118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ot.zhonguo5118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://cc.zhonguo8118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://tp.zhonguo5118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://qh.zhonguo3118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://mn.zhonguo1118.cn

[E14] URL 编码与 Base64
来源：https://vt.zhonguo3118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://op.zhonguo8118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://pa.zhonguo1118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://iw.zhonguo8118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://wj.zhonguo5118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://ss.zhonguo4118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://ws.zhonguo6118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://oe.zhonguo2118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://hi.zhonguo4118.cn

[E15] HTML 转义 / 反转义
来源：https://xz.zhonguo1118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://wa.zhonguo1118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://sv.zhonguo3118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://fw.zhonguo7118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://kg.zhonguo3118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://wn.zhonguo7118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://pn.zhonguo5118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://ik.zhonguo5118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://ab.zhonguo5118.cn

[E16] 数字千分位
来源：https://xt.zhonguo6118.cn

Py:   f"{1234567:,}"
来源：https://fr.zhonguo8118.cn

PHP:  number_format(1234567);
来源：https://hu.zhonguo7118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://be.zhonguo7118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://bk.zhonguo2118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://ds.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://pk.zhonguo5118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://pa.zhonguo8118.cn

C#:   1234567.ToString("N0")
来源：https://kl.zhonguo8118.cn

[E17] 首字母大写
来源：https://wt.zhonguo3118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://mm.zhonguo1118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://ds.zhonguo5118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ub.zhonguo8118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://lp.zhonguo4118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://pk.zhonguo4118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://wk.zhonguo3118.cn

Ruby: s.capitalize
来源：https://fy.zhonguo5118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://qp.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://uc.zhonguo4118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://cl.zhonguo7118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://sv.zhonguo3118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://gq.zhonguo8118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://xl.zhonguo8118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://vs.zhonguo3118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://mq.zhonguo7118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://to.zhonguo1118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://yp.zhonguo8118.cn

[E19] 多行文本按行拆分
来源：https://ko.zhonguo4118.cn

Py:   s.splitlines()
来源：https://sv.zhonguo4118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://hj.zhonguo8118.cn

JS:   s.split(/\r?\n/)
来源：https://yl.zhonguo7118.cn

TS:   s.split(/\r?\n/)
来源：https://vx.zhonguo3118.cn

Java: s.lines().toList()
来源：https://rt.zhonguo6118.cn

Go:   strings.Split(s, "\n")
来源：https://yv.zhonguo3118.cn

Ruby: s.lines
来源：https://ca.zhonguo3118.cn

C#:   s.Split('\n')
来源：https://iz.zhonguo4118.cn

[E20] 判断字符串是否为空
来源：https://xe.zhonguo8118.cn

Py:   if not s:
来源：https://gp.zhonguo7118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://ft.zhonguo5118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ig.zhonguo6118.cn

TS:   if (s === "") {}
来源：https://vo.zhonguo3118.cn

Java: if (s.isEmpty()) {}
来源：https://dg.zhonguo5118.cn

Go:   if s == "" {}
来源：https://lh.zhonguo3118.cn

Ruby: if s.empty?
来源：https://ve.zhonguo1118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://yg.zhonguo1118.cn

[E21] 超长截断加省略号
来源：https://bi.zhonguo6118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://cd.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://by.zhonguo7118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://aj.zhonguo2118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://pq.zhonguo4118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ki.zhonguo7118.cn

Go:   // 按 rune 判断长度后截断
来源：https://dt.zhonguo6118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://bl.zhonguo1118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://jd.zhonguo2118.cn

[E22] 字节长度与字符长度
来源：https://sx.zhonguo8118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://ma.zhonguo8118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://xx.zhonguo1118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://zv.zhonguo8118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://cv.zhonguo5118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://fo.zhonguo6118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://ns.zhonguo7118.cn

Ruby: s.bytesize;  s.length
来源：https://dy.zhonguo3118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://fz.zhonguo1118.cn

================================================================================
来源：https://bb.zhonguo6118.cn

F. 文件与目录
来源：https://wy.zhonguo1118.cn

================================================================================
来源：https://ea.zhonguo2118.cn

[F01] 读取整个文件
来源：https://hi.zhonguo5118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://xb.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://st.zhonguo7118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://nj.zhonguo3118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://de.zhonguo8118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ob.zhonguo5118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ii.zhonguo1118.cn

Ruby: File.read("a.txt")
来源：https://oe.zhonguo3118.cn

C#:   File.ReadAllText("a.txt");
来源：https://gf.zhonguo2118.cn

[F02] 逐行读取文件
来源：https://dk.zhonguo5118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://nn.zhonguo7118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://at.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://zn.zhonguo5118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://pc.zhonguo6118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://mj.zhonguo4118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://dm.zhonguo7118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://pp.zhonguo3118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://nj.zhonguo4118.cn

[F03] 写入文件（覆盖）
来源：https://mp.zhonguo8118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://sv.zhonguo7118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://zr.zhonguo1118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://dp.zhonguo4118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ap.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://zw.zhonguo2118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://oz.zhonguo1118.cn

Ruby: File.write("a.txt", "hi")
来源：https://tf.zhonguo8118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://du.zhonguo8118.cn

[F04] 追加写入文件
来源：https://ks.zhonguo1118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://yh.zhonguo2118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://ox.zhonguo6118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://pb.zhonguo7118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://cz.zhonguo8118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://ba.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://xl.zhonguo2118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://bn.zhonguo7118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://av.zhonguo4118.cn

[F05] 判断文件或目录是否存在
来源：https://xr.zhonguo7118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://vf.zhonguo8118.cn

PHP:  file_exists("a.txt");
来源：https://aj.zhonguo6118.cn

JS:   fs.existsSync("a.txt")
来源：https://ni.zhonguo6118.cn

TS:   fs.existsSync("a.txt")
来源：https://rz.zhonguo6118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ai.zhonguo4118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://rk.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://fm.zhonguo8118.cn

C#:   File.Exists("a.txt")
来源：https://rv.zhonguo3118.cn

[F06] 删除文件
来源：https://qp.zhonguo6118.cn

Py:   os.remove("a.txt")
来源：https://ki.zhonguo3118.cn

PHP:  unlink("a.txt");
来源：https://hh.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://sc.zhonguo2118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://uk.zhonguo3118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://bu.zhonguo5118.cn

Go:   os.Remove("a.txt")
来源：https://wx.zhonguo5118.cn

Ruby: File.delete("a.txt")
来源：https://jf.zhonguo6118.cn

C#:   File.Delete("a.txt");
来源：https://sd.zhonguo7118.cn

[F07] 创建目录（含多级）
来源：https://dg.zhonguo4118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://tg.zhonguo6118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://do.zhonguo3118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://qv.zhonguo5118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://vj.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://jk.zhonguo5118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://pg.zhonguo4118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ts.zhonguo5118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://vg.zhonguo6118.cn

[F08] 遍历目录
来源：https://zb.zhonguo3118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ct.zhonguo1118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://np.zhonguo3118.cn

JS:   fs.readdirSync("dir")
来源：https://qm.zhonguo6118.cn

TS:   fs.readdirSync("dir")
来源：https://tz.zhonguo3118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://jv.zhonguo4118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://ut.zhonguo7118.cn

Ruby: Dir.children("dir")
来源：https://kh.zhonguo6118.cn

C#:   Directory.GetFiles("dir")
来源：https://hw.zhonguo8118.cn

[F09] 获取文件大小
来源：https://yn.zhonguo5118.cn

Py:   os.path.getsize("a.txt")
来源：https://rq.zhonguo8118.cn

PHP:  filesize("a.txt");
来源：https://ae.zhonguo6118.cn

JS:   fs.statSync("a.txt").size
来源：https://lt.zhonguo7118.cn

TS:   fs.statSync("a.txt").size
来源：https://wy.zhonguo2118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://zw.zhonguo8118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://qt.zhonguo6118.cn

Ruby: File.size("a.txt")
来源：https://fu.zhonguo7118.cn

C#:   new FileInfo("a.txt").Length
来源：https://sn.zhonguo7118.cn

[F10] 取文件扩展名 / 文件名
来源：https://og.zhonguo2118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://gq.zhonguo6118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://hj.zhonguo6118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://gw.zhonguo6118.cn

TS:   path.extname("a.txt")
来源：https://bo.zhonguo5118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://ni.zhonguo7118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://pi.zhonguo5118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://nx.zhonguo7118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://lc.zhonguo7118.cn

[F11] 复制与移动文件
来源：https://am.zhonguo2118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://dg.zhonguo3118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://iz.zhonguo5118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://wq.zhonguo6118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ti.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://bd.zhonguo5118.cn


<!-- 参考信息 -->