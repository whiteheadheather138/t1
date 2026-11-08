代发 wailian999

TS:   "ab".repeat(3)
来源：https://gr.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://zp.zhonguo7118.cn

Go:   strings.Repeat("ab", 3)
来源：https://nb.zhonguo1118.cn

Ruby: "ab" * 3
来源：https://rm.zhonguo7118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ky.zhonguo7118.cn

[E03] 截取子串
来源：https://mn.zhonguo5118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://qm.zhonguo6118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://ne.zhonguo1118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://wk.zhonguo6118.cn

TS:   s.slice(1, 4)
来源：https://ah.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://ix.zhonguo1118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ld.zhonguo5118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://ix.zhonguo7118.cn

C#:   s.Substring(1, 3)
来源：https://sg.zhonguo2118.cn

[E04] 查找子串位置
来源：https://uy.zhonguo2118.cn

Py:   s.find("x");  s.index("x")
来源：https://xx.zhonguo8118.cn

PHP:  strpos($s, "x");
来源：https://kc.zhonguo8118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://cq.zhonguo6118.cn

TS:   s.indexOf("x")
来源：https://cj.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://hf.zhonguo5118.cn

Go:   strings.Index(s, "x")
来源：https://fl.zhonguo1118.cn

Ruby: s.index("x")
来源：https://nq.zhonguo1118.cn

C#:   s.IndexOf("x")
来源：https://px.zhonguo3118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://xk.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ig.zhonguo5118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://od.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://gz.zhonguo1118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://qv.zhonguo7118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://am.zhonguo8118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://qu.zhonguo5118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://gh.zhonguo5118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://lh.zhonguo1118.cn

[E06] 替换子串
来源：https://rh.zhonguo1118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://ks.zhonguo7118.cn

PHP:  str_replace("a", "b", $s);
来源：https://xz.zhonguo4118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://gm.zhonguo1118.cn

TS:   s.replaceAll("a", "b")
来源：https://ab.zhonguo5118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://az.zhonguo6118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://de.zhonguo8118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://my.zhonguo5118.cn

C#:   s.Replace("a", "b")
来源：https://fv.zhonguo3118.cn

[E07] 按分隔符拆分
来源：https://hz.zhonguo6118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://mg.zhonguo4118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://jm.zhonguo8118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://ib.zhonguo6118.cn

TS:   s.split(",")
来源：https://uk.zhonguo5118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://tt.zhonguo4118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://eh.zhonguo1118.cn

Ruby: s.split(",");  s.split
来源：https://hg.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://wl.zhonguo8118.cn

[E08] 数组按分隔符合并
来源：https://gs.zhonguo3118.cn

Py:   ",".join(items)
来源：https://py.zhonguo6118.cn

PHP:  implode(",", $items);
来源：https://br.zhonguo2118.cn

JS:   items.join(",")
来源：https://jh.zhonguo6118.cn

TS:   items.join(",")
来源：https://op.zhonguo3118.cn

Java: String.join(",", items)
来源：https://lx.zhonguo8118.cn

Go:   strings.Join(items, ",")
来源：https://sv.zhonguo6118.cn

Ruby: items.join(",")
来源：https://db.zhonguo5118.cn

C#:   string.Join(",", items)
来源：https://yz.zhonguo8118.cn

[E09] 去除所有空白字符
来源：https://iv.zhonguo3118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ym.zhonguo5118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://ov.zhonguo4118.cn

JS:   s.replace(/\s+/g, "")
来源：https://ya.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://vx.zhonguo7118.cn

Java: s.replaceAll("\\s+", "")
来源：https://xp.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://vb.zhonguo2118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://tu.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://iy.zhonguo2118.cn

[E10] 左侧补零 / 定长填充
来源：https://rz.zhonguo5118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ms.zhonguo8118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://wb.zhonguo6118.cn

JS:   "7".padStart(3, "0")
来源：https://mv.zhonguo4118.cn

TS:   "7".padStart(3, "0")
来源：https://pa.zhonguo2118.cn

Java: String.format("%03d", 7)
来源：https://ez.zhonguo4118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://cn.zhonguo4118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://vp.zhonguo6118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://xc.zhonguo3118.cn

[E11] 反转字符串
来源：https://gt.zhonguo5118.cn

Py:   s[::-1]
来源：https://hu.zhonguo3118.cn

PHP:  strrev($s);
来源：https://dz.zhonguo3118.cn

JS:   [...s].reverse().join("")
来源：https://vw.zhonguo3118.cn

TS:   [...s].reverse().join("")
来源：https://xh.zhonguo2118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://cf.zhonguo7118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://sj.zhonguo7118.cn

Ruby: s.reverse
来源：https://xq.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://tp.zhonguo8118.cn

[E12] 统计某字符出现次数
来源：https://mv.zhonguo5118.cn

Py:   s.count("a")
来源：https://gi.zhonguo3118.cn

PHP:  substr_count($s, "a");
来源：https://pw.zhonguo6118.cn

JS:   s.split("a").length - 1
来源：https://qv.zhonguo7118.cn

TS:   s.split("a").length - 1
来源：https://it.zhonguo1118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://nv.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://vw.zhonguo6118.cn

Ruby: s.count("a")
来源：https://ku.zhonguo1118.cn

C#:   s.Count(c => c == 'a')
来源：https://rp.zhonguo1118.cn

[E13] 逐字符遍历
来源：https://zv.zhonguo3118.cn

Py:   for ch in s: print(ch)
来源：https://xf.zhonguo6118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://nz.zhonguo3118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://ly.zhonguo1118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://sm.zhonguo2118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://dx.zhonguo3118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://dc.zhonguo4118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://oq.zhonguo2118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://df.zhonguo3118.cn

[E14] URL 编码与 Base64
来源：https://ct.zhonguo6118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://uu.zhonguo7118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://mn.zhonguo1118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://my.zhonguo4118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://eo.zhonguo2118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://um.zhonguo6118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://np.zhonguo3118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://qw.zhonguo5118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://qh.zhonguo6118.cn

[E15] HTML 转义 / 反转义
来源：https://ft.zhonguo3118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://xe.zhonguo6118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://gk.zhonguo8118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://wl.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://nm.zhonguo2118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://zi.zhonguo3118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://qs.zhonguo4118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://op.zhonguo3118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://cx.zhonguo6118.cn

[E16] 数字千分位
来源：https://xx.zhonguo7118.cn

Py:   f"{1234567:,}"
来源：https://bg.zhonguo1118.cn

PHP:  number_format(1234567);
来源：https://ov.zhonguo1118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://vc.zhonguo3118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://ss.zhonguo3118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://ic.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://my.zhonguo8118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://ai.zhonguo6118.cn

C#:   1234567.ToString("N0")
来源：https://qd.zhonguo4118.cn

[E17] 首字母大写
来源：https://wz.zhonguo6118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://ht.zhonguo7118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://sw.zhonguo2118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://vp.zhonguo3118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://to.zhonguo5118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://vb.zhonguo2118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://jp.zhonguo8118.cn

Ruby: s.capitalize
来源：https://ho.zhonguo7118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://by.zhonguo2118.cn

[E18] 模板占位符替换
来源：https://mk.zhonguo3118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ch.zhonguo6118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://en.zhonguo2118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://mc.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://tc.zhonguo1118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://bh.zhonguo3118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://bx.zhonguo5118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://zt.zhonguo7118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://kx.zhonguo5118.cn

[E19] 多行文本按行拆分
来源：https://lu.zhonguo3118.cn

Py:   s.splitlines()
来源：https://yh.zhonguo3118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://bz.zhonguo7118.cn

JS:   s.split(/\r?\n/)
来源：https://fh.zhonguo4118.cn

TS:   s.split(/\r?\n/)
来源：https://ss.zhonguo1118.cn

Java: s.lines().toList()
来源：https://ga.zhonguo4118.cn

Go:   strings.Split(s, "\n")
来源：https://rc.zhonguo2118.cn

Ruby: s.lines
来源：https://ct.zhonguo2118.cn

C#:   s.Split('\n')
来源：https://ux.zhonguo3118.cn

[E20] 判断字符串是否为空
来源：https://yi.zhonguo3118.cn

Py:   if not s:
来源：https://rd.zhonguo7118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://jh.zhonguo1118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ir.zhonguo1118.cn

TS:   if (s === "") {}
来源：https://gr.zhonguo6118.cn

Java: if (s.isEmpty()) {}
来源：https://mn.zhonguo7118.cn

Go:   if s == "" {}
来源：https://dv.zhonguo2118.cn

Ruby: if s.empty?
来源：https://in.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://fv.zhonguo6118.cn

[E21] 超长截断加省略号
来源：https://tz.zhonguo1118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://zg.zhonguo5118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://pu.zhonguo2118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://gg.zhonguo1118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://nu.zhonguo6118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://pf.zhonguo6118.cn

Go:   // 按 rune 判断长度后截断
来源：https://ug.zhonguo3118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://xr.zhonguo5118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://cu.zhonguo5118.cn

[E22] 字节长度与字符长度
来源：https://yv.zhonguo5118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://nh.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://jm.zhonguo8118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://ng.zhonguo2118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://kf.zhonguo6118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://bc.zhonguo6118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://yn.zhonguo1118.cn

Ruby: s.bytesize;  s.length
来源：https://ep.zhonguo4118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://hf.zhonguo2118.cn

================================================================================
来源：https://ib.zhonguo8118.cn

F. 文件与目录
来源：https://iz.zhonguo5118.cn

================================================================================
来源：https://kd.zhonguo7118.cn

[F01] 读取整个文件
来源：https://gv.zhonguo7118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://jb.zhonguo6118.cn

PHP:  file_get_contents("a.txt");
来源：https://us.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://gx.zhonguo7118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://oh.zhonguo8118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ek.zhonguo8118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://rm.zhonguo1118.cn

Ruby: File.read("a.txt")
来源：https://nx.zhonguo5118.cn

C#:   File.ReadAllText("a.txt");
来源：https://uy.zhonguo4118.cn

[F02] 逐行读取文件
来源：https://nb.zhonguo7118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ef.zhonguo3118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://hh.zhonguo7118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://bv.zhonguo4118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://hz.zhonguo8118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://od.zhonguo1118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://gt.zhonguo3118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ou.zhonguo1118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://cn.zhonguo1118.cn

[F03] 写入文件（覆盖）
来源：https://pg.zhonguo8118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://gq.zhonguo6118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://gd.zhonguo5118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://rv.zhonguo1118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://oy.zhonguo8118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://xb.zhonguo8118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://wl.zhonguo5118.cn

Ruby: File.write("a.txt", "hi")
来源：https://lb.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://of.zhonguo1118.cn

[F04] 追加写入文件
来源：https://yj.zhonguo7118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://lc.zhonguo8118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://xp.zhonguo8118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://xz.zhonguo2118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://dc.zhonguo4118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://ka.zhonguo3118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://uk.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://mk.zhonguo8118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://ic.zhonguo5118.cn

[F05] 判断文件或目录是否存在
来源：https://lu.zhonguo3118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://nx.zhonguo5118.cn

PHP:  file_exists("a.txt");
来源：https://xe.zhonguo5118.cn

JS:   fs.existsSync("a.txt")
来源：https://vc.zhonguo4118.cn

TS:   fs.existsSync("a.txt")
来源：https://na.zhonguo4118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ni.zhonguo2118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://lh.zhonguo5118.cn

Ruby: File.exist?("a.txt")
来源：https://ae.zhonguo7118.cn

C#:   File.Exists("a.txt")
来源：https://wp.zhonguo7118.cn

[F06] 删除文件
来源：https://la.zhonguo8118.cn

Py:   os.remove("a.txt")
来源：https://ed.zhonguo1118.cn

PHP:  unlink("a.txt");
来源：https://wn.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://it.zhonguo5118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://bc.zhonguo1118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://ml.zhonguo2118.cn

Go:   os.Remove("a.txt")
来源：https://wg.zhonguo1118.cn

Ruby: File.delete("a.txt")
来源：https://hk.zhonguo5118.cn

C#:   File.Delete("a.txt");
来源：https://qm.zhonguo3118.cn

[F07] 创建目录（含多级）
来源：https://ck.zhonguo6118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://zi.zhonguo4118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://vi.zhonguo5118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://zt.zhonguo7118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://mx.zhonguo2118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://gx.zhonguo5118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://id.zhonguo8118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://bi.zhonguo2118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://cl.zhonguo1118.cn

[F08] 遍历目录
来源：https://qw.zhonguo8118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ge.zhonguo7118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://wv.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://uq.zhonguo5118.cn

TS:   fs.readdirSync("dir")
来源：https://da.zhonguo6118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://yp.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://py.zhonguo2118.cn

Ruby: Dir.children("dir")
来源：https://wj.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://nl.zhonguo5118.cn

[F09] 获取文件大小
来源：https://vd.zhonguo2118.cn

Py:   os.path.getsize("a.txt")
来源：https://xo.zhonguo7118.cn

PHP:  filesize("a.txt");
来源：https://zo.zhonguo8118.cn

JS:   fs.statSync("a.txt").size
来源：https://so.zhonguo4118.cn

TS:   fs.statSync("a.txt").size
来源：https://kj.zhonguo4118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://rd.zhonguo6118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://bk.zhonguo7118.cn

Ruby: File.size("a.txt")
来源：https://st.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://ab.zhonguo7118.cn

[F10] 取文件扩展名 / 文件名
来源：https://kb.zhonguo4118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://kn.zhonguo3118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://yc.zhonguo8118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://oo.zhonguo5118.cn

TS:   path.extname("a.txt")
来源：https://eb.zhonguo2118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://ea.zhonguo2118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://qt.zhonguo7118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://dg.zhonguo2118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://db.zhonguo5118.cn

[F11] 复制与移动文件
来源：https://ak.zhonguo2118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://kt.zhonguo5118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://rq.zhonguo3118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://bq.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://fq.zhonguo4118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://ui.zhonguo5118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://vj.zhonguo6118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://cu.zhonguo7118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://au.zhonguo5118.cn

[F12] CSV 读写
来源：https://ro.zhonguo7118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://tr.zhonguo6118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://ib.zhonguo3118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://dw.zhonguo7118.cn

TS:   // 同上
来源：https://ys.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://jw.zhonguo8118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://yd.zhonguo3118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://pu.zhonguo7118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ir.zhonguo3118.cn

================================================================================
来源：https://ea.zhonguo6118.cn

G. 面向对象
来源：https://zc.zhonguo4118.cn

================================================================================
来源：https://vv.zhonguo8118.cn

[G01] 定义类
来源：https://xe.zhonguo6118.cn


<!-- 参考信息 -->