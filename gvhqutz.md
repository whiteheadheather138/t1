代发 wailian999

Py:   ", ".join(map(str, arr))
来源：https://aq.zhonguo3118.cn

PHP:  implode(", ", $arr);
来源：https://wh.zhonguo2118.cn

JS:   arr.join(", ")
来源：https://xg.zhonguo4118.cn

TS:   arr.join(", ")
来源：https://kn.zhonguo5118.cn

Java: String.join(", ", list)
来源：https://qb.zhonguo1118.cn

Go:   strings.Join(strs, ", ")
来源：https://xw.zhonguo1118.cn

Ruby: arr.join(", ")
来源：https://aa.zhonguo3118.cn

C#:   string.Join(", ", list)
来源：https://fy.zhonguo5118.cn

================================================================================
来源：https://bp.zhonguo2118.cn

E. 字符串处理
来源：https://fx.zhonguo7118.cn

================================================================================
来源：https://ii.zhonguo7118.cn

[E01] 拼接字符串
来源：https://bv.zhonguo8118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://yd.zhonguo2118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://hq.zhonguo2118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://tp.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://hj.zhonguo7118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://hy.zhonguo8118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://ud.zhonguo5118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://xc.zhonguo7118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://xw.zhonguo3118.cn

[E02] 重复字符串
来源：https://nj.zhonguo3118.cn

Py:   "ab" * 3
来源：https://ls.zhonguo4118.cn

PHP:  str_repeat("ab", 3);
来源：https://dy.zhonguo4118.cn

JS:   "ab".repeat(3)
来源：https://rj.zhonguo2118.cn

TS:   "ab".repeat(3)
来源：https://qf.zhonguo1118.cn

Java: "ab".repeat(3)
来源：https://vh.zhonguo1118.cn

Go:   strings.Repeat("ab", 3)
来源：https://gc.zhonguo3118.cn

Ruby: "ab" * 3
来源：https://pv.zhonguo1118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://yi.zhonguo7118.cn

[E03] 截取子串
来源：https://qh.zhonguo3118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://iv.zhonguo7118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://xc.zhonguo8118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://ku.zhonguo4118.cn

TS:   s.slice(1, 4)
来源：https://lf.zhonguo8118.cn

Java: s.substring(1, 4)
来源：https://hu.zhonguo2118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://yg.zhonguo1118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://rw.zhonguo7118.cn

C#:   s.Substring(1, 3)
来源：https://rq.zhonguo8118.cn

[E04] 查找子串位置
来源：https://rt.zhonguo8118.cn

Py:   s.find("x");  s.index("x")
来源：https://dc.zhonguo2118.cn

PHP:  strpos($s, "x");
来源：https://fj.zhonguo3118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://il.zhonguo6118.cn

TS:   s.indexOf("x")
来源：https://jz.zhonguo5118.cn

Java: s.indexOf("x")
来源：https://bs.zhonguo6118.cn

Go:   strings.Index(s, "x")
来源：https://rf.zhonguo5118.cn

Ruby: s.index("x")
来源：https://hw.zhonguo8118.cn

C#:   s.IndexOf("x")
来源：https://dw.zhonguo8118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://au.zhonguo6118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://pk.zhonguo4118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://zj.zhonguo3118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ec.zhonguo1118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://mq.zhonguo4118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://es.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://aa.zhonguo5118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://jd.zhonguo2118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://gr.zhonguo5118.cn

[E06] 替换子串
来源：https://sa.zhonguo6118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://lp.zhonguo2118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ss.zhonguo1118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://yp.zhonguo8118.cn

TS:   s.replaceAll("a", "b")
来源：https://ae.zhonguo6118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://gm.zhonguo4118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ip.zhonguo7118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://qe.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://ok.zhonguo4118.cn

[E07] 按分隔符拆分
来源：https://au.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://hc.zhonguo5118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://bj.zhonguo4118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://fl.zhonguo7118.cn

TS:   s.split(",")
来源：https://dm.zhonguo1118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://ja.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ok.zhonguo4118.cn

Ruby: s.split(",");  s.split
来源：https://fn.zhonguo6118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://wt.zhonguo6118.cn

[E08] 数组按分隔符合并
来源：https://hy.zhonguo4118.cn

Py:   ",".join(items)
来源：https://fh.zhonguo2118.cn

PHP:  implode(",", $items);
来源：https://ri.zhonguo1118.cn

JS:   items.join(",")
来源：https://ug.zhonguo8118.cn

TS:   items.join(",")
来源：https://uw.zhonguo7118.cn

Java: String.join(",", items)
来源：https://jv.zhonguo5118.cn

Go:   strings.Join(items, ",")
来源：https://ko.zhonguo3118.cn

Ruby: items.join(",")
来源：https://sa.zhonguo8118.cn

C#:   string.Join(",", items)
来源：https://gv.zhonguo8118.cn

[E09] 去除所有空白字符
来源：https://qx.zhonguo6118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://jp.zhonguo7118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://gv.zhonguo2118.cn

JS:   s.replace(/\s+/g, "")
来源：https://qv.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://wh.zhonguo2118.cn

Java: s.replaceAll("\\s+", "")
来源：https://lv.zhonguo3118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://mv.zhonguo6118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://pi.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://zw.zhonguo8118.cn

[E10] 左侧补零 / 定长填充
来源：https://gj.zhonguo2118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://sf.zhonguo4118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ga.zhonguo4118.cn

JS:   "7".padStart(3, "0")
来源：https://dc.zhonguo5118.cn

TS:   "7".padStart(3, "0")
来源：https://xn.zhonguo2118.cn

Java: String.format("%03d", 7)
来源：https://dt.zhonguo5118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://zk.zhonguo6118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://um.zhonguo5118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://yw.zhonguo3118.cn

[E11] 反转字符串
来源：https://ak.zhonguo3118.cn

Py:   s[::-1]
来源：https://tz.zhonguo5118.cn

PHP:  strrev($s);
来源：https://eo.zhonguo3118.cn

JS:   [...s].reverse().join("")
来源：https://ey.zhonguo8118.cn

TS:   [...s].reverse().join("")
来源：https://ly.zhonguo8118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ur.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://cc.zhonguo6118.cn

Ruby: s.reverse
来源：https://ra.zhonguo1118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ee.zhonguo5118.cn

[E12] 统计某字符出现次数
来源：https://ge.zhonguo7118.cn

Py:   s.count("a")
来源：https://zj.zhonguo4118.cn

PHP:  substr_count($s, "a");
来源：https://mo.zhonguo3118.cn

JS:   s.split("a").length - 1
来源：https://yr.zhonguo8118.cn

TS:   s.split("a").length - 1
来源：https://dh.zhonguo4118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://uo.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://sd.zhonguo1118.cn

Ruby: s.count("a")
来源：https://oy.zhonguo7118.cn

C#:   s.Count(c => c == 'a')
来源：https://iy.zhonguo4118.cn

[E13] 逐字符遍历
来源：https://ci.zhonguo1118.cn

Py:   for ch in s: print(ch)
来源：https://jy.zhonguo5118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://ek.zhonguo7118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://cx.zhonguo8118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://gk.zhonguo4118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://lv.zhonguo8118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://eg.zhonguo4118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://tm.zhonguo3118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://va.zhonguo7118.cn

[E14] URL 编码与 Base64
来源：https://aq.zhonguo4118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://wy.zhonguo1118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://nu.zhonguo7118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://ng.zhonguo8118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://bl.zhonguo1118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://sz.zhonguo8118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://sn.zhonguo3118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://bw.zhonguo2118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://ym.zhonguo4118.cn

[E15] HTML 转义 / 反转义
来源：https://yz.zhonguo3118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ox.zhonguo6118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://jq.zhonguo7118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://gp.zhonguo6118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://iz.zhonguo7118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://am.zhonguo6118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://av.zhonguo6118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://jd.zhonguo8118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://lm.zhonguo1118.cn

[E16] 数字千分位
来源：https://jq.zhonguo5118.cn

Py:   f"{1234567:,}"
来源：https://lc.zhonguo6118.cn

PHP:  number_format(1234567);
来源：https://hf.zhonguo5118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://wz.zhonguo5118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://ia.zhonguo8118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://wm.zhonguo5118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://mt.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://bj.zhonguo4118.cn

C#:   1234567.ToString("N0")
来源：https://db.zhonguo8118.cn

[E17] 首字母大写
来源：https://uv.zhonguo4118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://sp.zhonguo8118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://fw.zhonguo4118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://wz.zhonguo6118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://su.zhonguo3118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://bu.zhonguo5118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://fm.zhonguo6118.cn

Ruby: s.capitalize
来源：https://bo.zhonguo5118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://ug.zhonguo6118.cn

[E18] 模板占位符替换
来源：https://hv.zhonguo8118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://vg.zhonguo7118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://ea.zhonguo1118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://kq.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://lw.zhonguo7118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://om.zhonguo6118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://um.zhonguo4118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://dd.zhonguo3118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://is.zhonguo5118.cn

[E19] 多行文本按行拆分
来源：https://qr.zhonguo3118.cn

Py:   s.splitlines()
来源：https://ue.zhonguo3118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://uj.zhonguo7118.cn

JS:   s.split(/\r?\n/)
来源：https://ls.zhonguo3118.cn

TS:   s.split(/\r?\n/)
来源：https://yn.zhonguo5118.cn

Java: s.lines().toList()
来源：https://vb.zhonguo7118.cn

Go:   strings.Split(s, "\n")
来源：https://yl.zhonguo6118.cn

Ruby: s.lines
来源：https://sp.zhonguo7118.cn

C#:   s.Split('\n')
来源：https://jy.zhonguo2118.cn

[E20] 判断字符串是否为空
来源：https://bb.zhonguo7118.cn

Py:   if not s:
来源：https://ro.zhonguo3118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://ru.zhonguo1118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://mb.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://kj.zhonguo2118.cn

Java: if (s.isEmpty()) {}
来源：https://py.zhonguo4118.cn

Go:   if s == "" {}
来源：https://qm.zhonguo7118.cn

Ruby: if s.empty?
来源：https://uw.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://sa.zhonguo7118.cn

[E21] 超长截断加省略号
来源：https://zz.zhonguo2118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://mz.zhonguo2118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://ty.zhonguo6118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://hw.zhonguo5118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://bf.zhonguo3118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://xm.zhonguo6118.cn

Go:   // 按 rune 判断长度后截断
来源：https://pd.zhonguo6118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://un.zhonguo4118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://nu.zhonguo2118.cn

[E22] 字节长度与字符长度
来源：https://mf.zhonguo5118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://mc.zhonguo3118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://hv.zhonguo2118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://qw.zhonguo4118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://ur.zhonguo4118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://wi.zhonguo8118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://mp.zhonguo4118.cn

Ruby: s.bytesize;  s.length
来源：https://xe.zhonguo1118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://oo.zhonguo2118.cn

================================================================================
来源：https://cm.zhonguo3118.cn

F. 文件与目录
来源：https://qr.zhonguo4118.cn

================================================================================
来源：https://zn.zhonguo1118.cn

[F01] 读取整个文件
来源：https://eo.zhonguo2118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://xo.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://cm.zhonguo8118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://lt.zhonguo5118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://vy.zhonguo7118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://pp.zhonguo3118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://uf.zhonguo2118.cn

Ruby: File.read("a.txt")
来源：https://wk.zhonguo7118.cn

C#:   File.ReadAllText("a.txt");
来源：https://kw.zhonguo6118.cn

[F02] 逐行读取文件
来源：https://qe.zhonguo7118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://xu.zhonguo7118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://mb.zhonguo1118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://sm.zhonguo2118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://dm.zhonguo1118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://oc.zhonguo7118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://rh.zhonguo2118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ht.zhonguo8118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://wf.zhonguo5118.cn

[F03] 写入文件（覆盖）
来源：https://jn.zhonguo7118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://jo.zhonguo8118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://av.zhonguo5118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ya.zhonguo3118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://wk.zhonguo2118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ze.zhonguo7118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ov.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://wq.zhonguo7118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://zg.zhonguo8118.cn

[F04] 追加写入文件
来源：https://nj.zhonguo4118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://vu.zhonguo5118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://ko.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://js.zhonguo3118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://lz.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://jz.zhonguo2118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://ac.zhonguo5118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://na.zhonguo8118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://uy.zhonguo4118.cn

[F05] 判断文件或目录是否存在
来源：https://ab.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://pv.zhonguo6118.cn

PHP:  file_exists("a.txt");
来源：https://no.zhonguo8118.cn

JS:   fs.existsSync("a.txt")
来源：https://em.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://uh.zhonguo7118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://er.zhonguo8118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://oq.zhonguo3118.cn

Ruby: File.exist?("a.txt")
来源：https://me.zhonguo6118.cn

C#:   File.Exists("a.txt")
来源：https://km.zhonguo2118.cn

[F06] 删除文件
来源：https://sv.zhonguo3118.cn

Py:   os.remove("a.txt")
来源：https://nq.zhonguo2118.cn

PHP:  unlink("a.txt");
来源：https://do.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://ym.zhonguo3118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://ar.zhonguo3118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://gk.zhonguo4118.cn

Go:   os.Remove("a.txt")
来源：https://rn.zhonguo4118.cn

Ruby: File.delete("a.txt")
来源：https://tg.zhonguo8118.cn

C#:   File.Delete("a.txt");
来源：https://uj.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://xj.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://rx.zhonguo3118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://dg.zhonguo1118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://xa.zhonguo7118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://fu.zhonguo5118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://sz.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://au.zhonguo3118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://xv.zhonguo6118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://vk.zhonguo8118.cn

[F08] 遍历目录
来源：https://zs.zhonguo2118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://xa.zhonguo1118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://lv.zhonguo2118.cn

JS:   fs.readdirSync("dir")
来源：https://rs.zhonguo8118.cn

TS:   fs.readdirSync("dir")
来源：https://si.zhonguo2118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://ld.zhonguo5118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://mr.zhonguo6118.cn

Ruby: Dir.children("dir")
来源：https://kk.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://mz.zhonguo7118.cn

[F09] 获取文件大小
来源：https://hr.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://xu.zhonguo7118.cn

PHP:  filesize("a.txt");
来源：https://rx.zhonguo1118.cn

JS:   fs.statSync("a.txt").size
来源：https://tw.zhonguo7118.cn

TS:   fs.statSync("a.txt").size
来源：https://rx.zhonguo1118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://sb.zhonguo5118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://ct.zhonguo8118.cn

Ruby: File.size("a.txt")
来源：https://xf.zhonguo1118.cn

C#:   new FileInfo("a.txt").Length
来源：https://iq.zhonguo2118.cn

[F10] 取文件扩展名 / 文件名
来源：https://fu.zhonguo7118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://zt.zhonguo2118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://pn.zhonguo1118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://by.zhonguo8118.cn

TS:   path.extname("a.txt")
来源：https://ux.zhonguo5118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://dm.zhonguo6118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://oo.zhonguo5118.cn


<!-- 参考信息 -->