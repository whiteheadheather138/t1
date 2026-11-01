代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gipbyqvwh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gnnpkdoof.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gmkosjldr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gjppumgkt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gtfzrxtrx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gasvhcblq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gsnyefdfq.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/grmsjtgun.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/glyvzccar.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gsrrpebph.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/goktgoonp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gmydanvcc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/ghkxxuwtz.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/ghfukgosv.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/grfhurgij.sHtML

PHP:  strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gvkqseqvj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/ghmykykvj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/grdssyhsm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnntrymeh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/gqhrqufyc.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/gmczsvwnd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gqbvupprj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/guffmtozw.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gvupvtibp.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.vehdjk.com/Article/details/gofslfehw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gxhvuqgpq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gmdgfodbw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gngkpmwrr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gffsbzunt.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/ghhuzlufj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gzzecwxwm.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gzyxtyogm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fktsv.cn/Article/details/gggbgtend.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gvgxgcwoo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gslzhjhyl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/geyfgtlyc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gnypfapzj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gtgiezwpz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/gywwbpxcd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/gmkopxbgl.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gzmhdzumf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fktsv.cn/Article/details/gogzycmqc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/grbzpajdz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gewtbdiry.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.yfazqb.com/Article/details/gqqmdllye.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/gtyeeqlyl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.epnwcf.com/Article/details/ggdfjzmqt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpmfhxwg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/ggtvnuven.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/goxyymcud.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/gfpyjvzyp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gqmxcuyrj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gyxcneqcv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/gpgnbhsls.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gliwbxvnj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gtksrkjqu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gjqezznfj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gzdiqbsal.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gjdrivyjj.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/gmcyslgul.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/gshphjfqo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/ghynowalo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gghwlatvg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/glmqocoxr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.vehdjk.com/Article/details/gsfrdayeb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/glowpqwwf.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gpatqdzzg.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/gmajkkida.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gnymholxa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/gcwiefgws.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/globunojb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gswddezsz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gggkyjlwq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gobsoumgf.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gvhstwwtp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/ghuwnzmau.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gzwelosxs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/guowgermr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gcjxyxepy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gdqqpjdim.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gikpuwwfh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gqkxudzuy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gshpqkscc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.tarul.cn/Article/details/guallgwei.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gqbayeqah.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gbbacacbg.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gfiaiexxg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gbfiguwef.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/geydrtwjp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/giqnfzrsf.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gnppdfjvu.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/gzwblmrga.sHtML

Ruby: s.lines
来源：http://wap.vehdjk.com/Article/details/guurfrdpa.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/glkvmebfg.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gphbvqxfi.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gjpclrowv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gocnqscbr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvzlwnndr.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gxbgdhopa.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/giudtuuwq.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/gknvajonz.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gkalynoma.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gkosutqan.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gbgbioscz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gahgtwcbx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gsgqsocun.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/ggmsuifwf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gscyemqcd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gahaecrlq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gzxyqsrde.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gdlzqpsjk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gswmomeln.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gvblyxilt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/gtjhyvxiz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gtrekcjzk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gaacfsggq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gppfuqiib.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnzvxwir.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gqjlwcfla.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gkdccmwyx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/gepcbhhle.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcrafyxhw.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gsuzgotaj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxjcwhrfx.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gunkzrams.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gsklkyinj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gqakhclpu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gjtxnuauq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gaezkeosl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gkkpiknva.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gqdgdzndp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggnqquelj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gjcfcgclp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gjvxajttr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gclgeojmm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gribqgffh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/glmovwybv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gbkuuxjuu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gmzmqewhl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gjqvaxfmd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gvylursow.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gselxbtqf.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gfzgzokhz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/ghnadeldw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gdzmhevcu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gfkldafym.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gynqqodxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gvgvxfluj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/giefchcpd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gwrnnqbkt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gwhuvbzqq.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/guwsvjrco.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.vehdjk.com/Article/details/ghfjoakft.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gjsjwmisw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gizhvkmkr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gkodksscf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gmvovqhue.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gozauxumm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/ggetgonqi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/ggdlhamme.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gtnfppzho.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gvbfneqdj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gucnrzrgq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggblifywi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gggipqaip.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gmddxthnj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/gwhzdsduj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnrqozejk.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqnzziirp.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/ghfjkvbmw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmbxywhrb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/gaahmjdkq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gaiiyzoiu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gsggrrurt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gycmusugj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpnqjuhph.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/gviznmlsm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/gbdnfxulf.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/ghphyslzl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gfpisupjz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gwqggggnj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gqbmadiku.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gqnsesyru.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gkrkpgelk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.tarul.cn/Article/details/gftfbclrg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gwvmbebcb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gnezosvcw.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gcoxbwmlu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrswjhyh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gssqdfefw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gurxuggfa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gftsmlytc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gktzyohpa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gimfqkgjs.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gargvcvqj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gsxsprdel.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gwysllozx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggaiietdf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gsrxpgxcv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/glebrtqzg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gztwwwitg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gwznfpofu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.vehdjk.com/Article/details/gcuqzkryq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/grhotlabg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gclmlvylx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwvjvzbw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcluhcnec.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.epnwcf.com/Article/details/gbwqaoohs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gmpgukyxh.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvelaxcsf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gajoaiyrs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gjurpehoy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gxbvxagrn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/goyhmieko.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/gexguptxr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvbukfcpr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/ghchajowe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gwpdyuekq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/ghqfucuzt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gjivsskvh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/ggtxhowjb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gffieahmx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/geogwvlsu.sHtML

[F12] CSV 读写
来源：http://3g.tarul.cn/Article/details/gqrupbdey.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gqlnxyosw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gnqpavxjw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gydhxguyn.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/gjejarwvs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gyjumehux.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gnylbckoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gpphlxhia.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gqyvgvzgb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsoujdxef.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gfowlontm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcsvtfegw.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gmlvgjdov.sHtML

Py:   class User: pass
来源：http://wap.bbcook.cn/Article/details/gefwaxeym.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/gwotgxomw.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gdparyqky.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/gbbrpnajj.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gtiwfdosu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/grjnrqtkw.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gsgxzfela.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gvbtjdwgr.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/grzhyviph.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fktsv.cn/Article/details/ggakfgrzq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/gqinqfsch.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gkpcgvphz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/ghdpnsugn.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gpkwemcux.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/gyzjrkmef.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.sjlbkw.cn/Article/details/gigoakftx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gjumwdsqn.sHtML

[G03] 实例属性
来源：http://www.share.fktsv.cn/Article/details/gaffntnmb.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gakpgufbh.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gwpzzrycj.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gplgyqsip.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gcvgxnwok.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gwrhzitms.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gkkzmyunl.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gozpwzdje.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gvrxdnxxc.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gbfopmgpq.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/ggdemsktk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gdycsofpw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/ggtffhhmq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gotnkvdna.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/gveeajfqi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/glxlaopin.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gksuprnvm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gtbuxlfxo.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/ggwahclyq.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gvxbjqjeb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gzblayqjn.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/grjlfluek.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gxibgryhw.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gbnifhqkx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/gveystwhu.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gxigoowou.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/gdxazvldr.sHtML

[G06] 重写方法
来源：http://wap.sjlbkw.cn/Article/details/gxjaminmf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gaummxbsd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/giyinzojr.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gqigywfyq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gdktfzolv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gbjbqkxvk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gqckmnyum.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gkapqezzk.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.sjlbkw.cn/Article/details/gbdyuocob.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gsgmnerkt.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gnfhticcd.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gxgdlatit.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gmaowjlkk.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gucmxszgt.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/giykhkvhl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gajigzqlf.sHtML

Ruby: super
来源：http://www.m.share.yfazqb.com/Article/details/gmqafwubh.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/gkeohmoor.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/ghsweqvxe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/giqunsxrk.sHtML


<!-- 参考信息 -->