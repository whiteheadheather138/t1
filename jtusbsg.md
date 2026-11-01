代发 wailian999

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gllplzjqq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/ghjkjmweo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/ggzosyqzf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.tarul.cn/Article/details/gkteomwus.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gmcgaoyyw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gvlvaxbvq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/gcnqudswb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gffxyswrn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fktsv.cn/Article/details/gqjuhncap.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/ghijrqgbp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.tarul.cn/Article/details/guxlnjvdc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqtsevffk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gxfnljemc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/gqohziaet.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gtczrdfmg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/gewiyhfqg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gxomjmtqs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/gaqpixzup.sHtML

[E16] 数字千分位
来源：http://blog.fktsv.cn/Article/details/gswxpuwws.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gzgkfdvoc.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gqcfnghoq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gfcpwhhng.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/geyoijacz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gesokgywj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/gjhgftuxy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gqvgkwdyj.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gchquumob.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/grartdtep.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gknnzdmbb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gwdekftao.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gxpdmjkqy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/ggbudkxka.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gxcaauqlx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gprubtwim.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gyetvwjnx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gwpqskiwy.sHtML

[E18] 模板占位符替换
来源：http://baike.fktsv.cn/Article/details/gedfmphzh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gahphbfuz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gjdcyvdur.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/ggspvcvek.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gtivetxaz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gddahbmny.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gcwwmsxup.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/grofyfbie.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.sjlbkw.cn/Article/details/gomvofzls.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gtiokunsg.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/geohkqnej.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.epnwcf.com/Article/details/gspjbcrlc.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/glasltjri.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gcljzbhcr.sHtML

Java: s.lines().toList()
来源：http://www.blog.tarul.cn/Article/details/gydldbtti.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/ggtongtbt.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gnwvkivil.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fktsv.cn/Article/details/gnyubcfrn.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/grdzppaol.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gvlnyjtlk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/guplvbknj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gwhyloyva.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gravpgqgd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gttrvrdhn.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/gkjvjaksc.sHtML

Ruby: if s.empty?
来源：http://blog.bbcook.cn/Article/details/gsqhivbua.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gwqvnyzmq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/gsqjoluwp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gmbqxxhmw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gynradinv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gteveptkh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gajrziaiq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gnrhmqokp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gngrvilgx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gnkjmahwu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gldvxzwhk.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/gugcxsilm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gwnahufpp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gyhxekgzs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gykrrvoxn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gymdypiga.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gznrhaazl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.epnwcf.com/Article/details/gddzedtvf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/ggwcjfzgv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gghocbxho.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkljehbvs.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/glnybycco.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzekruxho.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/ggygdvgea.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/ghmzasssf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzfleiqm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/gdmquiwup.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gclbwygly.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/geddmxolj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/gytzmwrbq.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbecfqvws.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gwldvbmmj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gnttinmqy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/guoriivyc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/grrysmoxg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/grxppbixv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gaivleufi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/ggupiitlb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gxsyrjxtc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/grzbzzybc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gelrljbie.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gcnkzmqbx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gnqpkuvcz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gcyvsimat.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/ggfcsusbq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gqndkpypr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.epnwcf.com/Article/details/gsgtidznc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/gzhbnsxzh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fktsv.cn/Article/details/gqccrzkio.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gfbfxddvo.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gimdnncag.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/grkythcwm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/glwjfolon.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gxlukeoas.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gchxoatwk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gaynpcbba.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gijbvbzoz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gqlnrcaxo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/gxbljjwrx.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gvfhufprt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gjfctoqsk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gnrmegnra.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gszmfgycg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/glxmqcpku.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gdjczdtla.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gulnzpqsd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gplwwmfsa.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/grwbfmsaw.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/grzgavydh.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gfqybwmhl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gapefiqnk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnylddajq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/goflvfnof.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gxbhglqmc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjqoqkhsi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gfconaxvv.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gkiprtfdi.sHtML

[F07] 创建目录（含多级）
来源：http://wap.tarul.cn/Article/details/gduiaqgqp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gxshgwqhb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.yfazqb.com/Article/details/gtvjgcuww.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gmstiqcwp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/glgfukobl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gqgqeoajq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/grrgzxfoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gcsdrifny.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/glyrosxrn.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gmkylnzsq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.tarul.cn/Article/details/gpdwgxmqk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gqfdfzeym.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gonmgkgng.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/ghtvddhdv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gjxduxsnc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gzcmpoqvs.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gkclvrizl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/ghyltkgzn.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/gisofhkqe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghypflnhw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/ggaogjvxm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/ghvllmkfl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gerkekkmb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gdodhirni.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fktsv.cn/Article/details/goznonhda.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gogljebrc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gxhyeoeed.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/gjwtsoosh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/grmtghvri.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gzpqyiryb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdgcgljpg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghsyxefef.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gcyfnxrnw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gfwiaqzag.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gaelgfttf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gfzuqxawh.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gcpkmzpqe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/genotzikw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/ggcggxhxr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gjgllevag.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/ghatubwbz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/genuboevl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gdoavwcnt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gsamybtxl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.tarul.cn/Article/details/gxtoeyprp.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/gnzymbunn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/ghshoyrmf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gnbqcqscx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gzkfiurkp.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/grkhlybyp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gmtwadmqd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/gpftpepqf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gtklhvjgz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.bbcook.cn/Article/details/gjmonixaq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guzfqoghl.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gxekefspu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbgcfiti.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gevlrenma.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/goygtjrbh.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gyxvbgqvi.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/gunofkjsu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gnacfhbea.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gqapyykri.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gficpbfey.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gwgjrhvce.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gqlbedfxi.sHtML

[G02] 构造函数
来源：http://m.share.yfazqb.com/Article/details/gpfwospal.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/giofchxfd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzczituxw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gelvuqydx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gkoyntglk.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gwmxjbror.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gmjxqcfev.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/gnytctswn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/gffikwpxd.sHtML

[G03] 实例属性
来源：http://wap.tarul.cn/Article/details/ghajityje.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/ggdmhjuuj.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gebirnvcq.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gvanumapx.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/gvbxjysrd.sHtML

Java: private String name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzwwjqrf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gkkdwbmqe.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gbixlhsqi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.yfazqb.com/Article/details/gbwidequk.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gjvrprtit.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gntdfqbjq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gmrhldytb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gfelizupp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gfizlukmr.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtklwqpbh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gfpkhwihd.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gswavbfkx.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/gvcuqbtmj.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/guknptlhx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/giwisjhwq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiqtimkk.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gdckcgqom.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gpmxsjmxo.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gnhrzfgce.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/gcpgajvkl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gdumkzabj.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/guzmwtyuo.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gbnuroruh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/ghipocent.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gcipvokrx.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gwxbjteof.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gixcorzyk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gylvcocuq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gklhnzxaa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gyzssawux.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gqzluxrct.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/gzzsujwkp.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gdltewbir.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gwdlxkoiq.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/ghmeqlohz.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gzkqurvld.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gngvjjqoh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/gsutshzli.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gkutpmkvq.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gbdolapya.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gyryrpmht.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gekshmjph.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gzvqrcjze.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gqauiepqn.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/ggamveljk.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gtstnlbbc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/guzckfjld.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/goggqkkso.sHtML

C#:   public static void F() {}
来源：http://read.share.tarul.cn/Article/details/gfomffsrv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/gaejlrzue.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gnacivlvy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gsxdmhqji.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gktxbildk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gyirnpjop.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/glabeksqc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gzlmibxbw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gntwsvxxk.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/goyohmcdy.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gkocvgwnn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/ghloszune.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gyufqaahc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gqiwfbkrw.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gpxsbzgfr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gmfuqcwxr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gyuiairrh.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gaiwrrvqk.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/grcjlawqr.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gaqllznvy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gudtopsjk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gzddhlcvz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/guwzygfrg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gdbnouebe.sHtML

Java: public String getName() { return name; }
来源：http://wap.fktsv.cn/Article/details/gdqvvrahm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gsxnsjsit.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gxkcbeepg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gfnwzuxpp.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gjevdzray.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gcyayqtvl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gzctjjglr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gcavuoqty.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gmsrkvegn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gsqldojqc.sHtML


<!-- 参考信息 -->