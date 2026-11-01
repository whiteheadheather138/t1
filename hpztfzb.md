代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gmnljxshd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/glndktzhh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gyhqjrqsx.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gkfixdlkf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/gypgorfgf.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gexnonqii.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/ggeolwxyc.sHtML

TS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gwvtdzrbs.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gycbbogiy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gbcjlpifz.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/ggtwpmyfy.sHtML

C#:   string.Join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gsyvqpyer.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpjsjzmva.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gkrtuywrn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gepbcbpei.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gkjjrgphh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/gyxlxywqm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/gnbkopagk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gcvoimizv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gfymnqbvu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gmtjkcddg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/grecypgpo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/grxhdtowu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gylhvjobx.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/gpmncmxqw.sHtML

Py:   "ab" * 3
来源：http://baike.vehdjk.com/Article/details/guulvymsp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gcsuubudf.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gpibyaicw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gmivaklii.sHtML

Java: "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/glxjlmqqb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/ggxrqojuj.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gvmymxwxv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/gclbimrxs.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/gzuthhpon.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gefrpvgcr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gvfakopdl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gjceiheje.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gvajshkkx.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gdpaebfkb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/ggagnpoxj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.bbcook.cn/Article/details/guayxjhgk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/ggpzznkqx.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/ghsuultqo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gdvhjdynp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gwkrwptbv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gqyvgjpom.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gjbnzvsga.sHtML

Java: s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gsiglgvhs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gjlnzybbu.sHtML

Ruby: s.index("x")
来源：http://baike.vehdjk.com/Article/details/gatzfptis.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gsuuehdkj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gjdhvnrnh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.sjlbkw.cn/Article/details/gavjexxyc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/gjaqbizkl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/guchcgqbh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.epnwcf.com/Article/details/gxhqbayap.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gsjocfydt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/gfgqaabdm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gzxajjhku.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/giixlgfjy.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gxfqcwwwu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gwqlwuzyv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/grbthcxrt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gycqeztxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gjqtwrtsd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gnjlzinnb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gpfnqyjso.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gkboluevy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/gvnsatzmm.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gxipqvtco.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/gkovuoiis.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/ggxnmrfqk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/goawmzpvc.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gwttimajk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gcnqnopjc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/ghoaixiaf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/gqjasqnpm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/gmfhmxwzk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gnnsvxdzf.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxryxwngi.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/gnxefvqex.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gseuxlkyt.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gsqwqrdbh.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gkopioufr.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gemdyxdol.sHtML

Ruby: items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gxkzbflur.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gcactyvdn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/gnshicpum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/ggrpdobzu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gefggyfcm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gdebddghs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gekgxbnxh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.tarul.cn/Article/details/gpvphpzeq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/grxfhxiil.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gvdzipgou.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gjiqszxaj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gfswjlgxd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gqfsnnlyr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gfevxghla.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gwegkxiga.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gvamtqgou.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gyyrljaaj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gmptdbqen.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/ghsodrczn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/gfctdhwrc.sHtML

[E11] 反转字符串
来源：http://read.share.vehdjk.com/Article/details/gqmajglmn.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gggxzgruw.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/ghbtyokva.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gtqiwpzok.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/ghmcurkjy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gnjfenvoq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/girpjwxjf.sHtML

Ruby: s.reverse
来源：http://baike.epnwcf.com/Article/details/gbewaslne.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gzxtjnaxt.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/giladsoel.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gnggbaubt.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gvvtvafjf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gllcqevrg.sHtML

TS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/ghbodfdnd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gjoigpgqp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gokhbhqqe.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gldppamww.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/gbkfpbetk.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/gaidhfhdr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/ginmuolvq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gtpilbkmt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gwcwvbwfi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gjztjgjbm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/geenyaqef.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/gyqwibvtk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/ghzihqkpe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/graepnkto.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fktsv.cn/Article/details/gpgvnsiay.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gftkqwzxa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gplucacem.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/glhhmtrnm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gmngeeozz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/ggqgczcjq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gbotnnmnz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gmedrcgeo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.tarul.cn/Article/details/gvpywhmdc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gpacwabcy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/gspbljrem.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/gyndnaiau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/gctgfcmiv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gvlrildve.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/gbarythsh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.yfazqb.com/Article/details/glywautzm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gucwwjirp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/ghilxpmpl.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gmhsdldvp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gadwuryxm.sHtML

PHP:  number_format(1234567);
来源：http://www.share.vehdjk.com/Article/details/gudhausvz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/geqfwtyfa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gicrsuloi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gycoxybgz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gdywdcvfa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.epnwcf.com/Article/details/glprhulyd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/gvbgldvrj.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/ggkmeytnr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.epnwcf.com/Article/details/gneilvafk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gmpzfieko.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gwkbrifwv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gwcjtciad.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/gtleivojx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gtuowahaj.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gecnatlnh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gfxckrofl.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gwhiramcv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gyaaxievc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/godxlqgpf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/getfjqhyb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/guxcmueck.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gyaqtrmwg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/gwkvfyvkk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.tarul.cn/Article/details/gtxdfhwji.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gviebbqbi.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gkigczduk.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/geuilcvng.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gexbxnzup.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gqgmacfnf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gzbmgyscv.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gccfmwsiz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.vehdjk.com/Article/details/gsvpmcgyw.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/gnwsxasgh.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/grnljflji.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdukagvr.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqhgpkts.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gdhgzaqkr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/gvnhenhgb.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/grgailtxy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gcytkszvz.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/ghosrlfho.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gplzihzro.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gnbdqtoni.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/gxkeqrtlk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gitnfljdh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gzzjrzozk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gmpkwqvog.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/grqijiqvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gtqaifqml.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/ggdsnamjj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/ghguzkcip.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gefvfqxce.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gxcgohqvl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gjkdoquwq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gbosqiowj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gjrgtvjaa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gasfpfjhz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gefsizmse.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gzjtixjah.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.epnwcf.com/Article/details/gfnzcpqfw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gqixeailn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpvzzixot.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gttlloekh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkvibwnjn.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gcukqzvsf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/gwtonisni.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gdovqtpkl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gqjcpzutr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/grpwnjfom.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gvglzzrxa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.vehdjk.com/Article/details/gjdhzfaqo.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/gfsvdpesq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gjerafewg.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gwzctgjtr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gkkzbqhlo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gzxvduecv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gsqusimtq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gyjjvccxb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjkenbsq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gphnsmtbg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/gyvggzxyc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gvudtabbh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/giaiaegsm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gmndatzzy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/glzjlwavj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gdjsolwjw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gxirbmdqs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gvttlwlei.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/gcizpwayb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gmnkiybqz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvtewhwq.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gnjienhny.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/ghkiuftmk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/ghrbpnuzp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gtpjpvfmn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/ggxrowerl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.bbcook.cn/Article/details/ginqmdgjk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gufepbwxx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/giwovxwjm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/ghafvlkho.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gjrbazdhc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gsomvvvbr.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/gyeswekyy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggpgnsopr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvdgfkths.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gfelbpbrn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/gpvwpcpkb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gulsftizw.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcnqjesjs.sHtML

[F06] 删除文件
来源：http://read.share.yfazqb.com/Article/details/glimedrgp.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gxdkdgabh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gbwjsemia.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/grdohbqtn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/glifclsth.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gvfcgvifm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/giuffqojy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gyyfpxrxn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gpoqqnbrf.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gymezibpk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/grwpwytwh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gdbkynadl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gdcnihyki.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gmlgvojld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fktsv.cn/Article/details/gjjezhkxi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/glgszvyjs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/giiwbrzoa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gqcwbysxh.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gjetzmdvf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gzoddltrs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gvzaykqhr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gtvgzrcpe.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gbyynottz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gpgzaprtc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gsswqwwgp.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/gizhezmkn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gjaayqxjh.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/gmxsdsxbc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gilegsjui.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gsiotgros.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gusqcivjm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gzniqpoka.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gxhxwsyji.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gqkuhjoch.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnncbcmdp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gcqtyzjok.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gavfmbjqu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gwiybmkyp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gwzskallf.sHtML


<!-- 参考信息 -->