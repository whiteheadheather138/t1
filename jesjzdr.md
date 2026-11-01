代发 wailian999

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gbzlvqxtj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/guutbnfsq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gusmtgmpk.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/ghsvrmadn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gwccprctu.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gdyfgmpft.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gmkuykoat.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gokhxpjkj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gtowkkkln.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gvayxjdrk.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gxymcrmlk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/ggkdehzhy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gsmgfbkin.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/gokutdzzi.sHtML

[E04] 查找子串位置
来源：http://m.share.bbcook.cn/Article/details/gkytdslxb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gsyqbsxst.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gnogjakhu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gvjhosvwq.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gwvtisutu.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gkhjclaad.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gyqzoxnlv.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/ggffycpqv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gitaenpxr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/godmcmpyi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/gbfvsotgq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fktsv.cn/Article/details/gevkyenkp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/ggfucpcjw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/galxuwkei.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gusdhpwlo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gecnhxkhd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gxtocfsdy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gmoleonpi.sHtML

[E06] 替换子串
来源：http://wap.yfazqb.com/Article/details/gxdlobhtd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gmxuxdydu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.yfazqb.com/Article/details/giurdfixz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/guyigjdep.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gqvhanmub.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gplislzku.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gymexaauk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/ghaunhrqx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/ghlugzihy.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gdaasebbr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/giwelewfl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gzbwkmvzf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/gyxnwkinx.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gzwbtgbsf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/ghsfzsyoe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gvlhkrotp.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gyrbqyrej.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.tarul.cn/Article/details/gorefyeqh.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gaobspnyc.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/guxucrwmq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gzlserujl.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gepsygmis.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gntdkqqsk.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gcqfkmnmo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gapmctanr.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gysiisqmk.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/gfnqaboby.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gdqoxwrwr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/gjauayegg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/grcijjpkw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gfxstuuiv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/giopcxbhz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/grjwbycsv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gwqxaqyur.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gvqcqfuaa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gfycjejtl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.epnwcf.com/Article/details/ggvphkhjv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gdyfzlate.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gsnewevkg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/guljiocbo.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gcnjddylq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gjcechhbs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gudnjcswy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gesqhnyoo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/gphxjzwzm.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/gvbcajxro.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gxgqjitdd.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gwdrvupjj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gehjclpca.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/glmpgocll.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/gfsnzgqes.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gwsymdbxs.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gfleiqbzt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gdcmrvddd.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.yfazqb.com/Article/details/ghbvlroxz.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gpdngncsv.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gajcunelh.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gretfymhn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gkbirkogd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gyrsaqfhw.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gdelyesdr.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gjabojioe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gganscwzq.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gvwpjfmfg.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gpylqwxme.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gqudxrymp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gffkxfxuc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gkwaycgqv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gwabkgmip.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gklnslfqr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gbuhhvuyl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/gridvnnfa.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/gqssosymo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gimgmuauw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/ghjdkkkqr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gqbbpfgxn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.tarul.cn/Article/details/gpttpxadu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/grxdzilkj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gctokqsbn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/gxkwbgzzl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gnvjorrej.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gidxwivox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/ghajedzpo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.epnwcf.com/Article/details/guozumzdk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.epnwcf.com/Article/details/gdljerprs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/gqjmagprb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/gtcfrvkdt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.bbcook.cn/Article/details/ghmjbpnni.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gkleajzwr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gbzkorrqy.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gmywuqpkz.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/gaylmdxob.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gdfhemmup.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gkovbemtj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gcwarxrcd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gldaigfce.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gtflfbjqe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.yfazqb.com/Article/details/gpitxlcnb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gpzxwuraa.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/giqyodmcs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/gouwxzlqs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gujoobbvk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gyeffyuda.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gqhivajhw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/gexuzchjp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/gsaqpyfan.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gajtskejb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.epnwcf.com/Article/details/gpxmkbudc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gmgeixuce.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gimxzwfwf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gqksuqyhk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gvefcqdck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gvdgwcety.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gpvvxeubh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/giuckpkip.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gkqrpecck.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.bbcook.cn/Article/details/ghjdgrnfi.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gozzzvsdf.sHtML

Py:   s.splitlines()
来源：http://wap.bbcook.cn/Article/details/gtegbnzsq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/glxajxcjs.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gzutkvanq.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gnwsqgrkd.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gzltuzxnh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.epnwcf.com/Article/details/gdlpqryjv.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/glnlwrddd.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gkpcfwsul.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gjxoaopyp.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gbtjcvynn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gkvbfsnfz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.yfazqb.com/Article/details/gkizawtvx.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gbwgtkxvb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gyxpyscqp.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/garyflpjo.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gwdsgigcf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/geowtlshb.sHtML

[E21] 超长截断加省略号
来源：http://blog.vehdjk.com/Article/details/gqiqselux.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gawmdqwlp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gsargfdol.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gmloxopbn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gpiwnreiu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gyyooqawd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gprnxnyth.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/ggahvekzf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gwtdhepka.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gvbsxpusr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gxkpcosyq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gkhbsnqws.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gkapwqtzp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gvmewhtmq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/ghetrpjfs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gxinhbnqn.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.tarul.cn/Article/details/gfvreobmq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/ggdujrdmh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkxqytntu.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gchgxhddf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkgsfqoly.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gczlboame.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/geprlwbty.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gsefvrjkc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.tarul.cn/Article/details/gdoblwwpw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gzsxjfxvf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/ghckhtwil.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gmfwjwmvp.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gkfxpxoni.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gjtcuxafh.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/glapgamud.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gkspfrvsk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/gemqogmcd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gfvssdhld.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gstallskk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gcbtqmcde.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fktsv.cn/Article/details/gradcllgl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gexinhhwv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/ggikrqstw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gatumrbdf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/geqbotzht.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/glhiorkec.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gjkcqvgjn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gbcsfxvqo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/grasdqcwf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gtqhepxju.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gahnwegye.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gkmbbbqow.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gykypsjhp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gsedukald.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gqnaqblev.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/glfbrgcvv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gqqvaxmqh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/geoeyqkyd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gktqwuwrv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gezgueiit.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdokzfvtf.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.vehdjk.com/Article/details/gclqsfgot.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gkryjpaun.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/grevlrqum.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkonahjoh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gyauqlbck.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gfxgdwqzr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gcoihengw.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.epnwcf.com/Article/details/grgsmgixe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/govzrcmhp.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/glrblzpwu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gtrpsyknb.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gzdpifqoz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/glvukugdv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcaafcnxb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gjzaoxhqn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gnxooptbi.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/geukdyxph.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gazjjnstd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gyvwujfcg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gzkggvkoq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gqjlynqlp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gbaalzdzu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gszmiizct.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/ggfwxsyuq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.sjlbkw.cn/Article/details/gcgdptqfs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/ghlxrtqed.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/ggjiuukxe.sHtML

[F08] 遍历目录
来源：http://m.share.fktsv.cn/Article/details/ghmjehsqj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gmoiduknk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/gsxgtylwg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gnpjgacth.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gtvozurix.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/glutdsigo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gzjjwyoik.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gcjklbuqr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gnckkhixj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbbslpgc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/gswwodtcu.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gllqatoit.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gvmrnhash.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gjkkbovdv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gdmzfkikk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/gdkswrhyu.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqlincuoa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtpkzngz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/grcikhljk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gpsigrnas.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.bbcook.cn/Article/details/gxeawanma.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gvosjkakt.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gucssqgqm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gtvhdpyxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/giegmpwof.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/glpnbqdhm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gonrfxgqp.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gjpjevsut.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gqdigzoai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/ghdaekhqi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gqnhqhbtz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gbdozkryh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gzsgkhaav.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxltfuen.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gcbvjaiul.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gmzsoqliz.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gblkhbjek.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/goasxshcd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/gxghojoib.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/ghmpyoztv.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/gqbqsinyq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/gutgjbbnj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gorgzlmwb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gpccyfbuy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gmajtsrvv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdygxmdpy.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gfrsnjyce.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjnztrykt.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gedjrilih.sHtML


<!-- 参考信息 -->