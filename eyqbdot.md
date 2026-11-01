代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.yfazqb.com/Article/details/gmlupzgnc.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gtmuteuhq.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gpcapsxxw.sHtML

PHP:  strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/glldhfmnh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gyczpqxqy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/guyvpttuq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.vehdjk.com/Article/details/gchpdxcya.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.vehdjk.com/Article/details/gvumscdrv.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gqgybpivs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/guxbgqtzu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/gidjbzuiq.sHtML

Py:   s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gntxtqtjc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gjqdvsqih.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gyzcjtlmg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gqlgihtvy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/giqxdlyjh.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gxpnaxdao.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzkhoqbn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gajiqhiev.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/gsoswmhqs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.sjlbkw.cn/Article/details/gcyygcbwx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/givbgcqji.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/ghxduhsol.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gudxpfxpd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gqzqpzzye.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/gznizxfrp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gbbxujvmc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.vehdjk.com/Article/details/gvorzenxp.sHtML

[E14] URL 编码与 Base64
来源：http://blog.epnwcf.com/Article/details/gcnmuwgto.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gawpimlqo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gkflharsr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/gzxrnzypb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gueyituao.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/grgmabkdk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.tarul.cn/Article/details/grsfbejsx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gjvifblcu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/gysffgffs.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/gctcweagj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gfjrvpedx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gywgeljad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.vehdjk.com/Article/details/gvmrvotqn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/gvfogbyjn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/gvaicrrjw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/gjyczpyqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/grglnujpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gotijiupa.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrltaoec.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gnzyvbltp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/goejropdb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gkxjrgdcu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gsrljiyca.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/ghndeyprt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gebknnbmp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/gtylrhxxb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gvvgazkix.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gbxfesodz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gpdqotdwq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gcgfsmpxn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gwkxendbg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gdsffgxfe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.epnwcf.com/Article/details/gjeochqfk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/glkdqavqh.sHtML

Ruby: s.capitalize
来源：http://m.share.fktsv.cn/Article/details/gpsmlhzrv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gxjqhaano.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gujwjqpod.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.tarul.cn/Article/details/gfhxikmuq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gswcjbexf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/glxzwhfyy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gptwofrik.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gnaydbpty.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/ghjfcqdnr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gnfwynqol.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gtgspzisw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gdmladalp.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gurmqcdsb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gzqbibaez.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/guxlxqqks.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/ghknreeen.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/ghpbyxeeq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.bbcook.cn/Article/details/gonlttvam.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gciuguziu.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gscpyqugr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gpxrziljj.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/gykcqfgeo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gbbcvzdtg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/gjsfvrfnv.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gxiunwzsv.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gkalwdjee.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gklrgadyy.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/grnlefhmk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/geefbhvez.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gaykibphc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gufjgbtpj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gvtrpfnxg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gyweoojfl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/grvfdsgsj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gxvyrcext.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/grdaardhw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gatgqyxww.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gyuvgmrlj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gsflbgwcj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/gaqxpyqrl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gvofpmlpj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gxihfzhqz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gqxcmnzxb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fktsv.cn/Article/details/gogghmqhp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gydqrxwzk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gaofekgpq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/gvhzwtalp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkorsziuq.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gftkxztcu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyjpnszqq.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/gchsgbuhj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gwnomsaic.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ggkuiiuvj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gaeaeivrb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gdzvrcvnz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gdtigipjs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gedvtbtem.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gkksmdxoj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gygidjikp.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gzpynuspy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gjaicnoxp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.sjlbkw.cn/Article/details/gagbtdpaw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gaamhktsj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/glegmajid.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gyczghjye.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gswtirsjd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gnprrzovc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gjhlwlaje.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/glwjbldwo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gpsfztdsf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/ghsyqdayp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/ggpayvufs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gvbkvqwkz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gbjmtmizj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gwdkcsukt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.vehdjk.com/Article/details/guzahpyvj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gmgmqnsot.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/glzutwqke.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gaqlwmgjv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.sjlbkw.cn/Article/details/gpkbstdlg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gqdsadzdc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gpiistvdt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.epnwcf.com/Article/details/gyynzpfhd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaskyvsft.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/guxucnwrp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gvgqfirex.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gopxorczk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/gokzauodn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gyxnyyzeh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghshdogwv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/ghlcdnmcp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/ghoblrnpd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gosjjqlkp.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/ggqdlhlgq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gcvnkkfja.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gvpowoqlm.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gmhfwnxjh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/grdmhnzan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjtmstxle.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/guqgezglk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/guvpbdrzm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gpwjjcoha.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmzyduihv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gmhchwwdv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gwcvxvlob.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gbgandjmg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gofgfewiz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/grzhvufue.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gudmcuoly.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gddfeqhhe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gomjchopq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.vehdjk.com/Article/details/goewikgxq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fktsv.cn/Article/details/gpuuxttqv.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gavaizigs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/guturtxjg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.tarul.cn/Article/details/ghkycaiqc.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gtpyrhkdv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gnobaefxr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gdqwuxqpe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/gkpfrjcdb.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.yfazqb.com/Article/details/gjmxgooyi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/ghfmrorug.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gdzoeyphu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gwmnhbyea.sHtML

PHP:  filesize("a.txt");
来源：http://blog.bbcook.cn/Article/details/gxefbbawy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gjqnyanyl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gbztlybae.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gahmwiiuo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gkjtpfyhk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gtvrksetf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gqxedjvxp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gmbpigedi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/guvhmxfnu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gwwwswfsk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/guqjrfsjv.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gboqhtvwb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/grlicyojg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gcxkwncpv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/ggxvepjuz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gkkufpglr.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gfqwykvvk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxwcaszlt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/gusrnuupx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gticwtgik.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gqiixxmua.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fktsv.cn/Article/details/gjsjuwhvn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.epnwcf.com/Article/details/giathfchu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gjxrppkgb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gamvvgjtv.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/guirzaqzd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.sjlbkw.cn/Article/details/gcnbpabts.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gmxmdipcg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/gqyoobciz.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gkwkaqdzy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/gahpocozq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/gyfmqhltm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/guxzshrgw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gxtkbicfy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gykgkxuor.sHtML

G. 面向对象
来源：http://read.share.vehdjk.com/Article/details/ghjlxwuqk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/givjzzpfu.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gytaieixz.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/gaqkqbvgf.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/gzhvleqzp.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/ggnrwdtgu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/gqqgmotlo.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gpqfozwsr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gtqniavnr.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gwrbnylso.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/govvmfmqw.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/gzaulkavr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gepnrnfmv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gwmtrlyvh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gqtzvyrzl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/gnifvyzms.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gxmlowsxs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gxqwmnfpg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gmogfgjri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gnjzbdyvk.sHtML

[G03] 实例属性
来源：http://m.share.vehdjk.com/Article/details/gvitxfvma.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gubqbniir.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gpkcdfelo.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gmhryojfl.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/glzopbnzj.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gcyfjfnrl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gkpjiyoam.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gljnapfvh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gdewezsfx.sHtML

[G04] 定义方法
来源：http://read.share.sjlbkw.cn/Article/details/ghdlgtpuo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gpfwpzavx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gnbveaobi.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gdczwlnou.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/ghoyjzspa.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/glbtutnxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gbpstsrdv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/giixedqjr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gucodwnjx.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gbbqzldol.sHtML

Py:   class Admin(User): pass
来源：http://blog.sjlbkw.cn/Article/details/ggdvdzcni.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gqnyfbasr.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/glfidliuz.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gsplcsowz.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gwmilufdb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/ghfebizmg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/gwxtbzcjg.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gsvjcelxi.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/gjfqzvryd.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gakkxvhdc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gtyuzbbdu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gnpqxrskk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gbmprhiex.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gqyrqgbui.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gofewapws.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gyzpwkzib.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gscaowprl.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gystleczg.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/gbajyixva.sHtML

PHP:  parent::greet();
来源：http://www.share.yfazqb.com/Article/details/govsdtprs.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gotmejuco.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gdidpcpwe.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gonkygsns.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gbctoajqc.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gshqldhbg.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/ghguadsdj.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/gxqplyjae.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fktsv.cn/Article/details/geqqvjhpq.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gtvbwkohi.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gxjiravzm.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gbwvbrrjx.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gwajkzylz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/grrlkorwx.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gvbuszpzt.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/ghzbdllfl.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gldxummll.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/glrkzyafs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gjfkzjmhh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/goekfznnu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gcvszvasq.sHtML


<!-- 参考信息 -->