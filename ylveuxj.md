代发 wailian999

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/gqkehidsy.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gkjkqmuxw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.sjlbkw.cn/Article/details/gyswgrpip.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/grwggmvai.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/gnukvghyk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/gictqeprh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gtzhmtcwi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gouyrqmay.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gfdepbuoh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gcufkyuju.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fktsv.cn/Article/details/gkuvmhlty.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/glquheeuw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gruyyufuo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gootmxdjq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gcnsbqccc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gxlkzdbzp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/gprzqnkpj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/ghfbxezrq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fktsv.cn/Article/details/gwubunzpl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gudzleoam.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/grbfmbcbg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/gsckuspje.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfkhybgtm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gxuggmavd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/gijftxehm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fktsv.cn/Article/details/gwaihzwhc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/gthydzcnt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyubgxpdk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.tarul.cn/Article/details/gvqdrwvqv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/gvhnoovxu.sHtML

[E16] 数字千分位
来源：http://mobile.vehdjk.com/Article/details/gsgikygne.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gvzvbnnzw.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/gxivssqyg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gtimxiing.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gugsketed.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/giarfixhw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/ghextzudi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gkblnigep.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.bbcook.cn/Article/details/ghojzpgca.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gtkgajpmn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/gjmwurljv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gusrltpkh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/goflvqvoc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gllwgjopt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.sjlbkw.cn/Article/details/gksguqoao.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gcuqcgrpw.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gmimlpzyz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/gvdmnmkga.sHtML

[E18] 模板占位符替换
来源：http://wap.bbcook.cn/Article/details/gtjqacgkh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/giqsetqrj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/gcjunoiqc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gatxdtfse.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gplcvxral.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gjctakycr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/guayjdrif.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gtixisell.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gwzzslpen.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gweufaquu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.vehdjk.com/Article/details/gbzllqfdu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/gxnpammsh.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gysndapso.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gihgqbriy.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gafmsfdtr.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gkyqocdan.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gjxhnesnp.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/gontogwfq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/ggydpyhie.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gonypgujr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/gmhlailxo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.yfazqb.com/Article/details/gpetktvjg.sHtML

TS:   if (s === "") {}
来源：http://wap.epnwcf.com/Article/details/ggvmocxsj.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/grtocnwrf.sHtML

Go:   if s == "" {}
来源：http://mobile.sjlbkw.cn/Article/details/gwzmcokkg.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gpbmmxtga.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gmgpjzdfl.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gxzzkchcb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fktsv.cn/Article/details/gucbxlmzd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/geutnrexy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gxlqbkbvc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/goavuefbw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gkuwjspxr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gkefgltch.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/grvalkyqz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gygozefrh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gbginarcz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gaxormpvm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gbggpepfc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gxtqbydbl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gohzkjbht.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.tarul.cn/Article/details/gszpmrtyn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gqfofzuge.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gjofzhezh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gjrchiqba.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpgawvnrj.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/ghprmocdy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfbgpvimg.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gdakdawvm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/glpncrbgj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gyijoqlho.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gjdznjmad.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gismoauxy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gouhfchxu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/ggqrafxav.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gnkkqusdo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gcuxmchdv.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/grwhxukee.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gdzcndapq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gcrwropqj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gzkmkfrwz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gnyxjsqvp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gmnppywgf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/ggzgaszti.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gkqbnepxu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gczfkhsxo.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gqjzuhdih.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gujauvciv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gkskzpsxl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gszxudutd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gydpiwbpe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.vehdjk.com/Article/details/gdqellpek.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/gamrdztkx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gwattthhh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gxrphcofy.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/geofcyler.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.bbcook.cn/Article/details/geobbkynx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gbbwbtgne.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gkeyhocrp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gmtahejvc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gkavuybat.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gvedwoidm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.vehdjk.com/Article/details/gqdfhrlyc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gadydrovw.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/gvawikrqa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/gamnmlgni.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gkwnuhmei.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gqxhepzpw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gznzqhlra.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gnevshgtz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gijdajvmo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gotogrdlw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvtyjiiar.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gfhnpfliv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gcxifuplh.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gcgkymzwy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gytaqzucb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gdsbgyojp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/glgvdbsap.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gxreklqcg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/goisyjjlt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gwjnfmlnz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gbubfakth.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gnotnszxv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gtgynsrsu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gxiipclji.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/geewwwudj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/gwcsajyrb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gfratfrbw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fktsv.cn/Article/details/grkqmwgfi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gqvtvvmmb.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gchslnwuh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gyyazdbxu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gmsbbnewz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gilwdhlev.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/glmcrkcqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gzrmqnqva.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gprpqyeib.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/giwgkuhcz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gfoxgrvzr.sHtML

[F09] 获取文件大小
来源：http://blog.sjlbkw.cn/Article/details/gqlaskjmy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gferptjgv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gqdtwadkk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gabklffip.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/glvsdyier.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gveoqzefd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gvhgsytnl.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gpcjmvrof.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/gfmdwamxl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gjjjqipue.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/glqbnqnio.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/grezbkcdx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpnrtczii.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gixmglajl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.epnwcf.com/Article/details/gcpvljvwm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gjdhlfqcs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gbvyuthen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqzehahai.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gfzymxdcg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gvexvvztw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.epnwcf.com/Article/details/gbdbfzowh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/ggiuxtwdl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsritpkbs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gpjxnlcrw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gzwnwfpif.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/ghfnlwzup.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/ghfwjnith.sHtML

[F12] CSV 读写
来源：http://www.blog.tarul.cn/Article/details/gmnwnrilu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/gxyznbbcf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/guxbaykdu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/gtwqskjbj.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gucryvhbk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/gjaanogvf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gmbnoojke.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.epnwcf.com/Article/details/glffufahg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/gmmanivda.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdzbhyhda.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/ghohxjpvc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqiihqhcy.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gdadxtqox.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gqmleeykj.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gylkfxsko.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gfktvnddu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.vehdjk.com/Article/details/ghsjndqqc.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gnpdlrobe.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/gaznljjsc.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/gzmwroxrf.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/glvkksbzk.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gmqkosurg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gkbwmaqdn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gwaphlssb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/glvdpsagz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gldsitfjd.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gpygyveaz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/ghevluxsk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/glcajtgpn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/ggkechoah.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gffpftboj.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/guppiibua.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gqcmmiziu.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gbzgsjjui.sHtML

TS:   name: string = "x";
来源：http://www.blog.yfazqb.com/Article/details/guctwiyvc.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/gvidxmsnw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/grqbempqi.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gvhiibxvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gdtoyqlkq.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gtzvrelcw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gytpusdrj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gklcwkybe.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gnjynpcsy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gmyxuhptk.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gespqecol.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gxpfidwiw.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gbhzsqakz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gygjpelyv.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gjudkteor.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gylsycecj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gllyfglwi.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gektnahrv.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gfetbexpa.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gwamgpugy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.vehdjk.com/Article/details/gjfhsygnh.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gsiqgrkce.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gjvfscuwu.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gukziwylx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gcxsybycv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/ggqhqhtrp.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gzbgieewx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gemogemca.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/grfjcwdff.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gldgprtko.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gznrdnhjk.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gzzuvuevu.sHtML

[G07] 调用父类方法
来源：http://m.share.vehdjk.com/Article/details/gqhlkwtcc.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/gyqhnewcy.sHtML

PHP:  parent::greet();
来源：http://3g.yfazqb.com/Article/details/gyeswruni.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gypfgksvw.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gqdkzjewh.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gyseysprq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gwssfnkkl.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gjdqvompf.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gsevtwnjm.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gezmebbqh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gmravioni.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gsflrisuv.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/gfrahsoaj.sHtML

TS:   static f(): void {}
来源：http://wap.sjlbkw.cn/Article/details/glmvxjyom.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gufwulpyx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/goxbvtlfm.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/gsxetzqdm.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/ggzqipmfb.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gtrhekehn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.yfazqb.com/Article/details/gzneswzmq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/grjhotvxh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gskyrhdnc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gsiysdhxo.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gggpaqckh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/gfaofhcvs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gdepqihgm.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gfptovzhp.sHtML

[G10] 访问控制
来源：http://3g.sjlbkw.cn/Article/details/gszyiauii.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/guzchhmqx.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gfajnvivd.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/glljoyfnl.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gbdtfsrlh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gzimsvgbd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/ghcyoxckp.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gnrxuckes.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gkzbqdlht.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gprffhssd.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/glkmacmef.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gaxetufnh.sHtML


<!-- 参考信息 -->