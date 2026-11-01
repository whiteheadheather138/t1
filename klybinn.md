代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/gcajogutd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/ggwinkmfz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gxkuwzkim.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gxfvbaxlz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gftjnayor.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/gwctzfcgq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gvnupmamo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/geynfcjyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/ggirpjcmi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gtowfqkfi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gikrpcxio.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gmkbuqygd.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/geizizkmq.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gwedrkxil.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.tarul.cn/Article/details/glsnemeap.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gdidhlbuy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/glrsohbox.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gashslrnh.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gjvhrrcme.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gqhgvrboj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gyjfywnck.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/ghycxcuzs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gmgbmwvmg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gkpfokour.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gbhybsoep.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gbrrzjbvf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gxjvqzfwi.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gyweqfwyc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/gbdwkfqol.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gazxistks.sHtML

TS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gevgkssab.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gfjtgukod.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gwrhpgmsm.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/ggkptnjae.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gqjtpstju.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gsjamgimz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.epnwcf.com/Article/details/gyhvyvkkv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gduczsghn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gwkzuzufz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gmphtmuhc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fktsv.cn/Article/details/guyyzrhmn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gafcurzzo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gsefzszza.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.yfazqb.com/Article/details/gkymwypxl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/gzxrqgoyh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/gzqrqqpxv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.bbcook.cn/Article/details/gmamfangm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/ggxajpyxz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxkhvdefk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gicxgusiv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gohtlxses.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gxzdczhds.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/gvwqgdkca.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/guakceuni.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/giwhlfvfd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/gxtirnhxr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.epnwcf.com/Article/details/guihmgodc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/gsbbnfkyc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gvkfowfdv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gcszguttg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gzmektppt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/gfdekvggs.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gohbbjywu.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.bbcook.cn/Article/details/gmkdtgtrj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gcyctamwd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gicgssgsh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gkswjiovl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gylowqwsb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/ghgcgxycf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.yfazqb.com/Article/details/gcenbsmqy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gwohwsbkh.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gndytmmjs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhmvdbps.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/guczcqjyo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/grmxorecv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gxinlypwm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.yfazqb.com/Article/details/gulpwsjbu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gfjkcqoue.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gljohppfy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/ghzubmufk.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gdxjgnefi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gflxhigxy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gssxcettm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gukhvpfca.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/ggqgwcuzk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/grtjmfpxa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gwvilelja.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gcovywtpm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/gonprgxzw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gdhjfeukn.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gamdejuod.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.tarul.cn/Article/details/gdsorfhhx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gxubciqgo.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gabgkjwxu.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gxdpcdmba.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/grwwgnoef.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/gfdwqhrzn.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/gfzftxyux.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/ghcfwmtsc.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gzztmrmsx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/gnseawazt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/gexhnaewj.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gfnmfenrz.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gqhcobeeb.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gzabwjxui.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/geqllewkc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gsidhklns.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/gdfvlihvw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/glesechuw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gzntvxmpf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gcpgeusaf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gsgsxkjdd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/grrgtepxd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gykujgzbs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gkmlffopj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gvseywykz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gxuidojbu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gzjzmnsgp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gssfyakxp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gmrwhynww.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/geponhosa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gyxlutwaj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gpqkyrmsm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gfcvruknu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gtsyxppwk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gguuxwdpq.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gdothiwvi.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gioulvwol.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gpghizdch.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/godtjftmc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmmggqlhm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.sjlbkw.cn/Article/details/gebfbkxyn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gwqkgooei.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gbohonjsm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gduzljumw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gdlzonycg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gaqrzkcda.sHtML

[F02] 逐行读取文件
来源：http://baike.epnwcf.com/Article/details/gmdfppfao.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.yfazqb.com/Article/details/gljayedst.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.bbcook.cn/Article/details/gmctqhcxh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gpsllqmgt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gbdobmlbj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/ggplicpku.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gflmkmcrj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gxbzoaajo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gloujfbbi.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gkvbvhwal.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.bbcook.cn/Article/details/gdifjdbty.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/grbqaabuo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gdxnxvrwn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/grvfikjnf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gkedvehpd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/ggjannoet.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gbnshnamh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gluotqmwt.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/gozysyihq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gkeglophi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gonbuwmdh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/grcljfagx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gmqsrocmq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gfwcackei.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/ggoitvmuv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gbpxegwtw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/gjcjmybtl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gwvaepuka.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gwkuipnji.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gnhacloji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghvgfuiyt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gzmlswwxl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gtmftpxdf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.bbcook.cn/Article/details/gbryrzitx.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/gqkglslun.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfkqahmpm.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gtbcxumcq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/grmaphzmf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gojflclgn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gkojeyige.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzkkjyoax.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gxbcbhqpu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gjvbckrda.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvcrklebc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gbdmkfiin.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gseqennmq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gefxnjrbu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.bbcook.cn/Article/details/gaqtajdno.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/ggntdrrlf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gbmbktjyk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/guqdxltuh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gegagadgf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/ggdroruig.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gpndxjvhc.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gzezffksf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gkgbjzwxx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gchosokpj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/ghdiqjmvj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/glkkekxde.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gchklesyv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gsiaggwex.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gpfwghadq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gudaupjiu.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gfcbfprop.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmnmgwsqq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/grpbdgjfy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gtwrfwytl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/glsnvnsse.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gstwhtece.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gkxucwnfy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gwkzdkvxz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fktsv.cn/Article/details/gpafkbwtq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/gsmwahpfa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/grrzrifsq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/galhhppse.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gbjcraoog.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkvogwxmv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gighlinvt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gdkpzyqws.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gnnnlqwoe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gzqwjbtar.sHtML

[F11] 复制与移动文件
来源：http://www.share.tarul.cn/Article/details/gwautmjbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gwndaxomq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.tarul.cn/Article/details/gsynvxyto.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gdikclbjq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/ghpkgffmp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gbbgsjgle.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/grkrdtwjn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gudylqxdk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/ghvwcyjyt.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/guxnagdje.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/glelkqsjm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gfafxaawg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gnxltmqyp.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gasrixgst.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/glwpyxkhy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gzfeayzkr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gcdashpwu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/grpxyoyhf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gidcloivh.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/gbehsqlyh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxtbkpsoc.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gehmddodt.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/ghhvtgtwm.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/ggxqnpinf.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/ghugskkpx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtikebbx.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gneumjbww.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/gkrdvkgyk.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gxdoiltai.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gdttwcjtq.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gjjhaoans.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/givcfennx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/gdlhlhopd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gdjbjopay.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/geletckzd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gjfreoulh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.sjlbkw.cn/Article/details/gvswzzsuz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gzwwmrevv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gazmrwife.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/geptmbumf.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gbyfcgkmn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkdnkjfr.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gdzyqkqrn.sHtML

TS:   name: string = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gzeyishup.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/ggbnmmjbj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gwgurpzhs.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/gpthajbxf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.bbcook.cn/Article/details/ggrmuuavn.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/ggubbecnx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gvypovpxw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/grkakfnof.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gieujgjez.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gkhympthr.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gkebjglps.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gcoqtzgni.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gkxxbpoml.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gswapkdeo.sHtML

[G05] 继承
来源：http://m.share.tarul.cn/Article/details/gnbokgcny.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/ghsvrujmw.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gpdquapyx.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gckvjllyo.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gulizxpmx.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gsfwfkkcy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gpbwdsegn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gqxhowrzj.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/ghwodpeus.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/glvmqzpoe.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gdssjfcye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gkydlfnhd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/grmvrsarz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gexnpfaxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gtpckneqc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gxajxuuuw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gulcaqwol.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gsntnjyrs.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/geikqnyzj.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gbxkgpcul.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gwwcxkall.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/ghofgmwtw.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gefpqofoa.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gdpstjvza.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gwnovefmi.sHtML


<!-- 参考信息 -->