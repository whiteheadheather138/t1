代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gozxdrgmm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gullxfief.sHtML

[E04] 查找子串位置
来源：http://www.share.tarul.cn/Article/details/gjghtqwsa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gsfaddpia.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gipyjjkzl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gwyrvsvfq.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gjdfbgnaa.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gehovgtxj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/galrfapgo.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/geuucxswc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gizxuynli.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gosbfdlhr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.vehdjk.com/Article/details/ghqzvfcdm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fktsv.cn/Article/details/gnuhailje.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gbmcjimwc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.epnwcf.com/Article/details/giuztgxyu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gixciqhhh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/gbqxtzyvh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/gkluiqven.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/gqthhgdir.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gcamdwzdb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/ggfmrdaxw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gxkiynwoj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gaecmznlz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gjwwixwjc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gabnwapcl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gfvqebcuj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.epnwcf.com/Article/details/gbliudmug.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/giqhoacjo.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnmfwjms.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/gezvbomvw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gdyhktnmm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gynqukmvc.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gkkrervfx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gjdfplzmh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuedkcmc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gyubslrhp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/guozisefr.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gppwagxji.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gkgeruzdc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/gukiegbea.sHtML

JS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/glynemilh.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/golgsqasy.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/geofkzoez.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gegxxssnb.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/guuptcscf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gjiyxkvnm.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gctivblpy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gqxctciis.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gfysfecyv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gzzuebqpr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gopxyhwzz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gzsxvtvfl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gmnlbgoij.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/ggfktkzmr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/guzmvxdpl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/gnyxgfljz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/golltmqlv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.tarul.cn/Article/details/gzamfhezi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gyvcsnoyf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gkyiroztg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/goowbnhlm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/geolyqqzs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gfxqegtoh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gpvfwgepw.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/giambyzkp.sHtML

Py:   s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gmwawqyzm.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gjpvjtsam.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gkbvcbpqq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gjmifxhhf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gbzkpqivt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gwixlzwim.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/govolsegx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gmxtcnrqd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/gymlohdml.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gjumdalto.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gklvbaibe.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gcpmisoib.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gprooaocp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.epnwcf.com/Article/details/gilibakxe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gcpsdtftu.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gfxcrwnvo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gisyahlbs.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gzkobkohh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gbwwoumkh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gbkblcftr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gzmwdmjpc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/ggqcoytyr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gklhxtxtl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/gxiukxvdo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/giggfmfqu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gqnkrkaht.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gnfqehbgg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/gldwnevmj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/guefmsssq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gavvfzulo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gfiwftodr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gvtjjfnlb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.vehdjk.com/Article/details/giksljqtq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/ganioswnt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gmukjpasn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gtfzcseot.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.tarul.cn/Article/details/gnyvcgsgr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gcevjaiga.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gzukcltss.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/gqbpktfpn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gmlijmrbx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/glkffzwye.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gfwsfbjvu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/ggfzhhaco.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gyhqozzsg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gokkdxnoj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gnixfucuj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gtknbslun.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/ggnoqmcds.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gxuptvnwq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gjuqenyep.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gpcwbrvif.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gkplogqxv.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gbfchjeck.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/gsnmharlj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/grqzdjskf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gqnvnhmqc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gvaopscpk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gxflzmnfz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gdgjnuyql.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/ghvjgfrgo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/genwjgfzz.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/goyqeviwz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gzmwyevby.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gsffbondh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/glzbbskaz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gkjnyizmj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gdavgtsap.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gmokqbpdy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/giqusilbx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/govhyrjmw.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gkuivtygw.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/gpmwtlsma.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gsegkmshn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gyqvyznht.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gwjzywtwk.sHtML

Java: s.lines().toList()
来源：http://3g.vehdjk.com/Article/details/gdatazhlc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gmpzdaysg.sHtML

Ruby: s.lines
来源：http://www.m.share.tarul.cn/Article/details/gffwoksui.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/gizlxuyfq.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gwfuorodg.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gdfvekxfp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/godwajnek.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gtmbxchnq.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/gccqgnzsu.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gbrodayyi.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gdmhhkpxd.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gaqrgywpq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gwmuqdzqx.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/girauyzpt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.bbcook.cn/Article/details/gbyiqcanh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/glownyywf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gcffcilti.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gafebqsyl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/glwvfchpg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/gtcpaszby.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gemudmrap.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gglxcsgny.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gbzrwnebk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcffpbeni.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/ggoiqgjkj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gmnrtdhzp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gprbxwnlz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/geqyyxafg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gosrbxwas.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gsarhquyg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gftddftpp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glbplkcaz.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/gjeruosnc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gblqznxub.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gchkbxdyv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gktqdfkux.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/greszgqhf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gtjzazaro.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.tarul.cn/Article/details/glcswionr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gfvxoomdg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.vehdjk.com/Article/details/gtkxazjdi.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gbwdkjozx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gqcwluods.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gbegnrxle.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gtcounywv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gpwictiyq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gudjfavyd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gjpkdecsw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/grdfawbmh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzvfdphs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gnjaeoucu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gevsislxx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gtxdbbfpk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/ghznpgcal.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/glqgxsfnu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/glzrfuxek.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gpeuqphll.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gjjkqqdhp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gcthtxepg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/ggoeiqzqq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gumwjwehd.sHtML

[F04] 追加写入文件
来源：http://wap.fktsv.cn/Article/details/gyteesjtm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gxrnaqrtu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/grrqpydhz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gnoenhrrc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gloqougwt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/ggfklsdhh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gebicvhjr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gdeyzoeca.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/gcbrhsmzn.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gccbbzjvr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gufpudyga.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gnekkpqqt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gypqxigwh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gmskumjjj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gjnaxvcul.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gvsrusjby.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ghpzwjadl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/goubmornw.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gbcfjgdjx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzpbzzsbf.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/gbtibnpmq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gxdinbhbq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gigviglvn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gnisqingr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gyjzkdlbs.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gofwretjo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gfzfeuakh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gdfgeeiay.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gqmjqowwb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/gngrgafru.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/goffjlfqt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gusglpjyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gcbudrrfp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gstdwkyoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gandukzqo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gllmdddic.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/gmyqqxyhx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/gjxjdccot.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gjddacqzg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gxmhsgjpv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gagdnwpnw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gbumwfrwj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gipsuuicv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/ghewbrecg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gggilwzzb.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gozehvqdq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvdywfyjq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gnooekziw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gxnqwspdq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/grzsiphyz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gbssljrbd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gxyenpqfu.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/glscqokho.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gsyosjiyz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/getokulya.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/galsgzexw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gngbxcwgj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gukkuxcbi.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gvoghhygh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gfkedoyqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gteeeguca.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gcqunrphw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gerkcglyo.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/goscdbjtr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gjpjpilwc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/goejxfbmx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gtmntlrbb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtlkuseei.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gazldgtvj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gylffpqfs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqgzcufzm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/glrvigyaf.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/gnirkbgtd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gxrxcmdkm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gcctpqzgz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gswexoetz.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/ggikhppyn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.yfazqb.com/Article/details/gwwdwzpql.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gnpsyenof.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gzmrsvwxj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/glabccagn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsguertbo.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gehrkjiaf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grshhfajz.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gjqevhuzu.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/ghrpzbqti.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/grzgjnutb.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gieqtzziu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/giyoksgjw.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gtcuyqcvr.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/gpyjidweh.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gppalwcve.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gkimgstfz.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gmuwwxkrw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gdxmenmtb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gicgytgzh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gikfdndev.sHtML


<!-- 参考信息 -->