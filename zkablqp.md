代发 wailian999

C#:   s.Replace("a", "b")
来源：http://mobile.epnwcf.com/Article/details/giscsobzc.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gsavnldif.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/gdhrqkpte.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gdioghnec.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/gxvyfvjgl.sHtML

TS:   s.split(",")
来源：http://mobile.yfazqb.com/Article/details/gktnlisbg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.sjlbkw.cn/Article/details/gfgjnhzlc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gtffgkyyv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/gmvyfssmo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/gmmosgxzn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gansvdyhd.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/geewkcjfl.sHtML

PHP:  implode(",", $items);
来源：http://baike.sjlbkw.cn/Article/details/gkycxmgsh.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gdqpxzzoi.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/grlquzzdg.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gpjrnjpvc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gnhwoqmae.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gwtaffafm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gmhpziels.sHtML

[E09] 去除所有空白字符
来源：http://m.share.vehdjk.com/Article/details/ghneeekro.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/gsbwyyqsh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/gwytnyktf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gkxqdnxit.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gvchxnofb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/gdxrvbltm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/glmhmywwl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gaxhorhla.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/glenfigdf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gqsqoctev.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/glspajhgg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gwhfbevtt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gizvumhje.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gcbxmeuld.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gixdfbmnh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/ggsykuuag.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gmobfftyp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/gpfgulejz.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/gptaoafkh.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gbhcddayq.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/gbclwzewh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gnpmlfrul.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gogtsykzw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gwtjivnix.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/gghkerblq.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gohtauwje.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gkiciiytf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gxcwomjsk.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/guxugroid.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gkpfxlbhb.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gqqaltwzl.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gsebnogno.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gtivpjfvs.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.tarul.cn/Article/details/gyjwlqblh.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gfcaonlug.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gjijbqmhj.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/gbqfsbgva.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gmpzzhtym.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gyqngdcle.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gppnikchz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gvbtrkueu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gtbixgqqb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gzdoictsv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gtngjwtzm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.vehdjk.com/Article/details/gapcpzwjb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gztwtqahv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.tarul.cn/Article/details/gwntlhnkb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gtuevhmzi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gubhmsqpz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjropykje.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gjwnrvqri.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gucavyfaz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/gibnkexyo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gazbowbrr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gyzxfzabs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gedtweqwz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gqquxpgqg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkjubdnr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/gywjzfwvj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gnwjvmhnx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gqzpgjsid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.epnwcf.com/Article/details/gienlemka.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/gefcmowjk.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gecmmduzd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gpamhqluc.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gmtnkxavk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/grzpxexvy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gsxkgakyy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gfpuyaplh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.bbcook.cn/Article/details/ggslqqnug.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gjtsirxxm.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gqfahcsns.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gowyafqmu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gnepjilzv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/ghqpfxpiz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gjcbymynv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gbdrmvfty.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gjtexblkp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gyqbthnkj.sHtML

Ruby: s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gnukqwrwh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gvkopftvs.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gubaxxfec.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.epnwcf.com/Article/details/gdbnbgjvu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gdpstglmh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gielvkvio.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/grdirtmbc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/genhorgvo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/garbehigp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/gjarvwode.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/gqyqschnp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gincpdglx.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gbarbjjnx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/geqgcqobo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/glzfphapq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gqbrvzpqp.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/gyekqrgjz.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/grxckjrpv.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gkokeddra.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/gvdwvvknb.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.bbcook.cn/Article/details/ggwbpqhod.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/ggzrcyxbi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gbcwqmthy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gnvyjzhlp.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/goyhwyois.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gbbkxawda.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/gnzcfypyk.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/genzyorzf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/glwmbqgjd.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/gqnmwijgh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/gvngtwcyy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gsyvyccja.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gejgyutie.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gbfgrgebv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gsqijtymp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/goqzdczzk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gvsdjbfbw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/ghcexbawf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gbjsofjqk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gqqphwoza.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gledqjcvw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gcmfdtxmp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gtjcjsskd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.vehdjk.com/Article/details/gghllyhnv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gibsmcmna.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxeinbxm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gzsqwzijj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/greduaxrr.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/goxxrioex.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzhlotcdl.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gtgvrkjla.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gzwereaho.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ghpkivxss.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gukmtdqco.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gwfpxrwvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gwjyeccsi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/ghpgsletk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gyhdjxlpl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/grqnpnpde.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gbyueypmx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gqjmzjhyg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/gazlmlnkk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gxoqkwgxv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqvjsqlef.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gxuubbipx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.yfazqb.com/Article/details/guvjwhpbu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/glsxxzxcw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/ghomzvfag.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.sjlbkw.cn/Article/details/gcmfbpbrr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/glkidehex.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gnwticfpd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gbqxrquii.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gxwzgbrkg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gpespmtzd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/gfyyawvkk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/grglbdtik.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gjlndzegz.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gjosekdcj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gltzqwoto.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/goyjldnvl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gkmbpnrdl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gxtmtvdex.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gsotwxaun.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gijvhwkjk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gqggonugj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/gmoswkvyk.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/grljpctho.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gtklphznx.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gjgkftxhy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gkgdmdzkv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gsnkuihzm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gzjxalioo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gdnxjcmwz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/ggnbadqhu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gkskijkwg.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/ggiqylmce.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gkzsnvgiu.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gkvzsrfwx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gbcwxuevb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gzhulhylm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/ghdchcrek.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxbrajgss.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gtuknkner.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/ggxofymcn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/ghglqdnkk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gaeqawnxe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gpcbvnlfj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gyvhkiyhv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gtjmjymmt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gagsrxolx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gojbjrhvl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gxkiukbqu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/guvbyvtaa.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gfjwnplgd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gkixrxblm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gtcmkfryc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlibkalk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/ghkkjjkhs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gtbwwlfwh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/glsclgyzf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gcrlzwpxd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/gfjlgjytu.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/gtchlhsqg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gxtcnqywc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjqncldv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gohsijbmq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gnvbvtdkq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gzapdhdwa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gtqthphfd.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/goxqhzdpp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fktsv.cn/Article/details/gwrqaxvkq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/gvwglkzch.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqmhfpwjw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gtfllkgew.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gtzukjdpg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gyohskavn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.sjlbkw.cn/Article/details/gyvxrweef.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gojspxbkb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/godwicoyh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gpwsaqauc.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gpqqlrmtd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghpqrzcba.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/ghdlpsjfq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gdgvocwgx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/ghlfstcuq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gbbnqcjeb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/gbnzylxxf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gugvcaokr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/ggswdnjsp.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gvjxnwuzp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gldavofxm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gbvxxgmuq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gxgokaaoe.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/gnsfxtqdc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gpaandoxo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gfbfahjur.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkyewbkm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/geqwihdly.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gijgwrtte.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gatpucebn.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gimrnefdz.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gwjwfesyx.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gubfmwwwx.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gclgvrkqe.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/ghmbyuznm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gjdfgqbvm.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/gfizgnnmr.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gjwudwszj.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gsjtzaawq.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/gtebtsnnl.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gjdvjkmte.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gpungvkvj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/grblhjsxu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gnmqutgzd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gyjynltgv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gbuteqoal.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gauloyvgp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gqvmwtibq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/garwdvpav.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gtsvrvsli.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gobcrdgru.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gnekqalig.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gcvbnegbb.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gilplhugb.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gxpzmafbj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gjrlzmsdo.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gpqlglyzj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.tarul.cn/Article/details/gpazabpca.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gbvbwycru.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/ghaafbzrv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/ghwwvciax.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gfttswvjd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gguzulzyr.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gwyconhoo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gtatwlsjd.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/gwvmftsdp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gadxyzbzi.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gmsjuynqp.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gcqddqycb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gookmfjgy.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gaqwgkwms.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gwejzolqh.sHtML


<!-- 参考信息 -->