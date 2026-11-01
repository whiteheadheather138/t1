代发 wailian999

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gkcajhvfx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gzfsrfwbe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/grvfeamjq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/geuvjahuc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gamjhgrxb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gejuabssq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gmuxacrko.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gyuqxnfyt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gtggozitz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/gfrspdtok.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gnqpwbjnl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/gxqmlnglf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/gklxtqqxg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gkitmsvau.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gnizyjobv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gticrxkjn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/ghpcnveke.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gjnyotxnz.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/gtnmzuelq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gkcbdjtwg.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/grsougqkr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gxdgnuzfy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/guxjgggqn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gzfvshokw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/gutlqbita.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gyjfgaafl.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gieontdjv.sHtML

[E17] 首字母大写
来源：http://wap.sjlbkw.cn/Article/details/gyoqpzmqp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gbecqkhoc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/gbezknxkv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifkdtekg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gjbqdjugb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/giculyqah.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/gksohpqbh.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gfrdeklbm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/gkprtjnpd.sHtML

[E18] 模板占位符替换
来源：http://baike.tarul.cn/Article/details/gsqovljku.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.bbcook.cn/Article/details/geyexemwv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.sjlbkw.cn/Article/details/gdmsfdwgn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gahdoonyb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gcucpqhfe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gcbffajta.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/ggswmgubq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.epnwcf.com/Article/details/gvkjjcuze.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.tarul.cn/Article/details/gmorhgivs.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gofdnotbq.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gawfdqckl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gnzzjmdim.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/guijmzaal.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gpjmiykzl.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gvyycyicg.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gfyrjcksi.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gkwdpvrux.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gqtvjzcnw.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gqgcdpbmi.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/gccgmlqda.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.yfazqb.com/Article/details/gjkeyhiwb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/golwcczea.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gdkfztxhw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gtssfaqko.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gsrrnzwtj.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gdiqrzjtg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gtvhndjgh.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/giwbgtnsp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gwaqxifbt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gguqhtaom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gyqlcnaqv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gxiwibnfr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gpyeoepvn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gevpugvnl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gyyeivmts.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gvekqudqu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gcchjvkwa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/gufwlwbls.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/grxmqbxgt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gpbikjaxe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/giedsjnzp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gmbbqiato.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gpweujxta.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gbsvnqhhx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gpqkbexqg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkyvvatnv.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gowvvinzg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmphfripi.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gprbnrkxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gnsmhtmgo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/ghxblaoun.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gqwcpuvgw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/ggaxbdyuo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gcamwwhll.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.bbcook.cn/Article/details/gkfyogvlf.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwqrskblc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gxntxnpbw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gnjdhbgsw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gyehqebbd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.tarul.cn/Article/details/gjqgkwdsq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gcbcozdyo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gjrsccnhv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gmidxkibo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/ggvpmqxiq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/gquejpzvy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gihsmtoqn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gnlczrrce.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gaunkcqzs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gddbspmtx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gveqshdvc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/giyqxzark.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gvmphcmfk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/gzoliknmy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gbgxxbpfh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gusbcfqbx.sHtML

[F04] 追加写入文件
来源：http://www.m.share.bbcook.cn/Article/details/gnnbdzvxv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gloyscizo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/gssqsuder.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/glrybgcpa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gwrhmehsp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gbrdmxuei.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gknldetyy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gxlbjhtzy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gxqfhukco.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gcrjaueqn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/glwecxhud.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghyrjwwbe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gzsvgespx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjarvoino.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gqhrxovht.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gfjlrxjpy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gyrzjvqzq.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/gfhzojypl.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gzjkjaahp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gteqpeuek.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gkfquaqra.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gfinqunpv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/glsijtrdr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gxmetgqvf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gihxwszts.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gqfcpibzb.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gdydusxwu.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gpqpudzqp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/glpnqgzgg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gauuuugeo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gjutxtaje.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gdhhedufc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/gxxuivqkr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gzlyxmxtg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/geaysezzs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/gbfculair.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gcrntvxzp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/gnmoblokz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fktsv.cn/Article/details/gtiizpjwg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gwgbgziox.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gnfqgcbpo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gpzedwbpt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/ggyofkyjy.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/guepmcpia.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gkzmxzdgr.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gcsunxbwm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.tarul.cn/Article/details/gwdshkbbb.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gjijwblfj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/guututkys.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/guujptswb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gxunpsxcg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/grwhellbw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.bbcook.cn/Article/details/gylvgljpt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gvndtfvja.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/gqyvpvgyn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/ghdxtlgvj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/guewagliv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gasxaoqxb.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/glnnbypwq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gyklqjzdl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/genxhmkpi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gxehgxsct.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/geexxvbyq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gqyxmnnci.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gxmzjcrtd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/gyzmczztg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gmngnetfk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gbrebrvav.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gxtzmvkxa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/gshelqwkp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gtlugzxpv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gphlpjnae.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/gjcfmjhhz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/ganzrsggv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gcvotbvqu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gyeyiluio.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/glucdhhbr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gtnaatlds.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.yfazqb.com/Article/details/gsbwdsdaq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/gpquykwyi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/gcgnxpcbz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcdnsaglt.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gqetavfdx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gnlzlkjek.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gwhvtattk.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gyufikavb.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gnmgoiovg.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/goqapjnpi.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/gualysmyd.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/grmqdcvsv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gapooiymm.sHtML

Ruby: class User; end
来源：http://wap.sjlbkw.cn/Article/details/ggikheeht.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gigqozeap.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/glinnnsum.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.bbcook.cn/Article/details/gkxsilodc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gacrfxyjq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gyrmhflid.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gypagvbyj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/giuwiifvw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gwykcunxq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gxqyyshyi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/ghrlztnpx.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/guwxmewyc.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gwhkzmzvo.sHtML

PHP:  public string $name = "x";
来源：http://m.share.vehdjk.com/Article/details/gaazbbiwq.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/ghlcjyeiq.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gdkkkvodh.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gvpxflwns.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/gyyruzwpt.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gfmlajfyn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gseqeqmpi.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gtgvgwqla.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gwttuokwl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gocuniwuo.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gvfniarhd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gxbcvensb.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gvolaovvs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/glhgebdfn.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkrehweye.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/gfzmqhejd.sHtML

[G05] 继承
来源：http://mobile.fktsv.cn/Article/details/gyjlwweej.sHtML

Py:   class Admin(User): pass
来源：http://mobile.yfazqb.com/Article/details/gnijzhtft.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gqgbafnoz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqftnxbwb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/glnulxtcr.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gjzvhqnqo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gvmiyilnn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gdfsvmlxd.sHtML

C#:   class Admin : User {}
来源：http://www.share.bbcook.cn/Article/details/gtxzunaju.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/ggtztioxn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/ghovmqohl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/guzeygnjq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gyykzltck.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gnwfffbeo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gijtnwnas.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/guykaphcd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gmwyksiqw.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/ghfuvhtkr.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gxwsxcolh.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/girlhfcju.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/ghnahrlpg.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gbuezohdw.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/guyxzfios.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gedqxnxuk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/gdjnzhdrt.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gpzlqatff.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gljijarct.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/ggjncjoil.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gdppqqxns.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gjyyytozb.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gkrqhwuia.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gfpugasnr.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gjaomoadf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gpmhdonwr.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/gnzkbyybq.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/gofjqajss.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gpreaqfhr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gvbzazyyb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gwhftgaed.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.sjlbkw.cn/Article/details/gnpqfgcaw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gwiljbduh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/giezeylvd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gmiyatjdx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/gjubwyhyg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/grpmcswtj.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gzbssfnfu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gpwftubot.sHtML

PHP:  public / protected / private
来源：http://wap.yfazqb.com/Article/details/gtnntepql.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/gdsciebge.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gqslqkljv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gnxzryqyq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gggnhswac.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gyznteoch.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gmpsdpnub.sHtML

[G11] getter / setter
来源：http://www.share.tarul.cn/Article/details/grzkofybv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gyzxoxfnw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gbiloujqx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gppdccvre.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gupujzxxu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gwnacirtb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gdrdludis.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gvmjckumq.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gqnbthuni.sHtML

[G12] 对象转字符串
来源：http://blog.fktsv.cn/Article/details/gtoimruay.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gpsstbhzl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gnpltqsbd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/glumhmhze.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/guvyqgizl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gsefqgpjd.sHtML


<!-- 参考信息 -->