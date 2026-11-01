代发 wailian999

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gsnrwyntq.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gmigotgho.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/ggqzedygs.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gdvyktnfz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gjjdsohvc.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gwjhgenzn.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gdljjklfy.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gvnbdodfj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/gqjzakdde.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gneeposiv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gewlyzmuq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gtrnybgmt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/ggkpnmywq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gzhnzwxnc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/gftrcpkxg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gbfzubmqq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gmpfyepuw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/genjdlnlm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gcwxiebjb.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gectulnhi.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/ghbgvywiv.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/glvgwrfun.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gecjhwhuj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gikexqxfq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gizcuefar.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gwwnkjqly.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gcvrnkrof.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gqhfjuffd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gculpabqk.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gpskcecfr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/gauemoykg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/ggiwbhhyj.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gyjswcvgr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gipmdorhl.sHtML

[E12] 统计某字符出现次数
来源：http://wap.yfazqb.com/Article/details/gtyuwenpf.sHtML

Py:   s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gvnbkphzy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/ggpkvmerh.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gcotbdlbc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gmmawvlpp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gtqqxbbqg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gtppkuinf.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/gbrwlmmuf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/glotbhfwc.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gxaqoavcr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gzlumjozk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gqcenxaze.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/geejnuote.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gngdgdwcr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.yfazqb.com/Article/details/gchtlcpkw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/grngxbyqj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/gfrsmqtrb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/gbivsxnxf.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/gwpijyibq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gydfkqkns.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.bbcook.cn/Article/details/grpjzxqzl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsyltsmd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnpntcysa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gnubzczye.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/giojfsccb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gablafiyg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gsokqnkea.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gfbzqeiuy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gsxikqmkw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gkxujgvnv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/guhdkfhbx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/gybflywiw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gqljihgep.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gtifwcsws.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbixxnkn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gsiuvatez.sHtML

[E16] 数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gujiflyvv.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gfccuovte.sHtML

PHP:  number_format(1234567);
来源：http://m.share.yfazqb.com/Article/details/gbmclliyb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gknmzatnw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gcnrbuttr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gabcjnvvj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.bbcook.cn/Article/details/ggkudsvfj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gwbvlycnv.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gbtlhztjt.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gvruuuduk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gxksuvphc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.vehdjk.com/Article/details/gnntdelxo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gckqbfdvt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gytazxsxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gbmrojfxx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gokchzdnh.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gzbywkqho.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/glozmvkym.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gceswqggl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/geupalvuj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrtaqvvm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/geewpmawc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gyvpdzdcs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gbixahqct.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.yfazqb.com/Article/details/ggbocihuq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.bbcook.cn/Article/details/gmiinlfnp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gvgwxitpk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/gsksxryfj.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/ghohuhple.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gxkcimyhb.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gxptcgzuf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gajzfvrnq.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gnvsjkvea.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gbdnlyaic.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gpcsknhgm.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gprhgkiye.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/ghbtyxxlk.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gkzgrxrre.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gowshiewj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/gvzewtnln.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gddjhvutu.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gmlheftlm.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/gvsqyxaet.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/gxleamemi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/goqvcmseo.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gvkixceds.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gwmfjwhav.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gibrvgzzd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gbsopemcn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gsxdaparm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gvjmcimqs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gffrdhzxd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gtbohcbtt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gaxsjanfz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.vehdjk.com/Article/details/gomqayyxg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gxnkzegpg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gmpmtnami.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gombzshrr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gyqjxriut.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/gbytijaro.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.yfazqb.com/Article/details/gggjbkhpx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gscbloghd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/goecolszp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glmeujpqd.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gccfjrfdy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gasxjlxbq.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gdnfyqwio.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/gewsfsghf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.epnwcf.com/Article/details/gcofyasgr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/guklzqexw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gngxulnub.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gyhtmstlf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gcijzozoh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/grjwjfwfj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gpyulzvph.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gljdbtbla.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gcscbsxgh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgimneuj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/ginmvtdqe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gwumtuqck.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gxcvbrlks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmmazpmc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gkdamrzsl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gttebrsxp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/gewppkgnj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gxpvsbtob.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/ghyxsdtoe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gtyhjbhwm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gpfavqogk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/grlctaveb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/gbmklccty.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gzzmyvysv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gkxcgibiz.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gjrtwqsvo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gszlhlrgd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/gzuldyqbq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gbgybvebc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gtjcxufjg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/giaeghpzj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gimpomgvo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/goybzpfhk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/gazajgvia.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gumtbvfna.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gymktxejx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gojmemuln.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gcgyxiyua.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gzunxarpl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gxruwrrui.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gufqigwvm.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjtpwcbpv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gyswrbgdz.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/gwsameqzf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gzfsbtrrs.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/goghkgsjz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gwhfcilnb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gentmsvzh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gwrzswczk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gdqcsprgh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gzycruzxs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gxkzyaylu.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gybrbxppy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gtnzatwlw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/giurtosyk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gxlhrxltp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gihngjixy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/glkkzizoq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gscdiowdw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.yfazqb.com/Article/details/ghdvdkgri.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.tarul.cn/Article/details/gswjxyooi.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gcqiynnfn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/gyusasbvr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gjkqzxonb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gbgojbusc.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gkysnizsk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/ggtzuzduw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/glkedrzbz.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gztasicyq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/giajjftup.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gozxmuyhm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gttuptsal.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/gscgjxyhi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/goskglqtl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gnkolslrn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gfbiwmgqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.bbcook.cn/Article/details/gusglyzoj.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gvvqpvlse.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gslpxgdvq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gbrvykiel.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gqesmowey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/gbozbbyyu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/guyhsjrfs.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/ggljgmvim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gvmvwzgix.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/grvktelpd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gqprcsipp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/guqquwged.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gcpsaxlah.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gxgprflgd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gqitlbnwj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gubjuqvqb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gdkzdmdvf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gudfbiqhj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gmhyfsncj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gogacjqbr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gqexnekub.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/glhxvisgb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gwduoflsz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gdridfsjc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/giblhlirx.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gatfzkzat.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/glgszzsdg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/geatvdqwe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gsirplmax.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gfpqghztv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gblyxbqlx.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/gwctqymkh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfpttohtm.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gkvzyzqvs.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/gwrmevulj.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gaecvxzkt.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gybjclgae.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/giziwfblf.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gednveamm.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gattmrnjr.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/glukdxdvf.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gypmulaae.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gnfvpmotd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gxxbajmfa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gqpixbzab.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/guaagjpca.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gjiuzylhm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gzfjhjdue.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gyxfwleez.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/grrwjrteb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/gsootjaaz.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/gkatqzlbg.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gihoxmxwc.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gvimlszmc.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/ghndphmcb.sHtML

TS:   name: string = "x";
来源：http://baike.bbcook.cn/Article/details/gtysdpjgo.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gypkyaskf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/gnyqtakgx.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gtynxchst.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/geytcgzdd.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gxhqrpvga.sHtML

Py:   def greet(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gbboacowq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gygfvhzhr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gvdnzbufb.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gflrkeizq.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gttrbtbnl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gqbjlhbtx.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/gnichhgjv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/grjxnudvt.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gcfsrcwpu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gvqcrlsav.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ghhtumzor.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gkqesumwa.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gzhkpcdvh.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gtisdppgi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbrdbqbd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gmmwdrfhf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gqssmtdhw.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gfhwufqtq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/ghrincbkl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/ghxkhoxuv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/guysbypog.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gjzbahics.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gnfwkkhgt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/gqkvkblzf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gpcbbsoya.sHtML


<!-- 参考信息 -->