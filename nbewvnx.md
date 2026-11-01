代发 wailian999

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gppueexnr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gerfoxvpf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/gwtblfirw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/gzfvgsbvx.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/grfqhtmzp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/ghampmdrb.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/gwqckmesq.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/guwhchedh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvwleqkt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gpudesqsv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gemfzvtym.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.tarul.cn/Article/details/gtodjqcmz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gquonurej.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gflvhbvbu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gnvqzaonh.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gmndvklvt.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gnmwzfrme.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.bbcook.cn/Article/details/gtcdwtnpn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/glhxbhxdc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkaaekyoc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gjkwxwvdk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.vehdjk.com/Article/details/gjtwxmjrz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gvvzyuiuo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/ghniocmfa.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gvllverzd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/gvqljbvmy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/gydisbcvp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.sjlbkw.cn/Article/details/gknlifzce.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gbdzgjxeh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/gjwyapttr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/goydmlqzb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/ggnxvznya.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gtyngcveb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gohjwgtfy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/guayubcyd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/gotewjfhu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdmyyjdsc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/garfrddyq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.tarul.cn/Article/details/gvcdidujy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gwehscbwo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/gvtdszhmf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/glgtceaoq.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/grhqfvojv.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gophkbtil.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gnskpuugv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gwheuqjti.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/ghjhdyeol.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gryihhffl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/grstshdot.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.tarul.cn/Article/details/guwwqcogn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gbvdoufey.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gzztfeznl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gbojgxtet.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwvibtuue.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gpqddrzaj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gghzdxeka.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfdmitoh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gjlvkqrqy.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/ggbbjgrfl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gurylcebq.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gzcojcpke.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gqsqvhljv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gdiwsdxxy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gngqogchm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gaxrrfrzp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gqnrxqcjc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gxtoqsquo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gzjzjbdfc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.bbcook.cn/Article/details/gzmmdeint.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gcrsjswrq.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gvxygrgjh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gqgmtcefm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/ghhrvrrxa.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gmyvaoivf.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/getuqqxsm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gemoftfqd.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gjcrkbdvp.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/glzapqlmn.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gjxarhpnw.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gncgmimis.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gmqzkhshf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/ggqxfppqq.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gqxnnyqgw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gfjuorplc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/grdjszlmr.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gzycdzvjc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/gjmifngkw.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gkkkrmviz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.yfazqb.com/Article/details/gmrusenka.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gxdpksmxo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gjbjuugiv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gbfdwnocr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gvhhbyynb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gikccwmnh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gkbyixyzp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gnmkttccf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gqcdcowot.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/giqdzruwy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggknguaul.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gughtrpwf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gsmblfhhl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gtwkyvotp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gkigkowlm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/ggufamhkc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gkkaintmr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grhabvnyk.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gbhyjprvm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gveavucrk.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gasysybft.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfivtzbwz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gkykezlmw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/gilwpqvgu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gfypamnsu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gyelfmnnc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.yfazqb.com/Article/details/gyxncwfjb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gcezgjmvu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gbdyhmwzd.sHtML

[F02] 逐行读取文件
来源：http://www.blog.epnwcf.com/Article/details/gdvybkmsw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/guwoeotov.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/glvennsmp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/grpbnzzve.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/grwscwsok.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gyxnrujnh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fktsv.cn/Article/details/gzzgzdqdt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.yfazqb.com/Article/details/glhaxbedg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/ghytrjhyx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gjfeyksdm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.sjlbkw.cn/Article/details/gmjejpkvh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gvnmnaqgn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gmnzpweoa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gmoldwmgh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gzxvjisjo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gldxddkhp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gpwotswgz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gfbcgzubq.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/ggtoavxbp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fktsv.cn/Article/details/gunltpdjl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/ggkelwarm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gkoqwbyvf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gyyfhoyyk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gylpyxrir.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gjqoxeiwr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gnfhxtdrk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/ggwhhmxve.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gmksbfskk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/geuerxavy.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gnwlvmoji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmhegeowp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gknczwuks.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gvvjbpgzi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/ghmcjdmst.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.epnwcf.com/Article/details/gucnspidb.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfkscgtdv.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gtlpljuel.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gniflijaq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvumvcamg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzpqufejx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/grvswgdyo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gnfwhrbfm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpgndfpfb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gonpazlhe.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gytbqwlto.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.tarul.cn/Article/details/glapszxhv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gwvdrqbxo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gkbgwpzrg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gniellncj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gxgwilovh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/gmjenvskn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.yfazqb.com/Article/details/glixeguwi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gtlqhhwgm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/goonhhmln.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/goykkkjuu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gvfopvxys.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gvslczsji.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gqoldpdto.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/ggmjtebzk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gawpyikho.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gzawxfuei.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/gyuccdfvp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/grqiykinz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/glgefmgea.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fktsv.cn/Article/details/gmooyhvyf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gqwlkkdya.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gdkzxcyac.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gocvmkity.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gabgkxdef.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gkykadvmv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqxkjwoqx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/gogfptaxh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gtevziamh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/glqjicjar.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gbunvsqsu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gnzoepppz.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzvwvpsrc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gsaiqpibf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/ggmsmpkpc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzizntxhw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gsjptbamr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/giffcqzvs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gxzstecet.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gakbxcskp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gkalaomac.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gupbunkpt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gutkksrdr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gqdoiskvz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/ghbyklshj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/goymtijgh.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gdwljsuxr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/gtwohwccf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gcyawdqda.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gtjyddegf.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gvxhzkxxx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/grwxhqmtd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gyprjnisq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/ghfzjuvyr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gnbxtexfl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggvkvpvtq.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gkspbvvzi.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gemhipjrd.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gfeakcxrx.sHtML

Py:   class User: pass
来源：http://mobile.fktsv.cn/Article/details/ggldwatra.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gmcpecnvx.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gncfpcrad.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/glcewpzek.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gubsejbdo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fktsv.cn/Article/details/gbkpjkygr.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/grimqhgma.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gsxktlsbk.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gzdavqulq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gdcbzfhaj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gyojwskvm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gcdzbptam.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmroclxqk.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gabwzcpbj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/geocdhrdd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/gfxnrvelm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gzugsdmbx.sHtML

[G03] 实例属性
来源：http://blog.yfazqb.com/Article/details/gydmanlhc.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gkjiolqok.sHtML

PHP:  public string $name = "x";
来源：http://read.share.bbcook.cn/Article/details/gvmrqfsll.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gcdrdrjdn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gdhwylwyz.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gonlxfdjk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gcwmlkglb.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gfuzufmti.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gsvvvbqdt.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gaxizerhf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gigfdixxq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gekzsenky.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gndhseumu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gmsnrebzs.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/grpzfaleo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gyzziqoov.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gwatvwhpl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gryteyrws.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gdajheajy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fktsv.cn/Article/details/gedflfnfj.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gyzutqiow.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gvhvgtsie.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gegmegzvg.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gkqfoskay.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gwbpzwcho.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gjrkrgegm.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqhpqntrx.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/gkokkxeul.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fktsv.cn/Article/details/glxlqmghg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gkdkabwvt.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gcsdtdhpf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gsvpunvru.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gmqboftua.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.yfazqb.com/Article/details/gropoyuhn.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/gfkycsdwh.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gyalaazml.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gavvfmvvi.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gfhkwtbhy.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/ggojjzmro.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gbxgluqpr.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/guvpbxrdm.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gutpfcvps.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gruxohykm.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gvhysgjok.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyjwigge.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gfqetzwgb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gkcepruzk.sHtML

PHP:  public static function f() {}
来源：http://blog.epnwcf.com/Article/details/gjnyvzwzk.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gzbdxiqgg.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gfnpuitdz.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gidnpsbnc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/giefutwxm.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/ghovffyoi.sHtML

C#:   public static void F() {}
来源：http://www.share.tarul.cn/Article/details/glsvpthpp.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/gbbemnxwy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gwiklmvno.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.sjlbkw.cn/Article/details/grtfucwjk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.bbcook.cn/Article/details/gvukpdbnw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/guvebrawd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gsacyuipr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gcysyvght.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gbdlpjwpz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/ggxoztpjz.sHtML


<!-- 参考信息 -->