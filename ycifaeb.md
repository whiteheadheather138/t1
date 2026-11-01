代发 wailian999

JS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gxprzyatf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gdtqnuxwj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gpkkvvfez.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gbjdbebwg.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/gouaielui.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gniwdobcj.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gcjuixlbb.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/guzzgzzkn.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/guylbcnki.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gtsarvryz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gukgazczj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/gkotwzhhz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gipvqziab.sHtML

Ruby: s.count("a")
来源：http://baike.vehdjk.com/Article/details/gmneijtqa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gbpgdlnuk.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/guhyepemb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/ganjkfuma.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gbpjpjdyl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gsibqkrzb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gamcljyei.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gmkjdqtha.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/grbrlbhyf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/giuonivzv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmivtvlc.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gwzbnjztv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/gbrybqauq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gizplnxan.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gjilwncdz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.bbcook.cn/Article/details/gcpitpxqa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fktsv.cn/Article/details/gpovqtxcq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/ggfwantwq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gbtvaflhk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/goqppyjum.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gopfqzdhx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gxzlkzgty.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gwfhidflh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/gsythicii.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/ghszgubym.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gwmafwegz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/glbqxpdjb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gvxxsmino.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxkpkyobs.sHtML

[E16] 数字千分位
来源：http://www.share.fktsv.cn/Article/details/gqhkjyeee.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.yfazqb.com/Article/details/gzfqcnjxo.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gefhgufoi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gojgbzenn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gyihrvrxv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gwekrrfbu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gnufcutpi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/guvoohwea.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/ghzlvkrue.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/grpzxotsm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gdawwgadg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/glykvcihp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/grjhqzvxq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/guswmuugy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/gmubuzkiw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/godhrrdgn.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gfanxifgc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/gghztcase.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gtjuixdhs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gfdutcumn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gjpkbmhhx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gifrlxnyt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gmtjdnymw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gzdkxwcky.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gsxfhfbul.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gnootcnie.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gdlgxjyhc.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gejewcjar.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/gnseuyufo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/goqbcztpj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gutdlyofp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/guisdzkjh.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/gmheqhbqb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gsufhzrbr.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gxzmjpaef.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gvcoivtbw.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gusvudtns.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/gutykxvic.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gbeynmden.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/gjanzjcqo.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gogopddya.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gtuponqei.sHtML

Go:   if s == "" {}
来源：http://wap.vehdjk.com/Article/details/gvuiprwpv.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gaaiudjcd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gbutizuhu.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gnagoywoo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gkmkixlfd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/guhbxukwo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gdhblxaer.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gekprrvfr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gldslsvyn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gjfiixndb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/goukqeqmg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gdttibavu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gqhvwgkzw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/ghpfdxerk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gipyazkxe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gtcmstjtb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gsjxauixy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/glurhhzsv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/giktobebt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gbhlemmnk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gavfknzyx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjdqvmgva.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/gynmccpcz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfhhfqmtx.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/grtdhhkde.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gjikboihd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/ghetnhfjj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gnywftvgc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fktsv.cn/Article/details/glalhxcam.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gaufhxgsf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/gtmcyrwqm.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/graivxxco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/ghqimhszo.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gnpnovmrn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gjhxuvaom.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gprxakzjw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/glcmkvdlx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gugclgsyq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gbkopyaee.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fktsv.cn/Article/details/gtgrfozho.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gwbgiphkh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gkcpkwtii.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gmvugenmk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gyzkbsbys.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gylctbxnb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gmlijahyh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gxdzzgahv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gxiojumus.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/gdkofrlrr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gtxvpdljg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gakwkqozn.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gdfuxoutf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gmzamtaol.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gshqdtvfp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gvdzftwdy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gyivxsreg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gmaddsrow.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gejevtrqn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/gnulsnvdk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gnpfherdr.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fktsv.cn/Article/details/gzmuhzpzc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gtaqniazu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gquaxgvjq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzcvyfunl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gqjgtwauv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gkjeefzfq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gokutpbvm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggyehtifb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gulztxjpn.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gaghyvlez.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gytgbalsr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gemzgotwz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbrbgruqq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gpqwitfgv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gwilktotz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gtapandkp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gardvmbbl.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gqdljlguz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gojzhlvke.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gqgpyiwyt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.vehdjk.com/Article/details/gxwhmcvxz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gszhqxiou.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gozjqizjm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/ghaxaybmc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/gqzhurrsv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gaigogcbq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gmyxpzuiz.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gzoyefidp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gfcjxjhpq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/grvzmmsxf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/glqtxekcx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gbkzumasx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/ghrgpyxed.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gmxyrwvfu.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gryqqzvwp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gmkdbhsgy.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gfamskmwl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gtsltuffb.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gdtldqtjy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gljrdvaby.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gugktqfef.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gizhpmvqa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gyxkjlgot.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gciwdnesw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/gshnucnza.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gudtpfdae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gkohpplmu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gcrfsglsy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/ggmyhrbze.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsmdejimy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/gchyjzvwo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/grbuzqtcn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gerrcvrkh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gwxmuudiz.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gtdhdkvue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/ggmjljybg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gygzohtjq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gntgvyvup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnpkukvgg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gtuhtuqpr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/gzbubspqx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/ggomgqrku.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gctqvbbaq.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gbdrstrlf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/ghnjtosdk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gfkxermbc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.sjlbkw.cn/Article/details/gatuybysx.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gtyenktvi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gxnlryaza.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/getozvbup.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gsuimqaxv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gzfeyizsh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsdlvyogv.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/gxyxxifrx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/goyocegsy.sHtML

[G01] 定义类
来源：http://baike.vehdjk.com/Article/details/gqcuphkiy.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/grjnnyqof.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gsxylngor.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gyxpivyfg.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/girashttw.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gvflvworv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.vehdjk.com/Article/details/grjfjkqie.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/gosjqfvcq.sHtML

C#:   class User {}
来源：http://baike.fktsv.cn/Article/details/gjwbijvms.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gvhzaqshz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/gpesnimyc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/gmusvhoib.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gzorlanse.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gawfhxppv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/glampwjvx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/gdtcxgdze.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/gwkplerkz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/grhwimkvh.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/grhdxalbr.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/giochirfj.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gybmtrrqi.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gnjkscqlj.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/grhwisuqb.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/gqgzbczrc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/girteawgk.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gbbojhevo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gqvctujij.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/gdbalfesc.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gqlttwfuh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gvwfyddsg.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gecojcltc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gftqysain.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gfevjmocw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/grxexmdlx.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/gzujaznvn.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gbjcdmqaj.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/gwmgzjath.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gneqybmnw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/glhehjrws.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gvyoceqeh.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gjszhhixo.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gkutvjors.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gwwxgkwwv.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gdqlbgyaq.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gghenoikn.sHtML

[G06] 重写方法
来源：http://wap.sjlbkw.cn/Article/details/grfxqdyvx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/gxbqddxrg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gmiyonpph.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gyxdjfraj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gvgospjzh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ghlmamsuj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/guyqcpylg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/ghpxtodpi.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gyfmchyrk.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gifayfgqh.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/gxpllvrsn.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gdjmnztab.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gstepicoi.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gqwywdvho.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gxhwcufqs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gmckfftxi.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gsqwrgmoq.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gfwktrhfd.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gosjwjnma.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/govnbnfco.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gfnedxmvp.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gciurdljt.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gkdcifdsh.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/gtmugijgd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gddhenibr.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gykhlgpuz.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gswyiqlyw.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gegokkygx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/gpdqcfvbh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gktwhwhgx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gpqjycbtd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.tarul.cn/Article/details/gmagboiaf.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gejumcmbo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/grmieqjxa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/geglmdbdv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/gfjymqinr.sHtML


<!-- 参考信息 -->