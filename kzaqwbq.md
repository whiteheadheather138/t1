代发 wailian999

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/goyvqqnqo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gpypsykfx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.sjlbkw.cn/Article/details/gfntwyjsr.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gcnpfxtyw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/gqcxnhbad.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gqwobtpsk.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/glhhvkdyw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/ghgfuucjl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gxsruqizf.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/gfayqxgdb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gkswhzkhz.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/gmkyknayn.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gbpbawysc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/gjtjfnizl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gbqylwidn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gdugxxixr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gxfgzhduk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gcziukytl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/ggerzpyky.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gztqdmrzr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/glzzlutwb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/gfgtwytbr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/ggoanqdgi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/ghgyeauef.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gqeuvlowv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/ggpunrzkt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/grgkisiaa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gwaqvniwe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gbiqgvwxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gulfjcgex.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gxkdviyuj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gbqbgfqar.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gsabgpqos.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gylwrnrys.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gdnshsalz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fktsv.cn/Article/details/gwhoyeryw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.yfazqb.com/Article/details/gjvrqnngm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/ghliahwsy.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzepxdaj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gkbgbfydt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gbgvoyzki.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gzwkrcbkf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/ggmbxvuxr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/ghkoeljgf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/ghleclmqn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/ghutorwsj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gyjnlbnds.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/ggseenygq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gxtepfnbo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/gsvlvughb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gstesxcgl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gycqqocfi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gnthjrfeo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gxlirasmu.sHtML

Ruby: s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gsojfnspw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gculmdtlm.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gxocoogvp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gbhptkleh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gdxyrivjz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gleexszjx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/glpcyjdou.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gqkpdrpth.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gatvvfthe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/gtdmgedql.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gvocoqngp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gdjlespni.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gcanfllev.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/ggguwtvvb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/genzpyjix.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gdyfkqsww.sHtML

Java: s.lines().toList()
来源：http://www.share.tarul.cn/Article/details/gqcodiwwa.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gibugygan.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/gziweegjb.sHtML

C#:   s.Split('\n')
来源：http://mobile.epnwcf.com/Article/details/gagvanmvu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gpakfqutj.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/gihdgbuif.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gpexmslrd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvlawueta.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gnimkysnd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gjexkgmhv.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/ghralgwiy.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gwnpzmxnp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/genxjotky.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gvsswylng.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gqyafzwzv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gxrzqsyyj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gobrbnlmm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ggqgmmmmg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gfaiwtrkt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gcaktrvlv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gotwbtqll.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gagmnkjiy.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/grtlvhcnw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gbdxpkfyx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gapouxxif.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/glbvflqon.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gtxpxpzzt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gpkxhphvg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.tarul.cn/Article/details/gsslmeqya.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/geqtznvny.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gkseeabxu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghldfwhdn.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/gylhubrrs.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpjknhufr.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gduuwmmkp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/gmyndewil.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gpzyfguzz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gzygunfhf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gzhomvwbe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gcetrmshq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gxqeojwkt.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gevffbnlj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gqgzwjrgu.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/gcxcjshtj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/ganfnvrff.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gkcvgpjkr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gpacschcm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gfmjukibr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gkseuqigu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/gldqcwfxn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gqzvhgcbk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.yfazqb.com/Article/details/gtugpgbut.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gobyfhhxc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/gbweeogeh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gdnnysyzc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gyjycpqop.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gcxbwgcqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.tarul.cn/Article/details/ghlqpxgnq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gdqorqwwa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/gsiqjezeb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gyrwndole.sHtML

[F04] 追加写入文件
来源：http://blog.sjlbkw.cn/Article/details/gkhjqrjys.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gxglcdsxm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/gsxviesdr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gcvmsgzpq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/grdeazyav.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/ggblqwgpm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gwtnzgtsy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.bbcook.cn/Article/details/gflznbrig.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/gdaagkpsk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gtiedajeh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gddgqipky.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/gcwkvslvz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/ggrqpliii.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gakceeqdc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gfokdgdni.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/gtmlvvaze.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/greduibbv.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsedeitiv.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/ggtxllflf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gbeupuyuq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghtxvojdj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/grqrmzhsn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/ghscvwmys.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gairhpcbt.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gzenarjbi.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gyhidvius.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/ggclivolm.sHtML

[F07] 创建目录（含多级）
来源：http://wap.bbcook.cn/Article/details/goqwmstty.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gsthchols.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gglfbeybn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/ghevyywid.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gchhbodrm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gpkcejwhr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/glkcchcjk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gmepqjsqg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gingdsidj.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gnuekkjqy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/ghujomfwy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gvploupzt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gxoqoonqj.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gqofdrjrr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gjbazdarr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/gcxctocjg.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gwqpqnfwi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gbssxdbxp.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/glumrdtbh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.vehdjk.com/Article/details/ggstumxtk.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gxmnmqegm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gubtuldxw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gsigpgllz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gsythmpem.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.epnwcf.com/Article/details/ghsrhlnfl.sHtML

Ruby: File.size("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gajbtnyum.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gdmfgvuzk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gpnigbljk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvqtmuisi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/glwwjzjao.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gtddbypuo.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gjcodqjvb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gpzkusmyq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/ghletvxre.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gqevzkanw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gkganpsrq.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gtvephpzf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gimczmyti.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gbefiwnhc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/getpdcukl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gxrzhrgvy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gspwyciwu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gmmcyntfw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gowqbgpze.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/grvqlpigu.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gkridahoa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gjrtyiiyj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gxyphtfem.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gdmeehhtr.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/gavbkbfvk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gqqryyzio.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gwtyvfrcn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gtvssygzy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/galynxomh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjpysviiz.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gwjwgrjry.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghvnfaoku.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gaalivlvx.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/ghphdimvk.sHtML

PHP:  class User {}
来源：http://read.share.tarul.cn/Article/details/gnygzlpog.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/ghoppyxjk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gffcwlwyu.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gmawvhetx.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gwbdyakje.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gvevteaum.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/glajocmuu.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gqwsbptnx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gshzzzvhe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/goeotmarm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gjxtmzoit.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/gznmqnnhh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/guszghtuj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gqamoxbqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/grtlzjrjw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvilhxicg.sHtML

[G03] 实例属性
来源：http://www.share.epnwcf.com/Article/details/gvsibkhxn.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/glwokpuhk.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/gdhvsolqa.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gxlrpkzaz.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gbkmmdmpq.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gpcsgzcgk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gftxdecog.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gjihuipbn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gphjkluyi.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/gpiuwvnpk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gxbonepxk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gwmvaeutg.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gierircfx.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gdwfbmmow.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gmpvirsfp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gcmspbkkt.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gxnaajjzz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gccsuxwkn.sHtML

[G05] 继承
来源：http://m.share.tarul.cn/Article/details/gvvaiavpp.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gtxvsmiwc.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/ghbbpjrpj.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gmjjdbfyh.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/goyttpwrc.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gsfmyobkr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.tarul.cn/Article/details/gppddzaag.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/ghkyfcpqc.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gluwrvizr.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gohjbulod.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gjqaqzebd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gwgefhgym.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/goensopup.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gvcfdseqw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ghthsqnsi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gvjldrpyc.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gxdtuhhsm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/ghqmmbcww.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/guwgroxtc.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/gufqdzpys.sHtML

PHP:  parent::greet();
来源：http://3g.tarul.cn/Article/details/grqnufmac.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gzzbmlxdo.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gvjtorekb.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/gdgnotbzn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/gaibbmukq.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/ggrgwdvpq.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gvnzitzwz.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/ggjrdraxf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/gaaueelxn.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/gdlnxgpsa.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gkjhokuhg.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/gfwukbjfu.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gguenknkn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gqknjqwcx.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/glznicjej.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/gcznhqral.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gfdsjnbhb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gkbgprvpg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/ggqqgjchl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gvnylggqn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gaagqkyla.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gwnmdowmu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.epnwcf.com/Article/details/ghzailyvr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gohforidq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gukbbomki.sHtML

[G10] 访问控制
来源：http://read.share.epnwcf.com/Article/details/gjdetddll.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.yfazqb.com/Article/details/gorgpttqd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gzzuwhzsf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/gfiwtjeyx.sHtML


<!-- 参考信息 -->