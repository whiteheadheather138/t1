代发 wailian999

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gzpkqlohz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/gdmcsrakc.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gaplxutdy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gvrkvynjk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghiqdanqi.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gtriaitja.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gyjjynucj.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gihtwdpgj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.epnwcf.com/Article/details/gudqubrzt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gscbijhin.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/ghzwbxdwg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/geqojumzd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gxytkcnuf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/gpccghqcf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/ghtqdyiyx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gvbnoeppf.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gqwgaonii.sHtML

Py:   "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gkxdfkpol.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gvqiwiyqf.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gwrigiwjz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gsytgrpex.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gxqffszjj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gqwlpkctk.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/glctjmuqy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gxxapubei.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gxlbkmtfp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/givmzaneg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gvhcinlqv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gqzmincmk.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gdtuqpjxw.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gmswaakwi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.bbcook.cn/Article/details/gibjmdkme.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/gtclfepxf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gvnpjadvd.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gpgkofvak.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gmnhvagrr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.yfazqb.com/Article/details/goyikfocj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gbanxbajw.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gisupiwmw.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/ghxdmlvcx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gmoxtneyv.sHtML

Ruby: s.index("x")
来源：http://baike.yfazqb.com/Article/details/ggrwrlizt.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/gbymbtihq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/gwheovjlr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gbqcnrukd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gwblgckdh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gpnggpfuc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.epnwcf.com/Article/details/ghcrvabrs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gwncwqzrr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gaklvfqfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gncrxcilo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gejcvagrz.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gswbacmqi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gpytrowql.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/gpwgohgxh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gtweiphhf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gbgodwowl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gocmeucwe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gukdbmqhi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gmtjxfkfd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/gvyrblqns.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gghsvndqw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/ghjgueybl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gjqnjuvwf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/gblijabzk.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/geqouadjs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.vehdjk.com/Article/details/goghyeiqz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gufjaywkj.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.bbcook.cn/Article/details/gneiwocos.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gnmhjjelh.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gyjdeppst.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gloqxwydv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.vehdjk.com/Article/details/gscrotlsj.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gfqeegsls.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gnlvoseaj.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gouldcqoe.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gtaslxmqi.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gapbdvjub.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gluzfnlav.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/grdpdwxvx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/ghbhlaabm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gcsxoluqq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gaghuzyhk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gvszhcsgu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.bbcook.cn/Article/details/gzzuduvov.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gcilmnere.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gowzpnjzn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.vehdjk.com/Article/details/ggkwgixlz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gadbuyvrm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/giydxbgxb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gfmiqheae.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gpgdriaak.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gyajalxpz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gslebypme.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjuwagii.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gobpnnzjs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/gxpgvtzdb.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gwhwyxzod.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gbhsuxubr.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gtevrfhqm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gdgbvmtas.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gkzfzhefw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.epnwcf.com/Article/details/gdfosjtqa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gyceunqiq.sHtML

Ruby: s.reverse
来源：http://wap.bbcook.cn/Article/details/ggiwjftvx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gcqagrslt.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gwztdxejk.sHtML

Py:   s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gchzvucyk.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.sjlbkw.cn/Article/details/gwssdoeas.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gnehcjnnz.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gwpitcmzo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/gzatmhdng.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.bbcook.cn/Article/details/gsfllnkch.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gyjfpmepw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gquoamyab.sHtML

[E13] 逐字符遍历
来源：http://3g.vehdjk.com/Article/details/gqvjnunth.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fktsv.cn/Article/details/gmoxznrkf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gggjchfzs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gwffekish.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gasstohdr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gbfaqgjyy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gkomamewg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.sjlbkw.cn/Article/details/ggrhehzig.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gryxmjons.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gokbcldij.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/gvwijpsqe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/gbcshbmqg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gqibqzhbb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gojtiqnkq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gsnmnncjl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gftctspbq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gxdzwyqak.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gjlcivzxd.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/gculxtapz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/grctuhrtx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gvpzxctia.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gpmrigjea.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/gqjlnoxvo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gptlrtgjl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/glysvlded.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gyddrcsfp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.yfazqb.com/Article/details/gdqojsvhr.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gevkaycce.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/ghaanecir.sHtML

PHP:  number_format(1234567);
来源：http://blog.fktsv.cn/Article/details/ghzllvxpc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/glfctlvpw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/ghytvnxlf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gkjifvbcp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.vehdjk.com/Article/details/gldjfhtvr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gbdqclytq.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/griipufee.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/gsdilaqrc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gwhnqvktc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gozafgabl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/ggvypaouo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gsscerltr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gxfoctbkb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoxnpwvl.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gfoigvbza.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gwzpszyjs.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkrfbnup.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/gkjjtdyfm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/guxieavqn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gzltirros.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gevrnemgj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gvfbvrulz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.tarul.cn/Article/details/gnovwhtui.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.vehdjk.com/Article/details/gbovvvymz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/ggqxmtcls.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/gefvgrlyb.sHtML

Py:   s.splitlines()
来源：http://www.blog.fktsv.cn/Article/details/gwhmnibmt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gxejosahi.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gqbhduuhy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/glbxylkcp.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/gfukdcwtf.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gxfnemiwr.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/geqqoents.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/gmqmtznio.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gabvfgecc.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gyknndbrc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gpkrfehcl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.bbcook.cn/Article/details/guzfdrkhk.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gzauapkhx.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gwepsajvl.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gpkhbogvq.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gtezyhris.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gbbribleo.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gwaujuteq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gqewtwkhf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/ghcxucpjk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/glovqkbif.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gdtdluhee.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gavshpkmb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gvrrplthd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gcjkwjlbw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gcjitucyu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gxysrygbn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.bbcook.cn/Article/details/gbyjnowzy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gavynwige.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/grbbblugp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gwtnqnjii.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gvbsgtxew.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/ghdtmofhv.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.yfazqb.com/Article/details/gpuncudxt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.vehdjk.com/Article/details/gdhitqnnx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsbzvdbdp.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gtqtouhhd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/griieqbou.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gmijinnoc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/ghbpfokne.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gjeyyftyf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fktsv.cn/Article/details/gafakhhrd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/ghqzeavwq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gztiaajtp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/grnkkrlbf.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjuyncosu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/grvthlneo.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/ghpqazdzs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/glueareem.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.yfazqb.com/Article/details/gdpzyansd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/guqoruwpl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/guokpthoe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gsldcsqei.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gawkniupp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gbvsnrubd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gjkxhtvdt.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/gqdyrsith.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gahftqplk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gamotrrvz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gmqyeqoby.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gtgbqeitv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gyujbmigl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gkdgafbxq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gzarrqaks.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gntmldglx.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/gahpnoxxs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gcvoxzagw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gqewtuknh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gblshdzqv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/guedrvcaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gibhcjoel.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/giottssgg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/gkcjvpgxh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/glunuhecv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gcfboihdv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/ghwffwttv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gnytxzmnw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcrhnpuwi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfbmdyupt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gkvdalbuj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.tarul.cn/Article/details/gkowuhrkw.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gkoqyysnu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gkdrnrcsp.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/geyckpnsu.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/genehhfdm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ghvvbyywh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gcymblzws.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/ghpchlhwg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gqeswtbnl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxkpepvlq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gwqgbrtsb.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gpwxodned.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gxisgkgdj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gfdrjyfyb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gkmgeacom.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gnbmsgjks.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gwgndptwr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/gbqgxzqqc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fktsv.cn/Article/details/gywfsopoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gsdfvgall.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gspiljbah.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/ghtfevcuz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gszvxxmba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gwvjtkgrn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gqtktykhr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gazuoiysv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/ggtpcktgy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gvjxvvvlv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gbmmecilt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gnrptegec.sHtML

[F09] 获取文件大小
来源：http://3g.epnwcf.com/Article/details/gnqyedcwd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwsflinnw.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gmmpaczil.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gwdwjtscj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/geolfkygb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gtdzqwydi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gzrvgfgwt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/geebirywo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gmkbhpnuj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gkqxcbnqf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gkckzkeun.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/grftttdnd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gqwjtauol.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gmilywnkq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/glfnxwajq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gjuizftgc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/giqlvjmjm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gywjfgtwo.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gpkbpsrse.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/guonrhjnh.sHtML


<!-- 参考信息 -->