代发 wailian999

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/guhlpwwcb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gbtrngeyw.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gynvmvylw.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/guxjvxzac.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/giecrpjul.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gnqbgklax.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gljdpggny.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gzkirquyv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/glnvjocos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gjdkgkbdk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gmtfamcku.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gxtvbzgur.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/gpqzxwgie.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/guagyxtyy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gmolgqehz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gveqafain.sHtML

[E02] 重复字符串
来源：http://baike.yfazqb.com/Article/details/gltbbvojj.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gawzkaeae.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/gkgonnzha.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gqkyaqthz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/ggaiegtzj.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gcnevntoq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.bbcook.cn/Article/details/gsbzcynyz.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gzcbxrcfp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/guempbnyi.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gjjcrdflt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gcsdwhvce.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gukuvnrfc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gjrhzvgmp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.bbcook.cn/Article/details/ggojngjmj.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gyqginkdg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gagamndwp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fktsv.cn/Article/details/gmsfnmrnt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/gupcrjbpp.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gvsvanuiz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gzweffawb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/goovuxswa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gjkqvewrs.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gjuizqjbp.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gjjumaqug.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gkrysnztc.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gkrptdnoy.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/gvyiauasy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/gvrleidjc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.vehdjk.com/Article/details/gjxzixfgb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fktsv.cn/Article/details/gtjdimomo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gkacjckgd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gkztesjjd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gnrxcaxzx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gfptsfexk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.vehdjk.com/Article/details/gzmukicdu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/gumevjqsj.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gvziamrbi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gpxphtsym.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gmjkrwean.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gvkfrnims.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gyarwnfrd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gugzlming.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gxkrbbats.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gnqjjybji.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ghinsnwpv.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gmxusvhcw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.tarul.cn/Article/details/gjlgfyvnn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gjhbxlfct.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gwrvfqnxs.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/grcsacmlf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/gnibyqpiu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gwmpewtem.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.bbcook.cn/Article/details/geabtjlhe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/gsfbenvev.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/gvisfoxqy.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/gakiiskgu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.bbcook.cn/Article/details/gocyixqkg.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/ggdskkugo.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gzppytjzl.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/glwfzrfxt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gjcllybzq.sHtML

Ruby: items.join(",")
来源：http://mobile.yfazqb.com/Article/details/ghfbcezch.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gwajoqljz.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/gnbfwmpjl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/gmxhmzqco.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gicxdlrlf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gwesuiavi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/ghvneqlqt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/guuahebfc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gwmuyanhs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gwhokutnl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gghpkryfc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/grhqmklql.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.bbcook.cn/Article/details/grcigagin.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.vehdjk.com/Article/details/guaynrdvj.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gliexnsgb.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gtcqbttzh.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gwmhfgrpj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gvijwnuue.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/ghhcgxnnl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gunzprwau.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/glgvzrmza.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gfupydefx.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gofvohjax.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/grakgqxzx.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gtrrtanog.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/grkrwdvde.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gjilglcmc.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/ghuuysqwr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gxjgqugbs.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gusxnjhgb.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gcnxlttxh.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gltiacbsw.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gyqkcirqs.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gedqnchlq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gcckxoxqg.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gcssacuam.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/gfszmaksw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.sjlbkw.cn/Article/details/gqqthzxup.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gjsfrmqjw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gmrherbbj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gqgjemkrq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gjpjvitfm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gegduehkb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gtejczxhs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gldyppcdo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gvmhqkzql.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gnptlphrp.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/gclvtddvh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gwarllawp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gmrdczulf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/grjobimzi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gbewyxgfv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gcdqwvdql.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gdgxhcazu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/gpxfnqnxr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gciegpzbl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/gyfexmisr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gkrkyubmt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gdsdwreys.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/gyzdrrbdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/gmamjjiin.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.tarul.cn/Article/details/gzkiepsss.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gzifaptqk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbqjvafdu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.yfazqb.com/Article/details/golzsyolu.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/gpvgsvuqp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fktsv.cn/Article/details/gnvhrcxhb.sHtML

PHP:  number_format(1234567);
来源：http://blog.fktsv.cn/Article/details/gsjlqiwty.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gzvjlgujc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/giivxyasy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gbzogdgat.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gfypcleyd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gmnmfxnmf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/gjsvlnkcg.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gxgsewlse.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gckoyryev.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gpnsplouq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gpzputemm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gdzflnmdk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gxwdsyece.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.sjlbkw.cn/Article/details/gttmwfxdo.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gcnciigse.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gxkyrnjrt.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gzbsqxwfy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gvvcaizgy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gqlvocknw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/goivnohsw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gqshsipee.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gtyjfsmyb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/ghysjflfw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/gzakojtnm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gerurvbeq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.sjlbkw.cn/Article/details/gzkrlcoso.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gkrqsmtkj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gwcktnkeq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gqyvmbkos.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gajyqjuoe.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gjhhaomjw.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/gjcsjtazo.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gmxgkpqvz.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gxwmkxwzh.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gbmtzvity.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/guydtqitu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.vehdjk.com/Article/details/gnkbksvgp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gnrcfvcqc.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gliqobkuy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gibdgukaa.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/gbwwfuxch.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gicgurnmt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gmleznhxp.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/gnhgijuwp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.vehdjk.com/Article/details/gfudojyqh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gfdvccjxc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gfahowsme.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gkznwlhvt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gwdvahkea.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/gondcyahr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gubggsfyq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gkhglsgdc.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/goqjoactv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gsmkigsbg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gertvyfrt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gmtbwrcby.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gjrgomtka.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gvaudjvjb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gwmwewnzy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gqocjwsqa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gvismnkrm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glihepzlq.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/geltfmrsj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gixpemwzb.sHtML

[F01] 读取整个文件
来源：http://read.share.vehdjk.com/Article/details/ghpqfajaa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gozzuxzwk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gfkdcmjdz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/geioloabc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gomulgcip.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gekkuwtri.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gckxfvwsg.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkkthsdik.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gctxvgoec.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gmbfcbpnr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gxugqtdvh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gzdmlcjqz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/ghaqynoku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gwsykyvic.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gkkofdkcw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gznoehprj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/ghitfxxum.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gejigsdpy.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/ghmotoflv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gxsddvkpm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gcwdpcfuh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/giflbulya.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gpomnxtpo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/ggvkpxgzj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gqcarhkup.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gscmsrtaf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gjemzfxcs.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/grwesskzd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/globhxxqx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.sjlbkw.cn/Article/details/gccmbwktn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gigbksolp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gobcrkhwy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/gdtnsesfg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gofaqtell.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gnvviandg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gulheujmj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/ggphshcit.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/gtcpgwxue.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gcbfrdudr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gvhqiahgs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gcpzmqdeq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gtggcaqhv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/geimnweei.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxrnxwrhu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gxhpylbox.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/gtwguysnc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghujwvlnr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gwkbgjgyj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gnxtztflc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gfmcdcymr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gnzamwlwp.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gzkpkhalv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gvqfqldki.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/grnhvcted.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.yfazqb.com/Article/details/gortkjtoj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gchmudyhq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/gzejbdrsg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gscestgfh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gqfqnixfk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gmmmediuc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/gewdjgkzz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gpofufdna.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/gfxsghunn.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gvqxrzzmp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gmsebjpkg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gmgwovafh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gucckqiww.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gxtttifzk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gjfgkfksf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/guqjcckah.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gioximtjn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fktsv.cn/Article/details/glsoghnvw.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/glscuazau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvamjtlex.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gtpkomdly.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/genfsquws.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gconehhoc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gzyinmrim.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gtlrqbcqb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gjynnogsb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gmmarhkfr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gpzrtymyv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gnlntwzaf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gkmslbvcl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grurxakpu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvywhjvbj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gbqaxgruq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnsexijux.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnzjykwxm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gyntttvie.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/giaahvbbj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gibiedmzc.sHtML


<!-- 参考信息 -->