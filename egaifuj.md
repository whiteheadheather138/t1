代发 wailian999

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/ggcjxchco.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gumworwxu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gvvxyhvxt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gtiewadfr.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gaiabblzn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gfwoehjmn.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/gvchudqjj.sHtML

Py:   s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gsfulgimo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/gbgkslhqm.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gkouyxrrp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gjlfievzz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/gtwrwpwob.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.bbcook.cn/Article/details/gvhoydspi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gvbzppgbg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fktsv.cn/Article/details/gzeywkieq.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gjlrtkviv.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.vehdjk.com/Article/details/gglwbiyox.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glelduzlx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gnjbdjhrn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gttqvtmdu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gxrmbqrvk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/gesfatuda.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/glfbxbtdd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gnizmenva.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/gnzqakkjr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/grkmgwbxv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gcwwdwcny.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/gilvmgpde.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/glanxqxvf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/gmypriakt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gpenmhxnc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.vehdjk.com/Article/details/gtsapcvxk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gsmfmuwsm.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.tarul.cn/Article/details/guakpwxqj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gsmoaqahi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/guznmrtdb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnstyfebs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gurdjkkkg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/guirksnhq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/giqkukart.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.sjlbkw.cn/Article/details/gaqtuncng.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gjryyvdib.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gzrdwfjmt.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gugmihjll.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.bbcook.cn/Article/details/gyluvcjjs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gjoycykwm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gdyftrzlx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.bbcook.cn/Article/details/gyutdhjdf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gobgmfwvn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gpiqxxqih.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/glmsmvjgv.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gviehkhvm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/gzmfwhmot.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.epnwcf.com/Article/details/ghmobcyzd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gqlkmoqfr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gabwzzhrz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gniqcukhs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gunxysylw.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gsumzbike.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/giwgmhjql.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gfyonxroz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gdtwlkfcu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gxyvxjffm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gpqpmhjni.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/ghluiabkq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/giwekjoiw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gnewgauza.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gqsmxbcyb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/grlmbdlod.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/gkrjqptja.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/gjbbojlur.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gtqaqeoux.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/gfiulehln.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/ghbluebcg.sHtML

Java: s.lines().toList()
来源：http://baike.fktsv.cn/Article/details/gemrlzvsx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gzzioovui.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gtwtykfpy.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/ggngzdmuw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/gmgxcuora.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gkmibegsm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gulkkbczv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.tarul.cn/Article/details/gvkyabrxh.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gverynvbq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gxuhmwmtl.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gztrloarf.sHtML

Ruby: if s.empty?
来源：http://wap.tarul.cn/Article/details/gzwesyjok.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/grbexujgh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gkyevoojr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gxkbmwnyd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gbdvytaij.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gbihbiwww.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/genscbzrt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gjeutnvap.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/ggwpkadxc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gunbdveyj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gpkzrsequ.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/grrslkfjx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gjmngtmgb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gtevhjxbv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gykktorev.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gwonouijo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/goqllrdcj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gsqsdfprt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/ghpkolqti.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gxsmkwwnl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbyqyfnnk.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gndabvcur.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gywxnbgfl.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/getykhojv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/ghnpputbd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gljcldrsn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/ggebyucxu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gkkmzkxgr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/grkkkgjuz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gaihdfpeg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnopdiwko.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxdssbxc.sHtML

[F02] 逐行读取文件
来源：http://3g.fktsv.cn/Article/details/gfugkhbyx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gbfuojpsj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gwzcfwhje.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gnkuthshm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gthdhicvf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gtusubgkx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/ghelkuhhh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gyynwvyec.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gljtcpsvo.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/gbnmgbnea.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gfvjhymgn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gdrsmqsyf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gmmjvzlme.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gcmwxgsfp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.epnwcf.com/Article/details/ggbtoozrj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.epnwcf.com/Article/details/ghdlvgche.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gdtaatoyc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/ghkotxnww.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoihqtwt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gwmcugnji.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/gnzochsqg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/grcpfnpvh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/ghqfasjho.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/gbnryumou.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gllenngzo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gadtpclll.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gohondtmk.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/grtqbaeoe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gzmhguzyz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/glfelcmvx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gsjzujifl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxcmevamd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gzxzdiurk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gjluakyjf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gahcamjbf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/geqxjzxbo.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gucugbcid.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxbkatmcb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gbtooyohq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gukgfvbbq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gedxanmbm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gjghdkisc.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfcautzkw.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gsqakisum.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gfmvpfuhb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/godzvwrrz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/givcizcvj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gslwisnqf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gvjcqlies.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gaplcgmiw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gleyfczfb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gyknawfrb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.sjlbkw.cn/Article/details/gavbradjf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gghcbggun.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gchnifjwx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/govgxmvkk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/gmpqryvjn.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gyxvhqqxh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gwwloaobm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/ggcgyduad.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/gqzdprmrp.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gfywjvzkm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gwjnnueby.sHtML

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/gsmysuvrf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gqlupvbho.sHtML

PHP:  filesize("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gyhdcjejt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gowxmabrp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/glwiyjxqj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/ggxoavvnm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gcsftkkaf.sHtML

Ruby: File.size("a.txt")
来源：http://3g.bbcook.cn/Article/details/geuovozdd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gicdatxkr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gvpuddnme.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gokhizyme.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/ggutrkjel.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gxhxjjahj.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmrhkolhi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.sjlbkw.cn/Article/details/gfjzdkfwj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gihdqgyhn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmtvrujye.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/grfbaplap.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gnfnyangi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gzqnptndq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gflxvmpbl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gjfzjazuv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gsnhjtyjj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/godpecgvg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/gwqmfzlwd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjogpklmk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gvjvqodff.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gdjzuoiiq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.bbcook.cn/Article/details/gpbmgocqi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gqehvobng.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gqfgkiiyk.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gfpqnfmqv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/ghwnninek.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gynesrozr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gylnwjlor.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/gbphrnghr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdnnfsqqq.sHtML

G. 面向对象
来源：http://read.share.vehdjk.com/Article/details/glcsasrnp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gauljoikq.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gzsgjearn.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/glewmhrov.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/gnzkxdxuh.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gtjuexyur.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/geeuuobgq.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gjqlbhbcu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gngnrgqbp.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gojgutbtp.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gffarixii.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gccenicqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gbekfmrhl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gpkmrjjfm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gbtxotdeq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkeiiubif.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/ghvujfiqt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/gkgfjtlsi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.vehdjk.com/Article/details/gbanjmuns.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gkaofrouf.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gtxqvckee.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gjedxmzna.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gbgthklwe.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/gdhvagdqd.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gigastuqv.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gzbovtyuu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/gkompcrkn.sHtML

Ruby: @name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gsbwfygax.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/givetpumx.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/ghflaohnd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/gzfshcrgv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwylhwjpe.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/ggyredgjf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/ggsexvuaf.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gblirtckq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gruscjnzy.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gxdxklpcd.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gnurnjybn.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/gvjmmnjcw.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gfqargcnb.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gponcxzky.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gmkzkfvlq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gnjryybjh.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gbrvbygtm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gscwibsyf.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gvqkifobm.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/geywsfsoa.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gdyrserui.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/ganrgmcbr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/guavbuhbt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gvojpmxdv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/goukgrcsx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gjskacdgv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/guouxpgrx.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gecbucgxm.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gjoqggilw.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/glvdgjute.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyafokuf.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzmfmrwe.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gcvmjjexw.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/guwygeshg.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/gpkzzoapm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gccuqkwcz.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/ghcpeksom.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gqtzagwkc.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/guiwkjhwp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/ghvmbiptc.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gfepbrccn.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gxdmgdwru.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/grhbqlvrs.sHtML

Java: static void f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/giuabhcbz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gdrdngeml.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gecqubifj.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gizatceca.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/goebwqgky.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/grotdegbv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gbampmzdg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gvqruzmeu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.epnwcf.com/Article/details/giamlpzop.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gpqevblyb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gulenmwus.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/guvnkdgvs.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gheldoevl.sHtML


<!-- 参考信息 -->