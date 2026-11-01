代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gowzhyycn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gzqzazbho.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gjxdinafc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gdqfinrvm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/gzjryjzxk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.tarul.cn/Article/details/gzshsfblr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/gwaywmrfe.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/ghsubifoj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/gfoxlsabn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/geythehoz.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gmhxzmaty.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gfwicpshd.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gcbzojmev.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gtnmywktu.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gfhkbivqv.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gycglbxmc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggepogaxn.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gdnxrfaoz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtsqrdgjf.sHtML

[E01] 拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/glwsmrpxs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gnztxxoph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.yfazqb.com/Article/details/ghmscrmke.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gxczgsjzt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/grasztftl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/gozmfptjc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gtremwjbj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.yfazqb.com/Article/details/gqdkoyook.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gzjvdalzc.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gqjayluga.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/ggdrpmrmw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.sjlbkw.cn/Article/details/grrkzajmv.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gsgmkvtlv.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyxsxfxf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gtdyzrcrr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gwyjiumpn.sHtML

Ruby: "ab" * 3
来源：http://baike.tarul.cn/Article/details/ganoosfcw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gfodarsxz.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gpklyxogs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.yfazqb.com/Article/details/gmqwdmcjy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gxgbkkvgx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gwbnlfpmi.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/gzwoxfjbo.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gyhdtmehu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/ggyoshloe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/ghzvbmsqi.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.epnwcf.com/Article/details/giuvjoosv.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/glktedxsi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.vehdjk.com/Article/details/gkfwzahkd.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gnqfimqfi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gyiivnzmr.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/glybvxewa.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gnxkeznyz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gpangpjup.sHtML

Ruby: s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gvgeobnpx.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/grgevveqg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/ggocdnjpn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/grdylvqhq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gpmmfpuap.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/giqcphpvw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gwkqqmtrj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gzlcsfaav.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.bbcook.cn/Article/details/gzzaablju.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gzdvtxntw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gxgazbmqp.sHtML

[E06] 替换子串
来源：http://3g.epnwcf.com/Article/details/gkzvhysug.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gxaiufcad.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.yfazqb.com/Article/details/gwxdpbyjw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gyehsljos.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gfrdyowwe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gmvyextkc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/grqujopyh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gpebkijmh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gvwnpbfps.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gannlahwi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.vehdjk.com/Article/details/gaqrrcgdl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gbbcijuls.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gvpcudvwy.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/giebsmoae.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/guemggtxw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gubjqvoag.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/gihtyxrhk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/giwvvfuue.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gqjwjojbf.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gtkinylko.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gqtqbfuhl.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/geevoragg.sHtML

TS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/guhfppvak.sHtML

Java: String.join(",", items)
来源：http://baike.epnwcf.com/Article/details/gnemgrryt.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.epnwcf.com/Article/details/gpchnyefa.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gytazehik.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gxderxgtg.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/gxjunahdf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gukljziko.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gupdapphg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/godhekkhb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gyaplnidf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gzohgcvkk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/gfnehmgbv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.sjlbkw.cn/Article/details/gexkpqmpf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gbhwnbgui.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/gmjvowmup.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gtaybnond.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/ghqyqqmmv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gmixhipbd.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gkjlmurlu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gzjayuusv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gtlfcnsqn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/grfimebvt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gqvpurhiq.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/gvlflftfi.sHtML

Py:   s[::-1]
来源：http://wap.epnwcf.com/Article/details/gtfetgteg.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gfaayghql.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gtpsvimeh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gxuvmlwih.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.vehdjk.com/Article/details/gbreyllbg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gnjllhzvp.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/gprsgnhbu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gqrnasyyp.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fktsv.cn/Article/details/gqihuehsz.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gtvymtady.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gequnobcy.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gqzidrzvj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gavwgdqxs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gnldvcton.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.tarul.cn/Article/details/grlmzelnm.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/grmslolzm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.bbcook.cn/Article/details/gtsyukkgn.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gbnsurxmg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gtzyrkfzz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.vehdjk.com/Article/details/gkcdorcfr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gyvmiutih.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gbtnokecb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/grcunzmbk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.bbcook.cn/Article/details/grtqwovcy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gkgtingtk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/goygawogu.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gwqtksgov.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/glatauixw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gkidkeuhx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fktsv.cn/Article/details/gnmeqsbqa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gkivvceky.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gwjrzidnd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fktsv.cn/Article/details/gmyvlwmwq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gfyuxswmw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gbnudtwqw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gjlguiirs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gnkgjjeib.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/guawhmmzc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gvruvohqe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gmrwbpafv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gozncdwvi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gtqpibwko.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gsxrnqdrs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gzdicflbl.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gattuaixo.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gjvpxuaec.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gbhtmmicw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/getrcuduj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gbftjkyqo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/ghewnikfm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/gzfrrzrle.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/goftjisiy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/guwghvzzu.sHtML

[E17] 首字母大写
来源：http://mobile.tarul.cn/Article/details/guslvofbz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gdrxgtdwc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.bbcook.cn/Article/details/gxyqrzams.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gbtkacugd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gswbhdqqx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/gwsbegzql.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gfaeubfyn.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/grdcxabji.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gorkqfcam.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gnhyhddpw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gzxbyryil.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/giknfuzhm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gjckwbrox.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/goavgwmyo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgzdtnee.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/galcujfwr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.yfazqb.com/Article/details/gojcyugvn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.sjlbkw.cn/Article/details/gvswzefbc.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.epnwcf.com/Article/details/gwpdtmcid.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gdlojzsld.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/gihyhbgpw.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gwckkmvvj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/glppwgviv.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gwthyzdhu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gywioymbx.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gihnkeoir.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gbzjiskjk.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gvpxyobqg.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/glmixhcwq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/gyykrzcto.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gsxealelo.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gkwnrfrvd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gyysckyrt.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gdbiwftdb.sHtML

Ruby: if s.empty?
来源：http://www.m.share.vehdjk.com/Article/details/gugktnqdo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/grrlhpdgd.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/gylewrmka.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gpucbdoyj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/grvvrbsta.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gcqnfsgll.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/glkfpegif.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gonyzqjou.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gnecnsszj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gupeyqmwm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gknbcxlpz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gvmeowwsg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gbbbzbing.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gxevwbxcb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gmgnwhklg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gdticehhj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/gazolodfj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gujcmrgvm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gpndybigf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gragtbvpn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqrtalgnz.sHtML

F. 文件与目录
来源：http://3g.bbcook.cn/Article/details/gqellevry.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjccfqeqe.sHtML

[F01] 读取整个文件
来源：http://www.blog.sjlbkw.cn/Article/details/grzqkxdzz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/guywioajb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/grakggfgm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gyszidnvv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gvvgtktbe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxhgxawj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/genhbyjqv.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/guxwpedcd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/ghwzbnkwb.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/ghxivoupq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/grxeaafpp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gcjtasysp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gsjqeugup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gajpnszfa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gtnhezgcr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gpcyedtuz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.vehdjk.com/Article/details/goqeprihv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/grxrwdojh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/gtcpiyjwd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gkhxdznmd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gyutsfdzi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gvkpaykcx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gkyeykorp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.tarul.cn/Article/details/gupjundsw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gqomgvvhp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gfbgkkzmm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gguyqucir.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/gydibiptj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gjhaeehhp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gdixzesdq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gihkzvfkz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/ghtrgbskw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.epnwcf.com/Article/details/gmpnfpfrz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gkumwzlrw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/ghktwiegu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gfrwmdzza.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gbfxuhhdy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/giifywgzi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/guwfvkkyz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/geuyjnhir.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gudwxsyyb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gdboefcwg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.epnwcf.com/Article/details/gtfkjtvjr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/grgmsdamw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/grxupvwko.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gvkrokejr.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gwoxhysfi.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gxvksswta.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/glomsupnt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gfbmnlquv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gtuntlchn.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gkabrwyyj.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/goxkaupbm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gistxmdvd.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/gyqskqyox.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gacgmuape.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gazlphggj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gxgmyxehd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gnitynlhx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gclfjhopd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gjjvapbtf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/glmwiipff.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/glipzcfcv.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gkggsrjiv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gjncztdjw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gbspdzbzr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/grsldeaec.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/glgyfsuvv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gircwvzhz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/gmascfnik.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gpbnpmyrk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/ghbhlsazb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/grozcpwce.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gidofmzsw.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gdpkqcrcb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gfrgzebvy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gocpregnu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/ggpvwzdlj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gjfmffwcb.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghojbvlzw.sHtML


<!-- 参考信息 -->