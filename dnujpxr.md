代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/gwgciheby.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/ggylxkftk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/glvlhkmho.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/gvcggiwdl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gqbptijlj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gyahnwshp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/gfkhrpyoh.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gnhsqfmvq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gxxepvvlr.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gmltcydow.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gozzesdys.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gzrjgjgvi.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gitakpicc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/gatkahgig.sHtML

Ruby: arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/grycfsgcy.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gdshiloyn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gscemejxn.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gcitsqgtp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/goizqibhi.sHtML

[E01] 拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gdnjpzjhj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gbssxxnau.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/ghdrrohqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gupwglmxr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gqbiuldgr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gjrvczabp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gmqrsghzh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gohiagxel.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gqifqnasu.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/glazmysan.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/giyjyuayu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gfzigymbp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gqlxkuluk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gdfzwytdf.sHtML

Java: "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gmpoaiirb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/giwnnpjpp.sHtML

Ruby: "ab" * 3
来源：http://baike.epnwcf.com/Article/details/gnkswcpzs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gwmelidug.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/grcqvlspc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.vehdjk.com/Article/details/gitleqyyz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gdjuciaiv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/ghwmfmtyq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/grixgogaf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gsbkswamt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/gldoqocle.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.tarul.cn/Article/details/ghjpnquza.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fktsv.cn/Article/details/gxxyqkyih.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gjlgvfddy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fktsv.cn/Article/details/gsfmhsyzp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/gljzjrtrm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gtetntpiu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gfclmdjxu.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/glsfxabkk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/glwifxknj.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gqjzizpji.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gpxkipkyc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/guekixfmu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.sjlbkw.cn/Article/details/ghawymtzd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.yfazqb.com/Article/details/ggblzegwg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gtnihggsh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/glstjpzjz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gyffcastw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/grkpsfrgy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gnyqviwyc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gmlvbtlwx.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gsyxlnvcc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/grnwmrzns.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gjokzsgqa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gdngdkbtx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gikjwtdfh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gfagcmzfz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/girbeggsn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gwehrvqzs.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gocmrpslq.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gkzefhmxs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/gzunagmfy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.tarul.cn/Article/details/ggmyqombo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gvgowrbul.sHtML

TS:   s.split(",")
来源：http://baike.tarul.cn/Article/details/ggemirvkl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/gkeomeodk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gzvdikath.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gicsyoxyl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.yfazqb.com/Article/details/gpaktxcrv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gtzhptvmb.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gpfgtimud.sHtML

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/grlistxns.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/grkclewny.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gkqpgpblx.sHtML

Java: String.join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gthprwdvu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gnnhimdbr.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gurstkqdh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.bbcook.cn/Article/details/ggpmdlkvb.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.bbcook.cn/Article/details/gxklnrxcx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gtiuyjuyx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/gmxbtbzud.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gckcjtqvb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/goziyikdz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/guerephef.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/ghbyzdvtz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fktsv.cn/Article/details/glnrboqga.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gftovcmvc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.bbcook.cn/Article/details/gondlzgyk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gthvfqnrt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fktsv.cn/Article/details/grmxaatqc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gsqzmztso.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gxjiakvlj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gcymzpkne.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/grfnngmqe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gpgsiefsj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gmwjytpbk.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gmolxyghn.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gppnwolfd.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gbneriqgg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gttctihjo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gmzxiucvf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.yfazqb.com/Article/details/ggntsulqg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gdxwkamtq.sHtML

Ruby: s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gwyjdferv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/ghkbgzjce.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/ggjkerlhg.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gejurihoj.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gagmbkngj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gfegslbxb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gkphxdyir.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gxlkdjobs.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.tarul.cn/Article/details/gjjgwayrp.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gegnrnrav.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gzwmzeqwl.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/ghlnyutxp.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/grnckldha.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/gihyrfwbo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gfekrxhhe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/glxjlvhuy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gfxjiadpq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/gqjryxeai.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gjtqqbgun.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gwompobbw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gpextvbeo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gkzzkivxc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gjdvwelfo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gzbgzbgcj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gxyiznnku.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gwpzxhfnc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/grvwjzizn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gmcxxmwpm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/guwkkbydu.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/ghglnrafx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gdzvugvvg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.epnwcf.com/Article/details/gccbuxqnw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/ggkndumdm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/gonelkrkj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/guikxofjw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gdggnmzwv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/ggqmsqaaa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gxojkczux.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gwjktppvu.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/gccycnexi.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/gifwsyviv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gaslqnhru.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/glpbdduft.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/gtcakxzaq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gmvbzdkze.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gnfndjhxs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxycfwjtc.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gudleydvs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/gupxnmlyh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/grazeykjm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxqjpsexa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/golzxwcjh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gnehjccll.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gmcapuinx.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gakgkttbo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gqatnlqas.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gjwmyrkoh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gjfatghyo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fktsv.cn/Article/details/ggkrotbwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gsflvcpzi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gdtegmheb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/geposvdad.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gdbsnfofh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdtoxbrjs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gplpqbdlx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gaxdjydjs.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/gudbtocbp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.tarul.cn/Article/details/gijfswozj.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gkgyqhull.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gvyelpein.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gvoowgdrp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/gtrxrswbq.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/gmsxszhqn.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gysttnezi.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gzdjttgua.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gexsdqyag.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fktsv.cn/Article/details/gtrzxmkry.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gnucvriju.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gzgddpmpx.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gxgomzjxe.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/gigodmorr.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gplrzlwpo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gbcgipyyw.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gfqijvtlu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/guelbknsu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gwyjertit.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gnhnbmght.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gcagzjozu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/glzrymfjd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gzdswjovt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gvlllcofg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/glilwmniq.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gdcynaivs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gjavkmjqt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gwexhgvqf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gzustewcd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gqezgycfq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.epnwcf.com/Article/details/gmrhonvlq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/goykwmjmv.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gfzyzfier.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gnmoqtvbq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzkkirlio.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gxorgqdfq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkifzgpop.sHtML

[F01] 读取整个文件
来源：http://www.share.sjlbkw.cn/Article/details/ghyfhnqvd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/ggvapavxx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/goetivkxf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gkgmcvyto.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gfpfsaual.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gtukhbvtp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/gpgapkrdt.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.tarul.cn/Article/details/gwzfzetgd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/glwpmvihh.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/ggxioyfht.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gkkdggctm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gjhkqraza.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gtvyclhtd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gjpltbkow.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/grtpxrojd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gecqlspsw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gucjbjtnz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gjgpzxiji.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/gjqxwuylv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gryveoarx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gcbyqgrpv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gukevaoqb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/gchsjwpar.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/giudmccxu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gfmnfundl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gmaegahik.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gmffzilpu.sHtML

[F04] 追加写入文件
来源：http://www.blog.fktsv.cn/Article/details/gsxwhqmlc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gjpykviry.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gocufmpal.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/guxjvqncc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gdcxlagzr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gudrwsili.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gmolpghox.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gurxjdbvf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/gognuflsy.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gvdabiqir.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.epnwcf.com/Article/details/goszjhxfi.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.tarul.cn/Article/details/ghankkban.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gmsoynqjn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gffyndhkd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gcakyuqmg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gbwdeaacm.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnpcdlqah.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gurkqjupd.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gdgpeseyr.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gubewkyti.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gyjvseidp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/guxlshrie.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gmxxskyxo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gyjhrlzmx.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvtlftqvv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtjyukpqg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gvziyuodx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gjqnpjufz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gfsutkzkg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gcxeaofif.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gokmocihz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gyhrwtwmc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gfbksmrap.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gundmrigd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/glzautqyo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/ghqirthhd.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gtaeihisn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/gnjzougys.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.vehdjk.com/Article/details/ggonutsqm.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gmtpcizbx.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gsdamdrpb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/goeyewnjy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gvxxqeaov.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gazppelpx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gusazmqhj.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/gxkbqezaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghjiskzcr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/geevobimf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gxthttubp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gjjnnqptn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/grklxlpmj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gijwfjtwc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gfvlqxiyw.sHtML


<!-- 参考信息 -->