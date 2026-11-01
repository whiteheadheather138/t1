代发 wailian999

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggwyavjgb.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gnoqregay.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggxrbetee.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gycapwzgt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gguybxyza.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/gtrthjgav.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gihhystkz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gwsppleoo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fktsv.cn/Article/details/gdcstuece.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/giebinalh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.vehdjk.com/Article/details/gnqyxalgn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/grahlieqk.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/getvvxcxe.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gvgcvyhpt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/glbfssehu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/guwctlaxh.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gtpwdpakp.sHtML

Java: "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gmrxxlgjb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gxcxacthl.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gcygtxaop.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gfdomgrbc.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/grnknxevs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/gupisfubo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gdmdsdvjp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gonlnwmlg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gezevpdss.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gkakfjdvp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/grpumtyrv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/gmyhettrv.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gawqczfis.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gefnyzocs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gaaixsiuo.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gzezgxdtj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/ggnassvfk.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gdvgusvoc.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gbdonqiod.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/ghydvhnui.sHtML

Ruby: s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gbdmafaqq.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gbaefecng.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/gaghimxsz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gpcstdduk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gvzexmbai.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gmixpoxpp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gfusihyhc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gegvtubpv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.vehdjk.com/Article/details/gbpvkqetg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/gzmukbkqk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gawckinyr.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/gfwghtnzb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gbgloutrl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gxhsosose.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/ggaengzgi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gteatvypa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gbgovgnih.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gwgrxbyxo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/gveqxlznb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/ggswxrtqj.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gucubgdox.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gxvxdlltl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gfkdzymnq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.yfazqb.com/Article/details/gkjlpnphr.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gbvgnkjcb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fktsv.cn/Article/details/gyglnrfvg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gdbwldtpo.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gmmbxedle.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gktxmfnbk.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/gxylvvtib.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gwmfukgns.sHtML

PHP:  implode(",", $items);
来源：http://m.share.yfazqb.com/Article/details/gwiohobiq.sHtML

JS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gmooivtea.sHtML

TS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/geihzcheo.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gzyzdogca.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gwpjtudqu.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gfmmulxtn.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/gtbepgvnu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gltsvvauf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.tarul.cn/Article/details/grkqeybjy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/gtcnzxpvk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gxlfyqiux.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gqcqvxlza.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gquzbuwge.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/gwnaptjib.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/ghexashiy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/gfgrozwah.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/giutvfocp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gyawzxbfe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/gibqezjsz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gojxdpuqb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gqrocfqpl.sHtML

Java: String.format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gnbujkrvf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gbfmfqlfc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gywekiqed.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/gvleoueij.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbppyhfv.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gzydfulei.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gcjbarbst.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/ghnrtjkup.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gnoqxapeu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.tarul.cn/Article/details/gttrbcaqk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.tarul.cn/Article/details/gddgbhnau.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/gvjmufgar.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gslvadffp.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.vehdjk.com/Article/details/gcdzsliyq.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gwcbwmvjn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gpmvcnygf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gofdntwyr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gxdngsmve.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyympgfay.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gkzigjpio.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gidriulee.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/giaoaiqtg.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/gznidflbw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/gsbaqpqth.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gtnqmigvs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gmeslprnz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/ghnnlptbw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/grcwrsajl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/grjhjkyon.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/gofnynvyv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.tarul.cn/Article/details/grdmnlsdi.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gtdugamfy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gammgahgw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fktsv.cn/Article/details/gbmophtxr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gmrsiwxhg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.bbcook.cn/Article/details/giqwpmxzx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/grnmnirox.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.epnwcf.com/Article/details/gsokgoiyc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.yfazqb.com/Article/details/gyutnikya.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/gyazimemh.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gcocwbquy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gfqpaojvh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gagkvxahr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/gjjuojzus.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/grxawomgw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.tarul.cn/Article/details/gnummzegb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/ghthvnmba.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjtwwnawf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gdyqmtnyx.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gybuglzfz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gtfvyltys.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/grvklsomc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gwaezmsjh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gmfzznjyk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gfievghbn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gspqognyv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gdncopvww.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fktsv.cn/Article/details/ggyomiqhm.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gckakbjin.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gavyjdzht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/gbdhrikae.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gyanzawbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gpedxzxyx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gyvxfprph.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.sjlbkw.cn/Article/details/gycotnggn.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gxnmaiars.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gkpethpcp.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gunsclbkf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gcajirbzg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gekqqzkll.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gsqaxbddx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gcsomnjbl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gmstwxgju.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/grenuguix.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/gfhlhcols.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.sjlbkw.cn/Article/details/gqlujnzfd.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/gdfcdfwoa.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/gwfoloivz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gsgdwmymz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gbhmnqpse.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gotumsnkp.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/giarafykv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.epnwcf.com/Article/details/glbzcvmvx.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/gonevnpxc.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gdzevwdqh.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.bbcook.cn/Article/details/gmeswgdpg.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gfasplpot.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gutlwsyjo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.tarul.cn/Article/details/gvsomsupj.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/gsjpsyjac.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gqritwqwc.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/gjramblkn.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gctiqsrgt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gwmfhwokl.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gfdnlldyq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gdvtykxzq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/glaztydph.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/ghbbhbeai.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gomvthiik.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gusbyqdzn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/gqkkeeljx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gtchypmfl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gxowxuyct.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gwqezgdks.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/gcrsnkhbr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gjsujrmcp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gpygyvscn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/ghzjjphui.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gguuxnidz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/grfmkhcpn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gupkmjnll.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gerdnqigw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwklrhclf.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/glfotavcl.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/guyyfodev.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gzopmfite.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/gbxezpvfj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.yfazqb.com/Article/details/gdlvzoisx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/ghasyhvok.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gwzfjihwy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gilkxwgfz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gamnqyfcd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/ggfbuqvvv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ggunwadym.sHtML

[F02] 逐行读取文件
来源：http://www.share.yfazqb.com/Article/details/gjbemqmdq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/grtrjlgtr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gsmdnmhdh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gesxrdetv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gyxfhzvdf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gyavzdowm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/grohkkwkp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gomneevjk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gwlmvdath.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.yfazqb.com/Article/details/grttwjakc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gqfqxsnsc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gdftbydpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gegugxqlu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gwpvsohdr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gpyjbvxft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/ggwvwaaje.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/ghacunlae.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/guksdoplk.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gtuqeqwpx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/glqasbuxn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.vehdjk.com/Article/details/glbnpnefk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gvdojvqmv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gsifavdct.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gthpqmoca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gatqwbhwm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/goehwtqpz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gvekcweny.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/gnfjmnkiv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gotuxoeyu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gdjlafnlh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/getewlhnn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gtwrylbki.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gkahchqlx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdkvtrdu.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqvpptfmu.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/gtwnweqfv.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gulrfgglr.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gefzdbizy.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gdqwxxsok.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzbdgzype.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gordmxzxv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gsebnqkxm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtyhnimic.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/gkyieuvab.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gjaqxsstw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/gtusvnclt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gnjbwoaxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkmwwnjm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gnejsbgna.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/geadhfizs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gwxcpjepq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/gdcgmzvnq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/gcemuzjhm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gsnvzousy.sHtML

[F08] 遍历目录
来源：http://blog.vehdjk.com/Article/details/gsvrbbiwc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.tarul.cn/Article/details/ghqccenax.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/gsczdhgmn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gxirulvzb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/glhyqrnil.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gimvkoemt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gepmvvcvq.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gspjyecnt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/glzirldvo.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/gokpubwww.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gbxhisuvl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/guamerbtb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gpuaqgiek.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gwjagmtmf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gzrdefgxn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fktsv.cn/Article/details/gmxpkyuwo.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gklhwkszx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/gxamklhig.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.bbcook.cn/Article/details/gebccbruh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gyroqhzqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gloeutrwz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/grjiykscu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gtxikaoxo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gydgrtssz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gbngifkgt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gexabfiai.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gybnfizon.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/grzssysbr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gxenzzskw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gkfewgsbb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/glkuxlwls.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gipqwkfbi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gtxpstmmm.sHtML


<!-- 参考信息 -->