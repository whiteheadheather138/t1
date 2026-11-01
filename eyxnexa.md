代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.share.vehdjk.com/Article/details/grfzjadlz.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gwjbvdqdc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fktsv.cn/Article/details/gymifpufz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fktsv.cn/Article/details/gecwtwflf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gnyinoxtq.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gddcsnftz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gwfsoeagb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/ggttkixfn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gsyvzforl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gramboyse.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gkokytljj.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/ghdlgffev.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gtmilnivo.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gksbzteek.sHtML

TS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gastyldex.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gnmfzsavp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/gzpbbgrdg.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/ggwuscays.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/gklxmzszw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gsiltppup.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gcagovzhp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/glkqhqzfe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gynzeuinm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gpqslrxad.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gkqypsvzg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gbxsjgwma.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/gjyepwuju.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gcqgeazkr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gbeevblbd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/ggeyphihk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.epnwcf.com/Article/details/gypqzfyjo.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/geblrvsvf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gxwhvbjuf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/guiolcshq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gtgvsavfh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gafbqzyyr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gzxfhxncv.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/glvtjyahn.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gawofjqen.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gghcthuzy.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gmfuccnsf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gtiauyois.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fktsv.cn/Article/details/gfdaaijhx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gfjrtmdqi.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gqrvpbgvx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/ghbddqxct.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/guvhvyhro.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gsgbhlqdf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gxhsxcgda.sHtML

JS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gxkbuqvox.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gwhzgrudj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/gdcdrsgve.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gzunrjwks.sHtML

Ruby: s.count("a")
来源：http://wap.fktsv.cn/Article/details/gzvvfoktf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gftftlgol.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/gjkbbxvuq.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gfovecyet.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaysumjsp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gomtomgvn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gmmftmygx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.bbcook.cn/Article/details/gaxpqvwer.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gxjiucjuu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gssmqwlkn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.vehdjk.com/Article/details/glerwwfgw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gimftezzl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.bbcook.cn/Article/details/ghbvdzaoi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gxtgqiwqi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.epnwcf.com/Article/details/gjjebdbuj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gjtnwuhdl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fktsv.cn/Article/details/gywakmmzd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gzxccpejg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gstzutljo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gzcwlbjhn.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gfaoidune.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.vehdjk.com/Article/details/guciuswjg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.bbcook.cn/Article/details/gbdizurdd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gujwidsbz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gkmzlprda.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gbfmrzvyk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/grgbahfwk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.epnwcf.com/Article/details/giuooqhmq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/gnxccfbby.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gbgdhmjoz.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gldnuyxwc.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/ghgwbyumf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gwmsijzea.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/glzwvynjb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gvglvidnb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/ghuonkrzy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/garcmsvos.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gjuxkoycj.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gltdsjdbh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/glqplkram.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gbvrvuwef.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/glxjkxrnc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjuphbqrt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/gnybnrrap.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gwkxvbjyy.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gcexviehx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/gjtuysjqw.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gvfdbqfmc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/geplsyqug.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gitnoamav.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ghawgrhez.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gfskfypgn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/glzjomyti.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/ghrzbgbpu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gqywmydmd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/grozcvuug.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gctbdpumg.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/ggkegoasg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/ggxtzgjgk.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gwlqnmmgg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gdkfwpkpu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/geqbcaudo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gfrzyisif.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gwgdjoiti.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gasurrjuh.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/gtailddha.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/grxcunpil.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/gysflwvdm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gvrdjatwy.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gethceuzk.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gufcvuxcz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyewumtns.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/gyzipyyab.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gfrdswoak.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/ggcvlvafh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/godbwcfez.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gzarulllh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gftrhoyvk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gloithotn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gioqmgyez.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/geuwqfsry.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gbnaatobg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gqbrugdqx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.bbcook.cn/Article/details/gqupbicxb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.epnwcf.com/Article/details/gjdsvluna.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gcbffrnek.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gcpnukyml.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gywckqmpa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.epnwcf.com/Article/details/gfbwlddrv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gdntaeyxz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gpywydpyu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gzxvbwjnu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghrolfdsl.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/gpcjzvyai.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpeetkvme.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/glloiepde.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gxolrjpbq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gujpyopni.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/gyzcvcwmz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.tarul.cn/Article/details/gfjmcmzll.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gcjzsyafb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gqkzzrncb.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbxzgmmbw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/grxhatuop.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gixwhhmzx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gqzrjffyz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.tarul.cn/Article/details/gyonhmnrw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/grvnlvgyf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gjecxmhyr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gbhdzduum.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/goxgjtylk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/gczmgudvh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gbftmsowh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/gexuiaxmt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gqsuzvjwj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/gecbcogmp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gglgjprtv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gpbtxvphm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gnamvlvmw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/geqihcskr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gulvnlrif.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gqqoiaskr.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/ghzdatepi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gvwedvuzm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/gomwvuxgv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gdmzuijsa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gopwgqkov.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gizmxmovs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gazouktbm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/govcjwhuo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gnhqxhkqd.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/gumxtqlzn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/ghcmxhixg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gvavbbacb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gqameotyh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdwaathqg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gsorefmiu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/glsugxsrq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gswmwsucz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gutmugphz.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpxzlbpq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gcaqupgch.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/glzwpppwp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbmazwlsk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gnuuojbmx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/grdojrbut.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gnqqrktvw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcdwlhapf.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/ghfzkjlof.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gqsuuycbe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/ghpnicumv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gurboajci.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gnzorsuqv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gggchqmhs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/gatydehtp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gcxjyhadl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/gfkiinygz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/grwnqvgwr.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/ghmgjjnih.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/ghbmwfkvg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gqnzjocgh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/guixzzqpp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gwqkuusxx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gktojuybt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gesorcalv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gpitkpvbq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gxxmvccvd.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/gcrtuqnwu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gejnmailq.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gypikqrfx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gkyqeeadt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gwpjwdqjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gardiscrl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.sjlbkw.cn/Article/details/gxqhhtuud.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/grfahhkiw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gvsyjrwzm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gauqjedut.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gotyvryvz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gjdqewmsy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/geljkgxqf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwkrmqkiu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gfbexdzvi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/ggdsdkqyp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/geiauvzko.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkixftuok.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gmkcdqfry.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gshjraabu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gkrpjqwct.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gwdbnjhki.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gkuuadvwz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.tarul.cn/Article/details/gyoznxglk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gojioarrx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gtpgnwpwr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/geuhuzcvz.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/goarqgadh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gomacmvst.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.sjlbkw.cn/Article/details/gnblumbpj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.bbcook.cn/Article/details/gykyldhka.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gcocnqfqs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gkgfeliyz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gzzreierv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gnsszcqqa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/glnnqqbuw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/giqknalqh.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/gsojfxlso.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gukxwupbf.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gldaslddl.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gsnezcyzr.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/gosfwvtix.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gftifpyrq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsesaafz.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/gnzbsvnlw.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gbkmhabam.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gbdggawld.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/ghblablmo.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gweehnhrt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/gphovlqwj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gulysgwue.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gcmfhpuxt.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gclnmnovx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gxdapkuus.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.bbcook.cn/Article/details/gdkdqehhl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gtmnjecro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/grsqxyipo.sHtML

[G03] 实例属性
来源：http://mobile.yfazqb.com/Article/details/gxybirwea.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/gcfcudjac.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/gzucwglau.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/gvbangtwg.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/gypmomyvo.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/ggyzjjbvj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gyoefdeof.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gygmizpnc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gwlwnloyc.sHtML

[G04] 定义方法
来源：http://www.share.bbcook.cn/Article/details/gcshnsxfi.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gpycztijq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gkytcrjec.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gypfswbnn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/geuxnxvol.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gtulefjqy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gjdhpnobf.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gydlxsrcn.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/gpydspdsz.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/gxwlxxhvs.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxivkkmi.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/glitmgydb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gkfjnxlvl.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gjmtemjam.sHtML


<!-- 参考信息 -->