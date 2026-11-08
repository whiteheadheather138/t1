代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://ti.zhonguo6118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://fi.zhonguo5118.cn

[D25] Set 集合去重与交并差
来源：https://mc.zhonguo5118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://xn.zhonguo4118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://ol.zhonguo1118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://mh.zhonguo2118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://in.zhonguo2118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://nc.zhonguo1118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://it.zhonguo1118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://uw.zhonguo5118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://fa.zhonguo2118.cn

[D26] 数组转字符串
来源：https://ag.zhonguo1118.cn

Py:   ", ".join(map(str, arr))
来源：https://ua.zhonguo7118.cn

PHP:  implode(", ", $arr);
来源：https://ca.zhonguo4118.cn

JS:   arr.join(", ")
来源：https://xj.zhonguo5118.cn

TS:   arr.join(", ")
来源：https://il.zhonguo8118.cn

Java: String.join(", ", list)
来源：https://um.zhonguo6118.cn

Go:   strings.Join(strs, ", ")
来源：https://qp.zhonguo3118.cn

Ruby: arr.join(", ")
来源：https://bt.zhonguo2118.cn

C#:   string.Join(", ", list)
来源：https://yx.zhonguo4118.cn

================================================================================
来源：https://tp.zhonguo5118.cn

E. 字符串处理
来源：https://gk.zhonguo2118.cn

================================================================================
来源：https://xn.zhonguo2118.cn

[E01] 拼接字符串
来源：https://oj.zhonguo3118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://at.zhonguo7118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://wn.zhonguo8118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://qp.zhonguo2118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://hw.zhonguo6118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://kj.zhonguo5118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://lc.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://oc.zhonguo7118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://qu.zhonguo8118.cn

[E02] 重复字符串
来源：https://ah.zhonguo4118.cn

Py:   "ab" * 3
来源：https://wm.zhonguo5118.cn

PHP:  str_repeat("ab", 3);
来源：https://bu.zhonguo2118.cn

JS:   "ab".repeat(3)
来源：https://mq.zhonguo2118.cn

TS:   "ab".repeat(3)
来源：https://gb.zhonguo5118.cn

Java: "ab".repeat(3)
来源：https://kj.zhonguo8118.cn

Go:   strings.Repeat("ab", 3)
来源：https://cw.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://mf.zhonguo8118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ck.zhonguo3118.cn

[E03] 截取子串
来源：https://rv.zhonguo7118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://gx.zhonguo5118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://xc.zhonguo1118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://hm.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://vl.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://zv.zhonguo4118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://db.zhonguo3118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://qb.zhonguo4118.cn

C#:   s.Substring(1, 3)
来源：https://je.zhonguo1118.cn

[E04] 查找子串位置
来源：https://ro.zhonguo2118.cn

Py:   s.find("x");  s.index("x")
来源：https://lo.zhonguo6118.cn

PHP:  strpos($s, "x");
来源：https://do.zhonguo2118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://rc.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://jy.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://fh.zhonguo5118.cn

Go:   strings.Index(s, "x")
来源：https://vc.zhonguo7118.cn

Ruby: s.index("x")
来源：https://ms.zhonguo2118.cn

C#:   s.IndexOf("x")
来源：https://lf.zhonguo1118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://fi.zhonguo1118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://we.zhonguo5118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://if.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://cg.zhonguo4118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://xi.zhonguo1118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://xq.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://km.zhonguo4118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://pe.zhonguo6118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://mc.zhonguo6118.cn

[E06] 替换子串
来源：https://oe.zhonguo2118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://es.zhonguo6118.cn

PHP:  str_replace("a", "b", $s);
来源：https://cu.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://dq.zhonguo4118.cn

TS:   s.replaceAll("a", "b")
来源：https://fq.zhonguo2118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://el.zhonguo3118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://iy.zhonguo6118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://wo.zhonguo4118.cn

C#:   s.Replace("a", "b")
来源：https://sf.zhonguo3118.cn

[E07] 按分隔符拆分
来源：https://ku.zhonguo1118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://hv.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://ua.zhonguo8118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://qw.zhonguo7118.cn

TS:   s.split(",")
来源：https://yr.zhonguo7118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://qf.zhonguo1118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ns.zhonguo8118.cn

Ruby: s.split(",");  s.split
来源：https://xq.zhonguo6118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://db.zhonguo3118.cn

[E08] 数组按分隔符合并
来源：https://tn.zhonguo2118.cn

Py:   ",".join(items)
来源：https://pg.zhonguo2118.cn

PHP:  implode(",", $items);
来源：https://wd.zhonguo7118.cn

JS:   items.join(",")
来源：https://yb.zhonguo2118.cn

TS:   items.join(",")
来源：https://ef.zhonguo1118.cn

Java: String.join(",", items)
来源：https://ad.zhonguo3118.cn

Go:   strings.Join(items, ",")
来源：https://ub.zhonguo1118.cn

Ruby: items.join(",")
来源：https://qo.zhonguo5118.cn

C#:   string.Join(",", items)
来源：https://jv.zhonguo6118.cn

[E09] 去除所有空白字符
来源：https://fp.zhonguo3118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://di.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://ms.zhonguo6118.cn

JS:   s.replace(/\s+/g, "")
来源：https://ir.zhonguo6118.cn

TS:   s.replace(/\s+/g, "")
来源：https://cp.zhonguo6118.cn

Java: s.replaceAll("\\s+", "")
来源：https://qp.zhonguo2118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://uk.zhonguo4118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://pf.zhonguo3118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://qp.zhonguo4118.cn

[E10] 左侧补零 / 定长填充
来源：https://uy.zhonguo7118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ra.zhonguo6118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ik.zhonguo6118.cn

JS:   "7".padStart(3, "0")
来源：https://ig.zhonguo8118.cn

TS:   "7".padStart(3, "0")
来源：https://xj.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://pg.zhonguo8118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://qy.zhonguo7118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://ab.zhonguo6118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://sc.zhonguo8118.cn

[E11] 反转字符串
来源：https://xu.zhonguo3118.cn

Py:   s[::-1]
来源：https://rj.zhonguo1118.cn

PHP:  strrev($s);
来源：https://dj.zhonguo1118.cn

JS:   [...s].reverse().join("")
来源：https://xn.zhonguo1118.cn

TS:   [...s].reverse().join("")
来源：https://zm.zhonguo8118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ch.zhonguo1118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://ko.zhonguo2118.cn

Ruby: s.reverse
来源：https://ow.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://wo.zhonguo6118.cn

[E12] 统计某字符出现次数
来源：https://od.zhonguo7118.cn

Py:   s.count("a")
来源：https://mj.zhonguo7118.cn

PHP:  substr_count($s, "a");
来源：https://jb.zhonguo2118.cn

JS:   s.split("a").length - 1
来源：https://iu.zhonguo8118.cn

TS:   s.split("a").length - 1
来源：https://ug.zhonguo2118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://wn.zhonguo6118.cn

Go:   strings.Count(s, "a")
来源：https://nm.zhonguo3118.cn

Ruby: s.count("a")
来源：https://qa.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://ue.zhonguo5118.cn

[E13] 逐字符遍历
来源：https://fa.zhonguo5118.cn

Py:   for ch in s: print(ch)
来源：https://nb.zhonguo6118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://rp.zhonguo6118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://cy.zhonguo2118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ee.zhonguo8118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://cr.zhonguo6118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://yg.zhonguo2118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://av.zhonguo5118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://oq.zhonguo2118.cn

[E14] URL 编码与 Base64
来源：https://iw.zhonguo1118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://tg.zhonguo3118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://qp.zhonguo7118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://nk.zhonguo5118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://ei.zhonguo5118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://wg.zhonguo2118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://so.zhonguo5118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://xv.zhonguo6118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://pj.zhonguo8118.cn

[E15] HTML 转义 / 反转义
来源：https://yu.zhonguo6118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://xb.zhonguo8118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://nd.zhonguo8118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://do.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://db.zhonguo1118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://vw.zhonguo1118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://ai.zhonguo3118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://sz.zhonguo8118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://zv.zhonguo4118.cn

[E16] 数字千分位
来源：https://ox.zhonguo5118.cn

Py:   f"{1234567:,}"
来源：https://ez.zhonguo7118.cn

PHP:  number_format(1234567);
来源：https://zx.zhonguo1118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://qh.zhonguo2118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://lf.zhonguo1118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://qs.zhonguo2118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://ya.zhonguo1118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://yr.zhonguo8118.cn

C#:   1234567.ToString("N0")
来源：https://kw.zhonguo1118.cn

[E17] 首字母大写
来源：https://ge.zhonguo6118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://zh.zhonguo5118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://eo.zhonguo4118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://bg.zhonguo5118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ri.zhonguo1118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://fr.zhonguo4118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://vc.zhonguo1118.cn

Ruby: s.capitalize
来源：https://md.zhonguo3118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://qr.zhonguo8118.cn

[E18] 模板占位符替换
来源：https://zx.zhonguo4118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://jx.zhonguo2118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://fi.zhonguo4118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://bk.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://uh.zhonguo3118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://bh.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://rz.zhonguo3118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://rb.zhonguo2118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://sc.zhonguo7118.cn

[E19] 多行文本按行拆分
来源：https://rb.zhonguo3118.cn

Py:   s.splitlines()
来源：https://br.zhonguo4118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://bd.zhonguo3118.cn

JS:   s.split(/\r?\n/)
来源：https://ke.zhonguo2118.cn

TS:   s.split(/\r?\n/)
来源：https://yk.zhonguo4118.cn

Java: s.lines().toList()
来源：https://sl.zhonguo4118.cn

Go:   strings.Split(s, "\n")
来源：https://vy.zhonguo4118.cn

Ruby: s.lines
来源：https://ya.zhonguo1118.cn

C#:   s.Split('\n')
来源：https://bz.zhonguo2118.cn

[E20] 判断字符串是否为空
来源：https://an.zhonguo4118.cn

Py:   if not s:
来源：https://ko.zhonguo1118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://oy.zhonguo8118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ee.zhonguo6118.cn

TS:   if (s === "") {}
来源：https://yp.zhonguo4118.cn

Java: if (s.isEmpty()) {}
来源：https://st.zhonguo7118.cn

Go:   if s == "" {}
来源：https://wl.zhonguo4118.cn

Ruby: if s.empty?
来源：https://gk.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://eh.zhonguo6118.cn

[E21] 超长截断加省略号
来源：https://rb.zhonguo3118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://sp.zhonguo4118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://up.zhonguo5118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://gs.zhonguo1118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://cl.zhonguo6118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://rf.zhonguo5118.cn

Go:   // 按 rune 判断长度后截断
来源：https://uq.zhonguo1118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://eb.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://sf.zhonguo3118.cn

[E22] 字节长度与字符长度
来源：https://lz.zhonguo5118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://hi.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://hg.zhonguo4118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://zp.zhonguo7118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://ht.zhonguo8118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://yk.zhonguo1118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://sd.zhonguo5118.cn

Ruby: s.bytesize;  s.length
来源：https://pz.zhonguo6118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://xl.zhonguo1118.cn

================================================================================
来源：https://fs.zhonguo4118.cn

F. 文件与目录
来源：https://nr.zhonguo7118.cn

================================================================================
来源：https://kz.zhonguo2118.cn

[F01] 读取整个文件
来源：https://gs.zhonguo8118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://cr.zhonguo5118.cn

PHP:  file_get_contents("a.txt");
来源：https://kf.zhonguo7118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://fg.zhonguo4118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://tz.zhonguo5118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://sr.zhonguo5118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ca.zhonguo6118.cn

Ruby: File.read("a.txt")
来源：https://bz.zhonguo3118.cn

C#:   File.ReadAllText("a.txt");
来源：https://tz.zhonguo3118.cn

[F02] 逐行读取文件
来源：https://lq.zhonguo4118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://sk.zhonguo5118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://yt.zhonguo2118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://nu.zhonguo7118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://jj.zhonguo1118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://ts.zhonguo2118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://li.zhonguo8118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://gd.zhonguo3118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://li.zhonguo5118.cn

[F03] 写入文件（覆盖）
来源：https://gz.zhonguo5118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://zv.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://iy.zhonguo1118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://uk.zhonguo4118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://cy.zhonguo2118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ru.zhonguo1118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://qh.zhonguo8118.cn

Ruby: File.write("a.txt", "hi")
来源：https://lo.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://wf.zhonguo4118.cn

[F04] 追加写入文件
来源：https://fk.zhonguo1118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://xv.zhonguo7118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://us.zhonguo2118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://rb.zhonguo7118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://gr.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://se.zhonguo6118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://rt.zhonguo5118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://fi.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://wu.zhonguo4118.cn

[F05] 判断文件或目录是否存在
来源：https://qf.zhonguo2118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://mn.zhonguo7118.cn

PHP:  file_exists("a.txt");
来源：https://gx.zhonguo6118.cn

JS:   fs.existsSync("a.txt")
来源：https://vv.zhonguo5118.cn

TS:   fs.existsSync("a.txt")
来源：https://md.zhonguo4118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ii.zhonguo8118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://xe.zhonguo1118.cn

Ruby: File.exist?("a.txt")
来源：https://bd.zhonguo5118.cn

C#:   File.Exists("a.txt")
来源：https://vx.zhonguo1118.cn

[F06] 删除文件
来源：https://dp.zhonguo2118.cn

Py:   os.remove("a.txt")
来源：https://zd.zhonguo2118.cn

PHP:  unlink("a.txt");
来源：https://py.zhonguo6118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://ey.zhonguo1118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://rt.zhonguo2118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://lb.zhonguo8118.cn

Go:   os.Remove("a.txt")
来源：https://ek.zhonguo5118.cn

Ruby: File.delete("a.txt")
来源：https://ql.zhonguo2118.cn

C#:   File.Delete("a.txt");
来源：https://rw.zhonguo7118.cn

[F07] 创建目录（含多级）
来源：https://ry.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://oy.zhonguo7118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://lk.zhonguo8118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://bb.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://hm.zhonguo7118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://qa.zhonguo4118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://ho.zhonguo1118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://fn.zhonguo8118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://ol.zhonguo8118.cn

[F08] 遍历目录
来源：https://ae.zhonguo6118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://fd.zhonguo5118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://ra.zhonguo3118.cn

JS:   fs.readdirSync("dir")
来源：https://dp.zhonguo2118.cn

TS:   fs.readdirSync("dir")
来源：https://ir.zhonguo3118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://fz.zhonguo6118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://mc.zhonguo7118.cn

Ruby: Dir.children("dir")
来源：https://iz.zhonguo6118.cn

C#:   Directory.GetFiles("dir")
来源：https://ai.zhonguo1118.cn

[F09] 获取文件大小
来源：https://ko.zhonguo6118.cn

Py:   os.path.getsize("a.txt")
来源：https://og.zhonguo8118.cn

PHP:  filesize("a.txt");
来源：https://sk.zhonguo4118.cn

JS:   fs.statSync("a.txt").size
来源：https://az.zhonguo8118.cn


<!-- 参考信息 -->