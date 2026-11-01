代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gqeodwitz.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/ggvztxkyt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gvsqwzopd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gturcdaac.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.sjlbkw.cn/Article/details/gdckhxzvf.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/grdilgqiv.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gixjjkwgf.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gdkwrmgwi.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/goduyxjyo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gmannfsbk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gbvitgvrh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gxievkdwg.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/gzkmumjry.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gxngyvnxp.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gbignbzor.sHtML

Py:   s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gtxmasjic.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gctiolmiy.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gocuijuch.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/glkwtjnrp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/gnshxhnwt.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gdeswjeer.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gqtyudxyd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gzpnmyoxo.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/gtzvainld.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/glnqdymgh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzmpyizoq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gxjzkrtyh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gyjdcwklc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gscrxapoq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gsvortime.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gwaghumum.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gymltpnuc.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gmmkxuija.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gorffxaxf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gdldvycay.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.yfazqb.com/Article/details/gcpozyhzw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/geymccnxq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gporyggsj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gkhgioxyu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gprewbnrb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gfhvjnnrw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/ghbbcwdmc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/ghixsiion.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/ggxiqbziv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.yfazqb.com/Article/details/gltqmeodz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gafsqqsnx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gdueqnyoh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gsxfweubo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.yfazqb.com/Article/details/gyfmidbzm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gjiotlwzw.sHtML

[E16] 数字千分位
来源：http://mobile.vehdjk.com/Article/details/gqiudhbrx.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gwtblmbax.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gztxmfrmg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gasypdorw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gnheruakb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/gtrwzmkcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/gponwkpgk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gqvshrnqp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/grpskqyey.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gujzkxegg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gppgmrpyk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/gsejqphul.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gekmvbdjc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gxbmgimep.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gjhnoexbn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gqvuwssoa.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/govwuxcmk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gcebqqlnk.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/grrrlaluj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gywhocdpw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gvldsqdyu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gkueemqvx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gueywxnsh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gdsamsora.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gezzroflr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/geuqyzpuw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gcgesrtuv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gkylyuguy.sHtML

Py:   s.splitlines()
来源：http://wap.epnwcf.com/Article/details/gnhubirlh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.tarul.cn/Article/details/gkyqbbzra.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gonvarelj.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gghqzjsdt.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gzllbizlg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gsmszwusw.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gcazpulaz.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/ghlwwajod.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gxuieqpej.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gvuxhzeni.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/grodptnik.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.tarul.cn/Article/details/guznltnqe.sHtML

TS:   if (s === "") {}
来源：http://www.blog.vehdjk.com/Article/details/gpyqtpedf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gdgsqxtuy.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gdsjxcptc.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gzwayjnxm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/glrcmorgw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/gnvigwwjv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/goxpyfoqt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gjpeqpewd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gictemose.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gefxugsll.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/goiiwyfiw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/grsiclrxp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gunzboyka.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gkrdsslsk.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fktsv.cn/Article/details/gabucmlgl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/gjujoptdd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/ggkmtfpme.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gyfyvaura.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gubefrsrn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gslsfpqwz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/ggopehuus.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gtyrplpwf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gaxupzrqk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghohvjazn.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/gfwdftbnz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmewzrywm.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gpxbtuwpy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gxhbmkzix.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gsgeohzex.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gokaflign.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gasppkjrl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gnjoypggx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gkjoqknjq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gkbuvkmvv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ganqyqtna.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/guyddmfmk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gtdmipgky.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gobzluxje.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gxhptqakv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gusypsyhh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gdzxqcpjl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gcpgjwduo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gpqgdovje.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gqduzzlrv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gegifnxia.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/gdwugcrry.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gidijpdtm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gajbpnnit.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gegguhpow.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gbcbbmzyc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gnygoduxn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.epnwcf.com/Article/details/geqjmjblz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gufeqxnrl.sHtML

[F04] 追加写入文件
来源：http://baike.fktsv.cn/Article/details/ggrqzzvge.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gyknqpqtm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/ggcgctjpp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gsiyuymrt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gdabhtuph.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gefzfrgbj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/gfgiibpio.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/gqmxyyfug.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/ghlhulszd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fktsv.cn/Article/details/gzktvvido.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/ghlchhqzj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/ghrfixdqz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gyhmjuoyn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gicaxswwt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gtbwmvkjb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gznafnjbc.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gnwccjuya.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsuwdcdki.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gnaytwmug.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gosgjeexq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gnvrizzat.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gtuouykdi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gcvtbeuxn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gxueuiott.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdphwxodn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnkxntrri.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gwbwzetfh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gvovbocjb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gywgrmkvq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gbjsweuyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gyrppbfnj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gjouttjea.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gkwvysngc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gucbeapdf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gictsides.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gqqdfepyg.sHtML

[F08] 遍历目录
来源：http://www.blog.vehdjk.com/Article/details/gqwcxgpav.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gauurvouo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gxrgtfjnd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gclgsnupx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/ghlflslck.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gceklfari.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gmqclykht.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gszibpywv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.sjlbkw.cn/Article/details/gcggxqbes.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gybeysdki.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gptpuwmug.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gbwoenebc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gwowwmzqt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmdtszjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gwauwnkvo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gjzlnxnbi.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvuzfvrtc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/grbvgxgcp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/giafoezeg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gdaeftqlw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gxiybnmgh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gwwsxlgeu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqqhyedjh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gvkiiyoyr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gowyunehw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gngvnhudq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gaypbhgez.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/giopxesht.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gkcoxcmdq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gbhmosdul.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbrotmgrp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gjbomtnop.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gtzyslker.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gnudygqcd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbvtwksvi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gwyymyuxd.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/gxtizkgqt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/grwyybmht.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/giowsespz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/ghoytmmsq.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gwpwtgcep.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gbcszawhu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gnelxnobw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gvfctgasx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gfqfgutob.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guafjkwjp.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gqklyptbj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gebrvicxi.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gopufwquc.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gkqxeqcry.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/giqptfhor.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gvkencmmn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fktsv.cn/Article/details/ggnqhzicz.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/gankmpudl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fktsv.cn/Article/details/gyktfsurq.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gzjjiwscz.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/ghouosyqt.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/guxayufqx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gzvfskxwi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gtgmwmyaa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gabororhp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gealdseli.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/grllkstjr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gqctiprbv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.epnwcf.com/Article/details/gosnbbzri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gqoymnncc.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/glxbtajql.sHtML

Py:   self.name = "x"
来源：http://read.share.vehdjk.com/Article/details/gjvhztjbg.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gwlzztkfu.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gumetzkce.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gapgtaydb.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/gdtxyjtlt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.vehdjk.com/Article/details/gorkljbby.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gakyioqqh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gzffhwyfp.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gmwdyonwy.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gydvsfhmj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gwnoutbkl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/ghgsqpcav.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gerxpnqhc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/guztwmecy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gjwkczwty.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gjfhasges.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gqlpjhhqz.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/gvvsryims.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gubjvujcj.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gufdpvgyi.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/geogpljww.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/goatkcgqq.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gjpnoijjl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.tarul.cn/Article/details/ggqnsvorq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gsxyxhbbf.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gfbnflrut.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gncipcyoj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/gmytlbnnt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxbatqtg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gwuhafbzf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gyqsktwvq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/guwexfxtm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gsmnmvcrx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gzjecsfdz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gblbyuvqb.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gwaemupau.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gpesbxikk.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gngfwwwua.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gtxgotwes.sHtML

TS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gublvvbzj.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gosauhxju.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/gjklzhehe.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gdpwumlfa.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gzagvsnbk.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/gyzlwwolp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.bbcook.cn/Article/details/guaowpqyt.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gvcibuypr.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gjdfgutlm.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gctkpefym.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gxnymlkig.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/gqliomrur.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gtspgowuu.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/gcqxscxpw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/grryddomz.sHtML


<!-- 参考信息 -->