代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/gvmsrtpzk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fktsv.cn/Article/details/gygjgeanv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/glytpiacu.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gnjxckalh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/ghncnalbn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.tarul.cn/Article/details/gudyqrwpp.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gmtniqfhe.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gfbwbrhdu.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/glrvhwbdd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gdleihvqn.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gazcplkfx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/geovclaww.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfjdfyfuf.sHtML

E. 字符串处理
来源：http://blog.sjlbkw.cn/Article/details/gkjtbindc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grghxnvkt.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gvtbdthpe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.vehdjk.com/Article/details/gnsgqvvpt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gpmunbuho.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grmprygzo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gtzcwtxld.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/ghszjokrl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gonnhadqx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gwpuutbnu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gccmpfukb.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gqtokqxhf.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/geqqwqwav.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.sjlbkw.cn/Article/details/gtaaumton.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gyszcuzrn.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gipniprus.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gwjeaaxtn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/gxclkpkvv.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/gvmppbdvb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/giefbjdzv.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/grrhspunu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/genkeltyi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gvohdwbwx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gfiupdroe.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gitgdvhbl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gsfyamlld.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdmxdtyh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/ghscmyngk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gzjjsjlnz.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gqwtvujsy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.epnwcf.com/Article/details/gkzqfhabk.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.sjlbkw.cn/Article/details/grmajscae.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.tarul.cn/Article/details/gafysvbho.sHtML

TS:   s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gmhdbiiwk.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gbardmgpt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/gmsdwixyv.sHtML

Ruby: s.index("x")
来源：http://blog.vehdjk.com/Article/details/gubsbaahi.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gxguvlmfu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gstbjksyt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gguddrmvy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gsronelkj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gstcyiagq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gcaqjlqjo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gobqytovr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gxklzlgsr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.vehdjk.com/Article/details/grjichxrd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/grfytrytr.sHtML

[E06] 替换子串
来源：http://www.blog.epnwcf.com/Article/details/gazbfjvgv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gaqvyrvbv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gjlmqejzw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gukmvcwey.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gzlyvmkfj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gvpfzccjz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gnsekspha.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghufdzfwy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gikhaxuld.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/gknghzgqe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/gavnhmbrb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gcbwgyysj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.yfazqb.com/Article/details/gropvfurz.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/ghnjorlvd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/gvbxaocdy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gzdgwjrep.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gtvqspjny.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gnnbdhljd.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gorzjyrgr.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gcmpuzxfc.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/gekdmvczj.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/grlwohyml.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/glroealol.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gapusrzzo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gjdjnqdjk.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gzszzgufc.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gnqtamnwv.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gyacxagxl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/gtjrgvvcu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gioyhjscu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gaxlbfrcz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/glkcdjscf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/gjzmggwum.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.sjlbkw.cn/Article/details/gpaggojjr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gueefxijm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gbxtiupar.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gmqmlvkhl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gfaewrosx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/guzrnswyi.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/ghadpjdle.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/glcsjqijp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gansdtuqp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gixoxxivk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/goknacddq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/grflyzyjc.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gljexttjn.sHtML

Py:   s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gwdtgygdr.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gxjrldfnl.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gtpgxkahj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnohqpmf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gciwxslzx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gzbklchvs.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gylufjkab.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gqyyravzj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/girdlnnot.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/ggmrebbtp.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.tarul.cn/Article/details/gkwdiywfg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gnlxtxuxx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/goaexqaph.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gvmzthqhr.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gdfrtiumt.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/guzvsahpk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/grnweqcjy.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gbwgzlojq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gruwwtocp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gexuzemvu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gpzddmyra.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gqrjmrboc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gwtelpfoi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/glejdlgwj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/gvcurrkda.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gtsinbkjq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gyoqqlaje.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/gqysqbquq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/ggpvcblny.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.tarul.cn/Article/details/gccergqgz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/gzqyntwgk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gnlinqffx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gcgarjrsl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/ggmcujjdn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/ggqmxccjo.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/gepzixwox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzslxzvqu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.yfazqb.com/Article/details/gibeucpxd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gmyqmpwga.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/glfotzbwl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gldoevhfs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/grjdlyfqp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gkuknwtuw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gvpsqrxiz.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/gbmxmpbqy.sHtML

Py:   f"{1234567:,}"
来源：http://baike.vehdjk.com/Article/details/gwktlwxnh.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/gavvksnzy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gjwwevcal.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gqdykfkcr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gdsbfkefr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gcwyuleon.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gqomzuyte.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/gzmjasdbm.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gkmxuctaj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gkvcmgcin.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/giudmemgh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gdqfxkfam.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/glhmnpxen.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gqqabribg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gpaercuzl.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gldyzhldk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gjrvxtfgq.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/ghibvprdm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/gexnhivxd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fktsv.cn/Article/details/gcreqyaoj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gfsgsenta.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gcnzmxvke.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/goithnlbx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/glhglyrsc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gcsxwotpk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/ghxdmhzpl.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/gstdflleh.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/gtuzwhthe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gzacadgdj.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gztekbszu.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gqmgdnrho.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gjvzwcilq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/gyhoedfhk.sHtML

Ruby: s.lines
来源：http://wap.tarul.cn/Article/details/gdwhabild.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/gqxjqomvp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gpphmliqu.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/ggicctvkf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gjgjxdwbd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/gszqplfug.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/gmnydbkxm.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gfdcsfnea.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gkjfarhqu.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gvphftsfg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gypiyoyjt.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gylmepiqu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gitmhvgem.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gbpqttsqw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gnrfghmqr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gqlljmmdg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gzrnbjqwh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gkldlyzrx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gnqlzadig.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gwkcmbdzp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/glbmarrqy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gpfqaeioq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gammifzri.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gbapseukg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gimyprlqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.tarul.cn/Article/details/gsjdkdbzq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gwvvlnmbj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gozvxsbbq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/gmclqoxvj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gamqpzaas.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gcxcllhpr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtrlisewj.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gtaifffyi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gukwlqvau.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gqwdrvwhk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fktsv.cn/Article/details/gafgjtnmm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/geesdvdrt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gbszipudh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gdbrdpwoc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gvfsxwbwx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gjgxjrcoe.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gqzsvkfyk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gsipqlxvs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gskywjlbd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gvzhzgewf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gcyeusswx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gnzpxgmwm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/gwtklbknc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gezrusqnn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/gmnbtgfqh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gmtqgktqh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gviukxsdm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gljjlpatv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/giigctaxa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gqdvqdanl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gzynzgzzx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gwvpgjrie.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/gzvapsrdk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gvasrqupy.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gijwmbyph.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gopxzoanr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/gdzaxcilh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gfurislrl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/grhbthsak.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/goocjcttd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gkekmgwiq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gohwpltoj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/glmsyaviw.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gmyzmddxs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/ghgjhechl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gvwcgusbl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkyyiwzzy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gjqhsaqlt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gzqkowcdk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gvynbwopf.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjsnbdptv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gsvekqepr.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gmlckvait.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gwgoylueu.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gagiqbuds.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/grzmiyaiv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjkaxjpmw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gzcvayojj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdfqbzdnp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gurjbpajd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gyvcjoewb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/glbccxcql.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gocrysibl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gixkvivci.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gvtmzkhjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gpaenuptu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gnbbccjqj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gjadbjsom.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/gjyfatted.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxizxdpq.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/gzgjiaobe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/gxivaujgr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gitjnroda.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/grrbyxkqd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gnddmcdzj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/giqdmxexa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gsiuiquve.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/gimltgrns.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.yfazqb.com/Article/details/gptlkhuff.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gupflhkzn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/glxffjghy.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/giptngxfh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gurctwfuc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gbypbikyb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gvzjvkdxg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/ggfcbanry.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/gppatfykh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/ghjagltug.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gwvewuonp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gcxscuznk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gfgsuvibe.sHtML


<!-- 参考信息 -->