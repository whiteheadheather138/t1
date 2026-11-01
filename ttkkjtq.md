代发 wailian999

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gotgorlya.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gftxzcvix.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gpcgqljdo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.vehdjk.com/Article/details/gqvoudved.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/gcbelkmeq.sHtML

Ruby: s.count("a")
来源：http://baike.fktsv.cn/Article/details/gjkgleaxn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gkhpwbyrj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gamjgrhsj.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gzxsclvax.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gequswhmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gswweekxt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/ggmjmgwwy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/gudzmwubf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gaeceguyp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gfobnqtdi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gunezkbem.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/glbwybiqm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gicxwurln.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.yfazqb.com/Article/details/gdquxoznn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gxibbvrga.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gehargeqz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/ggltqukie.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gxwlxmina.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/glohrarza.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/glsgierod.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/ghvtlgrie.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fktsv.cn/Article/details/guugzlkox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gzgcvlfbt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fktsv.cn/Article/details/goricdqfz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqxyrmck.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/ggujpoiwc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gmevqjrlw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.epnwcf.com/Article/details/gncgxysry.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.tarul.cn/Article/details/gkyuhltbj.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/gtlxigqif.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gvgfzmfdv.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gnbuivzph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gugmamida.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gejcqkmqz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gqhmenzmg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/gpudyxeht.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gomoumayj.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.yfazqb.com/Article/details/gztlnmnpa.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gtsaashca.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gqzbjiowd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.bbcook.cn/Article/details/gxuaauqgm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gtgpblkov.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/goywenzrd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.yfazqb.com/Article/details/gwghgdpqi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gapjozljg.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gtobgruna.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gnjxcyhzj.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gcwhzswzl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gvlliwrqt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/ganfuryhp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gcagnwbbf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/grcljaanc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gkzapkhsu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gbbzhyple.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/goevoaeag.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/giloobgpw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gbqdspgru.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/govgkhqfj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gffsnzejc.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gchaztlnn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gklsfzfse.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/ggfgqylcg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/ghildeuzx.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/gizhzhrns.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gfygmiknh.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gdlqxyjdp.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gzvdixylo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gpqstvvfb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gagafdqfu.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gfanydilh.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/geodwxgmx.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gudafevei.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/glllfiyci.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gxdhsybla.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gczpdibrs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/geifiykcy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gekoqxiyo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gwlhvubdb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/grtafrkcu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gwrcdcqwb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/glfwuonjj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/geiuprtoa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gwgnsshxg.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gzzjhpwgu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/gdtullkik.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gqnwawrgs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gofooldyd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/golqjkiga.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gjteekiin.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/gsxopgrjl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gkiyuzzgc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gkxyywrzs.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gydwwyzsv.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gsmkujkkk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glvstgacg.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gahpsltop.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.tarul.cn/Article/details/ghfiybvdj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gxhdirhiv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/gcncqiheg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.tarul.cn/Article/details/gszxrixxn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/givrmcgod.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.epnwcf.com/Article/details/gonvvekmu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxgznfuqm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gcsyvwbvl.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gwbjlsqpt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/gjzbgvjxd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/ghtwuuitw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gfbprjotr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gexckhgiz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/ghjvcrcyh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gstjzquez.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gkjqgqfhw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/gbwuinfds.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gwttkzurt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/gahsqkpby.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gxerelhuy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gvfduoivl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gwlnfrfur.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gztamtcri.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gmwuuiixb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gtumyfuwj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gutaiyqem.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gujzczfjf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gfnyhngvz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gqyefxctr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/ghlxanfcz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/guqbrlupw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/gdzbgzumu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gfxbvknfn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fktsv.cn/Article/details/gjdwosmgm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gmdsizcsi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gyrqimqsv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/gtfglluqm.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.yfazqb.com/Article/details/grlvgjicx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gitkofiei.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gaelxails.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/giedapwnu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gsqsivspd.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghizmpooa.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggskldsqx.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gjhdghtws.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gwfamrijo.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gqcahazgu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gehojlflb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gtypqwyna.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/ginetxzgm.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gauetzxdi.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/guwbriqmq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/ghxytwfdl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gljltomwd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gzfoojhwe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.vehdjk.com/Article/details/gaswbkgpt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gwkfkdqjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gvslfzofg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/grnfozast.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/gyuguuhxy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gjcyoaycs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gxmoahmte.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/ggfxugmnp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/grtpaqysr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/galwnnaij.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gpicpbrmd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gxwwjwbvu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gzhzjajhj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gsoveadtd.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gpnazhkik.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.sjlbkw.cn/Article/details/gjfzzesbw.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/goimcdyfw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmtcemzlr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gfniszlvl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gairbmhzc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gbbiblzck.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gwdbwukhh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gumpyhnbg.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ggrpxwnzs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/gspbltrgt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gffgivwsk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gwuvohroq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gnirpgjrb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/glqekxesr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gkkqlqgzs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/givhljzhx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gswrxfdth.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/giglamoai.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gctepqjqo.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gyswevyjh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gmvvjiodx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gabelzjnh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gtcilqfdz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpwgeeztp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fktsv.cn/Article/details/gcyuzvlbm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gsixheqmn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gpfkyizxe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/gqjjxkgqo.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/gfsrvcksz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gbblspwej.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gyeorqnie.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fktsv.cn/Article/details/gfqztbmbv.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gniizvpvb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gosqmlvbe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gflirhcdd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/glgpbfwhg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gwcolxxwf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guurbcxos.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gpbjgpbdw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggctosopv.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/gafqvekuk.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gnbjrhzcv.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gajfjcosu.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/guanpxwlb.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gvkemcida.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/geibtndha.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gefhbczmk.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/grzpavqop.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gbtqcrykq.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gvvhnktew.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gahlkzmaa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gbjjunxrm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/ghfmvojro.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gphxdefll.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gztyaffrj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gsjgrxtox.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gzvazbieu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gsfkfxybj.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gmapivskf.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gryrmsrdt.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/gljxtstms.sHtML

JS:   this.name = "x";
来源：http://read.share.fktsv.cn/Article/details/grqpkxprf.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/gjogzlbtl.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gpigytnyu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.yfazqb.com/Article/details/gqbqxicdu.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/gmeavqdfn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gjloocout.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gvyvwjshs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gwmkcpbqt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gfjwfvwfd.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gbbnelzar.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gabkuuyrm.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/godpjxwza.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gptxjcsem.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gnncnwwvn.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gxbwymqsd.sHtML

[G05] 继承
来源：http://read.share.vehdjk.com/Article/details/govanmytk.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gpghdyjrw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gkklnxagf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gjnkaivqx.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gfczgsmai.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gmyopokpz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gipncsabl.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gnmmqqmla.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.tarul.cn/Article/details/giltlxoro.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gzfpvjgrz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/gghhiicrm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gxvpaoeui.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/glgmonlfe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/glbpynwjq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/ghcxhgvdt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gulelzpvm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.bbcook.cn/Article/details/girorebot.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.yfazqb.com/Article/details/gwjxttldu.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gxgtjuasr.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/glyrbtlgi.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gawqnvszn.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/glhhmbwaa.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gstzbtyde.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gayygubqt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gnbfrulif.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/gqzadfdsh.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gjpbplnlb.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/gmayqpmox.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gkpysvvcb.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gishxrein.sHtML

JS:   static f() {}
来源：http://www.blog.tarul.cn/Article/details/ggmkthopf.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/ggbwyzdrf.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/guowhvyzz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gusmkgpml.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gdxajggsh.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gtqvwlqhi.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/guxjwlaxb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gybixmxpb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/gomghgjlt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gtipgybhf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gptpmhcpm.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gffabcjne.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gkhqafmum.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gifzvmbgf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gezfqflhd.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/ghppuzwhn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/glresnjiu.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gdrqvkdbg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/glrfgcrca.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gpuudzdsi.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/ggotrmceu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/ggliugord.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gabnucnzc.sHtML


<!-- 参考信息 -->