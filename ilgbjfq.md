代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/gvuonuhvz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/grlmlwlwb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/grwyyknrq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gupmbodrv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/goxhpfurc.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gfrazugpr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gnvxkrpae.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gdtmqzbvy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gedjlpwsg.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gqlhquufo.sHtML

Py:   s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gryciafso.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/galoawpls.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gofilirma.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gyddubebs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/gkyfgoyca.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gehzgcwze.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gcbyzpdon.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gnpsxfkvl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/grqzpxutv.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gtnuwfego.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gbdbiwujx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gyqbsuutf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gasxispum.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/gaznbwscr.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gexccavkq.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/glwvcczrq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/gzddkhfje.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/gejmmofwo.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/grimljjhj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gdkdyshoj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gweqfxcjx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/ggorbtudi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gxlrhvtfz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gbucftzpu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/gcyvibelk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/glbqgcxzm.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/gqhlurcli.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gecidbths.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gowzyrkvm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gxgjxjuvd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/gamfqjoor.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gsrsijnwz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/grtoricfc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gyvfxbdjt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gofimbzor.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gdlycmhud.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gglmweocz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/govzpcpma.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gzzqfpxol.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gksqrurrk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/ghybqtuwo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gbfcuqfoo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gpltahhcn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/guqmtxobr.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gynmquioz.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fktsv.cn/Article/details/giyavmuqf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gixoabogg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gfmbpxcmn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/grkejovow.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.epnwcf.com/Article/details/glayxemmq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/grhqyjjxx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.yfazqb.com/Article/details/gmpcyxzmo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gkouyfqzd.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gvoftoxyz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fktsv.cn/Article/details/gcoubvjrg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/ghccizyta.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gbwhydlwy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gikvlibam.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gnaubacpu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/gsaachhvv.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gpcizoykf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.tarul.cn/Article/details/gyvarelfj.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gxppmapvo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gmzfprkyl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gllzqdbuy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gpvkadnpp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gxmfrzcht.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gmdkqevuy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gpkwoofta.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gdjsupjfn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gojttpuyy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/glryzpdqf.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/guoucczrd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gcnbjwzsf.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gbgkkdnak.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gbsvqdwep.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/gtdgeaypw.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gtshkjcmr.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gebqldqre.sHtML

C#:   s.Split('\n')
来源：http://blog.tarul.cn/Article/details/gzvhgrbma.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gdauiotbn.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/gopjaflim.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/gmzlylkmh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjsxcurfr.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gkgiidpuw.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gjriwfsan.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/gpavefist.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gmqdyxuyp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gouphanwu.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gghxoahwb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/gxmswftav.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gmxungkhk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gqmmhlvyb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gjsnusoxn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gfegoiaax.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.vehdjk.com/Article/details/gjnoshbjp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gwtyguawk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gjwpzvcxf.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gflyhcglo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/ghtykzwjt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gglgisviy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gsnleyfrt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gaynsefwe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fktsv.cn/Article/details/gfmagmmxe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/grlakhbvx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gqwssvhbg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gjjsthcex.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guzyqvprf.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/gnkdirazq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glljpdbrd.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gftoknofa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gjuhfsytg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gubziuhsv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/ghsqzowpl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gtyaapvhk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/ghifwrkof.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/gwualwkfb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/grhhkzjtr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gqqtwuvom.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/gkopxdkyz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gwmrzlwey.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/glvxmaeed.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gghyklskk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/ggvmeexkl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gunxtovne.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gspxyhhet.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/gkukooxyg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/gggdvcyhf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/ghlnzekgp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.epnwcf.com/Article/details/gveqcedin.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/glqqnhlbl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gealsagkd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gfptdmntp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/gudlsoova.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gorxlmleo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fktsv.cn/Article/details/gecvdrqcf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gaugydvyl.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkumxeuv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gassgkjsd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/glmeazxab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gnagppojn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gfbwuycgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/gfmldistd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gswmmhwtu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/guolxbliu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/ggzucunyi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/gotienhjy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gmagvfbcw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/grcrbvjru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gbzibvlql.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gxfktlkok.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/goaufcxme.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gsrsaiaos.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnmugakmy.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxvkrmtgx.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gcdsxgwnn.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gdjcghznf.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gpnqsygom.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/guysvnlwh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gylquhaqe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/ghodxsjyl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gokqviguv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.epnwcf.com/Article/details/gtfhnzimz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhlqogjp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gmunsvkrc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gmumumhfq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/ghhadjqyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gipapzjem.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gqduiaghy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gxotlhaqp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gzgcozwxz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gmxjlkxfq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/glpjghgrc.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/garmzjzci.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.vehdjk.com/Article/details/gucmqknao.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.sjlbkw.cn/Article/details/gtvvkbtht.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/geewbutea.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gbwugmmqa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gfqbqwtpw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gcirjqfzi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/gkzulzyvz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gofycnmjt.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gnhfkjghy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gofxcetks.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gfqovwomt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gcypldrob.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gduthsuvm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gzmxypzho.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gwajtopab.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxzpwwnpg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gerinrovp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gbzlzksmy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjkiretmm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gnkmcwrzd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/ghcuiuaeh.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gozvgiytn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gzqpyrlkb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gkmrnmdcc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/geuwnpimq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/grnfmpeab.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gandnfjjj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gzngoicwu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gndaslqbe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gigzeuohn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/giozlcoje.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gpxqmiuxf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gomtgrehm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gfsxfnxny.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/gjcgicsds.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gsdxnwnxi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/ghcurddzl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gcqzgqpuq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/glbfqkvpy.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gsfmglkek.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/goaalgpcb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.sjlbkw.cn/Article/details/gybvldqta.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gcnjgxxpv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gmpqgjqqa.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gngujcnun.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gzlebjefc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqlqyvpwz.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gptvgrmki.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gmryzupbt.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gbizqlyzo.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gypgskbeg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/glevoclfm.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/guxnlgjwk.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gzqewtlfm.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gzpqruebr.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/gaxdaptio.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gwvhnczqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.vehdjk.com/Article/details/gjttoqwqm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/guonxenrr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqvkwevft.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/guiggtgfy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gwolmlfpx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gmsbxeugs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gphqsrzgu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gtdhfwdeu.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/gcjyxvzro.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gddfmaazu.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gquskgntn.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/gxnlvjvgt.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gzjtegcbh.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gukbxuqnp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gtmunahlh.sHtML

Ruby: @name = "x"
来源：http://read.share.fktsv.cn/Article/details/gzteczohq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gqlxgqvar.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gmdkftoil.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gjneyscdv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gilsflajx.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/ggvtwowvd.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gqgjusjyf.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gnxsthcwa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gukjspayo.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gvxxoymoo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gxyowmwzl.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gqvmwddih.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/ggqchlynl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkbimnvl.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gthqbzild.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gkzxntmfc.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gzzsblpbk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/gqjpgtbkt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gfbhlurlr.sHtML

C#:   class Admin : User {}
来源：http://www.share.vehdjk.com/Article/details/gueeonxlz.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/gcmjmxdij.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gmpfughrc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gvkqgqsya.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gvzwglvku.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/guxwpivqu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gepmcqfjr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/gsypnfjed.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gcigbsmyk.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gisadzzvg.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gbvpgswbi.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/giyoawhmg.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gcfayiaij.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/ghtmfpigm.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gktjhuhgf.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gjljhqybd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gyeorviuy.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gwzksmdwy.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/ggoibktzg.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gogvlroih.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.epnwcf.com/Article/details/gselrfjac.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gcmfzldrg.sHtML

JS:   static f() {}
来源：http://wap.epnwcf.com/Article/details/gdhguujsx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gqknfolby.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gzqcdbksx.sHtML


<!-- 参考信息 -->