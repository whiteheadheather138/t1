代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://oo.zhonguo4118.cn

[E03] 截取子串
来源：https://wb.zhonguo3118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://xu.zhonguo5118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://oa.zhonguo1118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://xn.zhonguo3118.cn

TS:   s.slice(1, 4)
来源：https://ts.zhonguo6118.cn

Java: s.substring(1, 4)
来源：https://kl.zhonguo4118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://vx.zhonguo8118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://qm.zhonguo6118.cn

C#:   s.Substring(1, 3)
来源：https://jn.zhonguo6118.cn

[E04] 查找子串位置
来源：https://lw.zhonguo4118.cn

Py:   s.find("x");  s.index("x")
来源：https://ta.zhonguo7118.cn

PHP:  strpos($s, "x");
来源：https://pj.zhonguo1118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://bt.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://qn.zhonguo3118.cn

Java: s.indexOf("x")
来源：https://ew.zhonguo3118.cn

Go:   strings.Index(s, "x")
来源：https://aq.zhonguo7118.cn

Ruby: s.index("x")
来源：https://gb.zhonguo8118.cn

C#:   s.IndexOf("x")
来源：https://oe.zhonguo4118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://ri.zhonguo8118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://jp.zhonguo8118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://qt.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ez.zhonguo5118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://yf.zhonguo7118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://pa.zhonguo7118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://yd.zhonguo8118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://aj.zhonguo7118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://bg.zhonguo7118.cn

[E06] 替换子串
来源：https://zy.zhonguo2118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://sm.zhonguo6118.cn

PHP:  str_replace("a", "b", $s);
来源：https://fx.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://zg.zhonguo6118.cn

TS:   s.replaceAll("a", "b")
来源：https://lc.zhonguo5118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://qm.zhonguo1118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ec.zhonguo4118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://qz.zhonguo3118.cn

C#:   s.Replace("a", "b")
来源：https://ze.zhonguo6118.cn

[E07] 按分隔符拆分
来源：https://cj.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://ta.zhonguo2118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://jt.zhonguo7118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://lt.zhonguo3118.cn

TS:   s.split(",")
来源：https://qv.zhonguo7118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://ab.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://dl.zhonguo3118.cn

Ruby: s.split(",");  s.split
来源：https://jy.zhonguo7118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://pu.zhonguo1118.cn

[E08] 数组按分隔符合并
来源：https://kr.zhonguo3118.cn

Py:   ",".join(items)
来源：https://qt.zhonguo6118.cn

PHP:  implode(",", $items);
来源：https://gl.zhonguo5118.cn

JS:   items.join(",")
来源：https://zv.zhonguo6118.cn

TS:   items.join(",")
来源：https://qa.zhonguo4118.cn

Java: String.join(",", items)
来源：https://vs.zhonguo6118.cn

Go:   strings.Join(items, ",")
来源：https://rs.zhonguo1118.cn

Ruby: items.join(",")
来源：https://dl.zhonguo2118.cn

C#:   string.Join(",", items)
来源：https://rj.zhonguo5118.cn

[E09] 去除所有空白字符
来源：https://db.zhonguo2118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ls.zhonguo1118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://nh.zhonguo1118.cn

JS:   s.replace(/\s+/g, "")
来源：https://qq.zhonguo8118.cn

TS:   s.replace(/\s+/g, "")
来源：https://gj.zhonguo7118.cn

Java: s.replaceAll("\\s+", "")
来源：https://xj.zhonguo8118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://em.zhonguo5118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://sj.zhonguo2118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://hd.zhonguo4118.cn

[E10] 左侧补零 / 定长填充
来源：https://ge.zhonguo1118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ua.zhonguo2118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://hs.zhonguo6118.cn

JS:   "7".padStart(3, "0")
来源：https://kx.zhonguo6118.cn

TS:   "7".padStart(3, "0")
来源：https://xf.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://pd.zhonguo7118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://fq.zhonguo7118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://kp.zhonguo5118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://et.zhonguo8118.cn

[E11] 反转字符串
来源：https://tw.zhonguo6118.cn

Py:   s[::-1]
来源：https://ob.zhonguo5118.cn

PHP:  strrev($s);
来源：https://ng.zhonguo7118.cn

JS:   [...s].reverse().join("")
来源：https://cm.zhonguo8118.cn

TS:   [...s].reverse().join("")
来源：https://hn.zhonguo5118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ex.zhonguo5118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://rj.zhonguo7118.cn

Ruby: s.reverse
来源：https://dk.zhonguo2118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://mh.zhonguo7118.cn

[E12] 统计某字符出现次数
来源：https://em.zhonguo3118.cn

Py:   s.count("a")
来源：https://ro.zhonguo5118.cn

PHP:  substr_count($s, "a");
来源：https://lk.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://pz.zhonguo7118.cn

TS:   s.split("a").length - 1
来源：https://qi.zhonguo2118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://gr.zhonguo5118.cn

Go:   strings.Count(s, "a")
来源：https://dp.zhonguo4118.cn

Ruby: s.count("a")
来源：https://xb.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://wb.zhonguo7118.cn

[E13] 逐字符遍历
来源：https://ct.zhonguo4118.cn

Py:   for ch in s: print(ch)
来源：https://rq.zhonguo4118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://jz.zhonguo6118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://bh.zhonguo3118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://qt.zhonguo4118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://hv.zhonguo1118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://uz.zhonguo5118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://nf.zhonguo4118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://sj.zhonguo7118.cn

[E14] URL 编码与 Base64
来源：https://wn.zhonguo4118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://sf.zhonguo8118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://wf.zhonguo8118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://ph.zhonguo7118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://ce.zhonguo4118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://ci.zhonguo3118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://fi.zhonguo7118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://zv.zhonguo5118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://xj.zhonguo7118.cn

[E15] HTML 转义 / 反转义
来源：https://od.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://wd.zhonguo4118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://lz.zhonguo3118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://xj.zhonguo7118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://nb.zhonguo6118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://kj.zhonguo8118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://fz.zhonguo4118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://og.zhonguo4118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://uv.zhonguo5118.cn

[E16] 数字千分位
来源：https://oa.zhonguo7118.cn

Py:   f"{1234567:,}"
来源：https://pf.zhonguo5118.cn

PHP:  number_format(1234567);
来源：https://fd.zhonguo1118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://ob.zhonguo2118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://fk.zhonguo4118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://go.zhonguo7118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://mk.zhonguo5118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://pg.zhonguo2118.cn

C#:   1234567.ToString("N0")
来源：https://sf.zhonguo6118.cn

[E17] 首字母大写
来源：https://km.zhonguo4118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://qv.zhonguo5118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://dw.zhonguo8118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://dj.zhonguo5118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ht.zhonguo3118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://yw.zhonguo3118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://eu.zhonguo8118.cn

Ruby: s.capitalize
来源：https://ci.zhonguo5118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://zl.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://dj.zhonguo7118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ow.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://rb.zhonguo4118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://tm.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://in.zhonguo2118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://vc.zhonguo7118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://vn.zhonguo2118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://wz.zhonguo1118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://lb.zhonguo4118.cn

[E19] 多行文本按行拆分
来源：https://dd.zhonguo7118.cn

Py:   s.splitlines()
来源：https://en.zhonguo5118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://mf.zhonguo4118.cn

JS:   s.split(/\r?\n/)
来源：https://gl.zhonguo3118.cn

TS:   s.split(/\r?\n/)
来源：https://gg.zhonguo8118.cn

Java: s.lines().toList()
来源：https://ql.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://bx.zhonguo2118.cn

Ruby: s.lines
来源：https://hq.zhonguo7118.cn

C#:   s.Split('\n')
来源：https://on.zhonguo5118.cn

[E20] 判断字符串是否为空
来源：https://zv.zhonguo6118.cn

Py:   if not s:
来源：https://zl.zhonguo3118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://id.zhonguo4118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://br.zhonguo8118.cn

TS:   if (s === "") {}
来源：https://hc.zhonguo4118.cn

Java: if (s.isEmpty()) {}
来源：https://zm.zhonguo3118.cn

Go:   if s == "" {}
来源：https://ix.zhonguo5118.cn

Ruby: if s.empty?
来源：https://hk.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://rz.zhonguo2118.cn

[E21] 超长截断加省略号
来源：https://da.zhonguo2118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://bq.zhonguo2118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://xq.zhonguo1118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ox.zhonguo4118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://lh.zhonguo1118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ku.zhonguo3118.cn

Go:   // 按 rune 判断长度后截断
来源：https://sq.zhonguo5118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://yf.zhonguo7118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://gm.zhonguo5118.cn

[E22] 字节长度与字符长度
来源：https://ve.zhonguo2118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://ie.zhonguo1118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://yu.zhonguo3118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://zc.zhonguo4118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://dy.zhonguo2118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://dh.zhonguo3118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://fd.zhonguo5118.cn

Ruby: s.bytesize;  s.length
来源：https://ze.zhonguo4118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://qp.zhonguo5118.cn

================================================================================
来源：https://zd.zhonguo3118.cn

F. 文件与目录
来源：https://eo.zhonguo1118.cn

================================================================================
来源：https://ku.zhonguo6118.cn

[F01] 读取整个文件
来源：https://hy.zhonguo8118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://py.zhonguo2118.cn

PHP:  file_get_contents("a.txt");
来源：https://rr.zhonguo5118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://hj.zhonguo6118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://id.zhonguo7118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://qa.zhonguo5118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://bg.zhonguo3118.cn

Ruby: File.read("a.txt")
来源：https://le.zhonguo3118.cn

C#:   File.ReadAllText("a.txt");
来源：https://sp.zhonguo3118.cn

[F02] 逐行读取文件
来源：https://ov.zhonguo8118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ot.zhonguo2118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://wl.zhonguo7118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://zt.zhonguo7118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://jr.zhonguo8118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://bh.zhonguo8118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://cz.zhonguo8118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://vm.zhonguo2118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://ha.zhonguo8118.cn

[F03] 写入文件（覆盖）
来源：https://jk.zhonguo3118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://ot.zhonguo1118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://xl.zhonguo5118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://le.zhonguo8118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://fv.zhonguo8118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://pl.zhonguo8118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://xn.zhonguo5118.cn

Ruby: File.write("a.txt", "hi")
来源：https://jh.zhonguo6118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://mw.zhonguo6118.cn

[F04] 追加写入文件
来源：https://lk.zhonguo2118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://fj.zhonguo1118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://zz.zhonguo6118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://wb.zhonguo3118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://tb.zhonguo8118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://ks.zhonguo7118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://gd.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://kl.zhonguo5118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://gq.zhonguo1118.cn

[F05] 判断文件或目录是否存在
来源：https://yu.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://la.zhonguo2118.cn

PHP:  file_exists("a.txt");
来源：https://tj.zhonguo7118.cn

JS:   fs.existsSync("a.txt")
来源：https://jp.zhonguo5118.cn

TS:   fs.existsSync("a.txt")
来源：https://xe.zhonguo8118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ro.zhonguo4118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ps.zhonguo7118.cn

Ruby: File.exist?("a.txt")
来源：https://xu.zhonguo5118.cn

C#:   File.Exists("a.txt")
来源：https://uw.zhonguo4118.cn

[F06] 删除文件
来源：https://kj.zhonguo7118.cn

Py:   os.remove("a.txt")
来源：https://jx.zhonguo4118.cn

PHP:  unlink("a.txt");
来源：https://ka.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://yh.zhonguo1118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://qo.zhonguo6118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://jj.zhonguo2118.cn

Go:   os.Remove("a.txt")
来源：https://zy.zhonguo8118.cn

Ruby: File.delete("a.txt")
来源：https://as.zhonguo5118.cn

C#:   File.Delete("a.txt");
来源：https://la.zhonguo8118.cn

[F07] 创建目录（含多级）
来源：https://lk.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://hb.zhonguo6118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://vo.zhonguo5118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://mi.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://rv.zhonguo6118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://je.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://wl.zhonguo8118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://zj.zhonguo8118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://vn.zhonguo2118.cn

[F08] 遍历目录
来源：https://at.zhonguo1118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://qm.zhonguo8118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://km.zhonguo4118.cn

JS:   fs.readdirSync("dir")
来源：https://cy.zhonguo7118.cn

TS:   fs.readdirSync("dir")
来源：https://po.zhonguo8118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://aj.zhonguo1118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://kx.zhonguo5118.cn

Ruby: Dir.children("dir")
来源：https://yt.zhonguo4118.cn

C#:   Directory.GetFiles("dir")
来源：https://fb.zhonguo7118.cn

[F09] 获取文件大小
来源：https://ll.zhonguo1118.cn

Py:   os.path.getsize("a.txt")
来源：https://km.zhonguo4118.cn

PHP:  filesize("a.txt");
来源：https://aq.zhonguo6118.cn

JS:   fs.statSync("a.txt").size
来源：https://dy.zhonguo2118.cn

TS:   fs.statSync("a.txt").size
来源：https://ir.zhonguo4118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://xc.zhonguo3118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://so.zhonguo5118.cn

Ruby: File.size("a.txt")
来源：https://pz.zhonguo1118.cn

C#:   new FileInfo("a.txt").Length
来源：https://mi.zhonguo5118.cn

[F10] 取文件扩展名 / 文件名
来源：https://zg.zhonguo3118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://xd.zhonguo5118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://cm.zhonguo7118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://nq.zhonguo2118.cn

TS:   path.extname("a.txt")
来源：https://rk.zhonguo7118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://jp.zhonguo8118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://ix.zhonguo8118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://ve.zhonguo2118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://iu.zhonguo6118.cn

[F11] 复制与移动文件
来源：https://nz.zhonguo3118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://xb.zhonguo6118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ub.zhonguo1118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ae.zhonguo4118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://jt.zhonguo5118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://ly.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ht.zhonguo5118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://uc.zhonguo4118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://qq.zhonguo4118.cn

[F12] CSV 读写
来源：https://vg.zhonguo5118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ej.zhonguo4118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://ph.zhonguo7118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://gl.zhonguo6118.cn

TS:   // 同上
来源：https://iq.zhonguo8118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://ji.zhonguo4118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://bq.zhonguo4118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://oc.zhonguo3118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://js.zhonguo1118.cn

================================================================================
来源：https://rp.zhonguo2118.cn

G. 面向对象
来源：https://am.zhonguo7118.cn

================================================================================
来源：https://uz.zhonguo2118.cn

[G01] 定义类
来源：https://na.zhonguo3118.cn

Py:   class User: pass
来源：https://gv.zhonguo7118.cn

PHP:  class User {}
来源：https://mm.zhonguo2118.cn

JS:   class User {}
来源：https://jd.zhonguo4118.cn

TS:   class User { name: string = ""; }
来源：https://go.zhonguo7118.cn


<!-- 参考信息 -->