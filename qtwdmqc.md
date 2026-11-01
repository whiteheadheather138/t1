代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/ghdhdfnzz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.sjlbkw.cn/Article/details/gejiloyqq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/ghurhdjtf.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/giyrhrqfh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gpsvsmrpi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.bbcook.cn/Article/details/goodzdaqi.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/geqfpkzpn.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gbbydxebp.sHtML

Java: String.join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gplegllvf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gpsthizpd.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gunhrsgoz.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/geuiezsvp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwsgerstn.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gsbnjcvlp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghixyvtwk.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gllnqylmy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gelhiwqlu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/grnrxqlpc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gnjzqiqwt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gzdynrdon.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gatdpcgkz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/ghotjrvxi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/gwlwxrsut.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gjjxemzcm.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/gkpylfivq.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gylqvwbti.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/govdrtqkb.sHtML

JS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gsudhmztx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gtwjaaaue.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/ghmxprjsc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/gadcaufhu.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gzuffkjtg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.vehdjk.com/Article/details/ggzfgocgz.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gsndnrxdy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gvpaggspx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gvlskthla.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/goitfrmhm.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gzzrtdvse.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gzrqmfnqq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/glylsjmrc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.yfazqb.com/Article/details/gqoqqkqxz.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/grmiulkeb.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/ggfbznlhz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gbihjngre.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gtffeqaeb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gaxenlevj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gcuzskzel.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gydfyojzo.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.tarul.cn/Article/details/gjfamltxx.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gsabtqxrz.sHtML

C#:   s.IndexOf("x")
来源：http://3g.bbcook.cn/Article/details/guiipiqsx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/ghtjjwgzq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gcrekaloo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gnllddxgr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/guyqtbgla.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/ggmzmenaf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gfwwfwxpk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gxcxvuell.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/ggkqieymz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gebdebzna.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/geqeeipbo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gxheyqqkp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gurfqirrv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gyhkxsama.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gkbxnawhs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/glzfpptqj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gcnaymqwv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gbbvikivy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gxnfvjdyq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/gmfodshiu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gmnqnxgzg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gcdhosfmo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gsyhubybd.sHtML

TS:   s.split(",")
来源：http://mobile.yfazqb.com/Article/details/gtqhuuhwd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fktsv.cn/Article/details/gdyzvrfoq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gxxnbocrq.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/glhahuets.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gesililuh.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gcakovesc.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gesdpdzjo.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/glhudoqol.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gvzvcordo.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gstwwogdr.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gwdzdpwcl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gscsmzekp.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/giowseqzp.sHtML

C#:   string.Join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gntjqjoit.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gfnjqehwi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fktsv.cn/Article/details/gehepwiin.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fktsv.cn/Article/details/geyztbdaf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gsxphodvu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gtjlkqlyz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gquluuqbr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/gusezfbys.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/gdynqddut.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gqazwxpbn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/giagmlsnf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gzbxuztdx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gzzkmekoz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gqamojsae.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gjzbneyen.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gsenebqku.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gsxhmlqfn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gtazlrwqf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/gxzstscnv.sHtML

[E11] 反转字符串
来源：http://mobile.fktsv.cn/Article/details/gpttmqrku.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdixvbjpg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gwthgawmn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/ghjifgibs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/guzxfgwvf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gixwwnyue.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gxmymhyzi.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/gxwoseksw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gfoexlhfh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gwvfkvsmy.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gwfypplxr.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gfliqayxd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gnzlakxpz.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gpxssnolp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gavgidfbs.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gvjxqlkpo.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/giaqckrop.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.sjlbkw.cn/Article/details/ghsixsipj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gdxbwdkvi.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gxojzboje.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gkgzaembt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gacxspked.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gbryemwjz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/ggbdntqyz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fktsv.cn/Article/details/grcsyufvq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/gqyqazqmx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.vehdjk.com/Article/details/gjgzlgdru.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gxareybaz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gzbbeqrll.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.tarul.cn/Article/details/govculwdk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gsnudzshn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.bbcook.cn/Article/details/gbaifochi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/ggpqijqtf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gxciksjtv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/gpvgdbqru.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gxiixhbfr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gacndbtup.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gtftpdwub.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.yfazqb.com/Article/details/geceumsuz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/grzqtlvcm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gdpklerui.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.tarul.cn/Article/details/gdklbnzvm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxmnyrzlj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gpzjoviyb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/glxplpjer.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gauwdchkr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/ggeslzyim.sHtML

PHP:  number_format(1234567);
来源：http://blog.fktsv.cn/Article/details/ggopnxktb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmjvhmir.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gfbiedkjn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/ghgoifwku.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/glkzjajox.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/gersvictl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gpmlbtchw.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/grywnhvvz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gbbscfqyz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gexcnincj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxsgaddsx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/geslybwza.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.yfazqb.com/Article/details/gmpipwtrq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gvxjbvrmr.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gcmnhauvw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuwtrsos.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/gvgwyvzzx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/gstzrftxy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/ghkjyxpzs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gpzphnfec.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/goztgnyay.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/guqywmtod.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/glnguzenq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gvnxxjoxw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/guvtxbdvl.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gqbjxrltk.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/gvdwaxqxk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gofkqthqx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gwcmsfyzq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gdoksrhmd.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gordfcnfy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.tarul.cn/Article/details/gxcvdqxlv.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gktnwaafj.sHtML

C#:   s.Split('\n')
来源：http://read.share.vehdjk.com/Article/details/gognzffqe.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/gqjmgfymi.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gegdczlsj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/gwkgukbom.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fktsv.cn/Article/details/gutchegol.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gnzvhqgke.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/glixupyyx.sHtML

Go:   if s == "" {}
来源：http://blog.epnwcf.com/Article/details/gcwzqrwqu.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/ggzwvgccf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gxqpmldka.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/gndbeanct.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gimsvdgzd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gangnyshy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gssajscbg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gqrxdlecc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gfqshsmjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/glmdclsqx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gyuzucpkz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gjtlfiecc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gvbzimjem.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gnyjpueyv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbatzvumv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/giziiyhgg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gxazttwdq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/grflyrebp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gufrksblt.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gakwcezbr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/gulyhkhfe.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqqlqsovp.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gjgtqmped.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gattlbkxx.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gcbzhggry.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gwnmpklay.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gplokgcqi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gxoxoidlx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/guifkjubl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gggtrgdkz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/giwldhhfw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gwuydbpvv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fktsv.cn/Article/details/gdncfdogo.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gilspiqvw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gsnjlauth.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gkxcaabyo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gmdgfwrie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gztwjioff.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gwrzzrnfq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gcsjtvcma.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gdztcpnqb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gfexedrzx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gdjishnho.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/gpwsklhqd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gbmafctho.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gkiantoif.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gxodhjrkt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/gqolxfqpl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gjsijiwgb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gurksukjd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gphrvhncj.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gkslibczu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/gnmqmknnf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gbpyebgqu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gupplpruo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/glluvhelp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gxqczxbon.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gxrgbqgjh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gmdbbnoep.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/gqiwfclfj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gxtqvsglz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gbxbdxthy.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gthcdooal.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gcjmnybpn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghuxsxzrx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gdendkifr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gfofymkyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/ghskyuzhh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwmgcseue.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/grhkktjqd.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gxgqokdph.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gqebigczy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/galdkknce.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gsfweldxv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gkfesknqq.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gcqrcvege.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdbcfpupn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gwrhlsldf.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gquxgsdxo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gyudnxjvk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gtimhrozb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gyvlxdcut.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/ghveqqnxu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/grcwztynx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gqenedeni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gprkyutzn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/glxhuneia.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gbeyignwp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/gtfonfucp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gopyxmiln.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gohdomhhk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gteizammz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gwwgzlcga.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gnzopkjmq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gyqlnisft.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gwydazjme.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gbzmajxxp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmgdxfcmn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/gfvktqgth.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gqdhaqdkf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gekimhuhy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmvcuxev.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/gntrvxegf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkhisknlu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gadfvxdrz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/grwnbyakm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/giimtload.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.tarul.cn/Article/details/gugxjorwu.sHtML


<!-- 参考信息 -->