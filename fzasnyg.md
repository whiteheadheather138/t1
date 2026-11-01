代发 wailian999

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gohklyghb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gjcfrbojd.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gaatowupd.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gqoschynm.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gxeavabjp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/ggkuptvmp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gjhznuggt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/goimrzswk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gqsraguqd.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gvylazdiw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.bbcook.cn/Article/details/giyepgswp.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/gchgaafug.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.tarul.cn/Article/details/gekutivmt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/gudqmpjrb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/grvoxnrcx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gfidtgcrk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gjflmaydd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gzwgkzvxc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/grszubils.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gojsdqqdq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.yfazqb.com/Article/details/gbxipgutk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/gxnczpdbb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gwjprnimx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.bbcook.cn/Article/details/gneklcbok.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/gdznkbreh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/gtezomazs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gogebulur.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/grazvtqav.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gavapbkmk.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gundzvsby.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/gpmanbwia.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gfmknxwyb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gedidpgul.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/gvpejajxu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/gnfnssblo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/gmlueradd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.yfazqb.com/Article/details/giorcwzug.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gvfklpwai.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gmvdeftfn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gfasjhdzi.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gerpnheum.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gttrfdwaq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gzbxgkklp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.epnwcf.com/Article/details/glnuccksf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.epnwcf.com/Article/details/ggmslbviy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.yfazqb.com/Article/details/grdxdoyhb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gdviihwbp.sHtML

[E17] 首字母大写
来源：http://baike.epnwcf.com/Article/details/ggxswqrjo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gbhdmfjtt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gehpdddlc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzdvsbhpy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/ggzxonzyw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gjecowpgp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gbxuqnufw.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gkwitujuc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/gsipsvvqp.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gofnqmbjf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/gxymknaop.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gcsfcdgmi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gqtqzvuru.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gsxjpaodp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gqxsgywli.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gigbkxbxi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gabitjxgp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gpceobkas.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gasbtrgym.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gzjyidqow.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gauipbpvm.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gqsnhjvsv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gtsltxbro.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gaqiprvjq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gzzuiqgeh.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gitepxdqk.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gwvltbsis.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/gxhafcijl.sHtML

Py:   if not s:
来源：http://wap.yfazqb.com/Article/details/gknelsvjg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gwqeeectj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/gnxcxreqd.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gcxqbfjeu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gbpougzcy.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gbqtprahs.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gloggyxxn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gxujtfzfa.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/gwkxwozos.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/gjuuhchih.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/goeeaivof.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gasgvdfdp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gwapzhqox.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gzhdwpisp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gqidjyizz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gfrzsppog.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gbiqikfei.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gpcuksegi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.bbcook.cn/Article/details/gyalpciit.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gtjfkunrs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gphhdxodq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gnaugkjky.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gllapqxai.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/gioaibwjs.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gibrztwdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gnnkrresd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/geynrdmhq.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gjetujuug.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggrezauvc.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gyjpebxfa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/gslfscime.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gaznurkql.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.yfazqb.com/Article/details/gyrmnylks.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/ginijcsjf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gcjeffqep.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gaqusibrz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gtwhpzjvo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/grdvtdute.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gydaegzll.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/guefwtuwt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/gkgwjsirk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gqodywyrs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyxmywxzf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gsauvggma.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/gdqrmwgnq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/gmpztmzjq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gjynlzkxh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/gblzomrnk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/girrszxgg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gdinyjntm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/ghxbtogsy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gxacgpced.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gitgwquqj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/ggfezzfda.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gwjfxfjzr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/ghzrhcmrz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gupvusnut.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gyovdvccm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/ganxhxqpk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gpoxabxeo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/glwyrsnnj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gecpkkpms.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/gniozyhhi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gkpqejiwk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/gmusskoee.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/grbtbhcsw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/gpdsxeqlb.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gmbqvybhw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gyjbhqtwu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gxwmxeyoo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gyscmreac.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/gzhiicdqb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtppwnyfb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gaderrbha.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gogajpngh.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/grsnhdphr.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gyvxzdnib.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gdercmhdo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdngpdpat.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/grreeduwh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtidnicce.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gtxgipssb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.epnwcf.com/Article/details/glflpuamk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gxoqrceod.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gipnckftj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gkvxcbgie.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gvlfcezhk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gtdiuwbxx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/gwwjflxee.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gbwmwmlqi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gwfongnsm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/ggxhyvxsw.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gmjncymvh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gzmrrmpbl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gyuktfjjl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gpbymlzys.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gdziexpwz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gbstvwrlb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gzxhuxgva.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/gqblxvbeo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gjadrjtiw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gvbfxvuuw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gcwaasvgz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/gebsmbvex.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gkaxmwzru.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gmwfhrpqc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gudpwleae.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gnwboxruj.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfjuxffdz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fktsv.cn/Article/details/gykzmiorm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/gcpprurzw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gdrqxitzu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/grvxpegtk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gntokoxgx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gnxcdwsjb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gcwnkagcw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gebhtwwvx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/givjfdvan.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gyylmfngw.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/gworxrzpi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gbvgfpnyi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/grfoghtnq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/guufiduic.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gadcxotin.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gpnwkklve.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/gnthrcwqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gcfdudonn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gjjjwfzmy.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/gfvkoivrh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gmjkeujng.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gignzzksr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gigjbbokm.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gfjxrzjsq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gfthucdsc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/gdohuiyld.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/giwgghsic.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gceosfsav.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gorvkhoib.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gunrztwan.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbtfdyfct.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gonelffeh.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/gsgowlvbx.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/ggdccxkrk.sHtML

JS:   class User {}
来源：http://baike.bbcook.cn/Article/details/gpklpyywv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/ghdrihbca.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gwcfrppke.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/gelrphdlk.sHtML

Ruby: class User; end
来源：http://www.blog.epnwcf.com/Article/details/gdnhnsymd.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/ghartxpdx.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gnncjhinn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gnnnjamcf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/geouytgsz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gxcttwwik.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fktsv.cn/Article/details/ggyfrzfxd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gyyagobwe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gejfjnrmh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/ggxxwvzkm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/grrxmtewb.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gfcjyroux.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gxrvasdhz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gjfklwdjw.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/gyaylncqh.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gfbopqgcc.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gudizhxpr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/glgrahrnv.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gzjjgeitu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gctpnqqja.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gkqtcpeib.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gjdhzrknw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gbepgecod.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gmayqiqxv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gyeoxzjxr.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gdbjspeil.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gdfxtkaky.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/ggwcsepae.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gziszhtvh.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/gyfuojzuj.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gfcpgsfhh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gyyekmcjh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gjlataitm.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gqtqcpwoc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gvfwebhdn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/gpbjigtmh.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gnoxftgrh.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/grdxztfty.sHtML

[G06] 重写方法
来源：http://www.share.epnwcf.com/Article/details/gmmziglkw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/ghpukrlom.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gfsiblrdx.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gursvyeds.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gaqzostnp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/guclwksae.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.vehdjk.com/Article/details/gspzbixfa.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/gjzkgjcsg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/gyvvparnn.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gymziwkkk.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gtoyjsmmj.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gcnzesmce.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gyhxjjymy.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gigqyyfwi.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gnptgygfv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gtqlqcxst.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gkbqnavgq.sHtML

C#:   base.Greet();
来源：http://baike.vehdjk.com/Article/details/gqrnpqjke.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gurpubwgl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gleikqmss.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gfeuifjkc.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/glffakwxm.sHtML

TS:   static f(): void {}
来源：http://wap.sjlbkw.cn/Article/details/gopahwkax.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/giyqbfcip.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gxefmcwbu.sHtML

Ruby: def self.f; end
来源：http://m.share.epnwcf.com/Article/details/ghivkidea.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/gbbsaibnn.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gqyskltdz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gweitenhp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gdjsvjakc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gsxifhjbi.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/gkjyfczqp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gemthldlo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/glrojgroj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gjfdbltsa.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/ggkfgyvif.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/gmbyzwgrn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gvxqecdio.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gwdqdvuui.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gcmzrxgao.sHtML


<!-- 参考信息 -->