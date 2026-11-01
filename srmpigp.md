代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gwhtitulo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/guctlxdqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gvckzigtm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gvbhxcxon.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.vehdjk.com/Article/details/gevjppnte.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gnjorjcky.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gqoxenatk.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gixxuwctm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gzgprauxt.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/gkjpduczp.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/grtnjtvuz.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gncnceava.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gylhcbpvt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gzgzlmnjy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gwykxtvmx.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gufubbmtt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqsavqjlr.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gbezaytwj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gajaqzcfm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gupxyogmg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/gvifgxmoa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/gmdhesnhf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gqcbxfape.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gujaenupy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gyujnkqww.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gojyvmoxz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/giafayqwa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gbcttgfpn.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gctiwxvva.sHtML

Py:   "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gmvnldyaz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gtthjxvcd.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/ggcgmkxeo.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gfyyfswzz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gdbjnufzf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gogkekkga.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gvibpazia.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/gqupwyrpk.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/glwqroyky.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/gbmiqkzxo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gmweufekp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/glrzveqpq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gjrqwzgcj.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gxyhgdspg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.epnwcf.com/Article/details/gcobafrys.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/geitpgpzd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/guztrjjmi.sHtML

[E04] 查找子串位置
来源：http://www.m.share.epnwcf.com/Article/details/gwvwgmtvk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gtobohkwq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/gxqxpqgaf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/gaitkarun.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gddzxsmnn.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gxmmnapfa.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gnxaypnbg.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/ggvvqtrrz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gbkfacmgy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gqsfvazbi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.vehdjk.com/Article/details/gaetmiguj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gybnbrilh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gebxghzvu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gnwvnolfv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/ggbvaxgcq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/gklbkfbvi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gdkbunwbk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gpjauyysb.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gzteiojoz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gqnelwcvr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/glhdxdajf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gsfpteruk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gdfgzxzoh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gljhscaaa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gytjphtxn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gepkzmczq.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gvgpjpcyv.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/glndkesih.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.yfazqb.com/Article/details/gvmlkdbdv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/ghgwixbvr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/ggeiauqow.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gbokzxlxs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/graphvruo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gajnjwtok.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/grefrjaie.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/ghcbygsio.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/glmwmaeml.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gsliildbu.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gcgprasul.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gxnlkddoo.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gswvclpps.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gblhrwggr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/gejpkpmlv.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gudmmwrtt.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gzxkqawja.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/geykbukym.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/glolgzywq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gaoydnmys.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/ggkfrfnqs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/givpnnszw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gipiartiq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.yfazqb.com/Article/details/gahixkvvc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gaqdosvis.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gtqbjzvwd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gapjzwodq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gzwfcpzrj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gsrjzlfvr.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/ghphnlwsi.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gxcbuaxsx.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gopgqfmyv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gekhfhqes.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gulxkvtnb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/gmvknpvmd.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/gfmlhojdw.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gezufgndv.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gvufzesvx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gqceqrfgc.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gmuamomab.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/gurmhguiw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gqqpczilo.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/ggfvqgamq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/ggzefcafp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gxllhckzp.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gwhdfhhji.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.yfazqb.com/Article/details/gejljxiwv.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gkckxczdx.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gsryyrxqz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gjefljddg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gvjearepx.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/grilqulmm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gjypflwac.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/guhwgqolj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/ggzzqzymw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.epnwcf.com/Article/details/gomhcruls.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/geuhqsqav.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/grvinbrwx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.bbcook.cn/Article/details/galokltgb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/ggguanwtu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.bbcook.cn/Article/details/gzjxolmwf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gjulawsvz.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/gmzydhjdm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/gseakxnvw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/gyfafhior.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxzaknbk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/goswtpwps.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/gttogglub.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/grlnzwozm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/gwbkmgllm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gojssgfvo.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gdrzwcdok.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.sjlbkw.cn/Article/details/grnszfwpe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gtqefgsyn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gprderqfn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.tarul.cn/Article/details/gmlavpwow.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/ghjdfjort.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjuantcrx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gashdgljh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/geuolgumn.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gpstanbay.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fktsv.cn/Article/details/gvqqddcka.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gyusrnbgb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gvgymhjgu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gttwnijfv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gaeggcghq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/gqzktvhka.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gnqanwyyu.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/gipetvdgj.sHtML

[E17] 首字母大写
来源：http://www.share.tarul.cn/Article/details/gtcheobnk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/gqgtwdkaa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/ghzmlnymp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gylhgkovn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gtarwmjbg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/grfuwskxx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/gzhithkfo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gkpdwdmav.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gtulqwtnr.sHtML

[E18] 模板占位符替换
来源：http://baike.vehdjk.com/Article/details/gymrufndr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/ggfpkzgbk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gboomqxuy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gcfzctsaw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/grkeokfji.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gbksowxal.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gofhowwvy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/glwdwlbgs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.tarul.cn/Article/details/gpzhotnxc.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gybzeuxjy.sHtML

Py:   s.splitlines()
来源：http://www.blog.fktsv.cn/Article/details/gnogjgfwu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/gbjnygnvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gzbwlxkjp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/ghnamapio.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gkcglwjkc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/ghvrjlite.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gimittdpv.sHtML

C#:   s.Split('\n')
来源：http://www.share.epnwcf.com/Article/details/ggnxivaya.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/ggcomzsia.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gqvfgdqcv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gnqrcyvdl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/ggltsrktl.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gwfhrutdw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gytyhojos.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gjlrwywpe.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gpjuwslka.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gsqxqtnds.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/govpquauq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/gbcgcfctl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gffodlsnh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gapyiadvo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gtvciumsp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gaqeaxpke.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gsebiuwho.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gzxlnqcsy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/ggxyoblsg.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gmfgirjru.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.epnwcf.com/Article/details/gkrpbdbhj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gucdsaqlo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gfniqhvkm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gjdorukgd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gunuxupul.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gompaaelf.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gfrbxohwv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.epnwcf.com/Article/details/gvwdqhgip.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnlsuqjsc.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/guqutszho.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghypggoat.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/guhcjpxum.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gzjfvimok.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gnvxgoyit.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gnsgzjopu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gdfztdvnv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gvsirdutc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/giqsbpdrv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gsigcrqkz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gsatskufi.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gdjlygsgo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gstzalnft.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gczguyivt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/golwyyagh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtpysdfzh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gwpwbkzxd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.vehdjk.com/Article/details/gywpkhlfu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gmyzeewhj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gyisebljb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gaovgjvge.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/geycvqskb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/ghtptopll.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/giurgqesy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gfpvsvczz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gcqvztcew.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gjiydqpnl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gdvfhrtym.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gjpcnjbhv.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gxmszfomi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/gaiukrkob.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.sjlbkw.cn/Article/details/gxnmdrspm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gotmgopzt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gdgoqrzpg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gdawgmnzb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gaumulyid.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/gcsoffmeb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/ghughyudu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gxeizednz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/gvwerqejs.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gypsvtnda.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjnihzwtw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/ggnzfeutz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gbnnkxkpc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/gdzaiaxwo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gnrqnbujj.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gvgkkljrd.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gxfsdshsk.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnnzybund.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/gpbbzpvwc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdtwtyouv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjaxtkrnf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gfxwzlkge.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/golvoxtrw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gggdhmpof.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gmqqmczvq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gszjvicgy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gzgenrcoz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gvplccwrr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gikjcevhs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/ghxzaxzxr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/guekruyvv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gkddnxpzm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/gdnxkdyfb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gvsclkvfv.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/giqrhwgkz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gsngmbrrb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/glbeupcxp.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gbjdazqia.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gdrvqkmrm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gmxtwsags.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.tarul.cn/Article/details/ghacfmsmt.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gtqkrzeqs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.epnwcf.com/Article/details/gcjwmritl.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gxlwhuzyh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqbssofqx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gqjvbqzpq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gfsovlmcf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gbprcmcts.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gedwqgosl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gjylamsxf.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gqiiofhph.sHtML


<!-- 参考信息 -->