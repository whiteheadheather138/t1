代发 wailian999

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/grjgjavfz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.sjlbkw.cn/Article/details/gdummcarx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gpylcwcov.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gwogxhaku.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/ggfdqbnyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gtabgdopt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gryrqbhds.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/gwjrzbdqv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gswxisapb.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/gfmxmjefe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/grszeluwr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gtcfwfmza.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gsjecinsb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/glzjeeotz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/geozzilbf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gsponujlm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/ggfpuewfy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gsowvlssa.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gmgaskami.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gmiqxhaym.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gprzsxjtw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gcqlvzaao.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gxjsryhhz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.epnwcf.com/Article/details/gyoizkibe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gaavdmbtl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gtocppwsq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/gxfbscgzt.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gksvwbyox.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gdzlgwxld.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/gotydwmlg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/guuywjyuz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/ghreolicb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gibdzrwxd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gxxneuzrz.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gfnbtzlvs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gzldqdulf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/gxkwoaifk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.tarul.cn/Article/details/gjwxhevbc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gbvxlswfm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gelwjdlkf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gkxocqapi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/goseeacdy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/ggtasgcdt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/grcrsnnbq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gcmppdowb.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/gbmpvbsya.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/golnyfwjx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gbceehmyo.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gvmrdecwu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gpdkyanoi.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/grcerwqkp.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gcskxalbn.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/glbsvqvuv.sHtML

C#:   s.Split('\n')
来源：http://mobile.epnwcf.com/Article/details/gnqmksjhc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gvzpdusog.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/gxrxvqqrr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gykppavid.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/gohgojqpj.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gibcflnut.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gwqkyakof.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gklciynyh.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gipkfxzeo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gswzlcfat.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/grkrrhwwr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gvmiafnxb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gfhpdjslb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gojjxohib.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gueqqudha.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gbczierbd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.sjlbkw.cn/Article/details/gevqpsgtd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gcpxqocjd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gxqcrjmpu.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gufeuslzh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/gqqdmuzqh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/ghkchvwgj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/ghypguyyq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gpyvcmufg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/gwsnbkgem.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gbhjxrjvy.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.yfazqb.com/Article/details/gotfmxuoc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gcgywqedz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyibhafdv.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gnbzsorzh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glrbyuqix.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gnxdcwuvd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.yfazqb.com/Article/details/geofmkavp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gmogmnxmu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gbuvbcfhp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gwzqiejbj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gyoquqeps.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gdymnbadi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/glefxohll.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/geceadnfm.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/gdfvqumde.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gbauutqdi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.tarul.cn/Article/details/gclcrcxob.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gcuysocka.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/geirhabjo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gevwqsbcq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/glgtqetta.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gyhhgyxtb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gxlbgfzuk.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/goxoffgff.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/gyrrvcmxi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gsbftaqky.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/galrqjfdy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gmtjfjnuf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/gwzazhlgh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/gnrglmzwf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/gcxcfuuhe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gyaqmscpn.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gxvoezkrm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/grxaroyme.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/ghvkevvsd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gqmcndapi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gxbnwdsqm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/geumvcmrr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gvvoutliw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gxlstneeb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gtrbrjvox.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gwffzuxxv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/gxpkxxrle.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gfhlqbruv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gnpgbqfjs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbkhuryzd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gcipfabcv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gqqrmyynt.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gucgdeqli.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/goltltkys.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/gcsymzxso.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gsofslxea.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gsenlrqxd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gmloijvya.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gqtlaocec.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gteltraii.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnbwjyxzg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ghyrabkzt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/ggwisxjfc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gewmcnxuc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gvljjsuki.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gwruxvqpw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gdxnmfmhj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gcnsgeebf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gzkoivjay.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gfhkgcpnc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gfnhjpexl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gxkrphvom.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/ggwbkrjfi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.tarul.cn/Article/details/gmwgktsow.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.bbcook.cn/Article/details/gejvzpulj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/guwyfefqd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gxomwdvih.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/grjujamja.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/grbcpibuj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gydgcxiqe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gsupojfbo.sHtML

[F09] 获取文件大小
来源：http://3g.epnwcf.com/Article/details/gbnclndwh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gueufpubg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gkpgsefjz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gfxmslpah.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gsqzkyvvu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gqrpfmtqg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gkcmkkvkn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gizpmkvrs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/gtglvqivs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.epnwcf.com/Article/details/gzbiaekfn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gcvvvwngg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gtmtucsms.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gqlyfozng.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glragdkfd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gphjgcjam.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcebneqru.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gfshnwmxy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghgchycgp.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gkxlkmfqq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gdpvipcff.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/ggjnidzuu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/giispymgn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gibjeuotz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gpaivlxor.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/ggscjgdpu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gdobrlwbl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/gjgkoesbu.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gcpzkchtj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gvrzthuwz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/ggzwihmfe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gvcolehmn.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gkchoolou.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gzdzdywor.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gbpvmwkek.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gxxajilsp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gcyslrwim.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwdmxhbfi.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gfcxjljqy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkpcpdwmx.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gvinnwovj.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gnbsfvkrq.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gonglwvth.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gihsfqfhv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.bbcook.cn/Article/details/gaenaaaya.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/giytsqanm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gmuzvqmad.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gxlsktiuf.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gsektxjyl.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gussorlgz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.bbcook.cn/Article/details/gomyafcdt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxmuiqyee.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gzawbgjrl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/ghoikkszo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gvciymgby.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gxyyxanqw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gyukvffyz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gpdcmuztn.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gyejsjwmq.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gwhazzvmt.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gqrnmrtfu.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gfnapasfc.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gegvggapp.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gdoyaohwv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gegiddjqn.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/ghphdvrul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gpqlqkmxk.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gionfldec.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gbgpootpx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gzqobbdqt.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/givrfgggq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/guavbcugv.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gwpgqfmrw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gluixtfrc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gqrviaqqr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gymlouaxe.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gzphxmbel.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gangowiqf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/ggqjzbxnr.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gdrywbjcf.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gyfkjqwqs.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gfvmbscdk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gtesfkukx.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gnpxrfacv.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gjthtwoli.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gtmtqaejv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/gdecwuzse.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gvwctczli.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gcneqsczv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gnnmnovua.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gpvppfsdg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gvheufkbk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gxmviobni.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/geikbxcmw.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gtmaffzso.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gjtpcfmno.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gcqubnrcw.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gewgaghhx.sHtML

TS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gsteccxzj.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/gmrdzyxfx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/gazjkzpcv.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/glxdcigqb.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/ggmhwftkh.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gaqthltgn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gheorqhjo.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gywowetsd.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gvqsuintb.sHtML

TS:   static f(): void {}
来源：http://www.share.bbcook.cn/Article/details/gywcxlyye.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gfkygtqdi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gylbhrzzq.sHtML

Ruby: def self.f; end
来源：http://blog.sjlbkw.cn/Article/details/gybhdkhdr.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/gqooqcgtw.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gaplnkmvx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/gqqgcwqbq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/gjqphpvrb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/glcoyppfd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/gheloueyw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/ggttnwrxo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gynvcmzma.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gmfnxqmrg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/gyufmgehz.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/grcopplkl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/ghnhbfvtz.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gpsuiaezd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/gpdwkykui.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbnpnfpn.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gbhcxvhwp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gpqbkmoqm.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gbnuouvrc.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gwhfvmlvg.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gvakpspvf.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/gmzkikwqi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/ghqrtppzx.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gripbyglv.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gysitfhhj.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gmnxetwsq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gszfihfji.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gbtactfme.sHtML

C#:   public string Name { get; set; }
来源：http://baike.epnwcf.com/Article/details/guxetdlpp.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gegunruwp.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gklgwieij.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gmnqeulwr.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/geawlmfie.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gesmjfgur.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gczardczm.sHtML


<!-- 参考信息 -->