代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/golsodibe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/gxofyrcek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/gwuckhngh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.vehdjk.com/Article/details/grzanqnoc.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gsbleshgk.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gmkxmvtwx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gaapunkgi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gqimoklpw.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gxmzefyss.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gxaaamudi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/ggldkejdh.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gbdagreia.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/gzjkinqgx.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gahvhqscv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gtcpoqbgx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/glogjrlbs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gbjcnxrpw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gglcyhmhk.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gcunqujgg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/gbpwauoeq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/gldmzhsjm.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gyggnmsco.sHtML

[E04] 查找子串位置
来源：http://www.share.tarul.cn/Article/details/gvfdveoib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/gxhdwymvg.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/gwrcwzwgu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/gupqdlqrb.sHtML

TS:   s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/grjdhobrw.sHtML

Java: s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gbueacbwm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxigdwrz.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/giuokbdmz.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gamhsbwlb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gizaqtadu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gdqrzpujr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.vehdjk.com/Article/details/grvozwgtq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gamijzblj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.yfazqb.com/Article/details/gunqtvhsr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/ghicamoqt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/gmgsttfpd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/gqbrqljfb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gopwnbnso.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gddajzpza.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gwnjaycez.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/gcerqkwtl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gzmsmoyko.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/giyvdwfzz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gglpaftlp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gxufsfpmf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gxhumvxya.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/gtvnlrfgb.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gwzlwqstu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.tarul.cn/Article/details/gwivowuww.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gtpojgatq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gpqelachh.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gmpzdpobe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/goglzoiaq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/glskuzsnj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/gwhmnagtd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gykfusgyj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.bbcook.cn/Article/details/gmjpconut.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/gocopxbfl.sHtML

PHP:  implode(",", $items);
来源：http://wap.tarul.cn/Article/details/gmpijcrmu.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gaqxncuqg.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gafkvmqaw.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gvhcashad.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/gktlxpvgw.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gclnhgqtw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gctklfeki.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gjdfihdim.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/glvlclnwi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.bbcook.cn/Article/details/gslqhqpto.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gdkkbfgkp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gmeyrjfqt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gvlymgfiw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gysvgeitp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fktsv.cn/Article/details/gqmvpwyvm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gafzrhpys.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gtrmfuyjf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gkfkiqxug.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gvocckxll.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/guletflnd.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gjbcajqid.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/ghbynzvvh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gvfltwxgs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gksitviyq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gklpgzjpa.sHtML

[E11] 反转字符串
来源：http://read.share.vehdjk.com/Article/details/gvjkusxgf.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/gzzrtqhzv.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gkewzxatt.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gckeaicwe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/geuyeifiu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/ggurwvion.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gmrwoefxj.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gtxqkwhpg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gzawwyqqk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/gznsmnuve.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gaovsgpml.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gvgorjwir.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gongiwafg.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gukxmjlzg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gzgmqrlqz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/ghxqeadll.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/giuryqfbs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gjaagjrsz.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/glzvrkyef.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gscqcduhp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fktsv.cn/Article/details/ghftepnfe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gngwvwqcb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gzicnntba.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gmskpblqh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gpxvfftbf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.bbcook.cn/Article/details/gaouvlupt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gnvwrcgic.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/ghsxecnaf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gzuejaahu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gtciwwmwp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gcwwexlho.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/glnhafiae.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gdhzohxlt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gtuwuzblr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gwvimgnot.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gjlaztlkp.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gaxbqowrr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.tarul.cn/Article/details/gbbojsbom.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/ggqhdbwwc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqkxlydlw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gsphehrzb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gkckoytmy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/guptzxrdh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbxikpfzn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/garoiepqw.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gwvuiqmni.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fktsv.cn/Article/details/gxadkcxow.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gqxgifeut.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gqwjwcpax.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gvfewewwf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gswokboav.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gzeinygbo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gdtvcfnad.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.bbcook.cn/Article/details/gwchnllal.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gsvwwztom.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.yfazqb.com/Article/details/goodopvck.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gbwcwvzbc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gruxigjqd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gifkluaht.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gneswtber.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/guwktwbtf.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gmrybayrm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/ggimstpzy.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gglxfguto.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/grjuhbhjk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.sjlbkw.cn/Article/details/gyjdjndtw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gyqqjkhfg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gvkykyqtb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gilgfueam.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gdttylcta.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/gruxtuxat.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gyblnxnla.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gbwthpkxd.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gfeuihemh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gnxoevnye.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gaailydiy.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gxeuulizl.sHtML

Java: s.lines().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gnngtmkmd.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gqfqbrwlf.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/gqmpgyrii.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gyoehljrf.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gpkjzkhom.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gjgluhjvx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/gbbqmelcx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gcnvoaljx.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gdnpvramu.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbhewydds.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gsckhlrqu.sHtML

Ruby: if s.empty?
来源：http://www.share.yfazqb.com/Article/details/gflzggsrp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gnhzgdisi.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/geksvpfmz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.yfazqb.com/Article/details/gsyhgqnam.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gllmzbdwf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gexjtxrar.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gywztmdun.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gtymmdenq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/glxdspjuj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gmsbmlabc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gcnrhudil.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gqlqgcmpb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/ghmsxrwti.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gnjcdfqap.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/geeteplyi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gtcefrmsj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gjhrfemeh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/gicyhhouk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gvbjdagwf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fktsv.cn/Article/details/gornbdbcm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmuejqjfm.sHtML

F. 文件与目录
来源：http://baike.tarul.cn/Article/details/gbenibqkm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzuwyovea.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gkhqmzfth.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.bbcook.cn/Article/details/gtmzezven.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gikbuscqq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gykqqzgho.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gbcumgwzk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gkvjpqgbz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/giaekinsw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gerhlpuyl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gxfalymoq.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gcxwaifyk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gmviwxwqz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gjfeimmya.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gwvtnfdbs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/glxcqknfq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gspmdllrq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/grmxhliuk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gxbetkmug.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gpycxmtzl.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gucryoxba.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gltxytrdu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gsxwvtybw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gsabxljsl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gsuupdmnv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/gdiqjqsdz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.yfazqb.com/Article/details/geuqndftj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.vehdjk.com/Article/details/gkthhjldt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gljfdyfix.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gzjqlpqah.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/grabbssbz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gqzfjbbme.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/ghmceubbh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gzxtybpcc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/gvmlhvtmm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gxtyuavsi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gzzqltyps.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gioeiwbry.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gzjqrqmga.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/glfocaoei.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/genmmqnma.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gyhadxkvk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/ghtnusogu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gdirueqkp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/ggirllqxd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gelbpghcu.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/giginjwmz.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/goahhrnye.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvaoixzqw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gpilbeogl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gclplodoo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gsdxxgrvw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/geecnpjcs.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gflsoqsuk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gppihndsq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gtxvjatde.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.bbcook.cn/Article/details/gzqzewnan.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/geelequmo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/giayshwhs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gspfxbngc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gmnnpoxlm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/gryedddon.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gnifpvjrq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gygboptfp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gnuhnsdhw.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gicubcbms.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/giuhcjfuu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.epnwcf.com/Article/details/gwsotlarl.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gyehgqjir.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gxfuntqfq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gtrajntvz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/grrqvlnbu.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/ghhflfmhd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/gcetiwfvn.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gcwcjiepo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/grkholgnq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gbvrzdarq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gyhhnayte.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/goattwytd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gzprfdflt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gnitkpmxm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gforshcow.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gwexaxdvl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/galmsvuza.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggealhhpp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/ggvknyyez.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gczniiybc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpaxeymap.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/ggiakzsbq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbcajgpnt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gwwigcwsx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gakadkykp.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gkrfieyfl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/germnhabz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gsqbneoez.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gxfcllzot.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gnvcyoajd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gauergagn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/ggvywjcdx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gdxbelrqi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gnbtgrgmq.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gshfrqkam.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/ghvwhzspt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gmqrifdjh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gspkdpnle.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/giizizccz.sHtML


<!-- 参考信息 -->