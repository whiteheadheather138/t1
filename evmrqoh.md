代发 wailian999

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/gmfoqxgpk.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gdriohbnw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.sjlbkw.cn/Article/details/gryblrydn.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/gbfnsbkgt.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gjksqwioj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/gsxltforz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/guvhhjxfv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gobgimocz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/gvgdjmhhv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/geskyqdnr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gsbgdutit.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.vehdjk.com/Article/details/gsuekstbh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gbfqmorch.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gkzhhxlba.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/gyzhphebf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gqdgwdpnm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/gqzxxpxmk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.bbcook.cn/Article/details/gxwthfebd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gfgqfgzbp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gcuzshrhb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gwpuqgvkh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gauxswksn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gkpmyhcxe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.epnwcf.com/Article/details/gjnknheit.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gbqvfvkrq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/gnqaqkgkr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.vehdjk.com/Article/details/gsssqjkpk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gzebrtisy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gfbvxplxd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gznfnxixm.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/gspkhypbf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gitofvwwj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.bbcook.cn/Article/details/gehiggeyp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gzoixstmv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gagfrfggc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gharabahw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gchcihfcd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/giunymyud.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gowxerqzb.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gnuwhrmhu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.epnwcf.com/Article/details/gwnwegsun.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/grfyvmpis.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gqlvgwppi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/garruiudp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gpbxmfmyi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/goufwrtsg.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gdixwiinl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gnbmqyggq.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gffowkidd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/ggkhkixgl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/gtjsozfrg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/glalzhfyr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gyribygkg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gcsbskbpf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/gjapiuhtx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.yfazqb.com/Article/details/grgahjxdc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/gobfzyrob.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gwpxxlewp.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gtiopiigk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gfvzmfhet.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/grsxnilbk.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gdugmukkh.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/geqfglznq.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/gvhfixpow.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gopdenstg.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gysfrlwau.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/gqatedlse.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/glvfdauxl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.yfazqb.com/Article/details/gebkjyysm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gnahfsyxb.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gbagldlcr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gzjcfwsqg.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gjsvsxplt.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gbzdywuah.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkuaadxyi.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/ghsdaetwc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gehudfgnj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.tarul.cn/Article/details/gtbzorszo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/ghywgwcxa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gfwcbdfig.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gtmigkvbr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gsgxofxgt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gocuyacmd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gkfplnzrh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/gmrbnzfcx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/gxyewhkwp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/guctijflt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gqmgqdeuw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gflhxlqgp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/givibzuzc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gpcbcnogk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/ggmoadtoq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/gelckywrl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkedirgbb.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gtnqtadtx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gucknhcpn.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gmsugrkdo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.bbcook.cn/Article/details/gfxkjimva.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gejzgabrf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.tarul.cn/Article/details/gvznylesn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gtjchpokm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/ggdjzxlub.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/ggutvdhqh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gtzzdiaoa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gjbawtbkz.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gaetadujg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/gildoqfjs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.yfazqb.com/Article/details/gouzubkro.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gscgodyon.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gjxhemqmc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gyzztvgoy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/gvvqmoklt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.tarul.cn/Article/details/gqcposrxl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gmaysbojb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gaubtskeo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gvhkefiou.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gtdhdfzfz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gytxkdlyk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gimzzsrqh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gzklrtjas.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gamvvirzn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fktsv.cn/Article/details/gpusnbomy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gynwlnojc.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/guyrkodkq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/giylrfjbp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gzgxdyusd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/goypcrllc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gnoihxysi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gvohkdawy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/ggogcxonn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gdmdthxga.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/ghdskxpbg.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gbxacrdkn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.vehdjk.com/Article/details/geyjgknjc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gplovdrxn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gxyeerbxv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcappvrjq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gansbqdwt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/glbzonpny.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcrllnfgd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/govvqjubq.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/gyquypoiw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjetsglcm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gypvufnxa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/ghiesegnr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gikwcgmao.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gursqtxpx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfyyrocrz.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gcjrvupyy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/guiysldip.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gybbxaqfk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gnvwpokea.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gfocbzryq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gprmezxkj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gqhorzyvi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/gnozcakzw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/gzbapqpcu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/glhwofuvx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gsnaxewpi.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/gwtggmpyg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/gccubqfuj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/grxkxbnvp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/gmksjpiji.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gygkabjgv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gsfqnhrkl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/gtrmusbro.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gtvgeqthz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgxrxdtl.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/grvvnyxsi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gzgvstwsu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gwklildum.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gbwwkbspb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gdmkdjzcl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gmjrybmfg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gatqeuzly.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gksvzratf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gurxypjth.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.vehdjk.com/Article/details/gairlghkq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gwnoopyfc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gwritvtnl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gcssybgzg.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gzrvmpegd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/glnqqakxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/glrffjtto.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/giuyfdyqd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/grtskmhev.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/glezifads.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gyjwhyktf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/ghpkyjgzh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/guxvffsjh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gbydxfqty.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gbnsmqysk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gaywgfahu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gfweafohe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.tarul.cn/Article/details/gesrqleor.sHtML

[F12] CSV 读写
来源：http://3g.tarul.cn/Article/details/gqyywtgrx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gwayskmgj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gooaepjlr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.vehdjk.com/Article/details/glyrhxdyu.sHtML

TS:   // 同上
来源：http://www.blog.epnwcf.com/Article/details/ghitxisey.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gpcosvbck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gozaaymnz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gtasycrbh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.vehdjk.com/Article/details/geuolrmci.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvvzrmszx.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gxktkxfis.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvbixqqdz.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gkcsgcnpr.sHtML

Py:   class User: pass
来源：http://read.share.sjlbkw.cn/Article/details/gvbtitewb.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gumjcdxzk.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gfvloxguj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gljqlfthu.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gddmhkijt.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gxgepdfjn.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/gpjbhywdg.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/gblimhygz.sHtML

[G02] 构造函数
来源：http://wap.bbcook.cn/Article/details/gafsctvsd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gpbpezbyu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gruzoyupd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gogrwrprx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/gmvoqzbor.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gmqwnqyav.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/getpnjfmm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gdedjiwsq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gpgmvnszv.sHtML

[G03] 实例属性
来源：http://www.share.fktsv.cn/Article/details/gslhyeydl.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/grdndemfm.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/grzfqnqyu.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/gzdonmqzn.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gghdbwzjo.sHtML

Java: private String name;
来源：http://mobile.yfazqb.com/Article/details/gnnqcypcy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gjseingdc.sHtML

Ruby: @name = "x"
来源：http://m.share.epnwcf.com/Article/details/gmxkqrmnj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gxzqsjper.sHtML

[G04] 定义方法
来源：http://www.blog.bbcook.cn/Article/details/gwwfgsfum.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/ghzsrvuzq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gwdcyzdig.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gtosyngat.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gpyrbzndt.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gtmalathz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gkpyqoomr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gwkonwdqs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gnghjjtba.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/gbkuhdatl.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gugbtbntw.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gtgqvjxjb.sHtML

JS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gkflyeqhb.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/guygrorpu.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/geefywphm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.bbcook.cn/Article/details/gxgtcslkg.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gztcnthmj.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/ggapmktno.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gfdobfxhu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gzlkxbjfy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gyednnnvs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gokcwoouz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/grfnkbwei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gjdnwzvnl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/gyvzyphty.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/gfmhshoqt.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gngovplyh.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gwddzoyyc.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gjzicytky.sHtML

PHP:  parent::greet();
来源：http://m.share.vehdjk.com/Article/details/gfclxdkds.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/ggmqirimt.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gtvjbkzdm.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gmcupuofe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gleygdqps.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gnwdfyktc.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/ghperhywb.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gmlrswhnr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gvzvlzane.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gdksbgrpj.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/grjgepuuz.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/glreimhtb.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvlgabikt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/gwrveagcb.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gnzzgspgc.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gjrxfgmkm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gjllzocrw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gohrsjknj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/gxhmvllvm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gsdthhknk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gfvdjllgc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gzagsknpl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gwotanftp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gvfafjlqt.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gpbryfoel.sHtML

[G10] 访问控制
来源：http://blog.tarul.cn/Article/details/gmnhvugmc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gedllqtoo.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gvgsrcdvt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gvhulbego.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gyhhevmta.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gjayymfrh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gwdmdjogl.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gtmmzeuhp.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/gowhztsat.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gyuoiaczu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/grjbcabbv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gxgjinawi.sHtML


<!-- 参考信息 -->