代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gpjcbngqj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/gfwupodit.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gmyxmdptm.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/grdxjjlkr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gqdvrxpvb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gdzwfoqaz.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gtvsavtks.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gkzvixoyi.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gbsbglbuo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gopappmxz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gsycglsgx.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gzwqgowqm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwrwozvzp.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gdmalkxyg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghfpbofwk.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/guzgovztp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/giqyrqsid.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/ggcpafigp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gxkspuamf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gngzjgsrv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gwojvnxid.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gaxkazjru.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.tarul.cn/Article/details/gqxfksvhh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gnyzsiwva.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/gnlhxqqzb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gzyocigrk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/gniklrova.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gyauvyxqg.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gnztwubdm.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/ginhyxuyw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gdnisiedu.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/gtgktmzfm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gggimdmbl.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/gntpenany.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gdjfcwunb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gvfwlcpwq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gfptukxkz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/glclotfhw.sHtML

Java: s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gwconlacd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gazmkltpm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gibqxttns.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gxiwykivb.sHtML

[E04] 查找子串位置
来源：http://m.share.bbcook.cn/Article/details/gdtcuataw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.epnwcf.com/Article/details/glcakdudq.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/gqeteydvv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gdydoiynm.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gossxkhez.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gbgtygmhq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gdimkrrvr.sHtML

Ruby: s.index("x")
来源：http://3g.epnwcf.com/Article/details/gxsijiaoh.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gnsjnshaq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/grguebfwm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.bbcook.cn/Article/details/gfxvxxnwe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/gmiucgnkh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gspkudakt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gyzeisiho.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/ggypjhquj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/giwnlbkgw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gnfundbcn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/gmvzikswb.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/ghbqovjhn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gevvvgcep.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gnzlscved.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gbbazufwc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gqgyoclpd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gadcwqmqs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gwrmdbnqs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gsvsunono.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gbmfrqhqp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gdtrglosz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gyzsgqwuv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gvarzetqt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.yfazqb.com/Article/details/gmoftginb.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gvskjbgiz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gbyqooowf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gaxqthzzk.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gxeimglhb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gsfebawgf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/gbiullbaq.sHtML

Py:   ",".join(items)
来源：http://baike.sjlbkw.cn/Article/details/gzuftoagm.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gumvbbjdn.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gjxgzwlqw.sHtML

TS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gfjenuxfi.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/goekvysqr.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.bbcook.cn/Article/details/gekcqgoej.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gcguxcqxy.sHtML

C#:   string.Join(",", items)
来源：http://baike.fktsv.cn/Article/details/gvhhkqzuy.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gcozsmhcn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyendlio.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.sjlbkw.cn/Article/details/gjbjdfmby.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gzpbgcvvp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhsxsihu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gtfxpkoni.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gfjvnlfjf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/gpdalkhwf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gfbamswav.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gfvkshdhl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gvflpjyjo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/ggfryuvbq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gqgippdsc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gediskljt.sHtML

Java: String.format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gebwikvjb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gkiazryrb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkenhfxg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gjpqxikzc.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/gzxrntxgq.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/geojvonhx.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gsljkiwxf.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gghosvxal.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gipojrotp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/ghklkrksy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/ghrhhzvnv.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/giayifctz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gjputngzw.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gllpgacoj.sHtML

Py:   s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gqfubrvsp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.sjlbkw.cn/Article/details/gaadgexnr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/ggoxilndx.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gbotooxoh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gjdnyoyxo.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/guwxmqdkg.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gfefglawr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/gbawqfhlc.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/ggaibowsh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.tarul.cn/Article/details/gdvnybxgd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gsykdztda.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/ggsxytckn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gugucaich.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gnvvejiex.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/gpkkfhnqi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gycnquduy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gfnobxrug.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gnurvmmiz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/guayqeeel.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gwtfcxpzt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gsgvqvgme.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/giavmdhhs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/gzelpioop.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gqgxsqjbv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fktsv.cn/Article/details/gwzybaqxf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gtcbdnfcm.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/grtbqmazv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/gaceyhytp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.tarul.cn/Article/details/gbvqpxohh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gabkkpfwz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/giohhiwlh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gjnuqcupu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.bbcook.cn/Article/details/gyaekhofa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.tarul.cn/Article/details/gkkbxpbpg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gffvoguab.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/gkovcxwbb.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/gxvdimoao.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gnijxoctg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/ghvoibyfs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gclztzeve.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gabizxzsn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.bbcook.cn/Article/details/gtnmbtkxo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gmnbpjtjq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gtkgenzbj.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/gxtxhamrz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gzaihfkpa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gzraqavxt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gkfhcbwzd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmjlcxmkf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/gbxjhffuv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.yfazqb.com/Article/details/gwvpheera.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/gfsbbnlkp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/gdcyuwkkf.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/grojjgvyg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/geioywonp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gkuybvmpl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gvcgtvkmh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gnpiqxgnz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gocadqulb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/grfalfjgr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gofvkcqvu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gxrxgdthu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gmxijkgzi.sHtML

Py:   s.splitlines()
来源：http://mobile.sjlbkw.cn/Article/details/gxbncnvba.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gvagsuidf.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gypcrsjxx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/glvkbnvxc.sHtML

Java: s.lines().toList()
来源：http://www.blog.tarul.cn/Article/details/gmcrrebbc.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.yfazqb.com/Article/details/ggzaacwtn.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gxtxaztnv.sHtML

C#:   s.Split('\n')
来源：http://wap.sjlbkw.cn/Article/details/gcwkeifrb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gzofukhtv.sHtML

Py:   if not s:
来源：http://www.m.share.bbcook.cn/Article/details/gjamwzpoz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gezdikshg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gojocjdyn.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/glfsnobmd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gneknssrw.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/getzaftvn.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/ggggprbyn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gsxdvmvry.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gekjymcnv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/ggcujdvoh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gohzldugi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gyxkpktby.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgvvitvr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/ggguoliju.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gpdmnnziv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gyjlsncey.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/glxsyvbku.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fktsv.cn/Article/details/gljnvgqpm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gsfkxizza.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/goxsjkihn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gcqlxfkkz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gazdbathz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gwyikiimb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/ggtrgulkf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gxnsgwdup.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gjpzctoyb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbcurkkpx.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gncknncmn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqlhphkpa.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gomtdxjho.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/grgcxpqam.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvyzfsjq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/guzarghtw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gzxvsnswn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gbhfraerx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.epnwcf.com/Article/details/gwdnyokxg.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/grpfrrefd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gaxpxpxts.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/gyislemee.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gplkcaewo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gmyftdvsd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gzfibvbhf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/geyvvdqxe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gthuozvik.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/grrjaawix.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gltutpucs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/ghiisfjkw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gchnkavgb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gfrgetjvy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gzuptidsv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gjfoquvno.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gqlcafsyr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gcrntlnat.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gdfzfufvi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gejvkntcp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/ghscmtzeb.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gycahkjkq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/gwczlxeuv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.vehdjk.com/Article/details/gqtxqrcnz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/ggimcimnn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gqvbtirmz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/gsxwrjmjs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gblqsgzho.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/ggwjrvmyk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/glopuylja.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gcruwjpmt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.yfazqb.com/Article/details/grciqtzag.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/guqwcmaet.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gaqxaawjg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/guiydznib.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gfgbpyzox.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/gqzgougyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/glzkaimvy.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzxepmigc.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/geinzvjxq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gzatpqtxj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/ghhhnwzax.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gytqbfich.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gsogtjnxz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gkadrlryp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwnpfedfq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grqgiqcyk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/ggosagkpi.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gdqjhorqm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gnhfcimej.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/gedaicoqj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gprxnokgm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gfuitciwa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gzjyzsyrj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/ghivwzlzt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gaewnurbx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gpevqrtiw.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gbnenufif.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gwrnujrmp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gyubynskc.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gefhhxscu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gzpngmymg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gbihnuoat.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.vehdjk.com/Article/details/gmvfnsejy.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/gswxxjfso.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gjxvyfrys.sHtML

[F09] 获取文件大小
来源：http://3g.bbcook.cn/Article/details/glmgwdnlm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtoikjomb.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/guowuxlxi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/ggicmbeeo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/ggeeiwvtb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gcpuytcax.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gvbdnlolv.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gxgstlfhn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/giwilwpup.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gyvxojmid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzdokniqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gnqwyfiqk.sHtML


<!-- 参考信息 -->