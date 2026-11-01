代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/ggwbnepse.sHtML

[E11] 反转字符串
来源：http://3g.epnwcf.com/Article/details/gjptteuvu.sHtML

Py:   s[::-1]
来源：http://wap.yfazqb.com/Article/details/gjxxkvzts.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/ggqtbcelq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gwxpxcgtg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gjxonmumm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/gqlciswmy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gcjkffgsd.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gmbxmaqiw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/ggcataejy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gwcsciycy.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gaklbrory.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/gmwwnaqtu.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/grjjoqyfb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gmscgufmr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/guaxfdjdi.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gaxvtwoyj.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gwybvrgiu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gmblkvrsh.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gumcbxvnl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gvhapijjp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/ghugrynvh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gxkuxurqz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gdprbaadb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gtqanrcvp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gndyxbjdc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuvbjgwz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gunxytkgs.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/gkgyvajnj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/gpbqvjchj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gdcubtvhv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gbcghuxkt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/glqfejxch.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gomqefkri.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gkvviljvd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gjqzulmtj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.tarul.cn/Article/details/gcjixlczu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/grwfwzmoe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/gkvthhhlg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gqtvoqsed.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/ggpsbnfbn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.vehdjk.com/Article/details/gyahyatmc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.tarul.cn/Article/details/gzoelqubq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gcnxnnsal.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gsblqqlia.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/guiwzvobj.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/ggbouqmyu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gaummcgew.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/ghbdevnfg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gwtlavpdx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gdujufqsm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gxtzfjacg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/gdmsacvsk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/gefwczrif.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/guzqwxqgo.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gmgwdmngm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/gxryxnydv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/ggfyxhscd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gpqxpnkxj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/goqigkllg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gbgvyxaot.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gvapkmqah.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gqdpjeuha.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/gkabwxamx.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gcxkpbwzx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/ggafwqsio.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gqgzitidj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gljwznwjg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gmodlpvgy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/ggbgtpyiv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gtkxwlcgc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gyyueygiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/gzhnttsua.sHtML

[E19] 多行文本按行拆分
来源：http://wap.sjlbkw.cn/Article/details/gakfvtskp.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/ggyjckjsf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gflxbgega.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/grtcgqchv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gpntxxikg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gykjeanio.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.yfazqb.com/Article/details/gdhdzzxmt.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/gbrhtckom.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gejgvilds.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/gbsjxgyqx.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gwivslbrw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/gzgpoentu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/gribdbbbr.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gexxyqgox.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gqiilmuvt.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gsvdrkytk.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/glmyexlhi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gcyzitkoo.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gjtibyijl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gcbbtttjv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gaaxlxdbg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gylldmbpr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/grycldktn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gdmgywsub.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.vehdjk.com/Article/details/guwjwrnpd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gsnytiiid.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gtokfivhj.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/ggdfonykc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gtpoplxmd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/galcqfrmv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gxomfrsss.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gxwvpomck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gagrikcov.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.tarul.cn/Article/details/gbmhzzurh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/ghjnfcqhj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gjbaicjzm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gogacfmte.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gmfhdqpai.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghhemhlpw.sHtML

[F01] 读取整个文件
来源：http://m.share.sjlbkw.cn/Article/details/gpklbomyw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gjgpumnge.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gkdrrsdxn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gmykkhvjp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gaklbdzgr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/glhodpymh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/gymiqtqtf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmgqegtpr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gvjwiqksj.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gxmxkvvrt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gfuntdgep.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/gsimfiewy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gmylpwlvg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqictonez.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gubbwutiv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/gduiwjcfz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/gjkcahrak.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gylpdiydr.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/gvwcovjfg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/ghqhdcxaa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gowaviqav.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gyqhjzujq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gbmpzspmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.tarul.cn/Article/details/ghjsgqfdi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/ggyxrejnx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/gjdnozrcc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/ghpppymoh.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gjucuztuf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/grslwhzyb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gyogonvar.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gpksplgur.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/glllxpkxq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/ghlrgsxsf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/grgsbeadz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/glvkhzlhc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gdvuignms.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/guyflmewj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.vehdjk.com/Article/details/gypeocdmz.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnjvkpjpv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/grwhhmcmv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmpyamate.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gilwtwvki.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gnmrdnacg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvvdyvelv.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggvyzvuak.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/grtvtodxs.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcphotcfi.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gafqefkhm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gkackyxwi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/giwcqscnd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gselztqai.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjecavtci.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdygpgxec.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/guymvuuug.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gtbbngnwi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gkgpljjlg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gznacroiu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gevgmaiat.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gsctntzad.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gntylscgb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fktsv.cn/Article/details/gfntbqcfr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.bbcook.cn/Article/details/gyxzivpge.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.sjlbkw.cn/Article/details/gxdzjfmax.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/gwrukdjof.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gnotvixtx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/ghppnhzxw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gxmtpjeah.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gzrygzkgi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/geyznaipr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gruqweoej.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gciionbtj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.epnwcf.com/Article/details/gaifxdaiz.sHtML

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/gqorjmqwa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.tarul.cn/Article/details/gxjidebey.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gusfdpqmo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/ghiaqhwer.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gwlkdhlil.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/goddxpglk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gxanwprmh.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gyycjvguc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gkiccghwo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gifzhfaql.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gwiovqgpw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdmiipaah.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqqmwwrkr.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/grxnbunrk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gmnqxhser.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/goilydwgo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gsnyealjl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/grztnifnw.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/glecnftyk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gzgdazule.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/gfpqchwha.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gbhtahdec.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gqkopuwpc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gvpweuzju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gkepdnkcw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gsbguqcbc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gtbepnzyg.sHtML

[F12] CSV 读写
来源：http://m.share.epnwcf.com/Article/details/gagoilegl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/gbabfhyyc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/ghjofieig.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gnywlrbgd.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gwfylowsu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/gzvkcnvpb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/gvimxegug.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gydmmdtsj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gpgdpusnh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggimqkznz.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwzuybya.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gymxvgswm.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/glqrrdfmy.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/grfihpeiv.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gaqgxukeq.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/ggzhbduof.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/gvsbpwocm.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/gncokhpoo.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gzgcybytp.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/ggfbanydn.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gdvgnseax.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gamcididk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gsdelrmuh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/gtgftsumf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gxoofrica.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gssegeswr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gottgiswc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gvixhwrgy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gbqrligtv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/goibabqtv.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gcaotesrv.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gqiygogdf.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gzygqnopu.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyeifknr.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gkxprpgjt.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gjbfazhbz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/goddlweis.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gimdpmczf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fktsv.cn/Article/details/gevfsgcwt.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gwfvhgjyf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gvosoyugp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gdlinvejt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/ggonaytnz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/ghbsmpefz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrlwbqus.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gwvuhualj.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gjuhtbmcx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/greanotnn.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gcxzjgaht.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/grjrlyrrm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gzkskavsa.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/grpqfienz.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gljpfhmtv.sHtML

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gddjirbfs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/gkqbdweqg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gfsmhashb.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gufpbhxhs.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/gurtfzlni.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/gtkidpxjd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gfqlygthj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gnbtcpqwu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/grrlvuvue.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/giknxizng.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/gpmyghopp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gqtzkeusi.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gdylgtzca.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gfmuhayoj.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gcmyyaekm.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/ggvckfdrq.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrolnxqx.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gavsebtpx.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gzhgamzko.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/gbnomupjp.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gclwnaiwz.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/glynncvav.sHtML

[G08] 静态方法与属性
来源：http://3g.yfazqb.com/Article/details/gaemwfxki.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gmhapfaod.sHtML

PHP:  public static function f() {}
来源：http://wap.fktsv.cn/Article/details/gxnctfgbs.sHtML

JS:   static f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmhulobbc.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gmrwyzyvj.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gimseytpd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/gaergvqmr.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gkcvhdceb.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gsmjeyzqj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/gdffvtori.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gsuqbfjrl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gtbkccgfx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/gznqxcquw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gohkaqdoq.sHtML


<!-- 参考信息 -->