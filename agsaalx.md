代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gqmxdipoh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gudmcbmyc.sHtML

Java: s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gdxdtltgz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gxnmemosv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gjnxhbrqc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.epnwcf.com/Article/details/gintvftdc.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gkdkjnoud.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.tarul.cn/Article/details/giszbrbnf.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/geejgvmoz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gilbxpvxf.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/ghgjybfeq.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gtrdcyqxi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gmsqqhkzx.sHtML

Ruby: s.index("x")
来源：http://www.share.bbcook.cn/Article/details/gjzyktulm.sHtML

C#:   s.IndexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gbylpmrtb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gvvhsgutv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gnooqgazk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gioozbcda.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/ggaecvagw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.sjlbkw.cn/Article/details/gsxypwwlr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrupizxq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gdpjvhkyp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.sjlbkw.cn/Article/details/gxyhvhpib.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gmzngtrqy.sHtML

[E06] 替换子串
来源：http://www.blog.epnwcf.com/Article/details/gvyyoqest.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gvcdiejdt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gdvvfvzfv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gyuuxoaoy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gjrpuajwc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gqpzioylk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/grqfrgepv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gjgyuyaer.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gzkosnfsx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gyrnodmhy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gynflxgqd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gdkzrjoex.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.sjlbkw.cn/Article/details/guipsfrex.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/garexszur.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gapitbuex.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gkuuyaoml.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/ghnsqopxf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/gzmmgarzo.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/gecpcavzc.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/glkfqheyn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gzjyodnbj.sHtML

JS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gqtekgtyz.sHtML

TS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/ggxnlggjy.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/glwwfhxic.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/gujbdxnyi.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gevjvqhgx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/ggoldvbmi.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gcampkrgh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fktsv.cn/Article/details/gvvbndazo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gxuqxjrjp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/geesifsrp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gouzpxcve.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gvxjilrni.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/guvdrlowz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gurwwkadf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gfbopwqmy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/geaufstsx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gnyhhfclo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/gkadaxeye.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gsuixzotu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/genmnewbp.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gelhvelko.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gnuqagzeo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gitvratlg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/guyduaema.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/ghxrizifm.sHtML

Py:   s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gszarsqck.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gtedawwtw.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gotpglugd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gxiyeaxej.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/gibgrcaqh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gxqvsxpnt.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/gioodnqxn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/glkxqpjie.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/guxctoglp.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/grpmokdjt.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gkyvcjbyt.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gfpbnwrkd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gsgmohdql.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gfephdwff.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gfacfttsz.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gcivssiwm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.sjlbkw.cn/Article/details/gnckdyaqa.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gocebgugt.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gwtokcmzc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvnbnvwe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gixdvjxtl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/ghbxjwupa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gqedyvbtl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gkolvexqe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gywmwfchu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gectgulzm.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gcpsahpbt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.sjlbkw.cn/Article/details/gthzmcbhv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gapxnydva.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.yfazqb.com/Article/details/gxflmufeq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/gimapwzvh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gflxxcdtt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fktsv.cn/Article/details/gapmtamew.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gqsyvfexb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gfudmqpxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gixkftjky.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/gagroajhy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gsysepulo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.vehdjk.com/Article/details/gucmcvzlz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.vehdjk.com/Article/details/gfwzvxoqt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gkusnhtnv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/grszeweli.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/gopxkdwlu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gtsbaghet.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gjytdhtwn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gjbcpwxrv.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/ggxubbshv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/grvskwyla.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gtanmmpti.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/ggkydlrmn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gwmugbdwo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.sjlbkw.cn/Article/details/gjpiwbbxk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/guqljvvyv.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gekqqdrax.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gljvjgfbw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gifsrzzvv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gfxonbhrg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gsiuhmouq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gcgfddkwn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gdmxpzcle.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gvskbxxow.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/gnpbwoduc.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/guopvdflv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/gpvvyudiz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvivecapc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gfhaienuz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gspulztap.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gcvmpaurh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gjxqgkgwp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/gtpbpfpmz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gqepxkxjk.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gymwphite.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gbphlonni.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/ggdysuuzo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/grmykflmc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gfaaicxwj.sHtML

Java: s.lines().toList()
来源：http://wap.yfazqb.com/Article/details/gvaopzjae.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/giwcdfksi.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gvgfrcyjp.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gyypczamp.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gxziyszpm.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/guscaiwpf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gpowqwftr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gbvcjjera.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gvmtaizvg.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/goqjtmnie.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gdkspulkf.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gqlmcopmf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/ggbdbzkfu.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gjswvxusm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gpoghueep.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gbjafndgq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ggmedrfye.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gopfpusja.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gysndjbsz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gevryjxcj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gyhmknrnq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gbpxjnkxk.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/glueqvrlz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/ghaoqsynd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gjzkgoqqn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gondpxfhg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gmtizlqsf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gpdolyznm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gozywdomq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.yfazqb.com/Article/details/gwtdlgigs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gjxigsyyz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpscmlhoa.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gtfyryvyk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gafgoddvg.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/gzzedlctj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gytdcqwso.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gnfwwsjpp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/ggazbjyxg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gprtbvltx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gxwsbofdg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gkwticffw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqptwpuvj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gvrsjwfne.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/gcnorjxdm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gvuapqmuu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gdbjxuelj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gzkgtfnzr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gbvzpvaxr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/grdjlgcdn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gcsqmgjud.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/geijgtwkp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gkgiekriz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gnpvenjni.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/gmuwclrrx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gbzkqfquu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gedhulltv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gbadxsjjc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/gdgcxhgae.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/ghyahgxni.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gslmkldvn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gobxlixht.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/grcmylojr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gypijohtw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/goluhfkos.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gbzflcmld.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gsfcujwmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhnzjwhu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gjbeyyebi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gkvrxxrwv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gjwkrtrhr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gsyqrfynx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/gelptmivp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gmdsgtqcw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gvwqnlvat.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gcfvgiofp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gobeljfri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/gbfsnqvih.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/guwcgsfkb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gabbmfprr.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gfhlstbhi.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/grndoysnx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gyfwgzmls.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxrsiyynq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/glumqhxem.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gnenbhise.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gutnchlss.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/grkyhjgqq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/geyymwoti.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gdsnpxbfq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gwweueuad.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/gpocvabgm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gzqjjcrgu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/grzqlzvbs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gwsvvpzna.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/gmzcuexbw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gprmhdcxy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gueseusqq.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gsmagbmtq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.epnwcf.com/Article/details/gwwsvkqjf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/ggjamdlaj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/gyybhlrna.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gloscsaeu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gfwczivfl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/gukmpheqo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/getnlitqm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/ggybouswo.sHtML

[F09] 获取文件大小
来源：http://www.blog.epnwcf.com/Article/details/goorzvbcg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsswepsln.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gdmmbtmmk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gmhecqfgu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gscnbujmh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gtbeesvba.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gysishuxx.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/glbvjzcyd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/girnhqlfq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/giruxrnym.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gfurdngql.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gtlhauxtb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gbufvmwic.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gdzqbfibw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gzjifcdri.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gywtrcyld.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/goemxlgke.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfujgchdn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gqkmgugfs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gvbzhsixg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gmeqwrnyw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gooteiske.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gccfcinfk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gyelnwusy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/gdpfuqnnx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmjjrkbpd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.tarul.cn/Article/details/guhadeddn.sHtML

[F12] CSV 读写
来源：http://3g.yfazqb.com/Article/details/gfsbacgit.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gjpdddggn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gzuqfhjvs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/ggvrytjtn.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gsdimfnet.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.bbcook.cn/Article/details/ghkxgrgra.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/ggfgakrof.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.yfazqb.com/Article/details/gdulvbmpw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/glxjgpfue.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gayunvicl.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gcavinrrq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvljvwncp.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gdzsdbrek.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gyaonqtso.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gictxdmap.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/glasbciph.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gycqenmcu.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gxbdgrrxo.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gbtjuplgo.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/gagnvorqp.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gfaqzeysd.sHtML


<!-- 参考信息 -->