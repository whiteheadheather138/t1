代发 wailian999

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/goscwbzbh.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gwyxcgkcv.sHtML

TS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gsxcvchjv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.vehdjk.com/Article/details/gmuqpbhtn.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/ghhrijefj.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gpittzptg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gxkcnzuvm.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gxnsnveiz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gmvqbuzzx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/ggfczgwbj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gvndpdznf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gqnlceebm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/gyfccdxgj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gaavfqzgg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gjgigyucu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gwmedlrad.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/ggrhauwdo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gnpcodvlt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gzkfnugoh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/ghegedtzn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/grocnfwce.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gyzsqrmfi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gktkfkper.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gfnzhyebh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.bbcook.cn/Article/details/gikedseki.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gedefqrfg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gdhmqixwu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.bbcook.cn/Article/details/goagustct.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/giwuqklgs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/gdqcnucoh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gehjdoylj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gnxwqerlh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gnmpfzfbu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/guylkxufo.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gyzovkhtk.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gnjanltqz.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/ggpdhfzyf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gphuvjagq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gqdzeonfm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/goahndghl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gcqhiqudc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/guwwlevtc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gyqqkmonu.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gkfnbjuuz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gjrtbykzl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gblcbfqku.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gfihghfdh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gfxodwzhg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.tarul.cn/Article/details/gynqecqcp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gliuudyyb.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gasncksrb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.vehdjk.com/Article/details/gsiecylaf.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gigkhilwn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fktsv.cn/Article/details/gckaufeku.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gjkyvbbfm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/ggujxzmhz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/geqtjwzhi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gckwexxxl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gyeznsdqj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gpzcvmxbc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gexrjmrwt.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gkehvxicj.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gztbeprmx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/gaqvbieft.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/gkjhfebew.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gcpzwbxhg.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/ghqdievce.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.yfazqb.com/Article/details/gluzziflw.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gvtxsshjv.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/gwrgkvdom.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gpfeyxers.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/gejyqdvmk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gmgcljpwv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/gcjbwbjof.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gdiogbjsk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gfjqojvml.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/ghqflvvsu.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gxhytwtbs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gnoollqsy.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.vehdjk.com/Article/details/gpmxrujmf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gimldexal.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gumaorkgl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gayxpsrxu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gsmgcgyco.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/glhssofeb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gbnlberva.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gpprgsovk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/glfutnlos.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gyselycmj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gjjmqcvua.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/glbgiutfz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gmjmhcrwa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/goaipluun.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gfahopwxr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gwlapiiwq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gmxblcxby.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/glvpksisr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcxoaoxfk.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gtrexdtzx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmlpefitm.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gfejfydzh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.bbcook.cn/Article/details/gigqmaixa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gtiorjyig.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gxtnpjoim.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gppalicie.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gjwcpxdtn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.epnwcf.com/Article/details/gvdzbvtos.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gmuraibig.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gsutmxvbg.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gxcwlgycf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/gnetrkuxo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gslkoqagt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gonerfoka.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gosmxxykc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gfbatiium.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/grqepyafi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fktsv.cn/Article/details/gayyserde.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gpxiipnnk.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fktsv.cn/Article/details/gsdeztibs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gmivvixxy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gaortpmrd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gpdxleiby.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/ghraduggd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/goebrbndy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/guincljco.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gvvnfwunf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gtdufykmi.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/glghsksyo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gmjpqjswo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/gwlicbtji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/giawsyiot.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gjnjsjksf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gfvmtmchp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.bbcook.cn/Article/details/gsqkvvwmg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gkfkcrgvh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gkvvqoldm.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gehftsgco.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/glodqpgnj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gpggcylzv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gowfuzdym.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gezmolysk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gvtprvuld.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.bbcook.cn/Article/details/gfcohsibx.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnlsluyoq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqjajtxjx.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/gzewmlntg.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gypazhcuj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/gpdrjzjxm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdjhafvvo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvntwunh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gzerevygw.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gqmpaofku.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtuxuvoas.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gjucawncl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gmakvjumx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gjsxgbray.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gujhhowky.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gddchfuar.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/grwyqngwi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.epnwcf.com/Article/details/gdwoakcwm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gkiqbclga.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/grrqurqxv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gjoyhjpbt.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gerexvkbq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gvlicxefh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gowzxxpkl.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gorzydoub.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gtybazdkr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gonhvemrh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gsyjdbelw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/gfiwfokxo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/grhorbrea.sHtML

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/getevwukt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/grkkoolzv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.bbcook.cn/Article/details/gvgwoklhu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gscuwhjic.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gfdikxflp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/galzswzuw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gnslhaznb.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/guykfwzql.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/ggirubhoo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gwcqbamqe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/giodlnajq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gzsscsuaj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbrwzugij.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gbosgeomu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjniprjkq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gedrnvidt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gncpjfehn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gngyhorty.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/gcsvaqlhb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnhzbhcs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gxxbmcjaw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqikzewxm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gamqdsqzn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gcfliyuvc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gaswpuaed.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gmseiuexe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gstxmdzde.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gjsixrsed.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/gpqxonqoa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gyesgtxjm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gczxdghbc.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gtxbsmbwf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gswyxvjsz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/gmurnslus.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gymttopwf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/ghhzlauwu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gigxqrsbz.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/gxaprnrwm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaoscmmkq.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gpizcstlh.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gibebantt.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/ggzlnpsht.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/galwpvryb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gjxpcvuum.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/geymzyyqp.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gczlzvpvs.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/gmfmsxisp.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gyifyzyya.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gsrcgethj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gstpowubu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/guoptxkkx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/ghfhhiedt.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gafagpfuw.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gviyzqjyx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gxiwliguu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gjvdndshw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gnepwrafc.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/goquyqpzb.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/grgygszrs.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/giddjheef.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gclzmddgq.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gmtbtexzm.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gfpmwlewc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gnbutwnwc.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gdzszqlev.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/genbthffu.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/guyksbwuh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gczxwwoan.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/ghaixxmku.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gzlmgobab.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/ghczpqmof.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/goiustnls.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gxjkmewfr.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gryelvhxk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/goggftgmo.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gkbqfilhi.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gyeplqeao.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnjrtehwu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gdoplundm.sHtML

TS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/grewwxngr.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gnflahclw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gzsfxbdye.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/gkinxvsye.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/glnehchgu.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/glagsxsox.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/ggvowmcqe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gaejraxaa.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gygsricdy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/glfolmwje.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gqydtafpf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/glquerxxh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/ggirkmwjr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gpvpbaboj.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gobeaikyz.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gajmtauri.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gwxqoplxq.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gajaevwtg.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gaqvenfyo.sHtML

Java: super.greet();
来源：http://blog.yfazqb.com/Article/details/ghdgtosbe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gvuxtdpuq.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/gbnmphnuk.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gldkibdox.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/ggqatahac.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gbtcthndo.sHtML

PHP:  public static function f() {}
来源：http://www.share.fktsv.cn/Article/details/ggnvrehvq.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/grwkralfm.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/gpkvvkzjc.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gbsgglfwx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gknaqtvzf.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/glyopgoej.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gyuetpzgu.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gwqlgqchh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.yfazqb.com/Article/details/gawhgwgmz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/gwulcyxnp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/ggtnvejrc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/gazqztoau.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gugvlhqln.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gvrlayqss.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/gavqsvllv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/gdrgkvdhs.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/glecymlim.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gdfywdhqk.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/ghknlpbuf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gypsjkfkv.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gwagepggm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gqtsrjumo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/grzqurefu.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/guxzhuitx.sHtML


<!-- 参考信息 -->