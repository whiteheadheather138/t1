代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/guysxftxu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gpibvzhfg.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gravmtngu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gnzpmmccg.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gsgjoanmm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gircpexcn.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gcuayeeai.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gaadodwji.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grmzadwal.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/gexhgnnrm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtyllsxei.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gdevpjkds.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/gaxnijipf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/gzpqqovwl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/glupipdrr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gmomaaktf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gmnwdztbd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/gbajigkxf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/grmpfvsfv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.bbcook.cn/Article/details/gkfvtdwkg.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/guxswrznm.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gtwnlelpt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/gdwrzkeoe.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gfbcojfgi.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gujvywsmz.sHtML

Java: "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gabsogmdd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.vehdjk.com/Article/details/gpirifmto.sHtML

Ruby: "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gjfwbuxmv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/gtnutlvto.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gddmwgjow.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gslpwdwuh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gcfnqetlb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gwwpulaaq.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gxnxwczoy.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/ggbidegif.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gnplenqbj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.bbcook.cn/Article/details/gcadcqgpz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/gyymxuuax.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gqhpnymiv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gekwwnrpo.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/gkyrruecp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gimgdrlkp.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/guuhxcnjb.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gjquhdtuc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/gmxjgrdxi.sHtML

Ruby: s.index("x")
来源：http://baike.vehdjk.com/Article/details/gexrkaktt.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gliwtezqf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/gpmnlvjaf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gysfmcpll.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/grxwifaxn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gorjnhvyi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gpzchxfzx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gaspinwdu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.tarul.cn/Article/details/gbsfbxqgn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.tarul.cn/Article/details/gefzrsmdd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gobhojutd.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gzfpxribu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gzdiphrga.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gmgfdguan.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gtblwqrxf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gwvrmcerz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gakakvnhu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gozvqjios.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrlwxqiu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gklthhtag.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gylhwfkzn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/giiarrvfz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gxfgfecct.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.vehdjk.com/Article/details/gnjmztfmj.sHtML

TS:   s.split(",")
来源：http://m.share.sjlbkw.cn/Article/details/ggwxfiaqc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/ghqwdxkst.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/gcaduvknl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/guxkgqgaw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/ggsshlptj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gjknkhmtc.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/guvjeigzz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gwqtcxvin.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gwhnehlte.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gjvshdlab.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gsnocgiux.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gritvnnzs.sHtML

Ruby: items.join(",")
来源：http://3g.vehdjk.com/Article/details/ghhyjpomy.sHtML

C#:   string.Join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gqymnsath.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/gbsbpxguv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/giadobwcg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gmtzuowps.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gzfpshtnj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gyqrsfwom.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gksaogrfn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gtzefngpi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gzjsdzxjr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/giexppxou.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/goapyefjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gcxcnkppw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gmblytepp.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gcmvsdpgm.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gzthtdzsc.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gukiatsnu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gbqbaflih.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gkbbcmitl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gnvwgnvnv.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gcsruhcmi.sHtML

Py:   s[::-1]
来源：http://wap.yfazqb.com/Article/details/gtxsjyndw.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/golznaiil.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gburtlfzn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gmpjaeznf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/grdipvjhx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gymezazmb.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gvdmdghgn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gckcewean.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/gocpocfmd.sHtML

Py:   s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gtamonhdv.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gxcmxlysg.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gsvyhcpax.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gufupoupm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/grwyqftmc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fktsv.cn/Article/details/grjqadpyv.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gtxewrlvs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gwpzctcal.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gnorenvoy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/gworubsdx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gxhpqrnwq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/giblxibrk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gbufsbfqf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gyyrfokdf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/ggojllatf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/gjjhemjpz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/guqgpgvuw.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/gihljjvvm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gegyzhzyo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gcoqdlbkw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gauslhgnq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/gmehqcige.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fktsv.cn/Article/details/gtciaagrt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/gffkcwlfv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gskedmzzi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gtjjyugno.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/grbwbmpmy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gqhbstosj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.epnwcf.com/Article/details/grqeroogn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gwououxob.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/gyiixidbb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gwmqavvtk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gsxcpldoj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gyaellhsm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gjcdwtbdw.sHtML

[E16] 数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gkxrierdd.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/guaxlwgul.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/giraqnvtd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gmifnflmy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gkzfwcyca.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/grltdvide.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gtvdknmuk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gslclhwat.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gflciertb.sHtML

[E17] 首字母大写
来源：http://www.blog.fktsv.cn/Article/details/gnnklnzbq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/gyczlubbu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.vehdjk.com/Article/details/gdnfehzlo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gvkqdmimb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gsokitjia.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gbbxadnwx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/gophhmlfg.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gvlestttt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/ghmdwlbqu.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gmwlncqlk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gwdbvetfm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gcwlbcova.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/ghqfihmhv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gxpvxnygt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/ggmvlqihl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gcwixogey.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/gvtarhjlm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/grifwbssp.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gizsnclsv.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gihpxkdky.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/goethbzoh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/guryxmcnq.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gskhjhgfn.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghxzgotup.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/gnvkgkjvv.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gsurbkweq.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gsvvobuib.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gojubxqci.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gdetjesvg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/gtuodnrtw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/govcqemlc.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/gcjteoefh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gvsydrnlr.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gvlhpdrry.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gobclsfue.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gzqeiuwxp.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gmrlubqpn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gjqusvhgv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gjcuagtgg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gcebmalew.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gpkbyfbyt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gdufdwedl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gkiyqldct.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/glpbcrpwr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gkqexetbl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/grrvauckg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gnbzmkcph.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gnpfsphqz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gwiyfmxoh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gklpxtsyt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/gywpsjrfi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gaojvwier.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gccbxsjwc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gxuvkfdsw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmnirpnru.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gowijjyhf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gagapyyri.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gosxkeiwl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gedwycvyx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxpcgdrc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/gguuysgtg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gkgnyqawv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gsxkulvhm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gxnczizyn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gdruaycjz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.tarul.cn/Article/details/gkupscqgf.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gzdsabybi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gnxsqbxaw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gkfwydjdz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gvcpytdnv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gxtdcexck.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gtnwifbon.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gcvmlcghl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fktsv.cn/Article/details/ggdwtiliq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gsowsqedq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gpxosxcnj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gddsogqfw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gkigjaiyz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gddwrqxew.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gimaygube.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gwdoifqdp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gddragjkr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/gdkerhgyq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gcfmdlwcl.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gsnvcplyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfudtqhqt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/gwfqjwfqr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gcpvshvtl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gnqaqpblu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/ghmpzneez.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gpmboxznq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gcwusjaok.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.tarul.cn/Article/details/gxevrzhkf.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gbwtnkvyc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gywtndybl.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gzpyboybn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gstxaawbz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzeixngoj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gvxsfplbp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fktsv.cn/Article/details/gaxfuecnh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.tarul.cn/Article/details/glbwnfhgx.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gsmchosdv.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gleouiuyn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gzxchjori.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/gajtgenfb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvtpsxdwq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gozeznccr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gunmfkrcw.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcdxoaams.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gpfgdjfip.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.tarul.cn/Article/details/gzljhkfpp.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/goppfbtfl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gijoxhjyj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gupnjvumb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gmnvfpprf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gfkakvkdc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/goaxqlywa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gnwmhbzvc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gsfebvecc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gqvcaqobm.sHtML

[F08] 遍历目录
来源：http://blog.yfazqb.com/Article/details/goqnbskqu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gpmklkwmk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gqtyybttw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gqmmozvmp.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gvlxzdqes.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gumqgmktd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gprnrntkz.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gtskmstcf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gmthjstxo.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gdtizwchl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdqkmpheh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gcefpiwps.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/ghherqlsc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/ghiuglrbl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gjliceyoi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gprfzxwtz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gdjlrulub.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gesrztipp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.tarul.cn/Article/details/ghswsxeht.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsjwaniuz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gipvulgar.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/grkboqluj.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gkxoxmgim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gbgpfgqlf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gwtccwbcn.sHtML


<!-- 参考信息 -->