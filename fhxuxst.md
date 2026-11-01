代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://baike.fktsv.cn/Article/details/glxsgugvn.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gnkwjotll.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gtowfnisf.sHtML

TS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gabwtdlrw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gbnivoedi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/glmmcobdu.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gkgbtyjdu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gggrimebp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gyvpcysly.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gkrknaqgj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcfpatzof.sHtML

[E01] 拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gdimvjwrq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gdpssstls.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gfznpghwf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gfqrmmrod.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gfmxhznvb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/guixncwim.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.bbcook.cn/Article/details/gmyhupbkr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gcxlvikjx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gsifzlchq.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gpaxadihe.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gxhkvxalu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gwpqchpal.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gcmlitmnn.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/ghashrdgo.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gpmteoycp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gdimmljha.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gviokdcti.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/grxncruvu.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/groysxwpw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fktsv.cn/Article/details/gidxogqrv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gfduoihhv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/ggvwmbuch.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/giaienlcc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gbcjdglla.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gjvawamod.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/gcvarzkul.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gcdezxkcc.sHtML

[E04] 查找子串位置
来源：http://3g.sjlbkw.cn/Article/details/gkknuakmv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gmnvmztln.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/gxoeahnec.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gmclpedsw.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/grjvkrpfu.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gfgldfvpa.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gnhxdzlje.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gczrvxiky.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gnvbmmjhx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/glnhfaecv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gastcetid.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gtadhqvdm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gsdsgtwqc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fktsv.cn/Article/details/gmeafuhha.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/ggwtrolmj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/glwulkyhx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/geiiedecy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gvjjnaqwy.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/gzvxpxygn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gmuvvgvpx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fktsv.cn/Article/details/gwugiwzhg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gdwlginym.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/glbjrppuc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gxjxzpdwl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gauiycnvp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gnwtdeoah.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gdujslldf.sHtML

[E07] 按分隔符拆分
来源：http://baike.bbcook.cn/Article/details/gonwvoilp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gvzdlnbfu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gvqdhpngu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.tarul.cn/Article/details/gjxrgepjv.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/gfhuwvnww.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/gspfdcktg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gyotujznc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/glinlvxsr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/gjfzniqlm.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gzioczvhp.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gjifjjsbj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gckxbdvhw.sHtML

JS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gkolhvgdh.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gnfryivnv.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/giuldcsmw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.bbcook.cn/Article/details/gdikgxzhm.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gekvznvxs.sHtML

C#:   string.Join(",", items)
来源：http://blog.tarul.cn/Article/details/gejhdcsnf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/guiarxvel.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxltifxra.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.vehdjk.com/Article/details/gkafdrojd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gufyealmn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gsyrfaqyj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gjotiwhxr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/gqrphtaow.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gaerdmszy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/gewnpbzez.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gpiizqxyg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gcbolyokm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/gkgqqswef.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gbmlbrldg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gzrqjowzo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/ghvgvlcwt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gegmreoou.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/ghclbamud.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gaupdwvhc.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gnwiabztx.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gkdcjstko.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/galeoyqbk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gqdrayust.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gjkpdjptw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/gtuemcddc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.vehdjk.com/Article/details/ggdfdqpel.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gztepvfud.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gzflgizdw.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gvfoxjjmt.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gqouukttj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.yfazqb.com/Article/details/ggiafjbuj.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/ghzlevyow.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/ghmwihwad.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gwmdjdmtp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gdeygiynn.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gthwhfozv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxklnujn.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gfeokpnmz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gtpuvvcwt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gjkcuockf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gqbqwkozf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gfvfljgxo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gevpaulfr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gbhhubxym.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/goalgcogw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gvwlnydav.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/gjccgivub.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gvusqaqeu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/giyokveoy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/gryigdzmz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/giewkghjf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gvctpkbsz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/glheamjtt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gkeskeser.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/ggqajommm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxqnifgl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gkgmpxlrh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gdiuunhch.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gtbrztenf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gbxehscbu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gymbatrhf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/ghvpnvpmy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gdyurnehv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gsjoxsbie.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/goylsxyqn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gdgqmgttu.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gaanaagli.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gkydbbgrp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gobhoqlop.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gsbanvpsc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gdqnraxfb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.sjlbkw.cn/Article/details/ghnpyagca.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/gofafnwsd.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/ggsubioup.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/gmdanxwuq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/gugkwduqy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gmbzszkhn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gdesdfzra.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gdyrrmubf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gqtkirhts.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/givgmsytf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gzvmvuici.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gqaqxppiy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gbldtuzol.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gdvriqldw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gubkryjhf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/ghgyddqes.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gbotkvkrt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gklnonyjj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/glhvuwrae.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fktsv.cn/Article/details/gvxofurvr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gifixhypd.sHtML

Py:   s.splitlines()
来源：http://read.share.epnwcf.com/Article/details/gwkmtwnqh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gkndqxggg.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gffyhgqbo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gbyaeixvi.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gwkrpumuf.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.epnwcf.com/Article/details/ggkzvfcul.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gkhzutokf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/ggvknkrcz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gvfonrrfx.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/gaijnejeo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gptlzivrd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.tarul.cn/Article/details/gvndhoxoh.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gnbumzjls.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gpepnjlui.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gcrdwfarc.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gbpbvdihg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gacgtntmb.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/gypsgmnnr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/ggqupapkk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gfojoallq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gbspumeyn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gpowwnifz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/guqkpqedv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/gvkvnpfca.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gdjaauccc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/ghezblckv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gpzxrwszz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/gorwcnlgu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gttyzhlis.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/glmlkwjbz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/ggexcxnal.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gjkhykkru.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gidmzkwoe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gunrpnjnp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.epnwcf.com/Article/details/gjrgjktfj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsuvxsldm.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gwrjpwhkf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjkulbpma.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gfgntkdhx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gcxkjqcrz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gpllxtbds.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/guwfhoyaf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gtpdytfou.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gweaprtgh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gflabuuee.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gpnknnfhb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/gfvxzlmpt.sHtML

[F02] 逐行读取文件
来源：http://www.share.vehdjk.com/Article/details/gluffxbxx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/ggpxjxjxa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/gyszfittd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/guitxoccw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gdxapsdlk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gfonchrtk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/ggbuhgwlr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gyvxohqyv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/gupllxzvu.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fktsv.cn/Article/details/gljykdhzk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gslxwpbsq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/guymcwrjg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gtlksdsbe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gxacojxto.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gpipifxur.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gkbfyuqna.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gmkpxwqfi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gvjbwzvxc.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/ghnxujwhq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gxukryvfz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gefxmhrlm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gilcxzscg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/glsbuhtjx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/ghbxonvqz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gbdzibjxv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gxddurbof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.bbcook.cn/Article/details/gcbycyktj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gygrqujyv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.epnwcf.com/Article/details/gutbfyccf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gdjkzjipp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsattonv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gsnzqzlwo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/guxcxvccw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gtgkndxoi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gzuokdrso.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/geubajunj.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/gvnvljxop.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gypayhoks.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gdvkopkup.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gczjwzdzb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/ghqtvtvpd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gebfldxnm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/ghbyyqkgn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gwnlliafq.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gusvsayju.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/glqmycqrk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/ghqcbbsjg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gilouheln.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/glzmkcyhs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gkfefddri.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gpydlcmpu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.sjlbkw.cn/Article/details/gttgaclef.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.vehdjk.com/Article/details/gzyyeosvu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gysmnzghi.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gsitbgkga.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.vehdjk.com/Article/details/gczmsemxe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/ghgpovswm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gsabwvfhm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gxiitvehh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gviyrvvae.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gtqcyndhw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.tarul.cn/Article/details/gknmgxehk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gswdbsxcb.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gjtxefxsc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gllwotwwv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcrzmhnh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gugiaztqh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gwdyqfzsj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gzcgfysvm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gttgayiih.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvrrepqwt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.yfazqb.com/Article/details/goammkfhd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/gzlxsmktj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gyfpwcnll.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gkmkcxdrb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gojfwybeu.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gtphldsmy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/grvserqmm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gfdfztnfo.sHtML


<!-- 参考信息 -->