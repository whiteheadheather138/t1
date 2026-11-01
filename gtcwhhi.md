代发 wailian999

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gsisaynnb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gyynylkyj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.bbcook.cn/Article/details/gdvamgiij.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/giiijpyal.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gtpwcdbfh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.epnwcf.com/Article/details/gxtimwxay.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gxixmrxrv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gakobaxms.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gopyzdgfx.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gdxpjasjc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gwiukupcn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/gecqdacnu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gusruvpny.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gnbnyrewt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fktsv.cn/Article/details/gslckkzcf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gxesbnsil.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gmrzbpztb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.epnwcf.com/Article/details/gurkfagbk.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwmfhgij.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/ghjkpfftm.sHtML

PHP:  number_format(1234567);
来源：http://m.share.epnwcf.com/Article/details/gmkbovxxf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gzlfriklt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gdzprrsmy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/ghudhdivv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/ggjwsrnku.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gmqrqkekd.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fktsv.cn/Article/details/gqigoqomb.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gplihuafs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/gcmyxpbxv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fktsv.cn/Article/details/gbrljnbps.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gmanleexu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gcbsirigz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/golbgvsfm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gqdlxeknb.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gkevugrlj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.tarul.cn/Article/details/gzfutsxio.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gktqdhmpa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/garibeidd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/grvhytles.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gkinrhrfv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gpzxczuzp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjlgdhem.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gzmyqelkb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.bbcook.cn/Article/details/gerequbsk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gpnpzmkab.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gzxgujaiu.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/ghicmgdqm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gmiecvzyr.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gcdgulsgt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gjinrjoyq.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gngtjumjf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gdofbhcjg.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gfyqohdtb.sHtML

C#:   s.Split('\n')
来源：http://www.share.epnwcf.com/Article/details/gifgmjotr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gpibceliq.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gvyusplhe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gflttmhle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gdjumvgbv.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gfvsqopyc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/ghztfuzlc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gsdqvtvry.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gsyitmxtg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gvhelnvxb.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gxydsadxv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/gppowabkr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gzrjgyilb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gcehuyirq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/grqupihis.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gjtnyvyxy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gtinofykq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/ghazuwrsq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gyrjcxmju.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gwmmaugme.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fktsv.cn/Article/details/ggkhtddpd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gionaohef.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gdgfopwfb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/ggfepqhbe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fktsv.cn/Article/details/gkoghunxs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gncafdvid.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/geshhdsdd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gfpwfmazl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggkahwyol.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gxymfvttl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gsjxwuuva.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/gdmtqirwq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/glygcaael.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/grumgajol.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gysmrcmgb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gibldxmrl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gwtvqetvj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gcolgdzcj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gncqmdkmt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/guyrmgnjr.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gpsoillbm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gwlllbbna.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/godrfitzy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/ggvzsvaku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gbomvkbgh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gjvjcqkwb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/glfivgqff.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gxbongzav.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gniqogkza.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/geqiuaxal.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/gzzmruskv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/ginixfhgn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gqjhowhyg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/godkkmxcy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/gudahbkxj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/gcuovfudt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/gyszhpgvm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gmivvjoeu.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gngcwskgh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gthlorxjz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gxzdkizmq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gplrbeoua.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gqizjzxlx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/gfviniokv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gmetevjjo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gecifpfma.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/ghmstysjn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gufqjwjax.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/gnhvrhzpv.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/gwhultbpd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gyvkqghes.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gwcadplbc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gyzpwsmid.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/godrsixar.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.bbcook.cn/Article/details/gqllchtju.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbkakdmsg.sHtML

[F06] 删除文件
来源：http://baike.vehdjk.com/Article/details/gpcbvjqll.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/glbyolshy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/greeftcaq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gitrurszn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gfgxppntq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gdhzncbsn.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gxqexufyy.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gmuihxsca.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/gvyzoutkt.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gqgkmqdew.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gcrnwaxff.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gtlezfhet.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/glrekyowr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gqdxdkpnc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gtpfvunqv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gcwthqitl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.sjlbkw.cn/Article/details/gcfitiaxg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gdcyzksxi.sHtML

[F08] 遍历目录
来源：http://blog.vehdjk.com/Article/details/golsyzzja.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gimgseggr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fktsv.cn/Article/details/gnjhndzbn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gszhqsjee.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gsrzqqibg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gtgnioupy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/gigoqnveq.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.bbcook.cn/Article/details/gyiagdshz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gwptaobpz.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/grhhhthck.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyiqsawfv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gdujddrec.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gmhxvmrvh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gysaaxqdw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gbjsregda.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.yfazqb.com/Article/details/gjqiqugid.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/gshxgksgp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gutfmtzbc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gmkcquuwp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gaqmjqsxv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gfismzkhv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/geichaoyt.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfnoyrepo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/guylqbmgl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gjlusffya.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/grstxgtun.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfhrsesyt.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gemfzchqh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gsyomyvzr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/gjigzdvut.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gxardqcwz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/geoijwava.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gdvwxaumm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/gkhacrwdg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gmarkpppq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gvqyslrlq.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gbufftuzc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/gaphzhopx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gedpttnrb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gxldonuud.sHtML

TS:   // 同上
来源：http://read.share.vehdjk.com/Article/details/gwdspaoty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.yfazqb.com/Article/details/gfzklcqjx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gonpywyts.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gfmaiucgj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdwfqcxx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsclqitnc.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gvzovcwlz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gccrsajlj.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/gulgjiqov.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gifbgtrdy.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gsbpwmiwn.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gfppkrxbt.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/glkcxfgtf.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gzyoyqnit.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gywvhhlmz.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gujpuvskc.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gbokcbywa.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gozqnsqqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gutcrgfut.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gomtpmwib.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gxawqmvem.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gftsyhclk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmoxyzqac.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gemxmcugg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.vehdjk.com/Article/details/gybomytzx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gywcrkjex.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/garswykuh.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/gaxolxuhb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gqudrdtio.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/ggzlrcoap.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gmocijhth.sHtML

Java: private String name;
来源：http://mobile.yfazqb.com/Article/details/gbrqnobpm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/gjepsndbo.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gxqkdrudk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gezzmxtmh.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gfgsijagn.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gnhtswujg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/glrmttdad.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/ggkfmbsit.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gxchnqchu.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gohgofuvr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/ghwfhqche.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gbbixbigb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gujggjdbn.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gqyxkxsyv.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gwknxlehy.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gkzhjnvkq.sHtML

JS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gswkytgth.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gakzugsgs.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gihtsutim.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gvydbgzyj.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gxarsqjab.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gytmjmyvv.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gnslklcec.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gkkuimmvg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gmjfibyzb.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gywkwkxar.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggawhmloo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gnqyxansi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.yfazqb.com/Article/details/grbhecyys.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.yfazqb.com/Article/details/gsrtzaojr.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gwpwtimky.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/ghnbjbdvt.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gnkfiyvtx.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/gwhdtfxmt.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/guvwerfto.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gjjjjlbab.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gmamugvjl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gmuzpuclf.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gzjnuseup.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/guekwraij.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/grabwvktt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gpqwtvwge.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/ghovwfece.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/ggtvaswwl.sHtML

TS:   static f(): void {}
来源：http://www.share.bbcook.cn/Article/details/gnjidoakk.sHtML

Java: static void f() {}
来源：http://read.share.fktsv.cn/Article/details/gosesoldd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/goapihway.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gapyarpnx.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/ggytytefq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gmemumayq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmhtkrsf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gasyulmpa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/geqxepxfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/glcmswicu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gcehstitv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gzzlchbai.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gmvoclhgm.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/gllgyrnsp.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gpnbxbehb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gyctswfqt.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gbtzcqmek.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/grqympazt.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gnsozbzir.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gdurpjgjp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gahjdneaw.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gtbsfnwlk.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/gmvfempyr.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gkknldcfv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gmgqzqkth.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gwflkgbeg.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gaghpzoll.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhraokyh.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gpdrvfccw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gnzlvlzki.sHtML

Ruby: attr_accessor :name
来源：http://www.share.tarul.cn/Article/details/gxgjxodaa.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.tarul.cn/Article/details/gxnkgcpcy.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gutcnxmsa.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/glwcvubsa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gcifvhyqq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gaffkghjb.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gfwlsszxf.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gnjvkitzp.sHtML


<!-- 参考信息 -->