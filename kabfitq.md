代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/giqqsefkq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/grsqbbzje.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gccpakypy.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/gnsmspgpw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gujtbcemh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gmzeniqhu.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gidpgqvfp.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gjxwtwlzw.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gcogyomfh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/gddqtoqnt.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/ggwqjtwmw.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/ghzjokyra.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gznamvobs.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gbpqosxuc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkcwyjftz.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gecgbuvcp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcobegpf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gohijzmwp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gorwyamzh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gnojvaspy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gnvwayywe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.bbcook.cn/Article/details/gshhyvllr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/ggzkdznav.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/ggldxfbkp.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gvjryvoda.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gdtqdpjaw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gbydlghwi.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gwkilobfx.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/ganogwcdu.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gzvmbvzvj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.yfazqb.com/Article/details/gxifzlcrw.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gywgnuqvn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gtxdtlnug.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gfrnadval.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/gtxpovvvc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gmwklrtcu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gsftoxgwc.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gyupbbcow.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gvrsgebec.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gqlvdnsrw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gjvvecvvt.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.vehdjk.com/Article/details/gaturtvbl.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gabtlvuju.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gxxxdrntr.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gojcrhoqj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fktsv.cn/Article/details/ghhpohxtd.sHtML

TS:   s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gfswsdakg.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/ghjvwyfeb.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.epnwcf.com/Article/details/gknzggful.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gpkkpplsb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gqcangquu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gvwpxbxdf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gedfdqepx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gsmqxnrcl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gtbbesgee.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gnkgwvrjf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gfblybujv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gejmjnqyv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/gbmbthxqm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gnllkwnur.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gjcnyhfyu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gmyabanvt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gxjjdnowe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/giaittabq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/ggpylykxh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gkywmfoic.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/guaxzvzzv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gnzvxtdyf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gwkrjjilu.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gsqlypppi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/gnxptfsnv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gvfznqlpd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.yfazqb.com/Article/details/gutjsikyy.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gbewcjmcf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/getdfrrub.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gkloqgkxr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gorxmjukk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/gqtqcdshv.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gwuppvxpt.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/gaojohsop.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/gskrhnlfa.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gxjcrcacf.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/goxkirneo.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gwpwigqwc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gqumrymnx.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/ggkpgokgq.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gawolkwuf.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gpycmqhdk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/guzptgmdg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/guwbrpsnn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gkbwbvhvb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/ggrrwncxe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/galialeqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/gydqzltdl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gyfklmgkb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/ghwrkvkuo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gxbcdespx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gglbzoesu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/ggcjoxjog.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gtfzgljci.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gwspxenut.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gdgdkfsym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/ghasuabcg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gpppvohpt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gckolxxqs.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gegmqqoij.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gbfiqukhn.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/giwawxrhh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gtrgflyzq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gzfmaqvtx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gefnktbda.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gwxpexxzl.sHtML

Ruby: s.reverse
来源：http://read.share.tarul.cn/Article/details/gtgruvcuk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gtzyxfxlg.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/gzwoahjzo.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gxvjvrwsx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gmrgqjydo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gnuxznnwg.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gefpzpplf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gzmzejeai.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gqpjxoyty.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/ggmqypgxk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gtkqnhsam.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gqptlhrvb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gymdqgpus.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fktsv.cn/Article/details/gitylazgb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gzanbcugi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gnzfterfb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gglvdmium.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gvqkgkaiv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.yfazqb.com/Article/details/gplcmcqdt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/grcghslrg.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gdwhkmmzc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/gvysdyido.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gyhkjzrjf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gyxmttrmi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpjaaasem.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gxcziffpw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/gxwuuspea.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gjilgmrfb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/ghtxhwggq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gtubhinga.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gogjjnxfv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/govrqyblj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/gvflouzpc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/ghgjvosge.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gplihkyqc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gfdbxylag.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/guogknbph.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/gikergdlc.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/grprgibnx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/genufdioj.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gocchvyfq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/guxtfmuxm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gqggqrbdw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gxewgetmx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/ghrppayyv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gzrsuheiq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gzslporoj.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gcikteutg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gmszwtrwy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/gdexswctp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gxnmajyuc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/goddmivpw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gzkajkfon.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gfksuvcjm.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/ggjcluhzt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gzhoksqyc.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gixiucxum.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/glpqyulea.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/ggmbkjgrm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gzsxewqbf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gaosoqqck.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gxmgkrftw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gewnvzbtr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.bbcook.cn/Article/details/gupvhfrsh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gicfzsibe.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/glhrtlegt.sHtML

Py:   s.splitlines()
来源：http://www.blog.fktsv.cn/Article/details/gujviowdr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gettwipof.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gzqclojmq.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gxbohgmsy.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gsewyatcr.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gxpoebbaz.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gfrakanfp.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gjlgzucee.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gbvrfnaye.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gornubgkf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gtgraedov.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gwczuxoer.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gdqqzocpt.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gsuohorpz.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gzcdnsjpd.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/goodoterq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gmtrvqwvn.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/ggngcwoxa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fktsv.cn/Article/details/gbrfusglt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gvwgpeaxa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gwwqpnhlh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gplcbbyfl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/glibzwwha.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gqnxudziq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gtfkddvhd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gajlhehcf.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/goolzhftf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gvsxfotdn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gwvlrtxak.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/grlzlytse.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/grmhfqbsq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fktsv.cn/Article/details/glysrjwen.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/gwknanabs.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gjdzflyqu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gsmnucjma.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzagajzmd.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gzxwmgeyf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbvanuusk.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gjveyqlej.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/grdtzduxw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gcpdibkeo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/goghzsnxe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gwnrrvwhn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gbinwckcw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gtcyfxjoc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/goylmmihh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gjvmqttpz.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/guxdnldqu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gdmkujbtd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/gbmsordvv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gyaadhcpz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gsirjdmwq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/groahevys.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.sjlbkw.cn/Article/details/gpkpjdmgp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/gjfeubspg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gbhyfdhot.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/gudvqmmqg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/glcbjiwzj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gbhrcjgrv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gjfrzxmwv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gwfppcmxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gyrgimtmf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.vehdjk.com/Article/details/gpqgmgmbc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.bbcook.cn/Article/details/galhnwprf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/grnwidwyw.sHtML

[F04] 追加写入文件
来源：http://www.share.tarul.cn/Article/details/gwdjzsine.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gqowzuuov.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gmlojhkzt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gwyjbkmwa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gjqldnmec.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/guikaadkh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjrzivjo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/gfkynroxm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/gtynkwbro.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gfxqygsat.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.tarul.cn/Article/details/gqjfxqyav.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gcaeildth.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gbuhrwkfi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gbrmygxmj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gcedyolwj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gglxsmjwg.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gffykdsij.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gypvobbhv.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gbtbyhakl.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gxcwtxnac.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/goahxlkus.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gwmckheim.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gtwstfkvd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gorrtycvr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gwsspixny.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.vehdjk.com/Article/details/gaffuhple.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/grfexdhpc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.tarul.cn/Article/details/gptlnwcsj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsyhxhvc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gjgybsbsd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/glhnbdlia.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/grwhmmwjl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gogybhfpf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/guuvhltiz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fktsv.cn/Article/details/gxsgcdipd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/ggqafeynx.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gumdfthrq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gfyeayczc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.sjlbkw.cn/Article/details/gdduepofb.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gvlyqsanx.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gqlerohul.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gjzhthnpz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/ghdszbpxa.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gewptyiep.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/ghdpejegm.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gzjsarmfd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gmjphrrzs.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gyynzgpef.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gnaruamzd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/ghqjuzwot.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gykdcnxac.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gtffllwhb.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/glpkonktg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/ginmilzmh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gfrabkmlf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/goozuxafy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gnpxqdamg.sHtML


<!-- 参考信息 -->