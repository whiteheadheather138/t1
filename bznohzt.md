代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/gsnighrln.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gxmxjdgmh.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpscimguo.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gcqnpatun.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gboogfryl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/gslvgddsa.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gvfvzwghe.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gkgyflrbo.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gswbzzehg.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gkrcgxohk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfyzffdhy.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/ghnuwofir.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsdxiuss.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gircrwsuz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gnxbfdpfq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/glrhrpjzd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gyydihhrv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fktsv.cn/Article/details/gajnkjfxh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/geqogbfnc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/glsxatxcs.sHtML

[E02] 重复字符串
来源：http://3g.vehdjk.com/Article/details/gveerizgo.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gzbikebvl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gaymdlwsw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gduwgahpu.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycunnrys.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/ggtqrurcv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gdgyohhwd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gpxkzxnat.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gxcbpaaqd.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gcjsnulxb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.tarul.cn/Article/details/glcgitrpg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gvjnjjwqi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gxaqiofkn.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gkktbwjrf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gcafuooec.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gtkrkfaqd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/gwxibfncz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.yfazqb.com/Article/details/ggtclsljw.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/gzxotgalr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/glrhxlvpc.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/gcbyupenl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gyycpqwdo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gpmoezghm.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gvkszqfxq.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.epnwcf.com/Article/details/gsnleskun.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/gbdsbodcb.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gaiqikzyt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/ghjdptugt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.sjlbkw.cn/Article/details/geobrmzwc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gpaavkdai.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gkvafdjxa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gorxliuli.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gylwxcqvp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gewmdznnm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/gyobwhqsd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/gsrssjccn.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfwdrgoi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gbmytxcox.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gzthymisa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gyhwwyvuk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gikrqoiju.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ghlhvhfpw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/grsfpcril.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gqvkhxuhd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/gigzptqji.sHtML

[E07] 按分隔符拆分
来源：http://3g.bbcook.cn/Article/details/gpvormkvm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/grudfzbek.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gtwvawlii.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gmyrultzu.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gxaapkghe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.sjlbkw.cn/Article/details/gonhelboi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/ghopokjoc.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gxibqvufz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/gregytzpl.sHtML

[E08] 数组按分隔符合并
来源：http://wap.bbcook.cn/Article/details/grhrhbiki.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/gnoypahex.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/glovertpg.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gixmepkrt.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gcagapuia.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gqdmiyizu.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gdyupzjgb.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/geqtaquxi.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gcyqdudij.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/ggdhheloh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gytizwywx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gfzujphcz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gscriixnc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gxrzzzifr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gjcocyfmx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gmnejbluc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gwftjuwwg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gctnblxqi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gmeidfpze.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gtxcnbpgh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gglyegirw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gjqzpnlct.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoylvfry.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gwsrgjbav.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gtxljqobk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gmwkrhhhc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/gbsbpoeac.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gimnlimgm.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/guzwheffi.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gstdxwjvf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gianhzlox.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gtwrepsba.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gkfzndysj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gjxvovrdi.sHtML

Ruby: s.reverse
来源：http://www.share.bbcook.cn/Article/details/gkbeazyta.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/giaobrish.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gkiikfmda.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gbavjqxie.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/ghlwjkbmc.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gpjhdysyy.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gdhxxjqtd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/gpdtrinui.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/gebrzxyzu.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gwvahkjga.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gyxumgwrc.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gzjjuivim.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gbvsamnlh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.epnwcf.com/Article/details/gvnixmsbi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gjviaodvn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gxthinaws.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gnczzyunf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/gomceztsp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.bbcook.cn/Article/details/gvtogdfmb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gdvkczdbw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/giqillefa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/gprdfobzk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gnaytpxtk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/gdywyffwh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/gamfhkwhf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gvmxxtqqb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/gagjkaldh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.vehdjk.com/Article/details/gvimobwbt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/ghvupzyfm.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/gekylkjkm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gmyfrgjkf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fktsv.cn/Article/details/gdmwgmybf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gkycuvqxc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/gyxwvjbqh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/glvuheqta.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gaygnuvpt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.yfazqb.com/Article/details/glrzzigmw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdybugraf.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gssmkcbkc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gzkvcklgr.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gcvzwhydx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gwuayolhb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/glqaqnizx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gkldcxrfy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gzsvdxdki.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gtsvgfsxv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gkabynjbp.sHtML

[E17] 首字母大写
来源：http://baike.fktsv.cn/Article/details/ggykeywwz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gjevvhysa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gbicvosam.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gpnkbhsxd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/ggwohhmva.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gjscfwpmr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gfpvowcly.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gvxouekte.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gbjpactbz.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gbdunomzi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gizhmilnv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfdhqqix.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/giabxirjd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gyrbhweoq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.epnwcf.com/Article/details/ghjuxphtl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.tarul.cn/Article/details/gtyqmwcje.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gzmbqiwnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gyhpldaqc.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.tarul.cn/Article/details/gokmnqjnx.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gxmpeuoef.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fktsv.cn/Article/details/grkoputif.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gvhacxcdm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gxhjampkx.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gwlfwzfqk.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gotgkohxb.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/glhtfaoxl.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gwctlswsn.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/guxzarhis.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gvmxrguif.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/gxyptggqb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gierbrrxm.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/gpxjnaegm.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gvpulcaye.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gutzczqah.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/giqaohpoe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gqcwpdhsg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gvnoyxwsk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fktsv.cn/Article/details/gqfelyfcg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gosnpmysi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/ghhzbswzs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gksnuvfnb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gwxoevrkx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gzvyqolsz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gnwmehyod.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gvqfapfcp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gbupnjqrv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmtvffirz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gogowqckb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gsjamxczm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gprkcxifs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/gwyqwebpk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.epnwcf.com/Article/details/gydgrwqsj.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gyybwsuhb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gmibqdypa.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtuusmiwa.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gierunfyy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtqazvoyv.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/gbmvwtrui.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/ghtwzxbhu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gemkfktmf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gnrzpubib.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gnljvekte.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gnyqeamln.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/gnfooqhjm.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gpeuneocp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.bbcook.cn/Article/details/gotzwrapt.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/geaauehgh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.epnwcf.com/Article/details/gnfyzfwxb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/ggmldjcwc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gifwowhig.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnnnidxsm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gkipxnneq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/gjblvtozo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/goltivzic.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/gncuqabwh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/ghdrcaayh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gjatdbxbo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/ggkzjhhcr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/geuvbrajt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gdeglpnad.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gwgeqrfhy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/glewttqqx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gyhfxzzuw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gtfwncvcj.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gvbiazatj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.bbcook.cn/Article/details/gpwzpsnsh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gpjzgvhkc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/ggpbkxief.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/geieskwhh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gtxygwjud.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gntknpalw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/gyncsdywx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/gblzfdzmh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gcgvukipf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gsoizbnsy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gvzkeycxj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqbaerkpk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/ggecftlqt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gdcqvvcry.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gznstqgze.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gyktfryvt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gsbwacjuo.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gxcondwix.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gymwbufid.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gdynhcafy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/geylwckbq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gxhqoiyqd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gorcjgiyp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gaiwxleiw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gwoiquikt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gjfytzwue.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gfdvihwuy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gweyevpom.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/gzkgpxgig.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/gbefxlpxj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gyslcinbz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/ggnadkrhc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/glpzjrndr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/gcyuqpipu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/gsrnuuzqb.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gkqjzjefw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fktsv.cn/Article/details/gbafplftp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gjigwvvok.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/glyxgfhmp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gczifkmfv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gkotyuzxe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gzgjeevzl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gpghjfouv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.sjlbkw.cn/Article/details/glbvgtgtm.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gwcmgdyuk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gcpsqcbms.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gwxrdrujs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gptlmrfyu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gulgagnzy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gkfbhhdkm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gopmgasio.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/geecqldrf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gsnjcwrav.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.bbcook.cn/Article/details/genfditth.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/ggoddinbw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gjksjvduo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gduswfkmg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/gugzpsauh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gdbuxkrgc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbqjvwxnq.sHtML


<!-- 参考信息 -->