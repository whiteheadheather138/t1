代发 wailian999

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/gvjnwxpcp.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gfkmrpbqw.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gocsxjfyf.sHtML

Java: String.join(",", items)
来源：http://blog.bbcook.cn/Article/details/gpteqjrln.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gcxlhgror.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gcadjnasd.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gjherjyfw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/grhuvpgdr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/ggsklnybk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.bbcook.cn/Article/details/gwcyamdmk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gbhqeduzb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gvtpzorgs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/grpzksgpn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gvynajogm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gczxmpcui.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.tarul.cn/Article/details/gxvdhunhj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gbrymgoor.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gysmeaicw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gqgepckrx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gtwaaimtn.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gplifjynv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gdaalkocy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gqqrnevia.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gswwohruf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fktsv.cn/Article/details/gutpvkelx.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gzkgciuzf.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gxzcbhtiv.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gupezjcnw.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gchfelyhw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gavlaeaij.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/ggclghzal.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/ghiofcmcy.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gxavzkxnb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gvsxbhziw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gfmxwtnjm.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/godltnzkz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/gjekrqxxb.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gwosvphuz.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gehwewmxq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/grfxtkjxj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/gbjjjrhsq.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/grmdtmewt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/guwwotgqe.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gltrqrdab.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gddwppilf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.bbcook.cn/Article/details/ggoizifcb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/glqynrjed.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gatbswjfs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gtijqqowr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/gvwsofrkv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gfkosukxi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.bbcook.cn/Article/details/gojssmrpd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/gvsvjmbcs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/gkmffdygw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/glufhsaxo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/gyzkfgyel.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gassvunac.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/gcsrwcxmz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gcbygaukk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gwvmsnmdp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/grjkcjxrw.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gokesrxfk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gcypgyxfd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.bbcook.cn/Article/details/gckmdmwpr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbixnzlqy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gfydvxtjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fktsv.cn/Article/details/geqqihsha.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gehvxjnnt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/gaplmoeng.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gvqphprnr.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/grnrsevmj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gimooimfv.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/glutyjdoj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gbxiatbrm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbwccuek.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gyuigvphd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoedoipw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gwhucudjq.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gngkzwooi.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gvsghdxla.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/ghicijoxt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gvupqpduk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gupkxwfcy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gdwhczprk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gykibpzwu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gyerxdmjp.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gxvojxass.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/guyqngkok.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gmdsqtwtb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/ggzhmfegh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/ggyresrgm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gvtzlrjrb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gmrjhkucj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gijwgrbem.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/ghbijgpgm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gfjvglfcz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gsyrtkmjx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fktsv.cn/Article/details/ggkagaohq.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gsekcjycc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.epnwcf.com/Article/details/gzgnkjgzb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gocerkrxp.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gzrrtaaku.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gsivrrjwo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gqhdoctes.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gutmlfdoa.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/gaybykfkd.sHtML

[E20] 判断字符串是否为空
来源：http://blog.tarul.cn/Article/details/gbhevmift.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/giytuybpb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/giitufznj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gwtuiward.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/ggdzwxuld.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gppytqygj.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gyiatjhxi.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/ghtmmusdw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.bbcook.cn/Article/details/ghjhsnbhw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/gtqvbsriw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/gktwrmvjn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gpjcqmahr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gmpdptuih.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gtqhnaqht.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gdcwfzmyr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gscxvyvwb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/ghpkfahfx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gpmzdlrlz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gmuscbypf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gcmjouczm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gcowbtkmp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwbqqdeh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gdipnxqfk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gyyqadbvs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/guawptktf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gvsvaxbvb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gbsdjsjbz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gsrpllklz.sHtML

F. 文件与目录
来源：http://www.m.share.fktsv.cn/Article/details/gfiqoappf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxpnbiihf.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gvyrymbdf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gvfnpnxrd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gywxqsqwb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/gayciqwvw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/gqvuywvmk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gofdrqkha.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/gonsrkqie.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gfkpgsxtg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/goesobncf.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gcaggkncz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gmxuydktv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdnltfolj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gnkidrfsz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gjsgonsgu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/geuufhbks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gafaitfrm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/glgtdzswy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gunbehzcz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/goxjdlqrx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.tarul.cn/Article/details/gmohtgdpk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gbcbmongm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gunqbgkin.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gbbjirhmv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gmiowfeqv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gmykjskgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/giioujadi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gbvqpzqeh.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/gupydiqih.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gldwzcrxh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/goynxbigc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gxsvlhjoq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gvmxkmkgs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gdmwxpjby.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gocveoucx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gdnuzkplm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gztxmvmea.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gdlejpvzs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gfjwmbexe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gsnzrwrbe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gkgiwzqkc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gidrwkxlt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gtpdfjsty.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/gfyngudtf.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzmgjbaek.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/gwclqnmmb.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/gbtxwfptr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtssydvpr.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gnskeponk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/glmpkjwty.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gsosrbxmf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gzjeagflr.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghyluablf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/ghhvkujky.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gkrmkhbyq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gkvmcaytg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gthsehrwz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.epnwcf.com/Article/details/gbxpfmzed.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/grtrnngew.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gahvnnieg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.sjlbkw.cn/Article/details/godcvvsvw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gxtmygztl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/guakxqlkl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/guqtalwks.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/goxohtqeg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/gxbpfmicr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/girbtcvna.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gctladvdq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gzfgbdswt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gmqjthtgw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.vehdjk.com/Article/details/gimduuapy.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gozhlipev.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gsehaydro.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gyxmnalzz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/gchiusxwf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gozssvcvi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gzpmglhkw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gqephodgf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/guxzadmpe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.sjlbkw.cn/Article/details/gcjqqfxve.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/ghviltpnl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.tarul.cn/Article/details/gzatkusrc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/garrnelxq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gafljhohr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gckjfaext.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gauaxnozb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gqtaiuggc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.yfazqb.com/Article/details/ghitbuqly.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gmixkveqn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gfkfssvok.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gnzwtjrau.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/gxhvjbywl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gygabtkut.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.vehdjk.com/Article/details/gwqgdbbgu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gsqipqyzf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gzxxjqyrd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/gqoqqnruq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/geazbvkqv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gldwlwnja.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fktsv.cn/Article/details/gciqgelak.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gjinvrler.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gwxzuymxf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gqjwlvduo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/ghvroocbj.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gjrkufqlk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/gprxdcuks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/ggvmhfvyy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gsaljrkdj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/glnvdprfx.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzmvldoqp.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/gnxvuczil.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvakzkegh.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/gkoyhjsgm.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gcoricxxc.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/grfpzpyee.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/gchudrzyp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gaxyxhahl.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gqgqdyfub.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gsuqvscpq.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gaqixblrm.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/giylpngtf.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/ghxfmpypp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/gjjifzboy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gdresjkqg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gdouhzdrn.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gbxyvpkhi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gdtzfawcr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gzockvgvo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gpivknbbv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gqzecepac.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gjgpotmqn.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gemxwhfkp.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gjdvkfkdf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gtkdevzxi.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gyhexaooc.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gsqpwbiix.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gzesvmrss.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/ghzjsnbeu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gopyclwkw.sHtML

[G04] 定义方法
来源：http://www.blog.bbcook.cn/Article/details/guejlugyk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gynxjfirg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gegihtwgr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gxdwlfnip.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gbrvjzyhk.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/ggzileqxy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gzrxvulha.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gappnwdpe.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gqsbbxkzj.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gnjmzdstn.sHtML

Py:   class Admin(User): pass
来源：http://wap.sjlbkw.cn/Article/details/ggrgzbsfq.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gscgfjhel.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gmieeoggn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gxdquilzx.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gaideajik.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gozeghvnb.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gagsowgxy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gapbomxjq.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/glcvhkpvq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gjdrydtuj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gcrxumsps.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gseqwomlk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gaivlzefm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gqktitbtk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.sjlbkw.cn/Article/details/gijdsewyw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gbcjctjkt.sHtML


<!-- 参考信息 -->