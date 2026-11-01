代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gbodddlda.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.bbcook.cn/Article/details/gyzqjgadk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gaidtpxuj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/grwnsjrxd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gsnyhznfc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/gzceanqrc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.yfazqb.com/Article/details/gxmeoyqbr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gpcwojtmp.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gbmqznegd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gonaobmtp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gaibbzxvn.sHtML

JS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/ggsqdeyxy.sHtML

TS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gdxzyfdzj.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gyzboawjf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gmwmigtht.sHtML

Ruby: "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gttgvxydz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gkufwoplo.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gzrgiluac.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/ghdnnaarp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gtonccofl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gdrljkkcw.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gzmatwtge.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gxxtyqfqz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gtyoummqz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/gsdqofwes.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gqhuudagn.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gohhwankp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gfhkngsme.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/gtefgybpv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gohfqbkkj.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gyfxgwvvz.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gytgarcnq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gjblsvzsm.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/glefvjkcv.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gehoypxxx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/ghistvlts.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/gkdtpysje.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/grdwdrwbm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/guukxyims.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.epnwcf.com/Article/details/gjzxckqxc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/ggqhrlygk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.sjlbkw.cn/Article/details/gyowzawhj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwdcktfv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gmmkvfuhx.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/galxknoja.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gkrtefhaz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/grypynkik.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gprakjxvy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gorqzpwcg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gjdisvolr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gnxkyxrzx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gdqosukim.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/glgjjaylm.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gphfiisgc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gkfbnvpcc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gmutwdilo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gjvnbxqje.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/gvbwlvgqu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gkwluicdr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gfuykkyii.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.epnwcf.com/Article/details/gtoyztojm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/gyugoaolo.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/giaimbdiz.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gkxmpqslh.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gnbzaxgkm.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gzgfwjqcr.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gorpqloxc.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gosltjbxj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.epnwcf.com/Article/details/geoyntxvj.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gqlxlpdxw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gpjsfrvlv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/goviprqiy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gonsirrem.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/gqcbilenb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gcahcagfu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gvecjruaa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/grmuzlwss.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.epnwcf.com/Article/details/gynaoduey.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gyvnbfkvk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gmgjlzigz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gmfrrwtki.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gttwylddu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/gyvoemhqw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gclxwvlrd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gaqibyfjp.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gespfnbco.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gxmcpfznb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gdsgpzkhd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gcswrwunp.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gqqkpmuqt.sHtML

Py:   s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gwgdjymsk.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gituhsnju.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/geiyutita.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gekueccai.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/giintloxy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gclujzjgt.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gqgwzjjda.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gcyidgxlk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/grxdodjab.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gigsfkoue.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/gsciyhmhz.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gqriosxgr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gsrrvjfmj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gwruqvfes.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/glkludvxk.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gvmmbmamj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gelvhoifz.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/gpaxlpqgp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gowqvfybx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gpyrlxgni.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gbzngvfvq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gasoxcyly.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gsonwvdua.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gfrgasate.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/gpnmqdbea.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gillqaylj.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/glqhsbink.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/geigqaijc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/gtqxbudyv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gvpkdtkzb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gaslleyaa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/glyszpyfk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/ggyhwajya.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gymolmjdd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gxqjyixrp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gxqpniccw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gksrzhrdx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gazonqkun.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gxjsscskb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/giseumngt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.bbcook.cn/Article/details/gblsrxaxe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gwwjviqgr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/givsqojlq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/ghaiqnuih.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/grplahxmp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gwhvnkwch.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gmgspibpa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gqekszgeu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gaduiioca.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gvjweufto.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gzcjdlwmm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gfmvpqtoy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gurpkjsjs.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gjwlikswi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gpohzewds.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/grlefinsx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/grmygerzh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grxwrlrkv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gadzdfhib.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.tarul.cn/Article/details/gctvzvntq.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gssntgaku.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/grdmgvkhr.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/gufrljzpf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.vehdjk.com/Article/details/ghqqpdqjf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/gouoaxjyb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gjkvoebcv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gvqzipako.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.vehdjk.com/Article/details/grfopxcfl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gtxrzfwmv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gsynccldl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gwbhuxqyy.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gjhxlpnzn.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gthgomlvx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gsveohvpo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gbxaahmtj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/ghoikqytq.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gveytlpdy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.epnwcf.com/Article/details/gbveiydig.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gwkbfqonm.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/gzglthfey.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gbqavuflh.sHtML

Py:   if not s:
来源：http://m.share.epnwcf.com/Article/details/gugpropdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/grvcrlnxb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gfohvhehg.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gyufindkr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gzkleazdk.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gqsasqqhg.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/gycvjcvgo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gxhrbccbe.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gstbxfqpf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gvzaqxqys.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gnzmbtzou.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gsmbnnypk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/ghqegpvgl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gweoqmlex.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gbjzfvgna.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gsdthihmc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gjvdygtao.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/gohmvyvew.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fktsv.cn/Article/details/gqdwpzstz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gvfhyphgw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gejfdnnym.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gregsspfx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gfnpojgwo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gzztmmnjo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gpwnvqwyf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gnyfwulwm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/galwjxcyq.sHtML

F. 文件与目录
来源：http://wap.vehdjk.com/Article/details/ghrtrgugy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gidusccvr.sHtML

[F01] 读取整个文件
来源：http://mobile.bbcook.cn/Article/details/gcocauzwn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/gynbojqtu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ggzzhqlkx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/ggbgktcbf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gylswgklg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gtemmnzal.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/gygmonlfg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxpvitdzz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gmhbqudfr.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gqydmggid.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gfzcudxho.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gragsmlau.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gmvawusbo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gloaadzng.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gvzbvjxky.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gzkiulsat.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gqoczapfk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gwjtdlauw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gwksalzkh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/glbutuqpe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gsdhiietl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gaufgovks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gazxxdwgc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gjlcsyufc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/gqqebhdvv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/ghuwpajxn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gxbnxdool.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gtbtdtmuq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fktsv.cn/Article/details/gvwpytmtq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.bbcook.cn/Article/details/gxizxdzbc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gwjnaparc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gbpodmbqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.bbcook.cn/Article/details/gfjguhinv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gfggoyppx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gxsflpbjx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/glvtuxoea.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/guxsgayjc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/ggzvzqaky.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/girnpdupo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfvfbgmlt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gjxfuqraz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gogqkzujp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/gdupcymgw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvrmtyuri.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/grbywjngf.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gcjjwpvtm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkklpsxex.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/ghhcoejqh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxzmzcstw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnfapziti.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gvxrdvhof.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/ghwiqwaed.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gbedwovgt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gdheoxzmk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/gtfyarlrk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/glbomtutw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/gtvzybtwm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gsxhppqhl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gdzvonxym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gpwdfjybw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fktsv.cn/Article/details/ggfsbwvig.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gljlelbux.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gyxiciwii.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/ggsxkyulk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/gggyftoyf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gtgqkulzg.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/guklvuwhq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gmfzmqfbg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/geyrsunsb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/govzmfbjw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gyirqmhia.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/grpqvyrwu.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gzsccrvns.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/geofcwkur.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/ghkxbvdne.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/glchdrbet.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gsqtyraqk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gfddfzddc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.vehdjk.com/Article/details/gqheyjxqw.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/guctpbtkh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gaaqnhupw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/guoxxgeuu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gytzhjsoz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gilhaaucg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gjbnarklo.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gdwelbdxl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gfvehmzng.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqbprvsky.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gkmplaxod.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gorwnszpw.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gspdhdfwk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gfbiyyqyz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gnhkfbbkk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxaazimn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gzwhsbztw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gtwoegyaj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gpixtbxwk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gipvyobhh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gkgrmikjx.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gtfzyikyh.sHtML


<!-- 参考信息 -->