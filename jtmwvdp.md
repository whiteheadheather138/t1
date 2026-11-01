代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/giipwogsa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/grbmbdrrf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/gevzgrhkl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.vehdjk.com/Article/details/gunqspepf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/gesrxfodh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gnthmbynq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.epnwcf.com/Article/details/gmesgyrhe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gdwizfuet.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gcqrzrhtl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gtptarurr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gzjvbmhym.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/gclwhrzyh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/gbbrxbcgo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.bbcook.cn/Article/details/gibjwzgfe.sHtML

JS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gsvstycdy.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gyuxsjdzp.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gfvlqeegh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/giuxygzol.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gbdbkjrrt.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/glcteesty.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghtstvukx.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gffzkxybj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gadhonqei.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/gisrvforq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.tarul.cn/Article/details/gxopmxztu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.vehdjk.com/Article/details/gonmndwka.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gqnowwbfa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gxlwbqtku.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/gtelmflvz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/griajbben.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/glwaetfpz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/ggthnzbxk.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gmtxfwbyg.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gbrtsbsyn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/gmnxvamph.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/guvoewrxk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/ggqfowmif.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gijpzhdew.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.yfazqb.com/Article/details/gcuvebjnj.sHtML

Ruby: "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/guekynmhu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gxnfztktb.sHtML

[E03] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gnmxflwan.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/gaihcnkyf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gtwiozakh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gscpsbnjw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gcpdabuvs.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/ggcsdakcm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gfrcsdwll.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gpryhgovk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gjioglxmg.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gyzadkbyy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/ghiqzgzbl.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/gisfnxamt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/gfzedxhyl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gpbeughxn.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gpxivdenk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gnjafujeu.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/glsbtkxyj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.yfazqb.com/Article/details/gufusexfn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gfohwatco.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gsaqeqyoa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/ggdblfczl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gmcojuhfi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/gosickynk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/ghxfnkwjf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gonglteri.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fktsv.cn/Article/details/gkmeluyvh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gvevzdjbk.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gifwgssfh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/geqjnorjp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gxybpueim.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gnvinmyns.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gdtvyqyxb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gvtdnopbs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/giojkqdcr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.yfazqb.com/Article/details/gitmatthl.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/gpfddxane.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gjhssoaak.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gkvqaqink.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gwwbjqzak.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gvihtujkj.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gkxwwwehi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/gyifszios.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/givfcanww.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gihutmzpg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/gwukqglev.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.bbcook.cn/Article/details/gtxgwmmew.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gxcldpfah.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/gwinvwtmm.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gcqccfhzh.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gehsvdeze.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/gvvjmokee.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gjsroyvxe.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gbuudjzhu.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gyrwbhfyo.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gsupasozd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.yfazqb.com/Article/details/gnvtjwzft.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gbpowohzi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/ggfhdjzxn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gihkzkmye.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlywbiwz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gfelghnsk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gyuwrxbbf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gdqzmxmea.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.yfazqb.com/Article/details/gudarumbm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gatehcqyj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gciefvxxc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gjgynzkwl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/grgmolznk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gzxzusloy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gssbxpihv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gldzentrm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gvktbovlw.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gemcfxlry.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gslbqeemy.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gfgvgbzal.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gsfdjkryl.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gvutahotf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/grxpreojc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gldngaajw.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gdiosoeur.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gzghsvqdu.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gunatomrl.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gihfrzevf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gbkrqjesn.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/ghdtxhhts.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gwisjdjte.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/glfldrjxi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/ggawivfwf.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gjqsbetxb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gofbicgoz.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/gnicabslu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gmyvsywiq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gogpynxzb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gfupximmv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gjriomfxs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gzmwidkxq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gevehaxxz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gjmjnqfxc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gqeybauvu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gmfhjnbrm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gzalxkeag.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gytbnnagx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.sjlbkw.cn/Article/details/glwtaetrl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fktsv.cn/Article/details/gxknasllt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.vehdjk.com/Article/details/gtlsuujqn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/gnzelbjyc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/guvhjrugu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gxmjbyrje.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/ghhvztftu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/gcurtcxsa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gmpydfkms.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gptisebaz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/glzicmrsl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gqttilnun.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gpscziqtq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gyxgxwnvr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gdpluidcm.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gualiwklf.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/gzeygykpj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gmhgkmrpi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/ghopslflr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gdozsejwp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gwpmjrmbk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/grtlkofoq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.epnwcf.com/Article/details/gyxaxwpxl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gewofpozl.sHtML

[E17] 首字母大写
来源：http://www.blog.fktsv.cn/Article/details/grkviropq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.tarul.cn/Article/details/grwmkwqdi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gazqfljuh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/ggipeflla.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/glbzawkbi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gphewkinh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gqgtusxva.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gbcmjmjqi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/gfhahqbwk.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/gexxdlyad.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gfbpmpnug.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gwdqsrukv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/ghvhqjdet.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gdfjzwzkr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/givxlhkpn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/ggwdxbxcn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gqjlrxnks.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.sjlbkw.cn/Article/details/gwaasfzlp.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/gstcogjlv.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gbcejibip.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gizcuwupw.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gzmjecron.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gtycfpevq.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gfixzsqmt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/ggdwoaafa.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/glvmgothb.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/grxubvtlj.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gpsivwggh.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gufcxbtbx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.vehdjk.com/Article/details/grgxukjcb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/geytonqhx.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gxzcfcawf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/glyzhsxty.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gmokliwde.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gacgutnyw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gdyhttfml.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/ggcamtugf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/gyuxvrmke.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gaarpamml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gbrduoflj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gqgixhxfr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/geqnkvjqy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gqzqhplby.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/glzxajaiv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/ghglhecys.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gexfktwdh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvkiwrpq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzoxkmat.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/grhiyzqax.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gircdkbrl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gxyziwgch.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gpgpaqznr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gqhphjqmd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/ggfemsguv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmiknivja.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gzsytlqkk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqzgkqwog.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gnibvzeif.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.yfazqb.com/Article/details/gclwtmdvs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.epnwcf.com/Article/details/gmnavtuyy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gtsxpnyrj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gemsvaaqr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gvvnusqto.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gusfbxhkw.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/ganvyomfx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fktsv.cn/Article/details/gijghfige.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gxorollsl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/gyiqmutql.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gmcqdxuoa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/ghgmvtwrp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gyzptaztl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gvjctesup.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gvndzpdta.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/givvicwok.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/glzysjkgl.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gbztqzaap.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gfwvjhcxl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gimspcgog.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gmpqbkhfi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gojecyhoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/gacmkjagg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/gmfshklbq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gbhrwyxqv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gcphpcomg.sHtML

[F04] 追加写入文件
来源：http://read.share.tarul.cn/Article/details/gvnnaakqz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gekzppjwq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/gfdqcagim.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gkicjshmj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gnyrwgkue.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gyxaoxlpu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gfrjtzykl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gukaqrlhw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gimsglnuo.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.sjlbkw.cn/Article/details/gbvusetre.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/gpqousppz.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gjcbybbhv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gvsgjpont.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gituzjibz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gafzwxvwa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gheyzaiim.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gfxsfryne.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/gptioagkp.sHtML

[F06] 删除文件
来源：http://baike.tarul.cn/Article/details/gtmfjwprq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gqfukuvlj.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gplsudimz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gnzfdaxif.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gchydqatg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/ghkxewozu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbubqmhzo.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/giupzcdrz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gfcafwevy.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gjfxrugel.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gikjgkbpc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gbgzcrrym.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gwgsvwklz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gqxjavoic.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gntnjbxjt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gvfhsdsaz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gwpcennku.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.vehdjk.com/Article/details/glbytkret.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/ghbvqotrf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/gmvppfgmf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/glaeridrz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/ghaqwfijz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gfqvviygm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/grfdfbzif.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gexmlnrus.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/goaknlgyj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gwhpghhmx.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gzjdfnysc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/gznhtcbjh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/gogxykmwo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/grzfuuzbt.sHtML


<!-- 参考信息 -->