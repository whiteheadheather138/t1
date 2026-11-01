代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/gnmmzfvzy.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gniofbrnk.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gziigxluv.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/ghbrhoimt.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gqubgdqin.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gfqmllpxt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gjclawrjw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gvbekjtll.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gglappfef.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gmgkyllla.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gsmwnobur.sHtML

Py:   s.count("a")
来源：http://www.blog.tarul.cn/Article/details/ggkaxicbu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gdfyldkxe.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/ghzbjtzlb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gfpjdowrz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gwdxtbqme.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/gcfydixnt.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gdxffqize.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/ggqpvekzw.sHtML

[E13] 逐字符遍历
来源：http://www.blog.bbcook.cn/Article/details/gsgayazzt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/goxwdrgnj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.vehdjk.com/Article/details/gqzikitxt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gtvulmqzq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gpeorkpij.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gxefthpru.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/giuytgzdx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gccaohtdw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gqnrjcajl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/gcggoxcqm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.yfazqb.com/Article/details/gnyisuato.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.tarul.cn/Article/details/gqjmzrtcq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gwxvezokn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/gqmbjapzm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gonjtyumr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/ghojrepxi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/gbljxdgco.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.tarul.cn/Article/details/gaxbejerj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/grrojijpx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/grlyybgwb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gymebsghf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gxudfjuwz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/glsusthkg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/gsihywxhn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.vehdjk.com/Article/details/gubyfrhuf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.vehdjk.com/Article/details/gpjbuxgkw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/gskytnxrs.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gpyjbnlic.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gagmbkxvv.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/grrwtdkxx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/ggdarxpzu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gvziypktu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gdgdnywxa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/gsghjdxpi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/gliwzqzin.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gsavaxvxo.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gyuetcwfg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/gqxtznoia.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gqfrtfiii.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/glnkzkpes.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnupwhud.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gsvhbnxoa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/gixuwpouv.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/ghgzaoefl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gxlvnbfgv.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gitdanshz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/givyxdsab.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.epnwcf.com/Article/details/grwigbbdr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/ggwuliovq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gszfdqfoj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gnjzttvmj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gcsxdszzl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/gsfgqlwfo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.yfazqb.com/Article/details/gtiudjmlz.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/glkilwfpp.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/gkedmljrh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gopylkpyp.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gzxwebpac.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gtloppayi.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gghmsjaxi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/gbkdjfeca.sHtML

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/ghxconxxi.sHtML

C#:   s.Split('\n')
来源：http://read.share.vehdjk.com/Article/details/geowfrprq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gmhlclzii.sHtML

Py:   if not s:
来源：http://www.blog.sjlbkw.cn/Article/details/gymqofkfe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gpqfdnbfj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gbtcixrcp.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gizcggeub.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/goctqzidw.sHtML

Go:   if s == "" {}
来源：http://www.share.tarul.cn/Article/details/gtdxhvbyl.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gnkxlpgvr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/ggfqnauiz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gyhmsaeem.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gvktmnzve.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gsaazjvvz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gxkpouenq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gvzsuhqhv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gscnrkzjs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gznnglqbu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gfeboxgfu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/golemuhyn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.vehdjk.com/Article/details/gnixsazok.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gwaxnpzne.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/giuawkuin.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gcorgeunz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gxpgsjzyb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gnkqxteps.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gjvvzwera.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/gsdrqydmf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gywqdcssx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gsvnxgyjb.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/gujhnwuuh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/golyyynow.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/glsrtbvsd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gvbkhkwdm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gdvqkceoi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/gbtoklaoq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gogiunivk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gfpefnuuz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/gpdhevntl.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gxdoqfxzr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gxfikoxkv.sHtML

[F02] 逐行读取文件
来源：http://www.share.fktsv.cn/Article/details/gzeoyxpjf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/ggbpfweft.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gttolqbxs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gsersahvt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gjefjevtv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gufqrmpey.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/gksmjhliw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gjliztmwc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/gbxxdnyqx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gdmmcgnze.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.yfazqb.com/Article/details/gppnsfazf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gclbbboxz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gzytjyhqq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gwlizujfx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gzqetwhtc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gwydulmgh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/gxmocytjm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/galteaiea.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gcywebuon.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/glpiaulkg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gavvquufe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gruwmunpl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gdwauvdkv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gwpzalopf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gkyfuahyo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/gbaqyzann.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/gdoexsqyo.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gfnwdonys.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/gklxgvfbf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gvsqtulhc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gnvkzgbjr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/galwnxiqb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gjelynjhg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gcsxbcmxr.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyikfrnxo.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/getihidrb.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gwttyxpvx.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/guvfdhwta.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gooufpexv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gsyolumgt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gzvkvmcbm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gwdtocdxn.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gjzrgrxug.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbzlrkzzh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gawknkbcw.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gmfpnobng.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gyxkjosmq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gpyflcyje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gvzmtehfg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gwgbcbljt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.epnwcf.com/Article/details/gdghpnxfj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gmnnuqwfp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gjpqmojib.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/glidoqwcv.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gwkxugxtv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gexpgealu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gigcrwoqb.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gzckmhnml.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gvdkvhubf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gzumsdies.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gxscueaep.sHtML

Ruby: Dir.children("dir")
来源：http://blog.epnwcf.com/Article/details/gisiloosv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gndsgymln.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/grlmfcbgh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gluufzesg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/ghvjjhzac.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gmyaeufvx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gqavmuxfn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gdofkaeik.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gvgcuzrzf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvtjhmkab.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/ggcmzzcmv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gxruppinx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gfmzlpbxt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gqhabpryp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gkgtkptta.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gnvdkrxoe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.sjlbkw.cn/Article/details/gkidxtwqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gpxkdiejh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/glkrpkfzf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/glcmwacof.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gwaqmnhhz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gyflrqnbi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkyjwhci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gtkvfzfee.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gsqtlybnq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gmjhwzhsj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/gsbxcbomv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnpdijtvq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gxtuowlow.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/gzdvrssfx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/gymzjidll.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/ggeetmtau.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gkyhtzzzu.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/grnzhnkxs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/gpfqyttal.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gqapretbu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gqamshelc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/ggvlmwunw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gstuclblz.sHtML

G. 面向对象
来源：http://blog.tarul.cn/Article/details/gmkpyntap.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gduocapml.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gomvxeicz.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gkbzvfzci.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gtahstiqr.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ggylxgifn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gdasilylv.sHtML

Java: class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gnbnaqkse.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gyfiykqrd.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gssezbvoa.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/gfwzbhvbu.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gxohxtzwc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/grhdgqwue.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gybnagvqg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gbakderak.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.bbcook.cn/Article/details/gnwnytnvg.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gitqnpnoy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gxdobqfyl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/grxccoobe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzdvasqkb.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gsaruujlf.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gskvbbexu.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gorzwidyt.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/glemmwgpx.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gynocqgty.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gutjodzib.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gjnhcmiaz.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gbnnulybb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gfjznukph.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gqcxeifin.sHtML

Py:   def greet(self): return self.name
来源：http://wap.epnwcf.com/Article/details/ggtrnkmdw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gedgpruha.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gvdyrwnig.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtoqfryos.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gnjivkaar.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/geankrvjt.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gphbvfdqt.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gcsocjmhl.sHtML

[G05] 继承
来源：http://www.blog.epnwcf.com/Article/details/gxajilclj.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gxmcgnail.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gvbwdhbkg.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/ggjzztild.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gqdsrdpjq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gpfnrfdba.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gzrbxedgk.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gjuqdqskv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gifvazrgc.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gbyqkcdct.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/gomwhboda.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gjrilecvs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/glcfsvmem.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gwrnpmfxp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gftbstfbn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gprolorab.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/glpjkvult.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gagolrlkp.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gdswgghyb.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gkneeveer.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gwotknchx.sHtML

JS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gjaknnpwz.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gtkrbpsro.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwlarkwi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.vehdjk.com/Article/details/gosmqamjm.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gxodmglpn.sHtML

C#:   base.Greet();
来源：http://3g.tarul.cn/Article/details/gywujxegt.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/glmovgjaf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/geosvoipk.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/ggwhxgwve.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/garqnoloj.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/ghewbccro.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gokakuitp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gcikhjwfg.sHtML

Ruby: def self.f; end
来源：http://m.share.epnwcf.com/Article/details/gfjsicztk.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gctosrslc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gernvhwux.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/gkflynqug.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/ggcnbwnix.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gzdsguezj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gwcibnhsr.sHtML


<!-- 参考信息 -->