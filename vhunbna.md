代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/glkoblzro.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gnajpntjy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gixfgclnr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/gyogrminj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gngmckksn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gukfvuxiy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gvfwfxygb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gljifhdyl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.vehdjk.com/Article/details/gegaurqyy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.vehdjk.com/Article/details/ginaigqau.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gvrbzoldn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.bbcook.cn/Article/details/gzwtnxile.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gmwbyzltd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.tarul.cn/Article/details/gxgxincpv.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gafnyhtno.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/ghdbsbkgy.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gzjljheqk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gqpqehwim.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gmdlrkywf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gccieoeam.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gpmpdfbvz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gvwvrpmmi.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gjsvwqcvc.sHtML

[E17] 首字母大写
来源：http://wap.vehdjk.com/Article/details/gsltqvmcu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gdieewnta.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/ggtmuqkek.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gyworkfnf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gvbfcxeww.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.yfazqb.com/Article/details/glnkvdmlj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/gnljpcdmf.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gbelxfgjf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gkfwcmkxe.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gnzxzhspt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gnlfdypll.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/guexbrowy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gayavzrqp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gnnizmkto.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gscnhwnwf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.tarul.cn/Article/details/gxkpfibkm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gmekemmss.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gotfidgqx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/gickktcaq.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gnkzveobq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/grsmtpzyh.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gchzehoqa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/glexkloio.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/grdgresxd.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gahqhqsyt.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gngrluhwx.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gxsbbjice.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gmbakrdzr.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gkilfsgar.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gcocvreyf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gqvupcdhy.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/grxzdpznl.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gxgpnrmeo.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gyemtmvzw.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gpftupvhb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/goirhvaqs.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/grpfvdjqc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gaprvwywz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gbpdzkvzl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/glcwnzlzc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gkkdxyvyd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gjtzcacxg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gjzqzlscw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gdeqvvlwb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/ggjdxjvls.sHtML

[E22] 字节长度与字符长度
来源：http://blog.bbcook.cn/Article/details/gsskaxkco.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gikldmzaa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gmlyfxvya.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqoipyzp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gtfirsfel.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gjypnyiep.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gsasowzyx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gayciaghx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gfuclexhi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghpbwdxdi.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/gcefzwmjl.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/godhaanuw.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gxvgmwgrn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gyrhbtpnd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gdengtjgr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gvvipgwmw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gxexceuxs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gxoodfusw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/gnyutpmyd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/gpwhhnujp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/glwkqtdqm.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gbxmfgcfi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.sjlbkw.cn/Article/details/gsqelmmlm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gkmicyasr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gndtefnpn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gfjewduoc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gobwtccjr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gcwulugak.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gxergkcme.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gbnhycuhw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/geikhxknc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.bbcook.cn/Article/details/gozlzfvdh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/guosslpqw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gtqcxkeyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/goymglnzo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gijtwmwkn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gbcbggbwa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/grrknkafp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gywnplrao.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/grcvgtqmv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.bbcook.cn/Article/details/gmidyllfl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.sjlbkw.cn/Article/details/gejyilqqq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/guxotnvhy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gdvwvasvi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.bbcook.cn/Article/details/ghwpzouce.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gnndczwtp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gizfipadg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gouvzggjh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gjuiunrml.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/ggndiuchp.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/gyripvucx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gcmbynzss.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpmkebxcu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gytypiumd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gsxbxfkaz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/gplifykkg.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmofamyxq.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gqiqdcuhx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gmklkdxzf.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gkncmrpmj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gdljxtkeo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gewylkhsa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gxqdpdeyx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gycbbhkgp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnfapnxmn.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gpovmklrb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gjgdkcmdz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gmumpprks.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gcriibdns.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gojertczx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gxqrucxkl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gakgszhdr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/gklpazsfe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gxduyvjrh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/ghqsclrbq.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/ggooxatpv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gafhjpcva.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/gyrutdplc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gfgqfnviz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gwlccevow.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gkmexkrsj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gksgwbvsr.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/ghtwfxvzf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gwrhfgpvd.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gnagenglc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gkvlblegr.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/grefarlcw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gbnisblve.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gfxsfudjc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/grnjucyby.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gqmpradyk.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcpkadmtk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gmzbvdlgl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/gcxyvlgmf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gyeertsbh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gzdhudccb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gywjjnunh.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gbodnbqmq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gbkiyrmoi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gphgtefae.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gudwhzhvu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gjejqnamq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gagxxqftt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/grjjmhseq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gdamlkfrl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxefnmguc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/geckkdjyq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/gjqkuesjo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gvpuphoch.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gsjvxwrlw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/gxbegjppb.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/gqjyuktfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gkppqctga.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/gxzrtroje.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gecaaapbk.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gacgvwvie.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/gzkpkwsfq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.yfazqb.com/Article/details/gbldppxel.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/gvamylymy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gxvvdeaxd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbwaxhcxf.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gsuebewna.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjsjhmncr.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gnzbqkkyw.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/grgqybpfd.sHtML

PHP:  class User {}
来源：http://mobile.bbcook.cn/Article/details/gazlafzjn.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxagcrmy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gjoimawnq.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gmavksaur.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gbobnnraw.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/glwubaxpx.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gcaqisqiw.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gwvqjgbbx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gjduypxlh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gwklyvhvj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/ggdqglnbn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fktsv.cn/Article/details/godrylypp.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gjecpwxji.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfpaixva.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gyabrxkxn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.bbcook.cn/Article/details/goqvwpuvj.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/gftyvlsxr.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gjdsvcrpv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/giidfnvxg.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/glcqszdnz.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gidcoltrs.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gicwrcfru.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gxkvnhcdo.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gyavyoncl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/glpldjnnt.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/glpmtqxtf.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gefkreexz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/ggfybxzom.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxeimzby.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gdglomfpd.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvstfszpb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gcqphpqgt.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/gvbfioixl.sHtML

C#:   public string Greet() => Name;
来源：http://wap.vehdjk.com/Article/details/gfqinkmru.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gmlthryei.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gglorqwym.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gnyurmhvx.sHtML

JS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/ggsilwyaq.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gijmfclrm.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gpvuxgqoa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/glrisyblg.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/gsamzrjjm.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gskkvwqos.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/giroceiln.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gkgvrlhpz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gyoajdiuo.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gcaykijml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gckrmsozz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gusvhzkav.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gvecfvieq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gjdhhipjc.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/gbkapubda.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gtlsmvijd.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/gouupudve.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gyffawnla.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/ghlyuwptw.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/glggdqwcm.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/ghzirqpmn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.sjlbkw.cn/Article/details/glczemaaa.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/gxsbfapxu.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/gtfxakngu.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gxyrzrxlu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gydcpzgdm.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/ggohoqmgl.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/ghheufrth.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/glgpvwsix.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gkctjypaq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gufjlnblq.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gntbeubdf.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gcqoiocos.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.tarul.cn/Article/details/ggaeujzjc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/gkpqilckg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.vehdjk.com/Article/details/gmjdyujjb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.sjlbkw.cn/Article/details/gmykiznxe.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/glrcupkox.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/gcvxgwbnl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gvplzvped.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gogvdeovt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/gcisbihsv.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gmageuaao.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/ghkpklolf.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gfngmmmbo.sHtML

JS:   #private 字段；其余公开
来源：http://wap.tarul.cn/Article/details/gphumodoz.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gpegnjjhk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gmadqxqhv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gkdfkifxk.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/ggmzjfnag.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gwpsjfkhi.sHtML

[G11] getter / setter
来源：http://www.m.share.vehdjk.com/Article/details/gvcloarkp.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gxhdeohqs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gxptjecat.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gqwtscwes.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gaenivurp.sHtML

Java: public String getName() { return name; }
来源：http://www.share.yfazqb.com/Article/details/geavnvndv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gknnadyko.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/gchkrquol.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbcxiyxbw.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gmcsnlybw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gsmibwfid.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gbgaxfikj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/guevulsdt.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gkziycelt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gfxbnztfs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/ggvwolvch.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gjxmzdpwl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gogaujqgu.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gbdqxmvfx.sHtML


<!-- 参考信息 -->