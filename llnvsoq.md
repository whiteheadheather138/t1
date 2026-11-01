代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gjgcspyvi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gjuswmxsl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/gavrpjaer.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/gbwddjxib.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/goaegvoxz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gnhkghyxm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gkaednxdi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gvufqaebo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/ggrjdndmw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gomtdwszo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gabljepjt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gneselicu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gfolochbj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/gojonrtts.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/ggxogciez.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.vehdjk.com/Article/details/gaghqqfdr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtodctwvv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.yfazqb.com/Article/details/gxcvdzszh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gziasgknt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gxcmzisgh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gndzrpwmy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.sjlbkw.cn/Article/details/gzsfsxrmq.sHtML

[E16] 数字千分位
来源：http://3g.bbcook.cn/Article/details/gkioldodb.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/gkxxfvhgb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gxjisaouo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gjguogicl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gyeakbrjp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gtzanuppj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gbwrlhhoc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.bbcook.cn/Article/details/ggbhxdmvs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.bbcook.cn/Article/details/gistthceg.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/glxrbmwln.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gelfkvoyt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gujlitbqp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gsvtjjqmm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/ggachfztk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxuhbtlqz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.epnwcf.com/Article/details/gxqgcfaun.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/gqzcmpmrv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gzlpfliqw.sHtML

[E18] 模板占位符替换
来源：http://wap.yfazqb.com/Article/details/gusydexbn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gypkwzims.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/guqusnhpa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/geibxggdw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/grccpegif.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gavlmvznp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gmkfvyngo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/glebjtbhr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gwxmotbhw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.epnwcf.com/Article/details/gpzzorucv.sHtML

Py:   s.splitlines()
来源：http://www.share.sjlbkw.cn/Article/details/gvfncgzru.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/ghkqiwgxj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/ggvprvxtc.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gnqlfegia.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/gsiykhzxp.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/gfbdojvvo.sHtML

Ruby: s.lines
来源：http://www.share.yfazqb.com/Article/details/gnhcygcgb.sHtML

C#:   s.Split('\n')
来源：http://wap.yfazqb.com/Article/details/gxlikpgbb.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gjuikycdz.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/gixkucivt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gkhwyxqlh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/gafbuvixy.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gkvpdorxr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gyphghsgg.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/giprvjxpl.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gjjuwptxc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/glyaohfqi.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/gfmdgcxfu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/gzsknphaq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gszktshpr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gjbsrtcmv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/ghtjygbtt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/goafwnmti.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/glttwxvzh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gzmyhaglk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gkiwjtirg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gaskcpzdx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gkwtmbara.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gszjrwqbo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gznaatsqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gekksstfa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gmwvmkveh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gvdnhizkq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnadpfqg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gfpbjnakp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gquaqhbiv.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gvgzmcgwd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gslprukow.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gonywbhmi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/gjynolldd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gwiuazjvd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gwpmbxomo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gshunnlkd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/ghjvdnsco.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gwmvvuxeh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmygwztce.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gqjabmzdr.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gluunpypw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gwrroqzds.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcvbosnw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gtufzjwew.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gjyvovmfm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpjpmqlg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gelwlmuvu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/ganytubwy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/grhbkzcww.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/geinqknjk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gpzrgngzu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gkaftaqva.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gefanqyhs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gmgjdzucw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/gstalzdns.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gbikzyadz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gunevofvk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gfioearbh.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/gemadjokg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gfeaktrlk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gblgmoiws.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/ghtwynbmb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/ghhexwour.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/grgkcwqhg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gsjwpivpb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.vehdjk.com/Article/details/gocnuvqov.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gsnajteis.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gswbdwhui.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gnwpiandb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gdlnuwaiv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/geqhdqobx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gcgyxzrlr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gcoebthqp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/grvptdqey.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gcjedtrtx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/gfrrldflr.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gwzztskge.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/glxafzbke.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/goblxyucv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gcpzthyvx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gjhzeowfy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gfjsgtutk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gfaxfxjui.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtwwooqdh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gfdvxoaaq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.vehdjk.com/Article/details/gjmsvtnwn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gbpsmyhsq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gdjtyivso.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gyjjftjqu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gjllmcoej.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gyalbsybi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gebrigqwx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/ggheleksj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gdymdiqrp.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/ghgekzjlf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/guemusdfj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gmivnympv.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gkghzyxid.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfihixzxd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gsnjbpkpn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gprjfbbpg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/grfzvodpv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gqcmpotea.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gmxouwgpf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdkmmtjeu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.bbcook.cn/Article/details/gsxaberoc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gnqdyooxo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gevmfcvbb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gecdrxbra.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/gqhjpfdbu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcgmxwxpf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/ggiqtjajo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gmxdmeeiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gqgldkocf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gbouefqlc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gzxyuaxzf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gjikvafji.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gwgiyewwh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gshijqesy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gayfklnbz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqsefoejk.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/gbqsoaide.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gjedbtext.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gqtgiccjb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gqhsaejnw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gmqfuorrs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/ggrhyxzso.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gxreruloo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gigcbixpu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gxabllwie.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gwkgwryka.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gwqerxjqo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fktsv.cn/Article/details/gwvabvnfu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/glxpxadgu.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gkrbuwhqp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gmhxjcjjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fktsv.cn/Article/details/gnumegxoq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/ggccqgrmu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gpbnsfddh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsxxwupdi.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/ggfofcnbo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmnbpqfry.sHtML

[G01] 定义类
来源：http://www.m.share.sjlbkw.cn/Article/details/gxncesuqd.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/gfjukgblc.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gwoxzygjj.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ggjtxlzqi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/gikppiagr.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gzsaovyhw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.vehdjk.com/Article/details/goupfpqml.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/gudojnpox.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gqmxqdgca.sHtML

[G02] 构造函数
来源：http://read.share.yfazqb.com/Article/details/gikpmdwap.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/golkcbrzk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/gqvlxzsky.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gumzxfvff.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/ghjleiupa.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gcfpzrowc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gfyhvowst.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/gwshdfdms.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gmmwgcfxe.sHtML

[G03] 实例属性
来源：http://m.share.vehdjk.com/Article/details/gxmyaiwly.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gwqnvhozm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gicwjfxcy.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gharskxjm.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gsifnalpl.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gwkrtkpdy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.vehdjk.com/Article/details/gkfjgctcp.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/grnarzpby.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gakmkfiqb.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gwylhmrkm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gpvnufifr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/grcworjhq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gmvhkkbpp.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gtlnkgmfs.sHtML

Java: String greet() { return name; }
来源：http://baike.tarul.cn/Article/details/gwqyuhpef.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/glolcvpzd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gfnnfxcdy.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gaaudtjip.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/ghbcfqefg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gpdagltgb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpdvcdrx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gwqumeejq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gvsbiieox.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gxspyqgsj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gtdwowpsv.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gtyhshaxt.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gleeiotlo.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gwqzqjmah.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gaubgbxrr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gsqygeqcu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gmghvqshi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gwidrzkhr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gjtfhtgsi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gouwihmzj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gbkmvifvk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gngxlaoef.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gdblunlfb.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/gtkixpznf.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/gtgdciltt.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gddgvcmzy.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gypwbsyhw.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gjcqdjxph.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gejibdhfa.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gydtchwak.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gpbczwzqm.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/gjsxmvliw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gofbucmua.sHtML

PHP:  public static function f() {}
来源：http://m.share.tarul.cn/Article/details/gyuzahurx.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gcmomiliy.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/gowysuajy.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gvcngcccw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/grmhuubty.sHtML

Ruby: def self.f; end
来源：http://blog.fktsv.cn/Article/details/gfypgqsxu.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gsrcqranv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gmjdfpfkz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gcjecnweq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/glrnyxefv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fktsv.cn/Article/details/gcwftylin.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/gtqjibimk.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gvaibrvfs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaxyfkiq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gdqdwgagm.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/gvdxrapxx.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gjqzttzgb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gxulhihmo.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gsncklnvz.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gzsymrjys.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gdhowxmba.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.yfazqb.com/Article/details/gicfghmgh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gxgtrmclq.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gfulimcdn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gqxuiwnce.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/gphtaoxpc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/gylmckjrj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gseimjtqg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.epnwcf.com/Article/details/ghcwuthgr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gabpbzfrq.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gznszmskc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/glvudeqni.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gozpxnojr.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/ghannhbxt.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/gqwrxtsce.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/ghzbcjnur.sHtML


<!-- 参考信息 -->