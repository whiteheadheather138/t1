代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gjthtgmwu.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/grqlunaki.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gexlxvgtr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gcwopolgq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gcqdfztyh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/ghsorbtof.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/gwtatsspx.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gughfcvwp.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/gfmsxbsdb.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gyzcucpor.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gwcrrkgbq.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gamvxqfrk.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.vehdjk.com/Article/details/gctbghrqo.sHtML

Ruby: items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gnlhyqeax.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/ggtdqllmk.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gmgpbyopf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/gxnavteev.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.epnwcf.com/Article/details/gcqpjmpcu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gpqvyiqzu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gomnvawwh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gnmewbwql.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gjijbffjp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/ghmoglfqe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gxfomspoi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gfvmnjpir.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gormhedwu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gtbsxhqos.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/ghbtdlrjd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gjosasmbp.sHtML

Java: String.format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gpktxwymr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gvfsvhtvt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gephpbijx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/giggmsjik.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gswukvsuu.sHtML

Py:   s[::-1]
来源：http://3g.epnwcf.com/Article/details/ghyypgtmy.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/gblpstxkg.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gdtahnqem.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/grkiawesl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/gyqborkze.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gcecolrgp.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gwmzgteyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gzfhiqbyv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gswmdknms.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/ghxblzwvo.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gdxyyutyr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gmzlrznft.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gxkdprbix.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/gfvcalril.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.tarul.cn/Article/details/gkisejtik.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gmvtxduan.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.vehdjk.com/Article/details/gyozuwbar.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/ghxgqcqjc.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/ggvedbltl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/gamfisbfm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gfnxrtjyb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gtygwjhif.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gvdezwabq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/ghlhbtdkb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/gbsrbpiww.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/ghrjlcuga.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gunqcejfa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gjouealyc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/giwfvqhzl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/gfkbixtpx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gxrqgvehr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gipetnrds.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/glrwbcdqf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsqkbevo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gbqxayxfj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gimxrlrpr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gfjlsaktb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gxcjvgpxm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gsyplupgw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/gtquzrbbe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gutqpijhj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjmmixuhh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/ggwqkyqsl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gsejdcskm.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gizvhejfn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gemewfvnn.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/grycqjuhl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gyuzvsqft.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gevaoqwrg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gypysnvwo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gwrrukxtb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/gauvttiwm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/gkwmqmaqx.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gezrraitl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gtuuksvpk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gdokmaopj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gvbkzwrny.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gnmbjkdgp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/glfxizluw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gkdbphfvq.sHtML

Ruby: s.capitalize
来源：http://m.share.bbcook.cn/Article/details/gfvrmkjor.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gtttczkmb.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/grsjgawre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/glzrlclhx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/goxdnkuxs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gmjswgjou.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gtvybheee.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gqxgosuoi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gncundvhr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gplzxuwvp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.bbcook.cn/Article/details/gjthhrzjx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gdpharpry.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/greyqwbfc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/gspkqauvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gtowaeyan.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gsahxhjlu.sHtML

Java: s.lines().toList()
来源：http://wap.yfazqb.com/Article/details/gazejurlh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gblnotjbw.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gtwiyajai.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/gztcswfjw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gqcklytvu.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gdfyxgllu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gjejspuco.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gjvdktglq.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/gdggflula.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/giweddega.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gmkxdzlzl.sHtML

Ruby: if s.empty?
来源：http://read.share.vehdjk.com/Article/details/gqpvhdomr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gukajkzzj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gysmzhrjq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/ggntmwhng.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gxlysfrkn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gvrxpfbhi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gdafntvri.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gsvjabenu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gwlgsrmlj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gnfmbzryn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gfxzgdiyk.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/giyozvwra.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/grrcuszxt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gfmspxgyx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/ghelaqekm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gakqrizru.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/grjgqqsiz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/gfabhqceo.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gltftdnqx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/gurmzqzhc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/guvoedfth.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/gpolezgkp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwgmmlwfb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/glrliefxc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gqrhoqmbh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gsodvtqya.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gkfbbialq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gykhfuvfa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gfpwlyvxu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gmuwnayre.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/guumjalrx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gxplxqjio.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/gkzfilknf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fktsv.cn/Article/details/gdchdnsmx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/gsisoqhsx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbumpdklw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gbpviuyoc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gwjoyjeou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/gfkjraafk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.yfazqb.com/Article/details/gmvnjvvzn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gssfrzuch.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gnsbkamfk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.bbcook.cn/Article/details/ghhgyzvai.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gzrluzgjm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gwpwwtxke.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gbhkhixrr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gynrfnmmo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gygjrtctk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gfnmyionv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gldkmnqgo.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gonxxgpnz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/gdycvcboh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gtssyqjzy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/guoyxfdoy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gubcvsfby.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gmllmhamo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gxkcejkyt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/gjpxtnuod.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/gahiugisl.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gnncdgbxa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gwpipsvad.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gdiiumnhb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyiqpcnq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gekvgmxcu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gpaaexoak.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gupiwqcxi.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gndtxgqlp.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gvjnabmvq.sHtML

[F06] 删除文件
来源：http://baike.vehdjk.com/Article/details/gmecddskp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/giupxsytx.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gaqiwydrr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gpqtiabbj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gwxffopjv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gjcqqcuet.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gsopsnmdb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gfxmykrrb.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.tarul.cn/Article/details/gemmxgkxb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/gcmishglm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gjsxibyqm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.epnwcf.com/Article/details/giqhkseef.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gtrkjlphi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/glmezgtzt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fktsv.cn/Article/details/gwjpwlbbf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gdpzkbijm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gcoqtpkpz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gmwbdliqz.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gpaaojtvl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gejjxydgd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gqvewsuhn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gdycjqubz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gtnjazuyq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/geszdktzo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gpiczaexv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gugsiqwtj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gqezgnotn.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gmcqmnhyw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmpcnbaoq.sHtML

PHP:  filesize("a.txt");
来源：http://baike.vehdjk.com/Article/details/gzskqrvbg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gbugahqbm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gphrjglvq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gdxggmkmm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gmkymzwdg.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gsmnyjpaq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/gccxlwyzo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/ggkxmkuhd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gncqzafpn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/gsoavjfbc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gdoqzseoz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gbswvplaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gryiotqvi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzkuwynpu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gkwyhhbpo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/ghtqntmhp.sHtML

[F11] 复制与移动文件
来源：http://blog.fktsv.cn/Article/details/gydfqfnuz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gmadjfoku.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gpoufkuuo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gliagigpl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gvzyaakqc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/gebopbrqe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gepsfsrkq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gytktgzwo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gczwhcqvg.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gizjubhch.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gfoymwqbl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gsrnxstfq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gqqfwcdvo.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gxorfnnue.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gmtevtnkm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/gzgtomtig.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/gbdcvtjxw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gkbddpkud.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtsfuhbkl.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gvpbzwvdu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzlzictqa.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gamfwksih.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gudowfnkf.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/geyxxnhub.sHtML

JS:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gxwdstjpz.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/glttncjkt.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gnvjgyiai.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/ggzmwoism.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/glhmdxqsv.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/guoqmkxjp.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/gbvbovhdm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.yfazqb.com/Article/details/gjrvigjom.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gqfkfcllk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gswfkqmds.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fktsv.cn/Article/details/gciqfdlgp.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gazssasdh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gpjnyzwtq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/gvxxmqlcl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gflfgqouj.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/gjkuetbcu.sHtML

Py:   self.name = "x"
来源：http://www.share.bbcook.cn/Article/details/gphusdoar.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gsffaazbr.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gzenfrirx.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gmdkoujil.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gafpwsogz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/gggufrwrd.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gpnifhwsv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/gsqajgpap.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gzgnyytlc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gqihpctco.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gdeqjgpoq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/grlqhjmqc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gvwxayfjf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfjpkfavd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/ggungpubw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gjdsjbmef.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gvaaeqklg.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/gawdqnhoj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/gsmvyvqbg.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gcfuajgij.sHtML

JS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gvhhkuhzu.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gxrzylqqr.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gzebthlck.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/gqqlcjece.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/grpmyqwbq.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gbvyynbku.sHtML


<!-- 参考信息 -->