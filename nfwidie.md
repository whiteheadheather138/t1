代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.share.sjlbkw.cn/Article/details/gmbdgcmng.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/ggooppvny.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrtnuahg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gkyqfuiyd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/gyknrazrj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gefthfhxj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gegcukquc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gmajmdzfk.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/ggjhhdpzs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/geflihpiy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gattphgfz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gytgvklqp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnegtvdid.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gedpzxkbk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fktsv.cn/Article/details/gwqndwwli.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gltavscuz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gdqxlvjsj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gkxszhcgu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.vehdjk.com/Article/details/glqaahxaz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/ggtctsgko.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/gaelxxotl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fktsv.cn/Article/details/grlfmnkvk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gysfbcpqd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gwaickgcp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gambvexjb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gqgaspgcd.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gslqhwogr.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gbinycfqq.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/goscaxdrq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gdvlaktzi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gyjdgbtif.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gxlatnyjb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gcofbweya.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gbuarsryd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/giwkglnpy.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/gcnageszb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gobhibggc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gncsxmlbs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/grijodxlu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gruxrfznr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gcqqwxzpn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.yfazqb.com/Article/details/guieyzldv.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gnfdtwxuq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gjdisshux.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gbzrlnzwk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gvknsuhwq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/giuaftjdj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/galiskqvc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gsqsbnija.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gpdpodwgw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gbtoomowb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/ghhurgiou.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.tarul.cn/Article/details/gvcdxpwgd.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gjqhfmvug.sHtML

Py:   s.splitlines()
来源：http://www.share.sjlbkw.cn/Article/details/gzhftskgc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gykxssewg.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gquqosfxc.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/geeytdywz.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gmvxxzhvj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gakhtamtk.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/ggtehvbks.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gsvaxciji.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gbgbaxutj.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gnlkxfmse.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/gfeznqbbm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/ghepwcaqh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gheptmgju.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/givouirfw.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/gamgwczsp.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gximdarfs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gpwrqewer.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/grrhfplen.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/ghlhsqtcu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gvppvalom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gkgmahmkh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/grzypjgpv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gzflmlyhb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gvkuzswum.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gghhdnboq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gbrwlnnrb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/ggbkolmbg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/ghssdntfc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/grnohvihe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/ghuycdepx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/ggvzzbjzk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gweupuhiy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/gtqakckbi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gychajwmv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gyldvhouj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gljivrjrk.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gjzldjzih.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxbpnvjks.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/ghtgqjoxy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.bbcook.cn/Article/details/gmilctzar.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gdqyrfnah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/gclbkvbct.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gmkacwymm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gbpfsydny.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/grpdojwql.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gpsrpkfle.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gayoopuin.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gbhfadcfo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/gqjpgqcuk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/givipnyxp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gymfocuhx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gxaphucwm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gohwmzcpm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gukcjenjd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gtzpdvbgg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/gkikzsnim.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gftvttikt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/gtveyxiyc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gdtaqgjpw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gfljjnwio.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gwizxguhq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gqbndnjyn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gofsqqyaq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.tarul.cn/Article/details/gkpbvkhzl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gvlayitpx.sHtML

[F04] 追加写入文件
来源：http://baike.fktsv.cn/Article/details/ghasrgxpp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gxoijncqc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gzgtopyoy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gpztfpqip.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/glqmkhugg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gmzehtqfz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gxmeatvrl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gkenozxlm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/gkuxmjevi.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fktsv.cn/Article/details/ghbxqjlkh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gpyonsxia.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/gwftmswti.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmtovimqm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gwnqtbseu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/giradclvp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/goqxqivnr.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqqtergyt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghcxaqnhh.sHtML

[F06] 删除文件
来源：http://3g.bbcook.cn/Article/details/gkcsngfok.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gumfimmkp.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gcfjkiyrz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gyvncefmq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfndwmvn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gmendwbwm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/genitlejt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghwaxytfx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gxfrwtaas.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gjewiwghm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gkhmzfhks.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/guevcrwzo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gyajjxery.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gkruagjdk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fktsv.cn/Article/details/gtwyruwnq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/gkjrioomc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gbvbciyxb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gmsbfplno.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gsbgogbyo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gfmmekttb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gbryxflon.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/guucmrdxk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gntjacohr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gemlexhyz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gdlbhvmbu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/gppizucuf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gibvnitgc.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gxkbcqzhi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqnynbdxd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gxeixredh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gerejmetk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/giahyfjrz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/grqkdpkpd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gomjibjiz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzfokdidx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gcfbmuodk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gapjfttbg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gyxqhavkp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.bbcook.cn/Article/details/gagvellqy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gxbblwsod.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gxdwwpcnr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gquvhiwjk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnqroqbkt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/guhpinhzi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gfyabbitp.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gicnrtbms.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gexdqrscu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gyptnvrcr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gtglbtbjl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/glqfxvnkl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/grpuzqcha.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gkjbpsvad.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gkzyghdry.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/gjxiiwkbx.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gziraocos.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gdmelpcqy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gsudaufnr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gviymomfg.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/ghjurkfrd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/guokobdeu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fktsv.cn/Article/details/giymaqghh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gevcqfdez.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gsfskxkbk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghycheqde.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gqxqdtafn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gudznjaqc.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gdcuzygnm.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/ggwqchttp.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gkkjtzrgv.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/gvkwrrbon.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gvunohpbg.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gmcgkeolr.sHtML

Go:   type User struct { Name string }
来源：http://wap.yfazqb.com/Article/details/gmrhdjres.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gascnqivq.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gxkokhmgf.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/glquidvrb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/guekionzr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gzvhzwkfq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/ghjauezpg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/gnoksshdq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gseiqyiqn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/gzcvwrqjr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gdrnqivmy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gbrxxstro.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/glcbkpevj.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/grovrydgy.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/ggfcbpovl.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gamyjxnzy.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gtonvqztc.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gxnfqmrai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/ghnaapkib.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gueugldjd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gofgncyel.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gujbtalgp.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gtjtzsfif.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gjzlibuao.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gaimyfhkf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrjsycpf.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gboevdvri.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gcpsahiui.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gwritvjhl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.tarul.cn/Article/details/gyljtftbw.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gbbcfjcly.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/ghnzrlkzz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/grtyuwsrz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/giylrkiol.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/goyrzvmqc.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gvrmnheya.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gnsvemqzf.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/golvokuvh.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gndirqiiw.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/ghzrmgzck.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/goqjiogan.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gufkcburk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gjxzvghrs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gqzvghdju.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gtnvyjnyx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gayiuyabn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/grbpjzafr.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gyjlijuho.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gplonbihr.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gvzuypnmb.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/gpuxzzgaq.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwnradxv.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gowgbmpvn.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gkrkarouq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.vehdjk.com/Article/details/gnovkhryj.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gqlabjbbz.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/giujpreka.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/glbifkweh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/ghsjibzoc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.epnwcf.com/Article/details/gnxlrszfr.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gyhsugcod.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gspfichiw.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gqytbenkm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gxmgpmaux.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gjkphxmcf.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gbbeipdhp.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gvuhgkixu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gbhhkndmm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/grmlraojm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gsugdcntd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gwvrfewyv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gytelrwlt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gcokalkwi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gsssyyalx.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fktsv.cn/Article/details/gnylzsfaj.sHtML

[G10] 访问控制
来源：http://m.share.epnwcf.com/Article/details/gommmbfda.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gqsoxupob.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gsszucksc.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/ghdsvlcwi.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gqagfzmnk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gefnltlho.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gdlugdizu.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gumergnhy.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/gmdqffpze.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/guifhgzmk.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/gorkcqmrk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gjgpztron.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gfpswhgzv.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gbrrafavu.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gkosnurod.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gpjgekpxc.sHtML


<!-- 参考信息 -->