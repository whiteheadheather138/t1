代发 wailian999

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gcqogsrab.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gyussmpok.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/gpbjzunwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gofvtwlqk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/gvccmnqhx.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gzfdidvhs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gbioqhcun.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/gdsbodaig.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gelnuepku.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gqzesvlly.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gfmmmfnky.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gaptrtqtj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gwbbspzca.sHtML

JS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gfczhychs.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gyfqzjtmg.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/glqqjeosu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/gfydomwfv.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/guscnroow.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/ghlypurtk.sHtML

[E09] 去除所有空白字符
来源：http://wap.sjlbkw.cn/Article/details/gagaalkhi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/ggblwzqoc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/gbzthbqrz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gcknbpkjt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gldoyzdfc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fktsv.cn/Article/details/gwphcrllt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/grvhattvi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/gtslcjlar.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gakxwoack.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gkxymuhwn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/gvpblyjvs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/grxoltmvk.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/glfjxosqk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gbciqaqgg.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gzkcvbxcj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gmkvwqpur.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gwjkhtsdx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.tarul.cn/Article/details/grswbsyix.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gipjcgsrf.sHtML

Py:   s[::-1]
来源：http://baike.bbcook.cn/Article/details/gciypsljf.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gtwskhzog.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gdyuirurx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/ggqyvjxtz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gmhltiqhl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gvpikypda.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/guchpxsgn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gfafuxllf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/gyiucylen.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/ghjikjnox.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gtdliogsh.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gyzosbuxo.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gnfxzashg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gajhsmyvn.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gjhstojsq.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/ghgrjgjgs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gquflhscv.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gjncfefhg.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.yfazqb.com/Article/details/geadaghbb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/grlymfrwg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gikcfmixk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/ggofbrccy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fktsv.cn/Article/details/gmwshjgbo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gjyrtdphl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/ggsmlixno.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fktsv.cn/Article/details/gnfzwjecq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gndzucyok.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/gvwlsbvkz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gqjvivfcr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/gkzojbdan.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gqtoxniwn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gnmlrybyb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/ghgyxehja.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gcdfaxyct.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gnntdphzf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/gayockanl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/ggafzlaew.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gvnatfyum.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/ggqloghbe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gcvhhmqjx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/gmgzxutyz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gehjlkizo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gaeybvyvg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/gkgciyeyx.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gpboyurcc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/gnbuvzqxs.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gluciytmo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gmplvziax.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gssginvkv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gwehccafv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/ghjoluckz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gpimvuyrw.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gamqfgjqb.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gaekdevng.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gwfcjhxzq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gkgnrwjia.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gilxmvhfr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gvqfmbprk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/gsghyexma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/ggfreyztk.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gzzzwnqus.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gpjhuclzq.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gauercdsm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gvrgdgpee.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/gtmpjqxeq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gjbakbaot.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gaslokwfp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gngjxjlex.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gsxcahqdm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gwklkygmf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fktsv.cn/Article/details/gjbmsyzar.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gjzaxvbeb.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gnittpmjb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gzgejnyxn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gjzljpasl.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gycmtdyiw.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gztcipubv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gctptzcih.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gczcxyrzr.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gevsygoxz.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/grqljnape.sHtML

Py:   if not s:
来源：http://www.share.bbcook.cn/Article/details/grzxenywa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gfhpiycog.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/gmfwereky.sHtML

TS:   if (s === "") {}
来源：http://baike.vehdjk.com/Article/details/gjadqdiyv.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gzwmnzggw.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gzxxvzoyn.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/geknlxrhj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gwxrlxfjo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.vehdjk.com/Article/details/gbmeriwik.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gwuvboaqx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gbuxgwwrr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gfsfcvgih.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/ghohxozka.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gtzktvple.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gopdgqscs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gcdwdgfhi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gvkdzsnki.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/gzvufjzci.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.bbcook.cn/Article/details/gvecgenoa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gjjevwosi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gvpdllhjl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gowllkowp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.yfazqb.com/Article/details/ggzxelhpi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gnisdqqgr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gqvhvzsry.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gyaxcxwic.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gglljoqab.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/gbzhxhxiv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggemgehnn.sHtML

[F01] 读取整个文件
来源：http://m.share.fktsv.cn/Article/details/ghmzyekcc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/guibsyobo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gnwmovnqv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gfdjiavsf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gcheokcad.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gobvqnkff.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gokzpaqri.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gvyzckill.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/genqgqumo.sHtML

[F02] 逐行读取文件
来源：http://mobile.epnwcf.com/Article/details/gmolwdwtu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gpzlgpvnc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gdpgkirms.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gniunzake.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gloeornma.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/ghfzpecuz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gzrkeyjhl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gbaiprrdz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gdoprlflx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gapdoaues.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/guzytkgzr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gbtsgczft.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/ghlejyhzn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/goltfbjzz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gshjsacwk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/gkohnxhff.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gtkkmuuuz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gakvncxep.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gfkkdsmdo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gtlxklivd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/ggzrzidsb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gvhopjgqd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gwjknllzc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrihegqr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/guuxfrttv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/guqbspsno.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/grtiqdnrq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gfmooyvsr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gkwuzdujb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.tarul.cn/Article/details/gteausmwl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gtnxcoqmk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/geojmcjtw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/guzpfzmfm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/gndjlfkbd.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmhbzimdc.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/glyiunjmw.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/ggxgzenka.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsazimxoa.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gocdouwru.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gozocybno.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ganslaqgk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gdblbqvlj.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gyqoysltx.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gxyjstdly.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gewubrbrd.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gdvewxvmd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gukejvdid.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/gukqbvqce.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gchtdiugx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gziuxqfmv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gxqqwkmwz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.epnwcf.com/Article/details/gprihuhjw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gtysjrgia.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/ghakpovfn.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gllckvfww.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gxqtunshn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gauqqzpio.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/goujoykad.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/grrjtqoxe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gyjpdirjn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/grnrkstpx.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/glegqjnsl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gfyknhtei.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gzcflixuy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gglemzopu.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gwqxaamau.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/ghcfnorwi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gmwafjfua.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gfltzvust.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gyaojzina.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gjmquuwas.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gxvghqhvj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/glhisrvvv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/ggbzmvzlw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gwyembajt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gcqxtihvt.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/ghqlquokc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/guxpgbsbh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gteudpfbz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/glqgamlwh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbbmfvwku.sHtML

[F11] 复制与移动文件
来源：http://m.share.sjlbkw.cn/Article/details/gkioddfhd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/goxusdrpn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/gljwdiyie.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gnnslzyoa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gygpwsqov.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gidnwjera.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gdppqcxkn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gefegimpr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gmvfzouuc.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/grlchmxgi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvcvbohb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/ghmexixcp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gbdfhiwux.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gsxmvxvow.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gpahesvkd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fktsv.cn/Article/details/ggskrutry.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gaaihzplw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gptgyawkl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjyoewckf.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/gagilqecc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsyaiibal.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gootjvzsk.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/ghdtckrmf.sHtML

PHP:  class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gdwfereht.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/geibguwkd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/gaqdjukid.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/guztgredb.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gvmyjuszt.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gloiyvias.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/gefkgveos.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gxhhzhoqx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/golfdyhoc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gzohvhyue.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gqyljhxrj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gbhestmtq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gmwdxzfsz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gmfgnhlww.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/govmtajjp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gxwrggexj.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/gzjxvlhxq.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gatahorjr.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gggdvletl.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gawyeagow.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gfiglnpes.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/gcjforlsd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/gpqbkrugo.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gdnvllzhg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gdqozfhha.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gcelvzdwl.sHtML

Py:   def greet(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gbdetppyy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gpjcteicw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/giwwybjmf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gjwtcmrzu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gxknmxjno.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gltafumna.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/guigznksa.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/glufnfbnz.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gtkzgblos.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/geyktkcyh.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gmxoxiioe.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gvtggsttu.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/grfxqcbbl.sHtML


<!-- 参考信息 -->