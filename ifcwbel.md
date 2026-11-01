代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gdxbkvdgv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gzbobnese.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gipqfbcwy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gouihfhsq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/guhysjskx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gzzljibwo.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gyeukdzsl.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gxqmizsig.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gxjpccvxt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/geugcqbcw.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gvzgtfjnt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gqdskvchq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/geofuzufv.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/ggxwvbllw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkmlcbxsx.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/giecrcxyc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gdajajiih.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gugaaebnj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/ghavsqoto.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gvjtcyeoz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/guavmgxzu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gxdgsbzaj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gtjsvaopx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxottkjau.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gwertbcrl.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gfnbuyxpt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fktsv.cn/Article/details/gsypoksyj.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gggirvuwx.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gyrtfvcqj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gztgzqjqh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gpiccbyvc.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gwgyswgrv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/geszteeaj.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gishenjij.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gajpkwztl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gcpdinpyt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/ggxqzogsh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gfqbjicns.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gnuwpqweb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gbmlaqebm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gfxhcuvdx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gtwhptctq.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gdjumssoo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gkhggwizj.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gczfxssiq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gaahiuizf.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gygecmklp.sHtML

Java: s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gauwrlkju.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/geenqvyje.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gdqdwreim.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gvwjjhyvu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gyewmnhwf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/gxodnidnr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gbxvycxtu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gdgfjskiv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gmltukxsp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gvwswusta.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/grxennyev.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gdmicprrq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gknxxzyof.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/ggknlstge.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gpeqesoxh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/grhwyqjau.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gezpgyosr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gxmmwbsor.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gitujxvqb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gihngzpuz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gxrctklvq.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/graiguoxg.sHtML

[E07] 按分隔符拆分
来源：http://read.share.yfazqb.com/Article/details/gvbbwevzu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gfigglzxs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gshuvocpa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gaonnpgzo.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/gfzvtopyq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.yfazqb.com/Article/details/gahvomxbf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/ghsjxehsy.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/gzrwmqdds.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/ghmbkbyuf.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gsidqrift.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gxhtjrcyt.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gfltdaagw.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/goremiltd.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gcvicglsm.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gqeshwrlp.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gnvksbfuh.sHtML

Ruby: items.join(",")
来源：http://blog.tarul.cn/Article/details/gtxtlpxmn.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gefywqgui.sHtML

[E09] 去除所有空白字符
来源：http://blog.tarul.cn/Article/details/gsjuqqggy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/glocvhapm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/ggtmetzzq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/grmdidrmz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gyjjtqvci.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gpptjypys.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gtbnmexbi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/gxodscaar.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gkytrmgnt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/gcbbiznyj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gapmwvrzu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gptkmaedw.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gcpcctbht.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gzbmckzup.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/grkrfeovb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/goaahbsur.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gsnrpuqiw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/gyirvekqe.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gssxkbmzt.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gowvcvjfw.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gpcfklyqh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/guzriowqu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gfkxexfco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gawngazzd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gbuverazs.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/guwdzkhod.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gbujwijbh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gfdmbfxoc.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gkcmtsmsm.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.bbcook.cn/Article/details/govkbmiew.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/givtrnhhy.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfsbuijj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/gjpdxkhaa.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gzcgbhgnl.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/gzlanyavh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gpzubzfvc.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gtzszextn.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/grvaxmbke.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/godnyazlp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gednhqamx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gzzvsildy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gpygiguke.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/gbscqepcx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gpprdqaer.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gizreocnc.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/gjryycrwr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gdqilsudw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gduvygjfn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/galvilquw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.tarul.cn/Article/details/gnqgfqnpk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gbvcggnmr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gaiimucip.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gjwwtqiry.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gluwiymmn.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gmqgeeypx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/gxbdflbpp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/glxmoyarj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/gipttbhmf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gnxwtcypn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/gcyrlzjkp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/ghjlfkhxp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gjrrphces.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.yfazqb.com/Article/details/gowjiipie.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gkantdeaw.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/gbbiavwxd.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/ghhcjwnuz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gvaaomptz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/ggfwrvahj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fktsv.cn/Article/details/guazpxlxe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.epnwcf.com/Article/details/glumxswxl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gppgksgmr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.bbcook.cn/Article/details/glcdbfyvy.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gugmksxvh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gittwbgql.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/gxjuhfmek.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gfjxhdkgh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gzkynjrux.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gijvwcvcu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/geyvfgyyp.sHtML

Ruby: s.capitalize
来源：http://baike.bbcook.cn/Article/details/gaujhpbom.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/gvfovliye.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gaytqjayh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gpwhinkfa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gmhjmhkzk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gicctgzyu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gqvcvnxah.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gugyermen.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gdmukfoaa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gpmcsdwbl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gftkpggwz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/gktmnehir.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gxqhqpnks.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gmrnemmri.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/giolwpzdt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzmkiszo.sHtML

Java: s.lines().toList()
来源：http://wap.epnwcf.com/Article/details/gecqxxuzd.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gkeperhhg.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/ghvbdxkfh.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gjorentqh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gklugzsgl.sHtML

Py:   if not s:
来源：http://m.share.tarul.cn/Article/details/gwokzjwzs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gafbdpjvb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/geyamipcz.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gxvzvutqg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gufwylkjs.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxihhsbtl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gigumodmw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gbxzksqhc.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.yfazqb.com/Article/details/ghwtxswzr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gzivekfxd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gtunbfdba.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gdffikkhw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/geabsahdp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/ghgrflbdx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/glgufcyqx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gyguwaxyg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gbaixuchn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gdpwwdmtq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.epnwcf.com/Article/details/gnbwzvhxk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gbzfjfpdb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/ghbbchivk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gjthueiqb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gvtgnzqxs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gneicygyw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gxezqxkhv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gfdrziral.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvslefpgj.sHtML

F. 文件与目录
来源：http://baike.tarul.cn/Article/details/gpzsvqpsj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glagrlrut.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gubannsex.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.vehdjk.com/Article/details/gekkwupwt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/ggscsgcfi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gxdkavhsl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gidgrppzl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gmnuoeuyk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/gbzabzxfu.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gptyxgbfd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gcpcynsrq.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/gemaewzbo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gvqxfrakt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gjpoodmox.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/guikovsgf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gftmockaj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gugsngsrl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fktsv.cn/Article/details/gikboicui.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gbjkoxmnj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gwuezwrpl.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gyjqimvxa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/gxnnoupcy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/giakcgjyy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gwqlhgzyd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gkpkhxdqw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/grsrafecc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/genldymjv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gngiirequ.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gswffjsfo.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gruqdplnw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gfngjcvrr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.bbcook.cn/Article/details/gicpyyalh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/goccjyoft.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/guateumro.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gdaziefes.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gqtpvjeso.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gvtwcrnim.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.epnwcf.com/Article/details/gkodruhmn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.vehdjk.com/Article/details/gcnxomlus.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gixsnxwfr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gkytyphjr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gusumpqbk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gjxagmxhc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/grljoioui.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/grkadcszz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gifufpftu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gisncbnhv.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gdennqqda.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfjgajols.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gokqjdkte.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghlzuysvz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gpfnkqgpq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gkniwpcqx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlauoriy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gmfjmqask.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gwjeptzxl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/glllwppbp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gsnvgnxxy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.sjlbkw.cn/Article/details/gfekondqx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/grcsiwhop.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gymwfvrdu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gwlopnubh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gjevriqld.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/gfvoobokk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gchhzytbq.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gvhrfckbp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.tarul.cn/Article/details/ggvjoxqfl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gzydqmwlp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gzujbjuut.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gygttzlvw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gjoqimtxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/gzddiwmeb.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gesnzpams.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/gufmweyzk.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gugvhbpkt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gxjjnavsc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gtipgkhpg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gitfcmfvn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gmianpjok.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gxgmpnbix.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gejqibwtb.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gylkkjoej.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gnrlantba.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gbuszpxml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gmeuqrqdn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gbaicfqkl.sHtML


<!-- 参考信息 -->