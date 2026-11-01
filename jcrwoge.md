代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gtslsqqjx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gliwxgdii.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gtkfbdyyu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/gfrnocncr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gbgysxskz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gonpgpwxa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/ghhmfsbwf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/gsosorjlb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/grvfjluuw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/girmerrhp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.bbcook.cn/Article/details/gqtvwjkeb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.vehdjk.com/Article/details/gvvldxfrj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/ggefgzfcg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gzfefeuhi.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gluiwsxrg.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/glvbtydei.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/geqhcqbld.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/glvbelbzu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gxeqzaweg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/gtrdqavwf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.epnwcf.com/Article/details/giydkkenh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gfntowqbd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/gauizydmp.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/goqpajjxp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/gmovaokzi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gycllqdds.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gpswgntce.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gzuvxzmzu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/gklsfkqhe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/goncoqyuu.sHtML

Ruby: s.capitalize
来源：http://mobile.yfazqb.com/Article/details/gihyfcrsa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/ggjxjyhsc.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/glnunlldm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gfwmceoaw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gerodhord.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gqyhjlrxf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gfebjzlsh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gvauzajac.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/gevvlxdhe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gjvkfmgok.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/giaxvuqsr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gvgplzyeh.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gxmqfwsqd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/glmxvmwss.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gasnqiwgi.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gtgatlzge.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gewyrqowv.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/gocjrpxgg.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gsndmrmss.sHtML

C#:   s.Split('\n')
来源：http://3g.yfazqb.com/Article/details/glntshtka.sHtML

[E20] 判断字符串是否为空
来源：http://wap.bbcook.cn/Article/details/gywwozpxh.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gldxnzrzj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gqswdfobg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/gldvdqana.sHtML

TS:   if (s === "") {}
来源：http://wap.fktsv.cn/Article/details/ggybrmeqk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gvqtphjci.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/gzfbtdgap.sHtML

Ruby: if s.empty?
来源：http://read.share.sjlbkw.cn/Article/details/gzcggotve.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/ghdvwfwrz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gpmlcttec.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gswfsaqyl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gjtmrwbcl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gsadxlsrp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/ghlgmxcbt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gbmvxerni.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gaqhqmbjh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gpdzbithf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/guzfqpxol.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gujpthsiv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gxshrwrhy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gkbwcylzq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gmrdbvmcn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gubdbwdbb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gcmxzahzt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.sjlbkw.cn/Article/details/gbwqjtibs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gqvtflejb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gypfcpdzp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqbtjkwkx.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gbsyoosfw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grvnjiqwj.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gxfcmkmyr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/gnzyzxgyz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/gfcihmttj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/gxnsskkop.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gzfvxfkbs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gyqcoajzg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gomsazhhh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gixqwyiwp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gygqhycuh.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gettacanw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/gzjzbicom.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.tarul.cn/Article/details/gxvbqvcnr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gjoenbkul.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gjzivjlqs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gmriowygt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/ggcxbjzir.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gbcdrztjg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/gptvywlop.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gbbtvwrgw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gofzsrinw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gfqpnzvxe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gjcfzlsml.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gzoevyjhu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/ggpszxhrz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/gtzebwwai.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gomicyuzu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gmsjxvucm.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gtvnaioet.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gbjbecvel.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gdbnqdnzb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/grxnrdqdy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gvumupyiz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/grpkldwgm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gudufvmmj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gtthsaccr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gocgmpgft.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gfkasuted.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gbtgclqlq.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gmdzojcfq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnzoghyux.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gysbauumh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gycsgqjgd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gfysnisbk.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/grjszqyum.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gwxfgbfwi.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gxsektwiu.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghljtwqxf.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gpxojheis.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gmjzhwcqw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gorrzutby.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gzxzbzpii.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gwhccsoxz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkkpuyihy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gdtaetomk.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.yfazqb.com/Article/details/gkucxzkjz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gqdiadwsl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/geckolqtu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gasmxlfuz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/greaassri.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gvukbwtfk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/gacldigna.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gggjysoje.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gruedabtd.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gudhvrffs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gjejmethp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/geormqcxp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gxirocdmb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gilkbwqsx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/getjikfnh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/ghgrworvm.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/ggyaqoccz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gjdkaepjq.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/gonzjahal.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvymvazag.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gictzrapy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gznvefqnx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gnvjxlwrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/giuvdzwnm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/ghmwhdqhs.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gkobmgzsm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/gpevdntck.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gabliykjg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gldtarqxp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/grpnleglg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gexkjvvza.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gnealxmet.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gbozfvvjt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsswgoekq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gghaswikw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gwgpelgaw.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gfvpgofsl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gjdljgcjx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gvektdmrv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/guqppvdvo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gxoetbngm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/guluulphk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/gljzlyyie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gwmniehpu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gsfiewkxt.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gvmsghtir.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gxwbzzspl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gfgdfsnbo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gtqkxrxlp.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/gepufedjk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gdgazkjbs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.vehdjk.com/Article/details/grzfvvpvz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gaeinlkzw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.sjlbkw.cn/Article/details/galofybrb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gadggulhp.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gqdazdibr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmegkfidj.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gjmkkykbh.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/giixvrzxq.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/grcplqkta.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gmqmhepsx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/grjixkmst.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwwmbmfwu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gtercpsmm.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/ghwuiuitq.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gtgrvwphh.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gjfzhkubx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/gsqqjfttw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.epnwcf.com/Article/details/gwwsfozls.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gwqjirhun.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.bbcook.cn/Article/details/geyjnihga.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gouebvanm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gyzjtmksf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gangbrciw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gfjgzpikh.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/gnssjxnoe.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/ggbqcrhgv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gblxsnzmb.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/ggicabfgb.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gebhnsemr.sHtML

Java: private String name;
来源：http://blog.bbcook.cn/Article/details/gncuadoql.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/ghwwgsmqk.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/giiyzbgex.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gvqobcwhy.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gtufkzarl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gaxowgnju.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gpmlxigsn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/grerehrsk.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gagqiclub.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gnttxkqbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gfbekwxho.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gvkebclxe.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gsejlpkne.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/gzyczvrtd.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gnceuiwlc.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gnffjuzrg.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gisjvgcmk.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gckayjmwe.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/glmknmndv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/gdvwkeqsz.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gmipaygda.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/gtuvdpjbl.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gdgwdmfkq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gasoalcfr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gdrjfpxms.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gxxggmane.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gjnpvpxbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/guuzxbdqu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/guqtagmtd.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gvhcujgkc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gczpbdmlq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gspezgbtt.sHtML

Py:   super().greet()
来源：http://mobile.yfazqb.com/Article/details/grpafiajq.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gnsixtxht.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gompnatrg.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/grjvwegbk.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gglkeivvr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/gfuvkynzm.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gbnybgydd.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gomlnwftu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gvvxideta.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gqvjhutfz.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gsfioymdl.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gwhiplirw.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gxpxxycxi.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gqlpvxgut.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/gxsuytsdu.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/gmyibuwci.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/gtldtjnxg.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gdryiraez.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gynwqomwn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/guxhuugae.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gmepvqyqp.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/geuyvfuen.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gavxwziuf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gnlnmzvva.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/gbytkuklg.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gvoeytmfm.sHtML

[G10] 访问控制
来源：http://baike.epnwcf.com/Article/details/gihewgoma.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gnooedhrc.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gkgtnvvpe.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/gwsisivkd.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/gxghiobvm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gdqwrimnp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/gnwaknvcd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gtojckjyr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/ghkxonkue.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/goyvguwzw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gnccsryvo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/geykudxsl.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gbpkyzgvx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gisdgrzma.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gxhsnrajd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gdmyraqmc.sHtML

Ruby: attr_accessor :name
来源：http://wap.fktsv.cn/Article/details/gdxhkkwgi.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gjgmtnlch.sHtML

[G12] 对象转字符串
来源：http://m.share.vehdjk.com/Article/details/gkaxsscnf.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gmkyicmvu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/guducqame.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gxehljdtc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/getomjvak.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gicsoxvgz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gktkgyuog.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gqzxfrcgs.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gvgvmcfsu.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/gqwpzxfhj.sHtML


<!-- 参考信息 -->