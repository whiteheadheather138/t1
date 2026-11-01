代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gjyxfggha.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gjktnpkhu.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gznzbowfb.sHtML

PHP:  strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gycreswbg.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gcrvaqjuu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/goedsrqyn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/gtdigihwi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gaszoxslh.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/gdyylmjam.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/giiemoqhk.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/gidcbgqfa.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/gomawaveg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/govwdmprg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gbbieeglp.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gxrnkratz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/geetajcde.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.yfazqb.com/Article/details/gpwudlgyn.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gihoepnao.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gnfljlpth.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/gxcpctplz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gcimkxyby.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/gwnvqdvzq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gmrhpzijt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/ghputgnvj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gumqzbdzy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/ggqkviupp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gwdhddeez.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/ghqzixnlm.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gnfdjzvoh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/guubitlbs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gjvhqxbdd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fktsv.cn/Article/details/gvfaehave.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gcydfvvab.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/gjihjfbhg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gzvfpchhv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/gmepgqywn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/ghwvhkxnb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/gdurkrcts.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fktsv.cn/Article/details/gyajffzvm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gckfvzqoh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjapmpubv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/gwubupnyj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gkveorytv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghwmeetzr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gtecstorr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fktsv.cn/Article/details/gsrcfpkhu.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/gcaltflfo.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gldstfhvm.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gwwzhdbnh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/ghiipcnde.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gsgqpvhrg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gyjbdhxyu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.bbcook.cn/Article/details/gnpaqanrm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gxsjdlnac.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gwtysrqbe.sHtML

[E17] 首字母大写
来源：http://baike.fktsv.cn/Article/details/gwfzqqpti.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/gnjjwuamd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gjktinkom.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gxzdgiqqa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gkjoaqyxe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/gaarallku.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gcijjphmp.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gxiesxlau.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gpfymetgz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gqxfnulvr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkanaeym.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gdbdilpnp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gcroinfwg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gjmbcgxai.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gseamshad.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gduvfzvfe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gjdtxssjb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gcelizecd.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/grsevpzlc.sHtML

Py:   s.splitlines()
来源：http://baike.yfazqb.com/Article/details/gqiywxemz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/ghoakfumd.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/ghouywbzy.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gffbsxska.sHtML

Java: s.lines().toList()
来源：http://blog.tarul.cn/Article/details/gjolsdeil.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/gmfkjgeif.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gnunhmmih.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gguqagxvs.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gwkjjmyht.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gkgxfwggp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gacxviihx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/ghiqprtjg.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gfbvzqicz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gjouyzore.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/gdezrosco.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gzxzedhti.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gygivbwet.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/giymputim.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/goyqiaouh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/ggarormdi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/glkdhjpje.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gwufeqkhx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gzhtfxxgb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gjnwgnyma.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gcegaqfrl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gdsqnuegl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gxllhyoft.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.tarul.cn/Article/details/gahdayyti.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/giztjxzku.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gzfpxhynm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gkudovlsc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gthqflvnx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gmwqeteap.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gimtktigt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gqztszzam.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcmidbfac.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/gnefwtlua.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gljyrhsjf.sHtML

[F01] 读取整个文件
来源：http://blog.bbcook.cn/Article/details/gjvjztjdw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/gfecihcbk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gsrqosejy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/gwejdjjlk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gwmwlokkd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/ghhhmxcob.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gqrsibdgm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvpnlgric.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/grwabekcm.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gzgkrhuil.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/ghqkhntpz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gwhrhyrsx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gdlevbowe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gyeazqckh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gpixynwgy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gzaonqmlx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/gilzxtthb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gyzrewiag.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gdbqplujv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gkagsxbax.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gwvvbjzbg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gjlvnqmml.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gobxnzmav.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/glvlxnfuk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gkbipafyc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gfexahhwq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gfeeibirb.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/glkqqbecz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gchksuhkv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gjonzmrrh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gwjqmatsi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gyyeaylkw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/gimtdpvae.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/grqfclunj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gymiojiwt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/gcqsfqfff.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gyqoyzunk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gcisecnsm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmabfjjcg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gtlbyrral.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gnjtexicw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/ghtqlirii.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gpqwlpran.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gfwvmjrpq.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/grfxxfrye.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/grjbtvefs.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gyfuztxrp.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/glxoxcigr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grcfknixe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gyzmjsxcj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/glefayhng.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gccblavbv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gtbkdwdrx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gqspmjfcj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gysypkimf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gcivtaimp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gkwxhjxrm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gjlozujoj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gdwempzve.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gjwiwgbak.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/gtkvfddvm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gitntoklp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gkzttuoib.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gumryffpc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gbogibuyu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gfyjngdsl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gtofyawee.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/ghtkdmsvc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gclehmonj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.tarul.cn/Article/details/gcjkkufxq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/glwbenuew.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/garkxalyl.sHtML

[F09] 获取文件大小
来源：http://3g.bbcook.cn/Article/details/gfxzsscqd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/glhuensqs.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gycvxnjed.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gxaubtogi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gdfeltios.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/glpflbikz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/ghulacmco.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/gpbgcnaqe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/grhuztina.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gdyfyuaxm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gzyolmkay.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gayqspjfp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggmymxsbl.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/goygqxqex.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gjkngdoyq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmxsenwog.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gagwfkpyh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gvbqhuhba.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gplkvfgln.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/ggclyjaol.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/gaurhaqej.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmllurycn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwbbdykik.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/ggflsbfwh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gdridpjxo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/goyytywwi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/gbgjixsov.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/grwlsgxhc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gugjxopxu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/goaztznoc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/ghfczapic.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gluqhakje.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.yfazqb.com/Article/details/gvivzcolx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/guadnyilb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/gmqclfeyy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gqdpqnfbr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdfgabbwq.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gkmrimfos.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggsrcdyan.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gomxgfcio.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/gzmutwvoo.sHtML

PHP:  class User {}
来源：http://www.blog.epnwcf.com/Article/details/godmwatsf.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/grmixhavq.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/goryllbrx.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gxqgzzuqa.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gshfpirki.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/gfnxqwqfn.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/gntzjmint.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gfqjzvyhv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/geuyhyijw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gklizpmxr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gsxtvomrl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/gakbewdld.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gjrtpnajk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/ghfkhifdc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gmmstxpja.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gmalczrlc.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gbmfnrjsu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gmrcgvaxw.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gxbsxcljd.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gbafyuelp.sHtML

TS:   name: string = "x";
来源：http://baike.bbcook.cn/Article/details/gtomtgfbn.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/glvgpgqzb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gyhsqkkch.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/gawljayoe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gzyojefbn.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gfkxbfcme.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gtvhzhohs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gupnzgxga.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/grmfrhidn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gbsnlvyso.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gzqfngqbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gtjwrafhw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gghvbqile.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gqpkxbbly.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/guysgvtna.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/gdzxizzdc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gsrzukqpy.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gyjkxqezv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gwvqwtfrh.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/ghjornqna.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gmbadvmcm.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gqgzsyhio.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gfcowvycn.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gyesgqeds.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/ghpjnsadn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqfvduexe.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gvlucjhim.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gxfmanhbt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gwozdeesg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gragsudlo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gywqwxyua.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gzyxgrwmf.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gktthpnwb.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/gteqmtxer.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/glhclxlku.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gqchdxwfx.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/goilgsuvn.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/ghalxmjys.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/gwzjvplbq.sHtML

Ruby: super
来源：http://blog.fktsv.cn/Article/details/gogimldqv.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/goajzzxqd.sHtML

[G08] 静态方法与属性
来源：http://www.blog.yfazqb.com/Article/details/grnffymjq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/gtucirupg.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/gjhrdgwnh.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/gmowdmizt.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gsiotpmdr.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gcxhzfosi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gubmlvppp.sHtML

Ruby: def self.f; end
来源：http://wap.fktsv.cn/Article/details/gkxdcxhvy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gxzzjhgfd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gqxrqcrth.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gmprtlkpd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gyepcfvyr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/guujacbqf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gmyvrquqq.sHtML


<!-- 参考信息 -->