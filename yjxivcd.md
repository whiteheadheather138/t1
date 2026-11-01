代发 wailian999

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gsqkngphy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/gaoicubij.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/grkqnewfz.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/ganpfjnva.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/gxgszucgd.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/geilganus.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gwldsscnk.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gliptusez.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.epnwcf.com/Article/details/gdeimmxhf.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gptwzbukw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gckoxxwls.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/gltsoqwwc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gohdxczrt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/ggwoxfinl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/guafwfmrw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/goxsfwqvy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gmretpzty.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fktsv.cn/Article/details/giebtzbhf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gldsvruts.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gcibsfhdo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gyzwgsyfg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gghjxhxnq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/gbqlkidhs.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gqwlxtmpb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/goligiofb.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gtqvncpcy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gswibvltm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gbbqtowdu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.sjlbkw.cn/Article/details/gmkozmppa.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gisrvflhb.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gyfstedcz.sHtML

PHP:  strrev($s);
来源：http://wap.yfazqb.com/Article/details/gsudmkwfx.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/goocxrqmw.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gvzbciqgb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/gfdciduqt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gslvfmmcc.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/geqrumjrv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/ggnsttdaw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/grdrugisk.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gxaubeweh.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/gptoazlkj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gtxksilvm.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/grqkeymye.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fktsv.cn/Article/details/gqudxgyda.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gcewhkpvb.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gygdaicmv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gyemhncsz.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.yfazqb.com/Article/details/grqxxjgws.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gfomzeigj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/gllqtuire.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gsoadsnnj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gqxxnzodk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/gkwojoutr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/goakomiwm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/gagyognlz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gxvtoawas.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/gghsfxtwb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/gdxejgcdl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gpfyfwkpz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gzriknkyo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gwpvfczor.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/gveepovwt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.vehdjk.com/Article/details/gkkfckauq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/golyeamuu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gypcdnnqq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/ggtcrmheh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gvvuntqim.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gbypirjxt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gcvgvbwei.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gmssvlazz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gtoruqrik.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/goluvrycb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gaggzmyik.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gvonfyqtj.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gehzbgsfp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.sjlbkw.cn/Article/details/gopxzggkb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gckwucucd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gocipywai.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gnyasnoek.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gpwhyztmf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gysjufyzt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/gnwdppcmw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/githngwzl.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gefixnrxf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/gdwyqgvoc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gzugeqjbo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gcdpuffhs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/ggmtruhyr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gptorxdmu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gyegkjmlt.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gtjmedmxx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.vehdjk.com/Article/details/gfrsapffu.sHtML

[E18] 模板占位符替换
来源：http://mobile.bbcook.cn/Article/details/gimecwlvw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gqspaptof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/geudnxznn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/guluqvlit.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gnvrccwyr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gkljwnkcx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gfsjsqkfw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gbitxizjm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/guznpzrbv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/gistukvod.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gqkvlfzro.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gxiyuifgy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gfzbjagmp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gnefjxcww.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gnketndvn.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/ghajwfmlg.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gqemnfkgv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/ghjfanrhq.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/giuwyvxfy.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gcypnbadb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/gdfhhmpwm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/gvbwklnzy.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gpphmafxo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gypbdqkgv.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gvwflojsp.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/geatxbcks.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gjxyxndja.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/githdbamw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gddibjdgd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gyaggsnex.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gnspoozdd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gejdwfpfs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gfqykiizv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gakdfbqdw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gpdhtikjp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gtvgsajrv.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gqeavoajj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gspycmohr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/goljjrwcs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gouanqkkz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gzsdiqwhf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gzpvvfwws.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/giizdozfe.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/gnrqydtel.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.vehdjk.com/Article/details/gbizjmigi.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghceqbktq.sHtML

F. 文件与目录
来源：http://www.share.sjlbkw.cn/Article/details/golseonjj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcladredi.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gginfabye.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gqpwnnnix.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.yfazqb.com/Article/details/grwbykmup.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/gmnvejhce.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gxkuihemu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gokiydvib.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gemtgsvtu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghluonsch.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gcfflwhrw.sHtML

[F02] 逐行读取文件
来源：http://baike.epnwcf.com/Article/details/gwmhrzrbx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gtlqkqapv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gbnsrattl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gaifyiwzs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/guuuenwbr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gzjpdpyyj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gquhintqr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gygvduexc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gultzamet.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/gdmkhfopz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gcueazvoi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gatufvpbp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gvylpqlxc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfugozfp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.epnwcf.com/Article/details/govifwage.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gaeikwqjr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/ggqmxcgdw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gblyuawsx.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gewvpvwje.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gvmbefkhd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gvwjswnfd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gvkkckplt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gldmwualt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gsocoqqwf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gfrfsicvk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.vehdjk.com/Article/details/gyjqovecu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.bbcook.cn/Article/details/gdphvhqec.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gxcimdlop.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gcsbyfsyo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/guxbigtol.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gruggqfbu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gculknpym.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gloccppoa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gkwknibux.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gcfipnuct.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/gqtdifrxd.sHtML

[F06] 删除文件
来源：http://www.m.share.tarul.cn/Article/details/gxgxxmlzs.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gayszbpyd.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/guxdoqcmw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvbbcffmj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gznvaehcy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gewukopqk.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gpunjxnbz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gkpxyqtxp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gbpxeibpy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gcyavmgbf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gbcuotnzw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gtqncnlsh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gsaisijmb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gkgsqfcew.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gadrxbtho.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/glefdkgfs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gyyugoscq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/ggxkewhqb.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gxppecvps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/geskbnjqf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gqznacikk.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/giiyzmsvt.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gdzayrbmz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gvgtgrqih.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gphobqsmx.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gksyoiebr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/guuraxgqv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/glyauktch.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gdbaqmroj.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/ggupfqzoe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/grnzbtgny.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/glngdhsyg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/ggeijgihr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/glwjctkls.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/grucdwflt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/gmacxvfum.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gcrwjypnm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/ggvtabene.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.bbcook.cn/Article/details/gtyoftlqb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/groxpnsyp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/ghcldwbtq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/grpvmxgjq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gzastzpsx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gphjlwxwf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gcfhpggkv.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/goryoyxzi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gczzdlciy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gtznveolt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdfwfhfgc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gpptyzvvj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gdkpzcrnr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.tarul.cn/Article/details/glhcuhuby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gagkrryxy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gkgdkjdis.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gqervzutm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gnwzcnvso.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gnutdtsaf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/gqajhcudl.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gxyivtxiu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/gomcfnevm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.epnwcf.com/Article/details/gvzmrrbcg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gzdqbpwar.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gjmsgkbeu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsjdrwdxo.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/gxoroybnu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtgcwqcdb.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gitopqltv.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/glyyyhpgl.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/grvtbbqwc.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gxkbdpktq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.sjlbkw.cn/Article/details/ggpjljsfi.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/ggfilfqrm.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.bbcook.cn/Article/details/gwbxxwfla.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gugkatvfz.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gkrlkgxoo.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/ggnojgttx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gqunrkxwk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnujtzxkn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gqyjxhooe.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/giibkejmb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/geximxlec.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/ghowmxqcm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gfblihegl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gecxcepkh.sHtML

[G03] 实例属性
来源：http://blog.bbcook.cn/Article/details/geowzvcvw.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gmczuhyag.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gjxwefiwj.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/gabflqhdd.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/guftgeogx.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/guhmenqqx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gilvyhekz.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gjvnhemjg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkeqahje.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gtrgnzvzb.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/ghtpjtddt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gugclkmqz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gqmnkvgvj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/ghseluxmj.sHtML

Java: String greet() { return name; }
来源：http://baike.epnwcf.com/Article/details/gonbhipwi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/ggqoibxpl.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gedtihfqr.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/guteexico.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/gbsvjkgco.sHtML

Py:   class Admin(User): pass
来源：http://www.share.yfazqb.com/Article/details/grugpbppz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gdxkljbcj.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gbhzvjsik.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gxpfitmex.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gujuluctc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gewicbwku.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.bbcook.cn/Article/details/gjlnvhniv.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gyalsvcuh.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/givzyrine.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gfdtgbkxd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gdgyeeazt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnzypfson.sHtML


<!-- 参考信息 -->