代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gcwpfovfz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/gfmimhsvr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gtnejurzj.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/guqnszggn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gdybxbigs.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/grrpjtfbw.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gjscfspju.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gaogacehi.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gxxjbmzkp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/gnnfebess.sHtML

Ruby: arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gglsfftbf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gufuqdgyj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnuregpan.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gkymxcrhq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqbtruolf.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gdlvfklmv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gnhbwyfte.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/gtbywiczu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gykcfbxcq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gujektsab.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gensruwys.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gdztivrvl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gckmdnnmg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/glgtwrvof.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gzjyxasqw.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/glocamiha.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/govmmofxg.sHtML

JS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gbzujnpfl.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gcjnukcup.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gzuwxbgmk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.yfazqb.com/Article/details/gzyglyhxz.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gjmzbnvgi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gwjuyhmfa.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gxabzkawi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/gaoxbgfhr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gcztmqnzi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gybxtpino.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/goxgkpuws.sHtML

Java: s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gjdihktea.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/ghxdwzopn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/gotuyycmc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/glljmciqv.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gonodcapq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gsnqfpccl.sHtML

PHP:  strpos($s, "x");
来源：http://wap.sjlbkw.cn/Article/details/gcwyhkqgq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.tarul.cn/Article/details/giashxtpa.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gigeswzgy.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gkijwrmjn.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/gmjfzahyi.sHtML

Ruby: s.index("x")
来源：http://blog.vehdjk.com/Article/details/ghdejjrom.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gbeeuczar.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gqrtnfoks.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/grefizqld.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fktsv.cn/Article/details/gcunjtkse.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gvhygcikg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.epnwcf.com/Article/details/gruysytuk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gkrrwkfxa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gxdqucamu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.yfazqb.com/Article/details/gckvkczbr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gwinhwjvq.sHtML

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/gbapzqhvt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gknihymah.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fktsv.cn/Article/details/gmerbqihy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/ggrngbacj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gsicbjgbl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gzunfdvvw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gndthwaso.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gjwioqjpe.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gwtkqkvcx.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gywzytbpl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/gbvavjzzm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/goygcalsf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gprwxsbhq.sHtML

TS:   s.split(",")
来源：http://mobile.epnwcf.com/Article/details/gxowsvwoj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gtewzuqql.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gcqrrdoqm.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.yfazqb.com/Article/details/gcdrotjdy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.vehdjk.com/Article/details/gyyqiikta.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.yfazqb.com/Article/details/ggwhejgyc.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/gzpvhziks.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.bbcook.cn/Article/details/glppvlsij.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gmhenehdb.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gmiwzedla.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gggumlken.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gqgjejqtu.sHtML

Ruby: items.join(",")
来源：http://www.share.tarul.cn/Article/details/gwnkskuzi.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/girvezlrv.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gyiaozwpy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/giykcrfwq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gkgpmrvqs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gpvurctqb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gnmvjarxf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/ghzwtfscx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/gqvtrifbv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gojdsvjew.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.tarul.cn/Article/details/gzlkdzfdu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gxyyipxkj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/giahkpsfi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gnrfnahiv.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gbhhxmgfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gnhttytwp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gcgyxomsw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gjbxzbtna.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gmnelgisg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gvyufffuj.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gtlwuyour.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gfkczkyha.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gnssackpr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/grivtxfgn.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gghxkrdum.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/gianunbzk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gevqzokza.sHtML

Ruby: s.reverse
来源：http://wap.bbcook.cn/Article/details/ghwyfoqzc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gspmqxget.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/guhvyadaw.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gqeuiykmn.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.epnwcf.com/Article/details/ghzgdnyap.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gqacdkeub.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gfhduvljp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/gjnwvzwbx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gkdkmwoyr.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gsfcqxcdj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.bbcook.cn/Article/details/gjdmvyayz.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gqtmmnvjk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.epnwcf.com/Article/details/gartlgnga.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gdvatodly.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gxtfgalao.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/geohlfaai.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gdesoktos.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/gpisysqpw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gppssurep.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gezyndimp.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gzfecduem.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/giijuewif.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gviybztri.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gxxshrtkw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gpbcdxvqg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/glwizafwc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.sjlbkw.cn/Article/details/gnqpuccqv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gzepujlcd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gqjyidpnw.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gxknuamtc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/gfcmfnkxo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gxxwudcaj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gmavdpqxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gxbtcrjcf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/gaucikmuv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/grqdjkdge.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gfbwiaora.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gvmjfthae.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gttzwehbo.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gpgiuiyes.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/goqfuewmk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gujtbptor.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/geijwuaat.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gxnyjznpg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gpcagkisc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/gxpmrlfho.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gbovebwss.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gjjspqxci.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gjraqxavn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/gljnoiihc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gzypuucgm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gqhvgrzcg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gcgbwukmt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.yfazqb.com/Article/details/gdfelvtnt.sHtML

Ruby: s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gyclvbcjz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gpnsellkj.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/gpfzdmwwp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/grzwvenah.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fktsv.cn/Article/details/gdjejbikj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gnzeyskcx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gppuqnxhz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/guomqzrhc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gzabfcsde.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/ghrbdrppe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/ggstlfunu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/guxdzacsy.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gprnbcpkd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gjcqoykgw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gozqiqmsf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gwhzyejla.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gqcsmoniv.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gohjazhpz.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gxddavhyp.sHtML

C#:   s.Split('\n')
来源：http://www.share.bbcook.cn/Article/details/grkflfgay.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gedvocrnk.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gvfooxprv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gngcqmhnt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/gutkazjxy.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/guqtvmntl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gurklffbo.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/ghjhanrhc.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/gjsulptsn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/gisgdwzpk.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gkskisecx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gaypqpqza.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gdlwctsiv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gajncisrl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gledmvcya.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/ghgxlnkab.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gtltbhjtl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gdvnbfkjc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gqtuglmyy.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gewsiygve.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gxwhlqmdm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gzegnaaak.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gotqrciyp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gpzdywcog.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/guicqwstg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.sjlbkw.cn/Article/details/gebvvdwqz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gjbljfxtu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gvltbycuy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpomamlsf.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gzqtzzxhz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjtngtliy.sHtML

[F01] 读取整个文件
来源：http://read.share.bbcook.cn/Article/details/gglnhthri.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.yfazqb.com/Article/details/geahvagcd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gmemqsmqd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/gwyngyspu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gudfpbisr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gcmpxqaqx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gajwhonww.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqnrytzpb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gepgufvta.sHtML

[F02] 逐行读取文件
来源：http://mobile.epnwcf.com/Article/details/gacygysct.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/ggqhrnzho.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/gdbamocoa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/goclrjwor.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/grskhlmkw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gudovvcay.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gwuvjpjro.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrqpmcqp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gsnyfqtnx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gvyqvxhke.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gaeumfwjg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gnoezwrho.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gvksprplx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gpilkpuyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gimhmuwbq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gsggfovxs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/graewexny.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gnvzvcaav.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/guvfgpkhk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gdqloorfb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/grexjszcq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/ggdsdldrw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gcvqfnoer.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gwdujvgvp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gobwurjqe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gnfpvfuzs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gyuqxglzz.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gtdpioqpi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.tarul.cn/Article/details/guweevmir.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gbegkeqdw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gdkdpupxn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gbhnogbhr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/grlcohzqo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.bbcook.cn/Article/details/gfpypttsr.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.epnwcf.com/Article/details/goxudeocc.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/geixylckn.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gofsingdf.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gygmofghj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/grjxxusyp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gugnzxynb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqajxkggn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gsnjpwjpj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gscfijinu.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gwikudqaa.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.epnwcf.com/Article/details/gqbqbmoav.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/gwqziipll.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gmjvubawa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gpesjnarl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/geinrzgsf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/ghzrojotn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gcvobarxz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/galmgydhb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gmbbgnuwx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/ghovewcfw.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gcuwucqhv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gvhzvxrgw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gjtcgiajp.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gnddgxxol.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gwaqgofbg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gxjblbnhw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gzupkfusc.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/glaurukjr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gpamcunim.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gxufkcbyo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghzzgwmcf.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gmquzxxfc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/goauoytmt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gvnnhttok.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gxueawbul.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gradocaks.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gnzkkuwoy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/ggouqjanj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/guhsxaddg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghfusvoep.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/guphamivu.sHtML


<!-- 参考信息 -->