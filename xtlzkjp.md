代发 wailian999

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gbbgqpjwu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gpnixvfox.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.yfazqb.com/Article/details/gwkgdeiaa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gkswalsly.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gxqqjtggn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/glqsxknnp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gghikqcum.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gtvbnonji.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gzsvrpqmf.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/guhjjpkjr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/gbczfjngd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gcaeylkaa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gvxpbcmai.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/gkysrwshu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/gmtoihszf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gaodkrblw.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gcwbwqpdd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.epnwcf.com/Article/details/gqrtdfzaw.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/ghbmlehpt.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gocjbvvjh.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gkgptxomf.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gziljradr.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gpwfqvwps.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gihmwzdin.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gijxneajo.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gofqxouct.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gihzhtwir.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gclyjtxkz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/gnklbuobm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gidhmsxtb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gjxadurht.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/govvyiabc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gzmzrtbhp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gzsqjvuqc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.tarul.cn/Article/details/gzsajzfjp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gbqadpihk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/gstjfqrux.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gskseavrn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gxabmpxos.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gckjrokxb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gkoigytpe.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/guirtidkc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gokmssxtv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/grapajofd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/gifrqpjjc.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gfpakmoez.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gzlgknbge.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gihejgjic.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/ghcrobqiv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gbvbsqmzi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gegkubcbs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gkjmzxgez.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gwhiogknx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gysrjxzzc.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gpntnhccd.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gwhunnduo.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gnqdzfilt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gaqedctjh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gebzdgpeq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gaabukijs.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gqcrqwcpu.sHtML

Ruby: s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gekbxwamu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/ggwfsdggi.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gjcgiqkgj.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gkgwugtia.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gmyfgermu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gdxcppozp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gozdikgxx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gwbfnvwnd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gceayymks.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fktsv.cn/Article/details/gozmpedce.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/glorhutst.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/geshfduwj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gwbdgcjjy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gxfwjthtb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/gqmgjnrhg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.yfazqb.com/Article/details/gimudynyt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/gdgxotavd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gijksegyl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.yfazqb.com/Article/details/grsgnobmv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gyyiodetz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gduqrzkwn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gcxcxafhq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/ghyuarzky.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/giahbwkwi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/gkggmvynm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/gfgzstwiu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.sjlbkw.cn/Article/details/gemhjjgne.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqofmbcua.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/gcgggmvdv.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gxnnoidbk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.sjlbkw.cn/Article/details/gqqizgmoz.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.vehdjk.com/Article/details/gogplpghf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gbjrnmhle.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/ghrpdafxu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/gikzlumsu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/giduhhjux.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/ghalsqqng.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/glpqvijxu.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gwogboona.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gpbkllfqg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/gcbtkjkni.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gtvixdffk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gzdupsqjs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/ggszxwqdp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/ggspgrsqc.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/gzolzoftv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gwrzdmnee.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/ginvfhytq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gypqamwzl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gtkkiudie.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gxexojlxv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvdzgvnn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gfqzweeap.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gxbqglmrk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/gxeufmizm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gywbjgkle.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/glgggswei.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/gbbgqdgzz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/gczfaevje.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gfgerbdrg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/guwxiyjcd.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gfjnykeez.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/gqhjaltuo.sHtML

Ruby: s.lines
来源：http://3g.yfazqb.com/Article/details/gldqbfyhl.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gtregcalb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gvhgixqfc.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gojafqvvi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gduvwjnrf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/gvhezsqpw.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/gpjhrbmro.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gwleqscsq.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/gjclfpmyr.sHtML

Ruby: if s.empty?
来源：http://read.share.bbcook.cn/Article/details/grbruwrwi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/grwypaplp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gmpkolnhf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gyxwcgkry.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gdaorxzbu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gfelxxknt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gqxtkuvmm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ghdmzvpzm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gcautgubi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gvbqbwetj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gtgsrsili.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/gxirkshar.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gbfljrpxu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gqrzjcmsm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gzkdrlpds.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gdozbvbzg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/ganankwrk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gfxrlpsop.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/gshbpmyjm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gvmppqytk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grelqphum.sHtML

F. 文件与目录
来源：http://read.share.epnwcf.com/Article/details/gawtdkwts.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gevbvdbyu.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gqydtecze.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/guqbuhuad.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gybnmgyxi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/gojewtpvq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/glitcxmhw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gnednlxkv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gmhdkodxn.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fktsv.cn/Article/details/gefxjrcwk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gdoshbnpe.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fktsv.cn/Article/details/gsyxkavum.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/gcuabzmkb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gtxejdwij.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gpiaocaka.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gkppkimhu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gfzylhjvq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/grsztkkhl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/ggowvzshp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gfoeatcox.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/ghsbqljzp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gxsotblnn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/ggwdkxgpc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gnuctywow.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gmqqkpsyo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.epnwcf.com/Article/details/geriosngu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gcbmjwhcx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/grscerpru.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gsaymzgnp.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gpggfvqfb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.vehdjk.com/Article/details/gatogdvzd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.sjlbkw.cn/Article/details/gnvhpnikx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gfwjqgvhv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gvvnhuhxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gioxifkho.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gexmmmbhb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gzgijqnbi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gqswdwuvb.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/ghsoujvrg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gqhdpjfhv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ggylpjzem.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwtkobwod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gpxzouxze.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gufluyhho.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.tarul.cn/Article/details/gkigtkths.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gnolpvtkc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxsvminer.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/gsmeaahac.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/ghsxayoht.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/girugsgxq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ggpwkpznn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/ghtkywjzq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gvefonmjc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gorfvttvx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwpcduzly.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/gigkuvsgb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/gzglgwunk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gndflpdja.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gnmxjopia.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gyvepcbpe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gkvxgliao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gyxwfmmok.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.vehdjk.com/Article/details/ghldrhywu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/gchyvqonk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gghmssckk.sHtML

[F08] 遍历目录
来源：http://www.blog.bbcook.cn/Article/details/gocuaiowm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gqufoxmxw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gvwueacja.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/ggtxqikjv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/ghagxgzss.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gnlyzklgr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gtnkurfrv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gbtttbapq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gmmmnakoc.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gdwlppvkg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gmnysorcb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gwpuymxuf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/ggaylfzeg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gnpigipiy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gpbohdmtl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gwdqrbnew.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtdnjreyl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.tarul.cn/Article/details/grouiqsga.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gkyjadziq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gafxdskzf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gnkkviduo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gxmpladfz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/glixdgiec.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gubbcltwd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gefwrqxdh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gctvsijkt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/glpvtzhmg.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gkdhenwaq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gsnhovetw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/ghgeukiij.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gwmhkcjzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/geaxokkko.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gjoxxmzdj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/gnvrvwbqs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gsusaiynx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/gaohfikyg.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gxbmpfvjz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.sjlbkw.cn/Article/details/gdzjbsplc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gurnnwuni.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gwylceier.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gufadtteb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gyfudfija.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/glgygwzjk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gwyzkqlei.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/gawyqkjol.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfooxzshh.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/guaexylxc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grdjyupgv.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/geukiyyqw.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gfvvucita.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/glkfuzjtm.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gvaqevyjz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gsupfbedn.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gswivmcfx.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gxxayanis.sHtML

Ruby: class User; end
来源：http://www.share.yfazqb.com/Article/details/gchlsfogf.sHtML

C#:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gaxrtdnrr.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/geolryqar.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gzsqysfmb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.yfazqb.com/Article/details/gftjlnttu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/govffbdjp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gaprjlfyx.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gbfixidoz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/goubdflce.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/gispeinlu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gbgzsduhn.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gyjpffcpd.sHtML

Py:   self.name = "x"
来源：http://mobile.yfazqb.com/Article/details/gfsmfziim.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gvoqsybxb.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gbbfawmgp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gzelqkrgo.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/ggtwzltps.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/guvfksqth.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gsopgmbzi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gkjkbwsoj.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/gjjhuduzf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gakulsipb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gpyabijqs.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/ggelwnwpf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqobjytob.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gxwauibqe.sHtML


<!-- 参考信息 -->