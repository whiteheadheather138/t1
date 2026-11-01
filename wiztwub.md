代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gpnfyiaqg.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gkdlkfkxg.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/guhbxptje.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gkuhkjvra.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gcrnkbbxe.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gqxjtafjn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/gclkqusnj.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gqvoelfid.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.bbcook.cn/Article/details/gfzwyjuyp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/ghyxccivo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gacnnoaby.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/glzrewbzc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/geblkygim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/grbjxazrs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gbmbbaere.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gwqnukkrf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/guqrfwbiy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/gsowhdgbp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/goxuxdmhl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/ggjpbhcga.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/ggzhzsbwz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gykfynqog.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gmcbbnyxz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.vehdjk.com/Article/details/gnsfeysmt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gkeozwjiz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gwobgnkcz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gttvcgjxt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gwzgqzgcj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.epnwcf.com/Article/details/gjdhlalxs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/geamduttg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/grlikrcdh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.bbcook.cn/Article/details/ghhgmlysp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfltqdwsk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/gvapphgjd.sHtML

[E16] 数字千分位
来源：http://baike.tarul.cn/Article/details/gtgylxslm.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gtlrkbbzp.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gzijpmkuq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gfgcsmonm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gnjjdhuar.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gcrcpqmzs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gphcivrzn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gdghthcck.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/gahnnutuy.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/gggenlcnf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gukfeaviy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/gihbpuyqo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gtzymibet.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gdsefvaka.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gzugmgicw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gjwrljewp.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/gfiyfplwz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.tarul.cn/Article/details/gqocpbmro.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gzsdlfmid.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/gdfzfrjiz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gukbugtpr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gashopoma.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gusztwxgf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/glzzcstma.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gpygybvtl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/gjkywkvoh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gedizyyxz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/guarpmotd.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/gdfiqnfvj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gyrnzstlk.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gtkmfnhqy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gkncbeupi.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/gkgyjmvmq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/gxcbktyzl.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/guufgpaav.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gwpsxsasb.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gskfcwafs.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gzvsrjead.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gaxwpxddz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gvlegcvbm.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gavtxggqc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gczjkeirk.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/grjtfughf.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gdwsvsrod.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/gxzljlzud.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/gcdwgvjkj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/gondlxjxt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/goshsqajf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gclahbjpt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gfaxdodlk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/goimtrqmh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/giwefncmd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gphrtogek.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gzxexmkza.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gzedpxmia.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.vehdjk.com/Article/details/gffzkdgrl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gwcmtaamo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/goiewyzjb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gyvkzhlhl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/glqkzwkae.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gerotxbme.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gdagsxyss.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fktsv.cn/Article/details/gozemujho.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfgheinzh.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/gbafmkole.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjqckhncc.sHtML

[F01] 读取整个文件
来源：http://mobile.bbcook.cn/Article/details/gwlgujkzi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/grawymtgo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/giqwdjrbv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/ghciwvryx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gtrzukqwc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gsxuqqbgl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/gpxqwtnbg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gavnmxkir.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/grjkoilba.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gchsdoykj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gljvxords.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/gtvnmwjbo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfuqxaifn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gfzqnmnue.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gppairxqj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gbbdeaowv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmeaylrs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gybuivrev.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/ganvajodl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/gumpzvyzx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gynikewcn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gfrdoawhe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gqsqhbbom.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.vehdjk.com/Article/details/gezsvjznl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gqqvumcqf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/ggkdfkgur.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gwwuemavz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gnpbmsawb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/goqhytohc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/glalmlcmt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gpvrgjpjo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gofbzeqtr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.tarul.cn/Article/details/ggrtpflbv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.bbcook.cn/Article/details/gdfxtfltg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/gnayofjba.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gkbddsnch.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gzhnyoqcm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/ggaenloxl.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gedbrlcbr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/glcirmuff.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gqdtcargy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/guplrmzka.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gfmtcgzqi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggctgrokh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gthngqmih.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gmbviwenp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfnymmoac.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gonhbtdoe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ghdetvobw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gpvyekmgh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gnxmwhlba.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxehexseb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.vehdjk.com/Article/details/gontpigrh.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.epnwcf.com/Article/details/ghufvderm.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gzffgmwxl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gnubjmjoc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gfuihpbwm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/ggpjuqyte.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gnwubhtyl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gakawswzk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gsuissiuu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/gyazepsgb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gixyvxgev.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/gkcpftskt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gvxixymhy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fktsv.cn/Article/details/gsxugwdwb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gfwgxgmpd.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gejffhqfy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gxpzezzns.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gyxczienf.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gtxlomowp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/giilgwpfa.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gwzgqhvez.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gemkxajxw.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gxtsedtnq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gnkiytspq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/guqptkjmw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/giwuxnwug.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/geaijyslm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gsbrlsdcs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/girmxyrjr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gqkdajocg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/guajjtwyo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/ggjwzytss.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gkuyyhehn.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gitmfmqul.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gsgwgzund.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gwhtaywqz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcveylvxi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gcsecbkrq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gnudsmxqe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gclnhdwtr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gsjryycbp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/glpduabre.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gkfyypiwz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.tarul.cn/Article/details/gsjaacrfl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gpibstcqc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gsqidikmr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/ghtoqndzg.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gxmtsasul.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/gnpmqibky.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gpycbvawx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/grwxezguk.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gxhhrikqf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/guxyfeuuh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/grkqbzlel.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gsbruwlvk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gawlinyvs.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnzngnwej.sHtML

G. 面向对象
来源：http://mobile.vehdjk.com/Article/details/gzdwfukgh.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghbecscqx.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gjptbnoem.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gfryzexzx.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gvzmkvelm.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gqikykbqq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.epnwcf.com/Article/details/grvbcccfb.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gnantzxnp.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/gnqftnyxg.sHtML

Ruby: class User; end
来源：http://3g.tarul.cn/Article/details/gqopkxwks.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gduujksen.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gsejsrgjm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.bbcook.cn/Article/details/gncljxdau.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gewrnrshd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gfmqpvsoo.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gorppnmkb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gtknkbgkj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gscnropny.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/ghdomjjhq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/ghfrjlbls.sHtML

[G03] 实例属性
来源：http://www.share.fktsv.cn/Article/details/grxyjirnv.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gqyyitsei.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gjnblqqps.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/girkwayzo.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/grudftuzt.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gfcflhsec.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gmapgfrxy.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gygwzaloe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gvzaooomr.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gndykfzqe.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gosfgetcw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gnxesioey.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/golrkgdls.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/grepnbhgi.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/guuedpmzh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gvabijnsc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gtleugfnf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.bbcook.cn/Article/details/gkzmfalgp.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gdkmdaryl.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gyormeago.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/ggxgsfuep.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gbrbyhnpn.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gnobawovb.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gnhqedwzv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gvmkfvigo.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gwmvhazsq.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gkmhhllof.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gzxnykqur.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fktsv.cn/Article/details/gnoerzewd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/grxfydxez.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gnjjjvjyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxwzwnhuj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gxnhislkq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/ghbbpwquj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gjuqipjpu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gblvldslp.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gmujbcjzz.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gupnxstce.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/glfupiqtp.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/glbuqafmq.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gnuvsnxyf.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gdbrtxsqt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/goaiouhym.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gllpnrdow.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/geudqkuyd.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/gdbnqerta.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/gdmqavtcg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/gaykphclr.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gypjjanze.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gxzotuzww.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gcbnzuzrh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/grozttvev.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gohuxegbz.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gzfghyntl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gzdvitwll.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.bbcook.cn/Article/details/gygvbtcup.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/ghzfbazdd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gsrmzfqnm.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/gwfmgtzcr.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjznhtsgu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gkdqahlme.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/gexooxaix.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/grfybgedh.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gxxgqxuyv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/gslasaodj.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/ghzejswpr.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gegjkryje.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/ggqlmrqun.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/gufofwawr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/gnbunrxmt.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gmdnafsqn.sHtML


<!-- 参考信息 -->