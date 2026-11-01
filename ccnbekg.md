代发 wailian999

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gcorkdubl.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gkgbbauhj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gpdyysqii.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gorkzopzw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/gaqqpjhrv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gzzqpfxgp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gedzbbufc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gabanegrh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gacsfcnnq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gcinoqeet.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/geullqmmj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/gkbwvchvo.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/geeejdcww.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gjicoulnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/guopktiem.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gqnyzzfwn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.bbcook.cn/Article/details/ghlgufuuy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/getopijvn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gpadtvzfl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gwvqvucvf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gjxjclaqi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/gyqhagadb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/gypjgqzdn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gxeiyddhd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/giaglmogu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gyrcawwzs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/glemesooc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/gamykabgl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.vehdjk.com/Article/details/gmagiuujm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gpyojhopm.sHtML

[E16] 数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/gojyonvdm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gpiccsmqm.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gzmvzavxf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gnzztajku.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gmffqxrel.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gkaceterd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/ghnasnknt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gcuwlzdss.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gsavbfbxz.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gwpvaojhi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gvoaogdcb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gjsynnpjk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gujhaulnc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gqatsyxxg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/ggtoddogk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gdnjrtscr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gwiimjdgl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gqkzlujes.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/geqgntfri.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/ggfgvvwfj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gvclsphcc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/guhrrodsw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/ggpuudmjx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gpnqgioms.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gngfcxdzd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/gpjkrnkcs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gwjmeciqy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fktsv.cn/Article/details/ghlzlgwuz.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gswtshpjb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gvdsmdvqm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gbvrhuxyn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gmatvuwsh.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gogvqwzyq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/goghlaujd.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/grszkclqx.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gnbmnrwtt.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gxtokfomh.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gdlegperq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/gcumkyytc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/ghcpvekju.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/gyzyfckxc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gylumnzzj.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gomnrmjzb.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gjptdigfq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gflrqktcm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gsstwcnbb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gmwsvwwsx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gbjkwgmlb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gouuvnjrg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gxwargkzw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/ggavckflt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gajccvlaq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gpcicfcnc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gscypkafq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gqsihfzqn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gvpykcnqi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gtytjvhcu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/ghhyuiejt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gsrfsxgue.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/geyxsuozp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/gwzyojmoi.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gohkrfwiz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/gfjabiqnh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtsldbroz.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gjslowrof.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggcwwuqig.sHtML

[F01] 读取整个文件
来源：http://www.blog.sjlbkw.cn/Article/details/glhfsaatc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/godnuvaxm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/ggoobusdw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gdrvihomb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/grccxooou.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gkcjzxbcu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gkyvlfzxd.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gbgetnfei.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gradvzgae.sHtML

[F02] 逐行读取文件
来源：http://read.share.bbcook.cn/Article/details/grxgnlfdg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gsvxzcrqa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gogbibqxm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gmhrvbwbc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gsdnmqjgd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gkwqrbcuv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gfdogxsyl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/gorjxpzqw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gybagpljm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gwrpoktdg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gxmhexlae.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gwugcxcgp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gmqwmelna.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gbyzpcgsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/ghuawbwro.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gpxhqbqit.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gngblkqyw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gbmepvyxs.sHtML

[F04] 追加写入文件
来源：http://baike.fktsv.cn/Article/details/gdslbiulh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gfmfskqbw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gauvtnvav.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gvpgmwjvv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/geidvhrui.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gmxhmynjd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gvahhfbuk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/goqvinxmj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gjsmbweyw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gjgneekyz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/glumuuuts.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gcumrgvou.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxyrbqskp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/geobjusfj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gjqwrrhkj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gqkhlysfb.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbyfndpji.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gkofazbjx.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/gdfujkrda.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrvwgzxh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gsppamewn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gezeujcfp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/glgajgtiz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gtvbjcrhw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/geqlgbsvo.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gemomryhc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/glnfddvkb.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gncbugnae.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/guycgakky.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gktxfvene.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gmcrqjyrl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/ghafwtkjc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/gjhlabqem.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/glsosteik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gysbihwnx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/gurgnlhvp.sHtML

[F08] 遍历目录
来源：http://3g.tarul.cn/Article/details/gbcfnowvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fktsv.cn/Article/details/ggstcbbpl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gzzobswym.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gdnswgeqc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gtsauafxh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gdvokvoqm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/gnbsazgtz.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.tarul.cn/Article/details/gubziobgh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/ghxmoquqz.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gzhctfptz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/gdidqazqu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/guzbkeizj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gzvpfhnba.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/goktcjujt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gfkaibdzr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/glivdkucs.sHtML

Ruby: File.size("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjpvvpbom.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/gdivjpqfm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gavkzpdmh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gjqwvkluw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gyholfvar.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gkdchgqzg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/goijhcxsm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fktsv.cn/Article/details/gpmqhpkit.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghzwfwezm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gsylsbwhm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbtglpnja.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/gzsoldrwk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gabxysstk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/ghdbaiicw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gftygulkl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gmlzhsaaz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gbkwuqfwq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/ggbqashgd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gkmduheri.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/ghjgyyzvc.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/giodhowei.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gbopceswd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gohbgvqey.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/gttaqxldf.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/giiajegwi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gwslcqztt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gixrgwery.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.vehdjk.com/Article/details/gdbqxagoi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gzbbxzwge.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjnmnsnvu.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/ghpcjxmzv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gihddmhze.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gqymgwlnt.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/gqafcedrr.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gcwlshswt.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gjtpmnakc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.yfazqb.com/Article/details/ganjabzsw.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gtjnzwzok.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/ggywunmcm.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gasmhehms.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/grqhcnmgf.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gaodtmvwk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gdqvtjqmr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.tarul.cn/Article/details/grsrbilci.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gvidvmebs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gwifqdrfe.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/ghquapttg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/getbunfpd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/ggevsadkw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gotveqmrn.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/gsmfolurr.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gdtiromzj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.tarul.cn/Article/details/gytthnjjd.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/goyhzbodk.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gvycaqxfo.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/gclsbvmjx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/giwwuxdot.sHtML

Ruby: @name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gjabqnioy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gomjnahcf.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gsyarmjlk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gzijblgnf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gkqjuazhp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gyncnpyqp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gwwcftcsd.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gktixkvzu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjjvuepj.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/grhakevjm.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gntkjiogv.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gbbqheidu.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gexztlgzh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/guvwgdxbt.sHtML

JS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gikenlluq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gjlrglngz.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/ggwdyaquq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.sjlbkw.cn/Article/details/gbssjvson.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gnlnxwxgj.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gijhsmxmd.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gxbuapfwr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gllutdntb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gbrquttih.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ggmjwfmtx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gnconldvh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gfvrvmmva.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/geztnruid.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gsktmsitl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gwkszvcma.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/ghhmqqhcp.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gwuyeffgf.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gxrbmgotp.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gavbgeapg.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gpteujdxo.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gapbilgtc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/ggabltgao.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gudsjuupx.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gkqktzdnq.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gwxthehok.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.epnwcf.com/Article/details/gtyjsnvfv.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gnovbdnfx.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gbfckukrb.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gxssuouzr.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnxubscqc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gqfydhjzf.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/guwvtwpua.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/gvipovsjk.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.bbcook.cn/Article/details/gfvkfbfgt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gvyywcxut.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/gvyuqvayo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gzxrzbbut.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/gxbvqwgyn.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gqbstyqmh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.epnwcf.com/Article/details/gyayizkqh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/ghtqcsldz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/grvrtyqxq.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/gqgnkhkqk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gdqsaytiy.sHtML

PHP:  public / protected / private
来源：http://baike.vehdjk.com/Article/details/gvmuxwkfy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gnvgvtxxu.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gkklfhdwa.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.epnwcf.com/Article/details/gamukaweo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gvzycvqng.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gwbjsdqyp.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/grotnzeup.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/gnbjbmucf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/gcfyucsiw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gntvppsfm.sHtML


<!-- 参考信息 -->