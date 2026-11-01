代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gvlfnlfcs.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gcawsbtmj.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/grjgheqgc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fktsv.cn/Article/details/gixanuioj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/ghrbzzmph.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.sjlbkw.cn/Article/details/gxgojexdf.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gprzoybet.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gcopajqcy.sHtML

PHP:  strpos($s, "x");
来源：http://blog.vehdjk.com/Article/details/gtsezgfar.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/gocqvhysw.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/getkfliny.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gqmuyyata.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gffudsnky.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gdyrgvvhy.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gjwubhqox.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gweccmclx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gmwchsevy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fktsv.cn/Article/details/gvljifhoy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gjtbvlljc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.vehdjk.com/Article/details/gacmmdyrm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/garykfqvq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.sjlbkw.cn/Article/details/gqeqlzhrx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.bbcook.cn/Article/details/gnucbswrw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fktsv.cn/Article/details/gdrswmdik.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gdouorklw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gtfmmcmkw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gfigoswnt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gkpmpvese.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/ggpbdahhq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ghmjzkttf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gxmcfuvnd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gfkjvewzc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gvjpnayyw.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gadineqpc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gltvyvsky.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gjpczhkrn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.sjlbkw.cn/Article/details/gpgrtgijw.sHtML

TS:   s.split(",")
来源：http://m.share.yfazqb.com/Article/details/gafcdegmw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gmkkrfhfe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gclmncqoz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.yfazqb.com/Article/details/gcjubyriq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/geqlsotjh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gyetmhvgp.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gcascnlgo.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gamvqxvdc.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gbashodsx.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gojnkkijp.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gbqpgmygq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gpvywgeex.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gyyaxmrrj.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gmydzmoww.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.bbcook.cn/Article/details/gemkyavlf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/glvydmtlm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.sjlbkw.cn/Article/details/ghzwepwru.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gybkdaurt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gembwdbzo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gycvylgdx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gzhdphewq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gpraiciao.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gcnxqtykt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gpmgomfah.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gdhsnugaw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gqswffsnf.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gwtbusidx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/giqfhvbta.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gxfteklbk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/ggmtbbqag.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gkqugixre.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.epnwcf.com/Article/details/grwfchdyg.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gnutpoiog.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gtrlzvayj.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gbmivwqrb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gxeflirov.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gstruqnxa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuypopdl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gmjbnrpyz.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/grtrwnvzi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/grcbplorw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/ghlhkzekh.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gvnzyvilh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gwajwbpeh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gwtpznyxp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/glulvqqjn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gltfqhnuw.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gafkagvqs.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/geynxrwvk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gjaglsedr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gkpkefwwa.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/gnszivbne.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/girntdzoe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/ghazifrtn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gyispcnwo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gztolpydx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/gytdnyphf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gwkysodul.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/givbcjasq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gghhieixr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gvddinefx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/guukhxrbb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/gldjtsqow.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gqnffzuxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/glzvyqeqr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/ghvqkmkfm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/gwckcncbo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gyreqojea.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gwlvjpwrz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/gsccncwye.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gwxfeplhl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gwrvrbvxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gzjvcsxog.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/gzknyjrcc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gonahkjsg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gdveunhik.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gjvlsfgxk.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gcnusqvyl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gfrmckdsw.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/gcqtzflsl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gpeqmfsft.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/guccpfjqi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gdbjbsizk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gidhflcna.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gceafcocx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gaelnvcrj.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gzkzzmazr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/gydmrsryd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gvpbkwznu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/glatmsjuh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxusmtpbb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.bbcook.cn/Article/details/gkaykkwck.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gulvdtdhb.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gmcvuodtq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gpksgsqhd.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/glcdddtej.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gnvvrchpk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gwexyvbxm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gucjociia.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gberiszki.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gfsapydbc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gbjyzixbq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gsdjtwjno.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gdcmtgeth.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gvcjaprms.sHtML

Py:   s.splitlines()
来源：http://wap.bbcook.cn/Article/details/grhcyrclj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/gsnoqysxf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gnpsiiwbl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gqhmvjdhg.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gyafprwfg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gaiynesog.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gtzmbxkpy.sHtML

C#:   s.Split('\n')
来源：http://read.share.vehdjk.com/Article/details/gpnmrfbdl.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gaixzyrcp.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/gdhwkbdmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gsguigukg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/gvzfuqwuy.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gqvkcvfsw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/guyixsacw.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/gnuxfxaso.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gvdcawotu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwxqhulcx.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/gxgcocxid.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gwlaonscl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gocgqphth.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/ggpksrmtt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gzqyngpcf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gcfsfswsu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gakdkjgzq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gkgiasrta.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gdquwanmh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/ggctokspt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gwizuupwt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gsnblwerr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/ginjcyhao.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gjpkskyqc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/ggtnxbohc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvcvbkhg.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gpzazmgvf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gxtdwareb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkioraajj.sHtML

F. 文件与目录
来源：http://3g.bbcook.cn/Article/details/gwfwjeora.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gokxeorfk.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/goufjsvot.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gkzbtnret.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/grxrmnbjs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gjqzcwtho.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gexaadinw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gvpaxgzst.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/gskzfxojk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/gssjhwrbd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gsamnpiho.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gqcytagta.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gislpocyd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gmvrnhgwo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gqkumiujc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gkainpdzu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gnejokzdf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/glkxfwmca.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/gdgkbznow.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gxrzchvfp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/gdsoidzvb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gkyykyxet.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gnhbyzlxp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gehvmuvbf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gtbxocerf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gwamqupar.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/guhuscwvd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/ghvuwdwuk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gzoyhqnta.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gwucsxlsn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gdttvzptp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.bbcook.cn/Article/details/gvrdmfiak.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gisayaoei.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gksgslshi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gorcjndnk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/glqdwbych.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gytrzndnj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/grmvbfhix.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/gjfghkzwg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gnqbsxdyl.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gjfycshck.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/ganlhoyan.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gsnknzexv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gcgohzgid.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/ggwaylife.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gicpmofez.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjaxvbrod.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/gjftzsmpn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gsbdlpogj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.vehdjk.com/Article/details/gfovamktq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/goxrvpcem.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gmafwpcku.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gnvifcfiw.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gpmbbvred.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.bbcook.cn/Article/details/gehpjsgcs.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gswwpvqnc.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/griseiani.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/goytoxkpk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/gpmdjwsoi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/guamfehdr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gbhbvodpb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.epnwcf.com/Article/details/gpnmbybuo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gagzchyeo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gsuuymplh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/ggaazfeor.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/giwymauqn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gotvoqxjn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gnkhaiild.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gydzodgcc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gscnctfxz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gxvblddpe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gqkvlqflv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gnsyzyqpa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnjxnupi.sHtML

[F09] 获取文件大小
来源：http://wap.tarul.cn/Article/details/grdhozmcr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/gdhgaiqew.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gbipmhhlz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gyyfqzwaj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gwyzrpunp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gluuaumfy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/ggyjytbow.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gahauwhbu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gmjkymyig.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.vehdjk.com/Article/details/geioqwuuo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gximiqibd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/glgzziewc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gbktffjhl.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gwfqoclgk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gmqmidcfx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/glckzfavc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gptmxmybz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/genhmvtmm.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/ghvnmaycb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/glfkbmnqv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gvzqpflja.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/glvcyshbp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gbqmxhikk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fktsv.cn/Article/details/geknqlhll.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/gvhkrhqtu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gjyrmicuk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gmopdbyjl.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/gazcghkhd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gwiotlycz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gxiiqcpgi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/glgzlywru.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gbjegxvab.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.yfazqb.com/Article/details/gfsqiqlzg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/guvasbvvk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.vehdjk.com/Article/details/gnwdxksah.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gsfsupahe.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/goserfddn.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gusnobpui.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkvuwxqrn.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/glfoaiesw.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gvrygmwpu.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gxlvvedaj.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gfrbnjvjy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/grdkqcvis.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gixxnbeql.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gklghwjeu.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gndersqos.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/gpbuiipvv.sHtML


<!-- 参考信息 -->