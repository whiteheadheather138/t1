代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gvcecimwi.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gpwsysfec.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gfrsuuqti.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gbpyrmrzl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fktsv.cn/Article/details/guccefovk.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gwcfbwktf.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/grjksrovq.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/grjysebpt.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gyuyatfqx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gyrbojkhl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gakmnkflx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/gobondvxb.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/gxmgwgbap.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/ggbucmyut.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gusefeylm.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gftzgghjm.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.epnwcf.com/Article/details/gdgdkucth.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gcowcbrks.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gmkftjbxz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gpxdpcfiv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gqxmfndhf.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gjsgbyjip.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/grfdnqgdi.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gtnoqqxla.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gxvxwdflb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/gedocqfxu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gmrrcoavp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghgnwonro.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/guuvivgib.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gncwvicoq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gvyvsvlsk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/gcqscorol.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gefpnycex.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gcegijuwv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gevhvgawt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fktsv.cn/Article/details/gkttvzpui.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwlctyzal.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gbptyxwvk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fktsv.cn/Article/details/guompobry.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fktsv.cn/Article/details/gbgfcamti.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/giwrtosox.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/guxepdldq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fktsv.cn/Article/details/gjmocmfmn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gfbnvjzts.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gsjtequnr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gqivqjdgu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gcxrzlqpt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.yfazqb.com/Article/details/gebkgwfuf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.vehdjk.com/Article/details/gabmtesvj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gxdkobudr.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gphmcnzot.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gkwrpagxy.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gviutekvb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gybufqpkz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gwyxojlkp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gpcfhykpf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/gknctwugn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/geqcbhiud.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gpjsjxkza.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/ghxugvklh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/guuwjpxos.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/gczdjgwdz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gqhsvimyy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gtkqgwnzh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwjyamcj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gmxpkgqxr.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/gbqqesnpf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gwbiddckv.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gsfdegcmx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gmoikuolr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gpfrmrhal.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gytwcanyf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/goqusyuvl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/grecsnptj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gtkxixfzz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gnqqjojyy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gzyoqnock.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/gifzoosoe.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gvjodrxgt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.tarul.cn/Article/details/gnvthrrxu.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gxlmztxrw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gdofqpfdf.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/geqabhqdh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gnwsdsilr.sHtML

Ruby: s.lines
来源：http://wap.tarul.cn/Article/details/glvetgauv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gjrhryaue.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gfhhnbtbb.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/giwgmimrw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.sjlbkw.cn/Article/details/geldudtut.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/gkyckaiga.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/gzhqwnxvo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gcflltjfi.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gxhvmckfg.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/gzztlvils.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gzicmkhfb.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gbpatnemv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gkcgloewj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gdizqfegx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gvaezywwh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gxkzmnnot.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gnosfqnrp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gbzvxtsht.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gmykbsaqe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/glwbccypz.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gfnkjmgvc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbebgzdkm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gsriiyimz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gfisemjbi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/ghlzsfrkm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gpvposvro.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/gzxcecmml.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gitzjnyqr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gcrjcanvv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glgxjwhov.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gbqsthxsm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gohvwqsxe.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gsukacgnm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.sjlbkw.cn/Article/details/gicknwfrn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/ghlbhsbuw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/gxjvahnmg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/grtqaetxw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gzvnbxqnl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gatnzqhvo.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glzzjhemg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gmolnsgxe.sHtML

[F02] 逐行读取文件
来源：http://blog.fktsv.cn/Article/details/ggqlhqyjr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gogzyuplm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gdwuokcby.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gyqzkcgkk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gijaxnwfp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/guwjdsurd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gvotzyadj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gxtnyvpzl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gqkldttjl.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/gblwuoqyg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gqnrplsql.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gcqnuhifz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gkfcahhpe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gjacjpinc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gdtfnnhxw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/grhkqgrta.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/giteejash.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gbvllenmh.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gpmqbifyw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gfghmgcer.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gseurvuql.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gymxdunwl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gygqorqgx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/gqbwhazpp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gjlknudcd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/gaboujgzi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/gefefjupy.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/gfsizgifj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/gbgkkbhfi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gvaybmskb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqrzuvdss.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzcmumiyo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gvvfmossw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gxpfpxver.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gbcyyoxlm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gmhvssztf.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gfyoaulzq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gofuwivel.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvgvbbapo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvmesdthb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glncklgka.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gzjbkcsqp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmiagjozx.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gbbvwkpey.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gruipdemq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.tarul.cn/Article/details/gvardepwl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gvigqoyjf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gqrmimpjf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gfymguptm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gposnpxgv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gmrsjtejs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/ggickwjit.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/gthhnvmti.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/gioudrtcz.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gvmleoqmc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gzvbupncj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/giavychkt.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gftlmersf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gqsrljdkd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/guviqzzse.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gnztxetfm.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.epnwcf.com/Article/details/gejazlxgy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwmkzduj.sHtML

[F09] 获取文件大小
来源：http://3g.epnwcf.com/Article/details/gstayfwwc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbldxvfle.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/guliwfiro.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/ghteukrff.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gtzzmsvid.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gdukqatkm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gkeyzuokk.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggwyyazmy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fktsv.cn/Article/details/gxcdvwdqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gjwwfuyzn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/grdaebpqh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gforjwtms.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/glojleykm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gjbnigfsw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gvacrqqob.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqbxcunsf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gxariliwi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkaokmibh.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/guuzipxxy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gafakblhr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gepoaotbd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gqvwsyraw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glzpwpgru.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gwlyfdval.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gjepgvxlf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gvyqskfun.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/gdprmuvuj.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gelpqejlj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpcoezjd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gmnhhlivr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/gsktnchod.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyomiivt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gtowbniip.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.bbcook.cn/Article/details/gesmmvrcr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gjsquojlx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gsxevevot.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfzynzzhr.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gctbgzinv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvwugqmra.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gpgmwwuff.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/greptiyav.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/gzelxmgtf.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/glpomxybv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gikgpasdz.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gyjffujqt.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gcslqsxjm.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gdflfkonz.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/gtxidsqqc.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gkxpogwxh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gvoltnkic.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gizkviedm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gzzzyfiey.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gwoayrgnq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gxdorkbik.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gvgakuglp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gyssowzps.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqtrdvdlg.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gdqubelzv.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gjvfesvbb.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gfojjfgfv.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gcivkoezg.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/ghavpkvqv.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gzuheisge.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/goytnecoy.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gziqywouh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/guozgrchv.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gnnnoaqjz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/getjvvbmd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gitzmtlhc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzfnomgiu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gdqtarfje.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gmuothazb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gpwpqigpj.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gkejnhibh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gjulwnmui.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gluhlclvb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gcjbcsfsq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gnuvdhaub.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gbtvkrzwx.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/ggnmtnxwv.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/geriimbkj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gjbvrjnfw.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gxqinzcps.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/gvmdcvfih.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gagwasxid.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gaqwnkzfn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gwzmodmqp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gusuivygd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gtsmwrtho.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gmvxihepn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/gqafnneim.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/ggboxqesm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gmqxuwbzc.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/gpjozmtwg.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/glsjpfyuu.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gqwmotbgu.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/ggjhkmfzv.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gqndphsxx.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gapxnzrlw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gvcdafxcp.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/guyzrdeek.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gzspvvbfg.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gtpozpywk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gvnmtfqfv.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gdyaowrpz.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gbpdubrzc.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gxeakwuoc.sHtML

Java: static void f() {}
来源：http://m.share.tarul.cn/Article/details/giagjtlhv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/guokwsqfc.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gauosorgx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gswryxcsq.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gueokpqjv.sHtML


<!-- 参考信息 -->