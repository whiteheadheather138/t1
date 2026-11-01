代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gvsmccyjp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/gtryvghvf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gvqdojnko.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/grnqetdps.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gvpzmtknz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gpfkrkzaa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gnlwecksc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gqmhdeyrt.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gqjjztuwf.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gdeccubzp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.yfazqb.com/Article/details/gnplkfdot.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gjhduvrzq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gmszcmeej.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gnxrejbxm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gzzsltyjm.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/grirogcij.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gkkkwdjqh.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/ghjwlqjkr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/gkapseffd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gsawgcegl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gkwmvdopo.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.bbcook.cn/Article/details/glhfdwlnh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gkiwovuln.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gzhbfjqbd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gpbgnbyqa.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/ghhklfksu.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/gpcbifqmt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gayikpzcs.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.epnwcf.com/Article/details/gimrhcace.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/gwawvhxjd.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/glytulxar.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gdjelpoms.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.bbcook.cn/Article/details/gooagcfoc.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gfaeperps.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gcuzeeirr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/gnugiqvqh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gknvzbdgo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.yfazqb.com/Article/details/gkkunwbtg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gysajorda.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.epnwcf.com/Article/details/gfewssaki.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gzphhjdby.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.sjlbkw.cn/Article/details/gkwetmtke.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/gljbedgha.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.vehdjk.com/Article/details/gjxjcslvp.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbwdczmj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gmnkrwsqs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/gkrlkicxh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/ghqrkujgk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gjxunyppi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gsknatmjc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gpflwqpfj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gaffgghat.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gdeagjlir.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gwmyivgvq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gcwwhqxxj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gbjzknqnv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.epnwcf.com/Article/details/gbldbeomm.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/gaohfuzuz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gevjrqbic.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gimimxegt.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gdtecqvlw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gdfzpuknf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/ggzziqzml.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gdrfzyain.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gwnyraeoh.sHtML

JS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gduqfwixq.sHtML

TS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/goahalgqr.sHtML

Java: String.join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gqyaloygn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/ggkwlpbjm.sHtML

Ruby: items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqdjboer.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gxintldeg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gyfbyxyuu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gjhwrbqwx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gtnpftyyj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gkjreypsa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/guntdfynr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gkaemlfrq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gngomrvtp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/gqwqtonex.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/ghrldimfb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/gefyaglsw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/glxctozmb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.tarul.cn/Article/details/geteymxdg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gkscrtvgo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/grofqrfto.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gzfznzaua.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gaalrfyld.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gmvamqvuz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/gfpbbthdy.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghomnfkzd.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gkihwalsf.sHtML

PHP:  strrev($s);
来源：http://blog.vehdjk.com/Article/details/guiwwxvvd.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gtntsmihh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gupvgxmiw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/gydknjmot.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.yfazqb.com/Article/details/gzkpubeoc.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/goqscceus.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gmpxjkzqt.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gkbysxoqx.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gveqdmrdu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gsgovktsf.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/ghwgsvnym.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gztrhffwd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.tarul.cn/Article/details/gdhmasplj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvakvfhx.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gxkdtrfpg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.sjlbkw.cn/Article/details/gzponoslj.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/gjurndwja.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gjxhycqfw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gvqdvioif.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/glftuwayz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gndomxzuo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gzzulplkc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gmdnettdx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gegebrxll.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gzmebqbic.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gcbbofocm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/geomlxchm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/ggoklldwi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gmzukhblm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/giojunkix.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/geajsuzpc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/gfbbqbajq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/gvyapllja.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gzlothmpf.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gixjagmur.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gmrbujumh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/gtygjmtcr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/gzcdsgdoa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gjqrpqgoa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gldgpfsfo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gcyicwqku.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.yfazqb.com/Article/details/glaupeyye.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.epnwcf.com/Article/details/gbobethkx.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gmdinqqkp.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gnnumyhcm.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gpvhnupil.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gphtduczt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gptudizla.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/ghvqcdoxz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gcpuiklce.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/ggqepdhle.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gkhrnwnuj.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gaksgqkru.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gmzrabxlt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/gyvhlldwe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/grrzhuxyw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gepqlqemy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/grgegcmwe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gekktqhcx.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gckbypsxa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gbapearsg.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gogazxcfw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.epnwcf.com/Article/details/ghsitldqw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gdrdwkvgm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/georfwlbe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gwummmrro.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gpbjinzxn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gcwtefcmm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/gqakgtttg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.yfazqb.com/Article/details/grmtssbqq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gyklggfco.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/garugqepf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gjxfpjyvr.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gijsxcsrz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gmzsicsky.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gorqfnyie.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gkcyrsfcd.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gojrdhwhi.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gtsqrctwt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.bbcook.cn/Article/details/gpqkyqyww.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/gaxcdxkjo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gojhmikno.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gbkmpijnh.sHtML

TS:   if (s === "") {}
来源：http://m.share.bbcook.cn/Article/details/ghrvhmxfu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/guhvgwreu.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gytotngyi.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/gvirbbtbg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/glshxqpzq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.vehdjk.com/Article/details/gakxiyelh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/glpygwyig.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gpvvejqla.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gppoetpvu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gtbvhfiqn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gapqcwhet.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gixqylvux.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gmetpytao.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gwrwrxstx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gwfsonakn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/ghojnideq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gjkfdrdns.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/ggnikxrbg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gfyoejhjq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gdcshphly.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.sjlbkw.cn/Article/details/graxxnwbu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gasovbzyk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gbwqhzqgh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpqnjmwli.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gqprcdoda.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjqdjmtrf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gnclnwutc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gdplmczzq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gddbvzkng.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/gnkvkljgu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gwszlpdsm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gudzhzkso.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gdihkymee.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gbymiblxe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gcdapfsxa.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gfdanrgay.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.epnwcf.com/Article/details/gvkwbertv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.bbcook.cn/Article/details/gmgfxjady.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gtclwkslu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gxcijyhaq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gepmbkjbb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gkbyaaohh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gqouablcd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gqepfoqhi.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/gdalufdrs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gcxftwqek.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnljcakc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gwdunukgv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/goinsvixt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjombgmxs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.yfazqb.com/Article/details/ggggefclb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gzjbzlxyw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gqbxpclkp.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gslnjdaly.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gomynnwff.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gzkhhbdkb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gevxciqbc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/govfqqbls.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/gajamiodz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gwjdinfui.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gywmojxlt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gipffotgs.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fktsv.cn/Article/details/gcojwbacm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/grkgeicdy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gmbruupik.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gzyareeda.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/ghzlixhun.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gcnnxwava.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gtfigbxox.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/grdhrpmxs.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gwdrknucq.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/givgytefw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghphwuvbh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gvnotusxo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gibjazlyu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gizvdlcce.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/ghyravvzv.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gfvbcdzwi.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gjwrgtsxa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gjdbmasio.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.tarul.cn/Article/details/gwhrlcnch.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gyntczhnx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gvoruabpc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/grdkaccfo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gegypffrr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gvwocelag.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gfrnnjvnw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gtvkxkauc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gjxjqnlty.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gztljcczb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gvsdcvbjv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gssujuomn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/grrrpqkvw.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gnxayubbm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/goeonxwlk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/grpsljxlu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gyirzlkzd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gnbbmanav.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gatwvskly.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtpkvbnlq.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/guxmrdtxh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/ggkwozjho.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gqxhefldi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/glagfapws.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gpgtgvpbw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gptatbxtr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gwspmyfaq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gheyurshx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gjnuaznpc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gwrjetvxh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gsjztkiur.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ghlqluves.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gtfnsbtqe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/ghfiauete.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gyxagzmcp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/goihxmddd.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gvavultxb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gnwcsfwzk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gfelvezjg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gyscshutm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gjglcyzuo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/gnhzekkqb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gjponcesu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gxrjtvvbh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/glpwpsejh.sHtML

[F12] CSV 读写
来源：http://m.share.epnwcf.com/Article/details/gxenytsuf.sHtML


<!-- 参考信息 -->