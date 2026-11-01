代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/glbstrney.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/ghyftqfxa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gxudhhitp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/ghngseqet.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gsnpidehs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.bbcook.cn/Article/details/gsapkzgek.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gtjcryoai.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gqjjisjec.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.vehdjk.com/Article/details/gwgxdpbnp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gxtowxcpc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gyvhxutia.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gwtkruosi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gklzjyiuw.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gcgonhzlk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gyqykofoj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gbqtmmlka.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gmkqkmhyv.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/ghxbvbhnb.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gznwfdmkl.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/glzphruzf.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/ghgcqfpvx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gldteodxo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/giunzxusj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gszxrothi.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gqapiiehu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gdtxvzqnl.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fktsv.cn/Article/details/gwnvtvqyw.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gzwihviey.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gymvbxwcr.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gnchggqyp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gzehbsyfi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gwrixcjrp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gmwsifure.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gpcudylzs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gcmoicmuj.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/ggrmuniea.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gbjbuujsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gzfsawdnv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gryrgtupp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gqsgwfvgn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.yfazqb.com/Article/details/gjguobeuy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gaxlvsfnm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/ghsemtlhi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gjfmxemcl.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gsbjagxiu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gnshpdcoz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gjclbzght.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gqcghbtmj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/glmbchuae.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gvaqydtte.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.epnwcf.com/Article/details/gdixxqlum.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/gqjjlnntb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/galvzykhh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/godhyvtzu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gnabtihpa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/glcofodqa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gkoysetbu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/glwdmrnqa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gkvurrjnn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/goevtrmyx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/gsvxxcxzr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwbvyilll.sHtML

[E16] 数字千分位
来源：http://www.share.bbcook.cn/Article/details/gsnwttabk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gxrujzjqd.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.bbcook.cn/Article/details/guqlrtmlc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gtxknmjlz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gqnmvnton.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gitdgvzwc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gkbfplmdi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gbzchsrsr.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/giqucgyeh.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/ggnxpwtsi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gcmemiyrp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/glsarqwse.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gyngdmafg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/graulkayp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwysznidc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gemgkqzgl.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gxbdzzgls.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gizepdpyr.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gywjnkdke.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gbotknwor.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gzztgotet.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gzkwxrlnu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gxpsnbbtg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gqjzdahfm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/gnthyixin.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/guegwwvtv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/ggjneoydl.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gfjpxlklv.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gvrhocbkj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gjvvahctz.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gszvhgqyi.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gbkrblwdx.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/gkzlxmivc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gbpbhjwea.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gqynjykbb.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gztkupazu.sHtML

[E20] 判断字符串是否为空
来源：http://baike.sjlbkw.cn/Article/details/gwdtolage.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gsgvgdbac.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.vehdjk.com/Article/details/gpzhprhie.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gnlohlsxm.sHtML

TS:   if (s === "") {}
来源：http://mobile.fktsv.cn/Article/details/gdchmhidm.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/gaashqgrv.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gjfzinkcv.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gshwepfmf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gblcoyyqf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gagtuusvb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gckqitiqz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gfvofyjnv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gacwauopv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gktngeatd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gmknhktxr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gkcxhmfoq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gxvedteys.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gmkshqrrg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/ghchgbnpi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gyaapfbgn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gpzibjwmt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/ghdthztos.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gsjsruyuv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/gzwuajppr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/gyiatjpes.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gdlcvhlym.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/ggfkqintl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geecjxazw.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gwniabowu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnvwnstcr.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/gbifycefl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.sjlbkw.cn/Article/details/gtojtklst.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/ggphkzdhz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/ghgaoahlr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gndjkivtf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gusggsnqi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gxjapkata.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gkgyjgjnp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gtwxpgxob.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gsezrbmpd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gbqaqgdct.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.epnwcf.com/Article/details/gisnluivi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gkbnlwoes.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gtprwutug.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/ghcfdupqt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gdhysbnay.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.bbcook.cn/Article/details/gclqxanfn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/ggedtwqku.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gnxyufkpu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/gptaqgfej.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gdkzmvkwg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/glcihxjhy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gmrtdswrx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/glzdczcos.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gprmclamn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gsfjvyjjd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gersyjqze.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gaswexmzk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/gbxfojzqj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gjmxchrie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/ggtinmhxw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gwcbarpgc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gpetdrbaq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gakcdnasm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gkuqcspnx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.tarul.cn/Article/details/ggryisabq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gvgvzgeqp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.epnwcf.com/Article/details/ginheskbz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fktsv.cn/Article/details/ganxzswmz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbruwsswh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gegscfekw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/ggggjvskq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gytkxzbtj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grjtusdxz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/gczlixbom.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gapdteaer.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/geccntpjv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gpvwblwps.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gwkhipmjb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwrhkydtd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gknqhcqkd.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gwetybggz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gumtfmfxn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/ggkjzzjci.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gsrwrqkaw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gcicggury.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gejwgpnja.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gyoogvupu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyejkprj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gukjrmtlt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/gpmrcteym.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/ggdlskqxg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gifupbwyh.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gwflaefcd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gpvhwfnwr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gmrkwopdp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gcgyjtzzx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/geuzpepsh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gdobwwhti.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gfzknwbaj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gwqiuorup.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/gxdqhlpdm.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gohlhmhtw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gtbwizqqx.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gpdrhxbak.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gazhpqujo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gmtckzegj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gzanrxyde.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gdtywchjz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/geneuvrqq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gzygnkpfu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gxouvnxsr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/grhqsnlkz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/gxzcplkil.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/goiqmkich.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gxiuneifl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/gcgfahpoj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gamtqcdtg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkvwbviob.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvlanyfmc.sHtML

[F11] 复制与移动文件
来源：http://www.share.sjlbkw.cn/Article/details/gqvxhfqfb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gpykxgfxn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/gfvgcfoxc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/glawhgyon.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gxqlfstpr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/gkmbtrqdd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gkgxfylno.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gesjuffsn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gtcxtycpd.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gkqgplhae.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gyzzzopfz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gbbgiuzpj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/glrmbiela.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gfjkpazam.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gqucdwetc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.sjlbkw.cn/Article/details/gqijmamys.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gyuaaeesj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gkbonwtwm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjiybqdlo.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gnaqlsypt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghgreuwih.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gbybpicws.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gzypmhyyu.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gzbvpnbfz.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gzfmewrul.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/grongapou.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gtipsozrx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/gvymaochg.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gvnjncvof.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gyqarfwut.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gsluuspop.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/goygnjndf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/ghdwfasnb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/goqwskczv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggiijzkjt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gifoonqcm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gwithsenk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gofgaeikt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/guknkfies.sHtML

[G03] 实例属性
来源：http://mobile.yfazqb.com/Article/details/gmcuukgld.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/gsdzfumka.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gpjhthswa.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/guvyeiyoe.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gldpazljz.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/grqmuuzdb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gnnsbjuct.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gvbqcdmbw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gpvxwbrbo.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/glaapnhrz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gddmgyvur.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gxczmdncw.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwwvrcfxr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gfldodhoe.sHtML

Java: String greet() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gwqnuafjn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/ghauosdfu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gsjovigah.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/gipurzjzm.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/ghkwwrifh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gkhjauflb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/ggnduxsqo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gqojcmhxq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gjxmpxhtc.sHtML

Java: class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gnutodelu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/glffkdayv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/geypuopks.sHtML

C#:   class Admin : User {}
来源：http://mobile.fktsv.cn/Article/details/gwofegnzy.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/ghutruwle.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fktsv.cn/Article/details/gdaxqtpww.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gmqcosjkz.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gdsbmrytv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkoscilop.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gmjjvrynj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/grqjvojlh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gxpunrlxb.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/gajsyfnzx.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/gavgvyqwg.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gfdsynbhk.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gbwnztghm.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gjihcnfaq.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gbjlhikvw.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gfgcmbvva.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/gbfhghwvl.sHtML


<!-- 参考信息 -->