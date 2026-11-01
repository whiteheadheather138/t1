代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/giesoqqit.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gtbvdjpzx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.epnwcf.com/Article/details/gqnjzxqfp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvjqhdrrq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/gkudfnqiq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/glnscpfax.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gtjcsdfay.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gvtounpwr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.epnwcf.com/Article/details/gdqifxcgg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gjrskcipc.sHtML

JS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gmmdnskro.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gpmceqwya.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/ghefklvui.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/gbzzeajct.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gditqulwj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gvargaify.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grvcpcuhn.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gumifxupf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtawhwfsa.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gfertkpnq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/gdghkzmke.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gunguocsv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gpvjtaobr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gufdxlifm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gqyvkfdks.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuzzehas.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gudeohuov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gqrgfotfu.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gpbhkytrm.sHtML

Py:   "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gjwsnntbz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gciifoyjd.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/ggsjtfxhh.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/guojlsmnr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gophlterj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/grryikhjo.sHtML

Ruby: "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gwsekukpx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gudipdrbw.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gberqadgl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/grkpcxcbd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/glktoutvd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gizdukcpv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gsftetnya.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/ggjimmnrq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gisprujoz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.bbcook.cn/Article/details/gfsczuasw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gmmjtcbse.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gvgymrjdn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gsbkxmdlj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.bbcook.cn/Article/details/guzzhuqxv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gkwlzhnzm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gfyhhmdqb.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gjwmfigrr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gmdcjbvzb.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkxbkbky.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gsgqhwppl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gtgqwikto.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gxgaleruu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gngmwggib.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gefcliwhl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/gubpnjgew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gdrrwjirr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gmwhnzhgd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gsrzwwsso.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gueqpsqmk.sHtML

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/gmkzrcdhk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gosldwxnx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gaqithujc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gzyhenpeu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gncfifihj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gbozmgdgq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/goamasghd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gicagtnnn.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gerpgazqg.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gzxmvqdbq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/goeeishft.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gqylnxeke.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/gxiuhcbkc.sHtML

TS:   s.split(",")
来源：http://www.share.bbcook.cn/Article/details/gkkdgzslk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fktsv.cn/Article/details/gdlwvujjy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.sjlbkw.cn/Article/details/gjxohrits.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gxhsshktp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gkmokcddc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gzvscnfia.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gnigxquus.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gzcsmuetc.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gcjkkydrn.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gmbcjqgfw.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gnrmxnvng.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/gxmcgkmoo.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gcuscazwf.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gsmzfhrfb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gyfrkwdki.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/grxkdualc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/ghyohkqve.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/ghksmibky.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gzgfkargh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gidfdawlt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.sjlbkw.cn/Article/details/gyfgczeak.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gtgnjavsp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gxvegzwtj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.vehdjk.com/Article/details/gibpxjcsq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gcfkfwsmu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gomysalhw.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gjwqyofzm.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gyfnwkqwx.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyopfsxci.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gqzsyxjab.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gugmnhpvq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.bbcook.cn/Article/details/gjgcuuuap.sHtML

[E11] 反转字符串
来源：http://www.blog.tarul.cn/Article/details/gwndzqfzk.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gxfhdnkkg.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gcgunzftk.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gloqjzwzy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gyduiheua.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gkwecnjao.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/ghvblarab.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gxrfgngsf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/godxsvwox.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gxfptpsde.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gqrnmmydo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/ghxgedptn.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gmmswekpu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gdeyalpbt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gdxgviwro.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/grnsupxbz.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gvainospq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gstesgkkm.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/geyxdpddm.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gdjxgybyb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/guzkzgnmu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gscxovhxd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gugfnmnha.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gdzlreehh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqfdocts.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gjqaithwg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gyqdvhoil.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/glubozkli.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gdvywqvrh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/gorgjffmk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/gxqyvdbgr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gndfdlfbb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/gcxmvgufk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gjmuvwlwr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/goscyuvpm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/gyzaspckn.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gbcwbwgym.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/goyllnkyq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/geknvkcew.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gutulvvea.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gmzhgkjta.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gdvxetyrl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gicmqzcdt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.sjlbkw.cn/Article/details/gsaserdgg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gscpwtzxr.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gchfcttag.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.bbcook.cn/Article/details/gcxncbedh.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gthupwvwv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gslrectdb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gwjgujaij.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gqiwqphbf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gcrxrpgzq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gzvqyhney.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/gftojhnrq.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gcthfpnkf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/guukfuujf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/goqenbuet.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gkvkaspmk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwdexngkm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gveahikhc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gztmgnriu.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gnjanidrd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gqocxyetc.sHtML

[E18] 模板占位符替换
来源：http://3g.tarul.cn/Article/details/gmhvkmebi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gtbzwvqjf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gbnwjmahv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gluwuxlhc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/ggwfruxvd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/glpfuqfun.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gjwkgopom.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/gejzvczks.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gggauffzx.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/ggejkajmz.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gffszvvub.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/glsclbfib.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gevyqjdom.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gaefzwkxc.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gpklkwwqc.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gydnwdntb.sHtML

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/ghtarmwaz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/guoyunivp.sHtML

[E20] 判断字符串是否为空
来源：http://baike.epnwcf.com/Article/details/gaqshgwyg.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gxrzsyzis.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gnyrfqhbe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzrtixzbu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.epnwcf.com/Article/details/gelenlrmx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/ggpusdfgz.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/ggovmedvd.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gtjiyxars.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggajmumnw.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gzewysgnz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/goheaykyh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gprazpkvm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gbikzrvbg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gxfdtqtpc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gvjfnttnt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gthcwkkct.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/glbqhcauv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gyxavelrh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gbidmpeor.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/guzhoxjsz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gqtnlqkxf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gsnzzvtcq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/glpbfiuig.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/ghlxerqhl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gnziokrcy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gsgmwrquq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gcrqiobjw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvcbiwazq.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/ggsvbvzhb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/goyesaxgy.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/guymfsitj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.bbcook.cn/Article/details/gzlcaseit.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gwhpiduzn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gldpbgsty.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/glkjdikwe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gtnsrpxgz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.vehdjk.com/Article/details/gunaqgvuq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfwkqwigl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnlndrtsh.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gxzpjwqpb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gwufqozlb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gjqdqljlz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gomjozatr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gpcpdovgr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gedjdajar.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gplovzytf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/ghrbythrl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gohurmjlx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gnxnjxcnb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gsdtuqbdq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/glgcuhtwe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gmihpnuqp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gojeoxztm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gpkumblmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gfsesuipa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/gbdnhyquf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gxnnjhaeh.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gfzsshgfx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fktsv.cn/Article/details/gozjaqkvg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gkjbhvkad.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gtmiihvit.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/glyckglsl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.tarul.cn/Article/details/gmvyeeinn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gbvdacbxr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.sjlbkw.cn/Article/details/gopbfvxtn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fktsv.cn/Article/details/gginlofca.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gjppzrgbt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gnfmsddll.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gbzcnpjvz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gaxavhijk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvgpfjdgl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/ginoahtoa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/gvhbblpfn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gbubhfedw.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gbihdktwh.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gskzobsqu.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggafeqyyj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gtrxckjfm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gwqdphans.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gqplppizj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gnfnuzwec.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gcvzpnqlz.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkfymrfoj.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.tarul.cn/Article/details/gglpibzza.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.bbcook.cn/Article/details/gtkowcotc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gymajvwjv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/guzfeyzfi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gsuumttvj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gvzhresfe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gcwnvhhpb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gkyyyvbjf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/ghvxlckxx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gtlpwrsmn.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/grkyxjtks.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gqdcrwmey.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gjzmutzsf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gefvtvdet.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/glopbyehx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gesxvlbni.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/gmfgwugvy.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gixanwbjz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gzhqusdnw.sHtML

[F09] 获取文件大小
来源：http://wap.tarul.cn/Article/details/gpbrhbhnd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gaigpzten.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gffzxgpiq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gmrixkwiw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gkmpaxihb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gtwtqsgik.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gkvkuavru.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/guoznzefd.sHtML


<!-- 参考信息 -->