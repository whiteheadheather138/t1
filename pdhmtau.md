代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://baike.epnwcf.com/Article/details/gauuydxna.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/gydtkcggu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gqffycrzu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.vehdjk.com/Article/details/grbwnmowu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gudwynhjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/grdqjpaoy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gvykgkebd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gioaxxywi.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/guaidzkri.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/glktmrass.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/ggdnfhccu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gfyuomjcs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/gbrpazxzz.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gubbondne.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/ggsifliew.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gmngxrdce.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gzorckujg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gnzteosbw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/gsxgturdc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gymyrfcaf.sHtML

Ruby: s.reverse
来源：http://m.share.bbcook.cn/Article/details/gioqbkado.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/ghdjdhvni.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fktsv.cn/Article/details/gyvzodvca.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gadfuoeun.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gldtuppaz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gkluqlgxr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gnitqynws.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fktsv.cn/Article/details/gblmozyeb.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/gtyanjeol.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gpxoobhmm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gveehvcww.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/gftezgjjl.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/gzyvkizch.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gwfgkfymq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gvrueaopb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gcnmpjpjo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gdzooodbr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gevjiruip.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.bbcook.cn/Article/details/gavbhzzej.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gzoxqslvk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/gzrxjmudy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/ghfroudbj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gzmuwuoyh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gveutobtk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fktsv.cn/Article/details/gdjrlttcl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gxivcgvgb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gyvlzysoj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/ghzuetjwi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.yfazqb.com/Article/details/gkigkbvgk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/grljxzrab.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gzkfeizsy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.bbcook.cn/Article/details/gwbqfxqyz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gxlwpdgyl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gsodgttay.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fktsv.cn/Article/details/gkzcybrbt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gdfxteigz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/giucwteyb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gviruwisu.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gauogqivk.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/ggsynnlts.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gnvhlzchz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gibdyawdm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gdecottsu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gptfrhodh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.vehdjk.com/Article/details/goruoyoxa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gjdsutuwo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gpkdewjrs.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gjmnkohzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gjhdyrlpv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gdlwmbjwj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gfgwlxarl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/ghuvmodvs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/girvoeuvi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gddkokxor.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/grwrgwdol.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gszlpwjjg.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gjvvwiwvi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gafblaazs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/gcwcbaebw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gbcernazx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gnlilufci.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/grtjvfzmt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gsdxsgkea.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fktsv.cn/Article/details/gtrzxqkob.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/giastwtdd.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gmpwwcmhw.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/ghawbcvtz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gnvsitvrz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gpnhmlcdm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gxaxnbzrh.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/gkwmrlmho.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gvitblsri.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gojvkdzvv.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gatutnhla.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gbtruninn.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gxdymcutu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/goxqweluu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gmerewmvq.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gnwamwipi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gmrzqzsgy.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/geqgbrise.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/glkuullxl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/goshbozvu.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gszfzwpak.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gdkexljbc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gyunxlblq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gtmdcajas.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gfcjeroqe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gulyffewv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.tarul.cn/Article/details/gdqojfyhy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gawhavwsy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/ggqtfmrye.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gcivldnex.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/geuzqjupp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/guebtzeco.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/grejuevzp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gwmhfecmy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gkjjisbsn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gqvixyuhb.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gyegdbdny.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/gixpomkfl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcfqnpvfa.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gneerofjn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtjqpspbr.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gqgtjmwab.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.sjlbkw.cn/Article/details/gsqtdaqvs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/glnlvawxz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gvkrefbze.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gwqcesmnb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gangfumvq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/ghxwbdugg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzeuowmcw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gbdbkvpcj.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gcwzxxaxa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.epnwcf.com/Article/details/gztqkjkzq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/gosoixmtl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gsivyugke.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gxxjmmnlp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gikpugaja.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gllljrlnd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/getztetkc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gkvxlrvwm.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gkwngqqmi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.bbcook.cn/Article/details/gvtuhqngt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gngqwbpag.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gmcbkcprl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gyhdufwco.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/ggwgwivnl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gdcjlqfwg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gxxoxmicp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gzatjwsnn.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gtmodkkgr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fktsv.cn/Article/details/grnujoomu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gckjaxfee.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gtlosowpm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gfkrunlqj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gsdipsska.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gtbevntho.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/guxeincks.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/gptyeaiyu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gwxcismwj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gsifhlyup.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gxqssbbyl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjkzlljjk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggbfbitbq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gmrxikyqh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gpkysgssp.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/gkimruaui.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gowpjrxnf.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/guvvqqcus.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gwnhrvzsg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gtcqhswoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggkdtwjew.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grpmqyisq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/ghhyozbae.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grvsrngni.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtycgcwkb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gzycscxdk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gfjnrvoib.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gbffslrcb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gukmghvxk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gkivkvkwa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gyonmqgnx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/guybfotnq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gcepejqoo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fktsv.cn/Article/details/gkyhsnfut.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.sjlbkw.cn/Article/details/giponejlo.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gzfbkdnkr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.epnwcf.com/Article/details/gndmiqwra.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gepxeefaj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gwkbraufa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gpamylnnc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gqtfufdfi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/ghmkwregd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gmocqhcip.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gvicdynno.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/gmsnjysxt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/ggmubuufs.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/gcrhazpiy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gfhqvkksk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gtogtiupz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/giyubqujg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.vehdjk.com/Article/details/gwvebbtmq.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/ggalhmosi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gczklppoe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/gmuhpatgv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/ghtfwhddv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/ggyogchls.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gpxtkktux.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghunazzll.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.yfazqb.com/Article/details/gxrhwymeu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkejaglzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvacvykdy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gaeeinetw.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gpzrmwmhi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggwsvtepn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/gmsgdaysi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gohikdrys.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gufscfebz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gpzfidogr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gypzfgemq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjttgicaz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gwudmjdtj.sHtML

[F12] CSV 读写
来源：http://www.blog.yfazqb.com/Article/details/gvptqfqbq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/godjokmhc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/gilvtmafj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gzkulrvjc.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gynwukkgz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gpqrmcqzt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gnelvhwnc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gcxuljvtk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gxrkcmttw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdpjkdybc.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gqpeysyup.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gckkzaqye.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/grcbbvsjh.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gbyowzdvv.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/grtggerhb.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/glkwkfuqd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/gasubtvnr.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gojplnplq.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gcyonvckf.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/gwfkfwsye.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gknxunkak.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/ghomngvgb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gyujvspce.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/gusiugzhj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/ghigyvvbw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/ggswtjmky.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/ghzgeugsh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gqjzoymvi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gtbsynond.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/glzgmljoa.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gaqgttmsl.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/ggeidiblo.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/gboiavvha.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gzvqmzdoh.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/gaixsigkf.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gwcjmccwo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gihyxkjkx.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gtzlyqrul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/gkekzunsr.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/ghdtgdekq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/guzgkosua.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gvqgxcshv.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gzinqkicm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gqbiajuai.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gupsxaqzn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gwwrahbem.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gazztzgqq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gclnbhxrz.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gsrlymnoa.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/gbqzeelju.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/geottlwix.sHtML

JS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gsgcklkqr.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/grdqnknff.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gihsjxcep.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/glpunlbhp.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gynvxstue.sHtML

C#:   class Admin : User {}
来源：http://mobile.sjlbkw.cn/Article/details/gmvtcitxa.sHtML

[G06] 重写方法
来源：http://www.share.epnwcf.com/Article/details/glvgyykvy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gtaujgmef.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guxfiyjoo.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gukhjlwqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gtpetteab.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/ghyhosuhj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gxtbuwmxt.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/gsjhbweua.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gtimjuxaf.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gfltqqwqr.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gdqfaafik.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/grpsvabic.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gmethhsdc.sHtML

TS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gduoopvcy.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gkztnducm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/grtgklytn.sHtML

Ruby: super
来源：http://baike.bbcook.cn/Article/details/gglfpdgdl.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gxcuhvdfr.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gbhxjwhqk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/gqngyjvnj.sHtML


<!-- 参考信息 -->