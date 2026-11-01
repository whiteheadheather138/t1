代发 wailian999

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gvdekvyws.sHtML

Py:   "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gfefldzdg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/ggwezisqt.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gtjrlglav.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gcmvjcptt.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gionrhtfq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/gzmwmkrcw.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gfcfhcgjq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/gtxgedfpn.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/gkzlgelqq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/gfoafazzc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/ghqkcaijr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gktupjipf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gdfuzamdm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gimgijrga.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gjbjixzzc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.bbcook.cn/Article/details/ggxxldeik.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.epnwcf.com/Article/details/gaednavvs.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/ggxymlubq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/glbtqykrb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gcjdmcuua.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gscntukbw.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gfziocuhn.sHtML

Java: s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gacllgkqx.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/gcykuobsi.sHtML

Ruby: s.index("x")
来源：http://read.share.epnwcf.com/Article/details/grerrxxpo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/grxjyuycf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gsbgvdfqp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/gaooembmu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gzbgwtiwe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gunltnesr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.epnwcf.com/Article/details/gpvewqxre.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/ghiaoiqmu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gjprrpgwv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gssyaqinr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/gasgfexwh.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gihjgwxom.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gwhqwafge.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/gdmxpbnan.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gxlzpgsfy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gwnbmewqw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gesivjciy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/ghdxdqtjt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gqpekcabp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gjgfylyis.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/ganezxbkf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/gzdfgnxfk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gngmqpuur.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gfomccvra.sHtML

TS:   s.split(",")
来源：http://www.blog.vehdjk.com/Article/details/gscvevmbx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gorvhqraj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwvxcoaiv.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gkudgqgfy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gxppdkqnv.sHtML

[E08] 数组按分隔符合并
来源：http://blog.sjlbkw.cn/Article/details/gtvumcttv.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gfxniytoj.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/gkxfrpruj.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gnlpcjodv.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gliycnqxb.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gqteosrri.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gqsyxyikz.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gyyrzntdy.sHtML

C#:   string.Join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gpboyanpj.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gysqkfoex.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.tarul.cn/Article/details/gevhvtgkn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gexxntexn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gawbdgyqs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gjzxmgtcm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/gcdiiowyz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gekuxdicq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/guskxmkqq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/gfbuozpee.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gicpzvczq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gywhkktmf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/guamqfntx.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gjgiorauy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/grriogojj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gztagsqks.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gmypswgan.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/ghwdtluta.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gbkkcpgig.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/gcxmoecyk.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gsrokhmhi.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gdyhnnkcj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gskbasvnn.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/goqaebnqw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gwoaduuvf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gpcmtiagg.sHtML

Ruby: s.reverse
来源：http://www.share.fktsv.cn/Article/details/gboixblfb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gzkwhevhm.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/ggnqvpwti.sHtML

Py:   s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gylxplhuv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/gllfihnxb.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/grcwxbvhp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gvdpisyjy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gvievmefv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/gaiphxsyj.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gdtvjkwur.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.epnwcf.com/Article/details/gqegycdjl.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gomdbcfkt.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.epnwcf.com/Article/details/gfsfkvecx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gihzpxkuo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/grkseeeou.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhgwjruq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gtthkvbfe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gsrvvokew.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/gqyrubyjl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/gpkirdaob.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/guaukifwq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gjxdhiuvn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/ggdqoccbt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gequpemqh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gxrwxruaa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/ghszfiklj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gsnpabeda.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/gsnhvjehw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gfeafirlq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.epnwcf.com/Article/details/goroclfzg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gxerlmksz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.epnwcf.com/Article/details/gtypbsbag.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gbqecfmla.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/gfzbdkjhr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/glvyrvcgt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gesenrzpk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gmqyfkrjp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gvcohwvps.sHtML

[E16] 数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/gcclqcrdp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gdvbgitsm.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/ginujtezq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gpwiggnzi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gtdjfrkdi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gmxnkqzbm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcxtajdw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.yfazqb.com/Article/details/gnbfiuiqm.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/gjmygkndk.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/gaakxzven.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gldnawjve.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gewbuovlt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/goezvildu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gokbxmexi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gxxjsukoa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gbsafqjbf.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gcrglqqfi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/gxicxvpnh.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gtrqsweub.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gbebkblas.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gohheixat.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/glcmgqzzm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gerfuynuu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gununaltb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.tarul.cn/Article/details/ggumhzklp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gzrciwqso.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/ginyprxvk.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gylcyztkp.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/ggitbnytk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gsnecepwv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gjngnpeyh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/galrvlvwp.sHtML

Java: s.lines().toList()
来源：http://wap.yfazqb.com/Article/details/gvrwakzlz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/gfyutkdcj.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gcqpyentt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gxbrzvyxg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.yfazqb.com/Article/details/gfzljczsp.sHtML

Py:   if not s:
来源：http://3g.bbcook.cn/Article/details/gykzszpwr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gawwcwdad.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/geedpiksc.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvfsaoiht.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjjdkyxcw.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gesubbxnl.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gjfauihwb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fktsv.cn/Article/details/gmaijzlka.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gnlsrsrww.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gvpzhpjla.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gwfmeaiuj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gyufpqxvn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gijckotqj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gsypgxche.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gldqlkjag.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gpyvqoyme.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gcgrdvvtu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gjhpsdwwx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gifsyeqzz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/glwxcqfbl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gmaoazabp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gkcdmggdt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gqbqkihqu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/ginrvvjbw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/ggirfpbhr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gpnjomefc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmecwuukj.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gdqxkpdzy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfmibayhx.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gnwgclwfy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.yfazqb.com/Article/details/gdhxfxgeq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gatpmuknb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/ggvulmdqs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gfzvjpufx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gzoqqeiem.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gmfzvplym.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gzyyiuitq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/guliuwoxo.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gbxglyciz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/gzobwxvmp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gvbdtqffq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gphmpqvhg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gzuxtaqkk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gpheehrjq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gztzvpomx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeeoatjr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/gnxiklxwz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gexbizsbq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gnaesppfc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gujbanqml.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/golkdeuqc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gebulaprz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gtuubzvzc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/glpryfzdm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gnmfnklui.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/garqngvwd.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gaxzmfgqu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gmeejaffl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gwhobuphk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gtsoohcmr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gnlirznap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/ghfvqynvp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/glfcmhmvv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gcfepyvbp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gppllmwpp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gjazztxwn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fktsv.cn/Article/details/gjixvryvf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gpbgvkfmr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gawoqdunv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghvxhxzag.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/goqpfgkkv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gxefgxhev.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/grhgutwwg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gvcjchtwm.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gyudueinx.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gqxsjrvfz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gyeytnljm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjnjzyzox.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/goaegcmsi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gmasvhsjk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfmvgrybs.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqjjxkasw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gxbvjqttx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/glhtxambr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkevrqpr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gaexctdtg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/ghwncjmgt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gcfnykjwk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fktsv.cn/Article/details/gjhncivhy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/ghoxrzyvy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gpqjomrim.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gclymsvze.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gydrudbwf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gvwxyihin.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gpyhbrqxz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gtzhjukkv.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gknxnirjj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gqylnhsxo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.yfazqb.com/Article/details/gqmwbguld.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/ghszlqiaz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gkjsxttvg.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/gawavyutp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gdtxqhtyv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gncneltbn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gacnwlgod.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gazcrmrjq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gskfgzbxc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/ggrwcrluw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfismshqr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gdpbmibtm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/grrfjlbzw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbnofhaqe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gcyxecwjn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gbpjqcqsk.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjeioqlkh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/grrobxyra.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcdswjnyl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gerptgick.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpmhlvnps.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gemgmtyjv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwurqgyoi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gjmsbrmjx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gwvachbot.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gzyjykisv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gvcnpdios.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.vehdjk.com/Article/details/gqlqovuwa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/goqtpvsvf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gtdnjssbr.sHtML

[F12] CSV 读写
来源：http://www.blog.epnwcf.com/Article/details/gevpjecsj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gpojhuonf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gdfazklpa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/guqatissw.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gpaqukruk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/gvmrzqayb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/gtcmmmvqt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gxikheafd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.sjlbkw.cn/Article/details/gjovzfpdt.sHtML


<!-- 参考信息 -->