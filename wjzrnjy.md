代发 wailian999

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/gnwgqypam.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gmjeykfng.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gcdyymppu.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gndckffek.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.yfazqb.com/Article/details/gzsmgrzhi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gmvlkxtoe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gccuparks.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/giskrlmrc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gsavtamxf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/grklitmfk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/gyyhorajh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gkibcneuq.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gkxaifnwy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gfekotllo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gvbkmwnhb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gfeklksvi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gczbvnmxb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/gpsedhzxa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gbubdlizg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.vehdjk.com/Article/details/gukmesxaz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.bbcook.cn/Article/details/gtcugwddz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/grgacmfxu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/goqsuvmgx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gamkheuoc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gjpzxgtns.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gjmtisurf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.yfazqb.com/Article/details/goqxpzhof.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gojjwtgzz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/glffknzwc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gaugmyxan.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/ggmpjujok.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/grwpkdbbx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/gdfevjenk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gvloxnmxs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gjngbvzby.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/ggezpqwgg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gehmkhahn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/guhhpscjw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gmfjeiqax.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gbcdrgsvf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gwgcmxgsy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gzxjncpzd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gmbkwpycf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gzzaljdgl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gwwnhgocm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gvlrfhqfr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gfgmbtyla.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/ggztcypxo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/gjnlxoljz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/gugledehn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gjlwoaeyz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/giftxdboy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gtbzltwxf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gopiayodc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gecnyddts.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/ghbyhpnwt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gqhdtwtdt.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.vehdjk.com/Article/details/grmzeyiqa.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/gxrvoedpl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/gevjpjqat.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/glgjbtfvh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gkmmurihn.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/gsadghczb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gvftwrarb.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gaeianrce.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gkcnplhnt.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gdqixcwsz.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/gxrykgumb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gcznputin.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gyhgyyfxt.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/gxgxgoyqg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gnjtvgkwr.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gbfcqxacz.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gzpvkiytk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/gvoxgpsbd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.tarul.cn/Article/details/gbutfulxs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/geyktwnoq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gfgycghcp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gztjlwlay.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/ggjikupiv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gjwrjgigw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/gyxbxiiss.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gdnoqwuoh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gdaircgkc.sHtML

[E22] 字节长度与字符长度
来源：http://blog.sjlbkw.cn/Article/details/gdbjmybyb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdxirutfu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gfvluxflw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gkktfoppj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gxjrmcfyw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gyqxqnctg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gtrrmflhe.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gvpxzmstz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/gyicvwcea.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gabhnillw.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gklpjetoj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glsqathks.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/glhhusiei.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/gozhtnvmk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.tarul.cn/Article/details/gwvlebgri.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/gtvtrqxfr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gskzdnyqd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gblyehiwt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gbpnougkf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grjmusdwr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvwxjetbd.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gatsezipz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gekoewcpq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/gyzbcvteg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gxtlnlqwe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/goqyeynyb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/glikpnyqh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gfpgjjhgh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.vehdjk.com/Article/details/gxijkdsyj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/gaqjbktrn.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gaafaentb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/ghaujaseb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gbpokvavt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gxcddmfri.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gmghjxxer.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gvtemidhn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.yfazqb.com/Article/details/gjryvidew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gcirlpayf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gusvxxykm.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/glcvriacb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.yfazqb.com/Article/details/gdiwyugry.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gpuubupdj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/glzmgtzaw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gkbvuzkey.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gqdaxumre.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gyxxcjris.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/gyibpfazl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gzsyczbur.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gxyhsgitx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.tarul.cn/Article/details/gzlglqgvu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gdczzkdfq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gxzcjqydj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gqqyhudhp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gmezeiuxb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gdkjlbzwz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gdnwgfcqa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/getwfynqy.sHtML

[F06] 删除文件
来源：http://wap.fktsv.cn/Article/details/gvqnwxocm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gtanbnnha.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/gpqhstept.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gzencumfb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gqainfvqx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gnzilgfge.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqchhyxqk.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxcsgwigt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/grwajetvw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.tarul.cn/Article/details/gmmghumjg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/giguobdgt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/gofkyzihw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gdyjdyuaz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gulnjfyhw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gdsyzxigp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwobichso.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gdlterioa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gvbkfiixi.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gtypkxtma.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gafhxhdae.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gcxcicdri.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gxybuvlgb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/ghbvadbnl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gzaijxgqa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gjmogndsp.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gtgebpryb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gkvrzvafv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gjschfiuy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gntdddhrj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gocbbcsnq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/ghgscaqsx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gnordqrvk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/grufixymm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gcmwinqxo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/goavnrone.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gktmvyxfa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gbnstujtd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/ghmaycnzy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gvohkwpzh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gymxbndai.sHtML

TS:   path.extname("a.txt")
来源：http://3g.tarul.cn/Article/details/gjybjtvgn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/ggsnvjwrv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gvnbuqbhl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkbwpkznx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gwaroqwaf.sHtML

[F11] 复制与移动文件
来源：http://www.share.tarul.cn/Article/details/giebicvae.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gufuwhiqv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gmidmtepg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/goviqwrup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gnmimbfrf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gatjobzwd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gfezhghtu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gheudgwil.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/gdlnbazul.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gvkmsregl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gdhqofagk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gewuvphjl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/ggzesoexu.sHtML

TS:   // 同上
来源：http://www.blog.fktsv.cn/Article/details/gpnpkmozj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.vehdjk.com/Article/details/glketbssz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/gvxnxhjkb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/glhddkvks.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gtzszmwyu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjiiqkymh.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gtkgstnaa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpkyypnwl.sHtML

[G01] 定义类
来源：http://3g.fktsv.cn/Article/details/gdjpgwvnu.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gcirvgtkb.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gvykhqvog.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gpslaqxew.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.epnwcf.com/Article/details/gsywkygaa.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gnknigprm.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/gjnzpcvdx.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gvshxcldy.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gnpdfrxub.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gaeaywdsm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.epnwcf.com/Article/details/gxchlicay.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gckuzvmrz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/ghkqlfxpu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gurkytywk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gmlvzrgep.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/gtbbsirjt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gfpnsrdsc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gjomwjvis.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gibwrrteb.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gubhqhssc.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gpnjpdpud.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/guzuidmhh.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gbcemiwcd.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gzhtlbcbf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.vehdjk.com/Article/details/gvfdhbxqu.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gmgzrcjeq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/guuzfqven.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gsqedkdcx.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/geakwukex.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gbglsiiys.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gpzkticlm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gdivxagsz.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/goexizwea.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gkzzbhrdu.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gwyjxmefj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gnvglvpjb.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gdbsvydpw.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/garpqeznx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gponemhiy.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/grfpgvtrt.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gcenvdlet.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gxjtktltu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gfectlojh.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gbuxnphok.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gjbzcotsu.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gwbohnaqr.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gplobuman.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gxnmfcbik.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gqofnjrfx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gevclhcop.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gnnltqnem.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/guffugdgp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gcosmqbvl.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/gcdkehwpk.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gfdoupjsa.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gogbpikxu.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gfesavvoz.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gbnhykkok.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gnizsvqod.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gtcmfikjz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gsqaelrda.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/gypyetnuh.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gaclqmoeu.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gdgnentlh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/glbwcqbow.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gigvzhdus.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gbaucprdr.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gtluijksb.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gfroqbjfx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gywqwaxkl.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gzovftylc.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gtsbbkexg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/gmthttkvv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/ghgbvwkyp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gufhycswf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gdhrufovy.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/gkbtxoipc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gduvidlls.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqvkljla.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.bbcook.cn/Article/details/gvxuvefey.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gxpbdetvk.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gxsaffjim.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/goampcltq.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gynarfwgl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gfownhcxd.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gyqcrmmzk.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gvustbxnr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/glribaoko.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gmegmnqas.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gdxtavdwo.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/ghpzqzpnt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gwupqwecu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gmubusbkv.sHtML


<!-- 参考信息 -->