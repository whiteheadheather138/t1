代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gmtdtznzj.sHtML

[E11] 反转字符串
来源：http://wap.tarul.cn/Article/details/gpqfwhyrf.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gtvitglgh.sHtML

PHP:  strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gtczbkxfu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gtylszmij.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/ginrspjti.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gaejpwmdm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gxictoelm.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/gmmfflxyn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gtjwcxozb.sHtML

[E12] 统计某字符出现次数
来源：http://blog.bbcook.cn/Article/details/gmamhdzex.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gchhcqyzw.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gyaowecgi.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gnflhwvhl.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gazrmllbz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/gjkdsxkhn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/genqjzawo.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gjnjfmnan.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/gcrlzpxoq.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gavxbsgbz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/giyzevxkt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/glcvarbyt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/glegmfadr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gunqxbliw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gsztihshj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gphjirteu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gkycklzjp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/guptmmbvw.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/gxrrryqpm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.bbcook.cn/Article/details/glzwpeejp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gmbvmfenr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/ggszpcinx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gontwioho.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/gipnwowhq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gqmjngqap.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.vehdjk.com/Article/details/gnrsfknac.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fktsv.cn/Article/details/gshomdhio.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.sjlbkw.cn/Article/details/gdmjinilj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/glmqsgpec.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gomlyammx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/grbkgogkb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gvdytjpgt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/guecvtmmf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gegtqwmpm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.tarul.cn/Article/details/gsbvpgrtr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/gsssaieol.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gzuvwttkv.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gosydozyh.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gosppxeax.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/giazwinvl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gwfkgzzia.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gufbqvbmj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.vehdjk.com/Article/details/gjyxnglqn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gdkwknqsb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/ghlypmjal.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gwqhobtzp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gjdktqhka.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gvboxczyk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gxugtnoon.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gbrzgpqam.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gngevfeuo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gawwgstjp.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gpailyfec.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gqhfnhzmu.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gnmpankan.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gdnetwovc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gdolvuyqi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gwxkbzzqe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gxazjdywf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gogqidavy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gunqxhnka.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gadfoivxa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/ghyhfxykj.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/glhtldmgj.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gtlsaoivu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/ghatecrip.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gkasiuvpz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gkvoyxfds.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/ggamwgmtm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gcqanmilk.sHtML

Ruby: s.lines
来源：http://3g.yfazqb.com/Article/details/gqxfklnqw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gpuredawf.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/gwddnfoku.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/gkemzlrii.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gyorxpgtt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gxspsbggw.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gvumualtw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gkzaoizpu.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gdqhgyqon.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/golouzrqu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/gxzonntjs.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/guacllzmk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/gbhktbscq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/glknhfufs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gtuqoooer.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gyqujpyne.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gfststywt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gxqbjorxe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gfodyjase.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gsqaszspw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/gdlgcdumv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gvsgxmxdz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gijusnjmp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gibvfnvdd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gnvhgdjpd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gjegfhkcj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gqbydcrye.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/glbzstlfq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/geigxcnrp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guqmdeyun.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/glonbaufc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grnwfxwtg.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gyuiuujbo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gjvphwdqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/gblllbomp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gessiuikm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gxlbrxkhx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gemewcqkp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gjqozwjvx.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/geoxjndtt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/ggwlimejc.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/gcbnrvhdl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gwsidxwni.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/ggjdqdpsw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/ggrpdmint.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/geuoidgtg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gdlaqiwoa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gshcmtqbn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gpoblsnsu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.sjlbkw.cn/Article/details/gxhtuqqxe.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gyxeiqmff.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gqvxdeflm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/ggifhhsdi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/grpvodcgi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gizypozcf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gzyfxgwiv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.sjlbkw.cn/Article/details/gcbkxlwza.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/gnzctoiiq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gqlcewryk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/giszciutl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/ggtlbmext.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/gfyglvbhg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gluxdrkhq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/giwkmuwfd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gkkdepwji.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gikmrmzfb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/glrpixncy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/gtkaipkys.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fktsv.cn/Article/details/gltpswpeo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/goqrowoeg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gkhdieyfq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gehafzezk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gynyyawsz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gmyxxbxsv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/guwjjorga.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/guqhnhhjv.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gxtewdsax.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/gcrkuibny.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdfvwgxal.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gnaptvtvc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/galgqemrr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpbdifqgh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gqsylxzfs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grnymyxqw.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.epnwcf.com/Article/details/gqrygkwcy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gmuyrigan.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/gdfjwdcxr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gqmlhptmt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gysytycwh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/geefucdtf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gxfskmlml.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/glvlkufvp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gqnzqathv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gqusvxeuc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gbytbubwe.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gidibjtem.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gxcsxnedh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gjabhvern.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gehipcrha.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gzmyxpuyt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gcrbqopws.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/ggxyypjau.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.epnwcf.com/Article/details/gmzorozky.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gaxskualm.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gwngcfwnl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gdxierfjb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gsqivcmuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gmzvqbhxw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/ghxnykflu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gitdeunjl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.sjlbkw.cn/Article/details/gjiacbhzr.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/guxvzrqlq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gtwnkhqpn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/gyfogeupm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gawsumaqt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gyyyketyj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmmckdrep.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcrecxodk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gejftdffj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gnlcedhae.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtahxcsre.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gprkpevvm.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/gqovqdfgi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gyormnmyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/giltjtzjs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/ggvtiemgi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/geiddvscj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/gxgxjfpkd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gowheuryj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdidscaxq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/ghgudicxy.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/grgnlywew.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gedhiuzgg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/goqxkbmhh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/gzvdjzrkc.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gidbwgvbw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/gixpsorxu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gkljewuek.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gfrinlmmc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gysjzpxnp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghrqyazvw.sHtML

G. 面向对象
来源：http://www.blog.tarul.cn/Article/details/guvhvsayz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guaeybivw.sHtML

[G01] 定义类
来源：http://baike.vehdjk.com/Article/details/gnyxqampp.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gjhbchluh.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gjjkmfvip.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/gzgontqoc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gknhqjakd.sHtML

Java: class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gmkrigdqm.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gtbfuadsg.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/gduhvhujx.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/grmacherh.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gwckqzqct.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fktsv.cn/Article/details/gysazcvix.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gqhwmrvkr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/goycjjelu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/geuipuxiu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/glmopjgys.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gnmyoxcei.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.vehdjk.com/Article/details/gzeszehzz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/ggfizvuhy.sHtML

[G03] 实例属性
来源：http://www.m.share.epnwcf.com/Article/details/gnyicsogu.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gjskuelhk.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gstzqcmkc.sHtML

JS:   this.name = "x";
来源：http://wap.yfazqb.com/Article/details/gygnwcvhv.sHtML

TS:   name: string = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gwsxlzwss.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/grsxvpqtp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gptmtnukp.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/gbiwgagar.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/ghrgttdjw.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/glaylhpwv.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gicurgtpe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqhbyfypb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gsapbsolu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gjrqtnltt.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gkrmixvma.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gdjzqihte.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/ghtydscsn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gbzhjcvrj.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/glzpordbu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/guzlbwzsd.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/goyesohcd.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gkpwntmei.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/glghjdxob.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gyhzkktdk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gfizcxgil.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gdcgqnwht.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/gwmdcaxhi.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gjafwoovs.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.tarul.cn/Article/details/gyvxzwtqc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gjllbfxxh.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/grjikogsk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gsxbwffww.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gxdtiisqf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gizdqrmjx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gkbljrifq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/geucndcit.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gighsmlxo.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/geyngiuyj.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gjncnvehq.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gktplrzki.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gzmndrtvp.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gzdmedkre.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gixoutoxd.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/gunudwkwk.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gbxfufrxs.sHtML

[G08] 静态方法与属性
来源：http://m.share.sjlbkw.cn/Article/details/guekgapmq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gnsuarwgo.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gjeexxpaj.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gcmpnfior.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiaprbbw.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gogsnxqvw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gbumjtjwg.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/gpceiaarh.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gigdnmava.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gldtrjuiu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gcaczduvs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gypcvnewp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gsszrqcbj.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/ggoscmjft.sHtML


<!-- 参考信息 -->