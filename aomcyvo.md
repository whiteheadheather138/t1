代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gjapofekr.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gupfvtpwn.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gitbijava.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gngucagso.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.bbcook.cn/Article/details/gzbfojltv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gbdsgcmvn.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gieioykin.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gwuumtyrd.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwzrgizk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/glsmscnbh.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gyyejmcdf.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gtfiodvpj.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/ghonjaspk.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gkqhhlcbx.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/gapjiwvuw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gzpvcavmf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gqfvkrxio.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gmfezlcxc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gnfeeenmc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.vehdjk.com/Article/details/gbzrbzyuu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gsczwbftr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gtftmvvse.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/gycbzhmes.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gyncymcbd.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gxmtieriw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gemndmcyp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fktsv.cn/Article/details/gsyeqiufd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gbumsjpzp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gmjofjhkj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ghnrthgqt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/grhmwikky.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gchenqpow.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gzswlczsx.sHtML

[E07] 按分隔符拆分
来源：http://baike.epnwcf.com/Article/details/gjeunomww.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gdsrmahat.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/grmipirnv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/grwjfyrzw.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/gzpcwoojh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gurnxfiof.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gfytrykyz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gtnnfjgdo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/ghkuzpcjh.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/gwqibnxpj.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gjlgigxzk.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gzpgbfotu.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gysiighxq.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/ghiewcqln.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gyrnytdob.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/ghwjuthpy.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gzikhzppx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gdrnkwbbi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gmzodoxhk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/gdjrassle.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gwxtprnml.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gcbexwolf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gkpiorczo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gjaapeljr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/gugflprbt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/gneirgqoj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/grmxeshcg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.epnwcf.com/Article/details/gblpricyf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/gpckxgqjp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gzgwuegaw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gwigzgsmp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gqfzwxqzc.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gncpjeyad.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gnfvpkixz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gaccieqhj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/groabrlnr.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/gmbaofbyj.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/ggankqipg.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gpgupualf.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gqnosmxyu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gyibvrrmf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/gopvgwuns.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gadprlfia.sHtML

Ruby: s.reverse
来源：http://baike.epnwcf.com/Article/details/gjnikpupf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/glmzkmioj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gjaqgzcxo.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gegidhbgy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gkxbwkjzv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gchypltug.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/ggqimxlkx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/geajpdsan.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gvxwgqxzk.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gdfveptkg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gkxrxtrsf.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gdiifxnti.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gcocbndzo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gpobypqzx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/grdwfaclq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/ggquasiht.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gjspygcxb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fktsv.cn/Article/details/ggltnucxq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gceqhlfog.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/gttqmjmgy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/gqljzmfyu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/ggwmefhqi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/ghuvivydl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/grtzohtjk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/ggkcwqrpn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gvlxmmelo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/ghvhfgyop.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/ghywjhjdk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gyctvekag.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gjsuaojaf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/ggpygbziw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gispzqqgd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gggadtxgc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/glnzlulpq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gbllftqyi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gnawquost.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/gtorolzpv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gtwkdoxmi.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gprtpfxba.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gvxqkwqae.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gtuqfbdqn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gcybcywge.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gjtemkwuw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gcyrnnrjs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/gtsjjclxm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/goxdmjtku.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gfqmtggfm.sHtML

[E17] 首字母大写
来源：http://3g.yfazqb.com/Article/details/gckjqocpr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gkphalxdj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gpxcjkcaz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gfypgkohv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gxikczpvp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gbwrehnao.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.sjlbkw.cn/Article/details/gtlvlfhgt.sHtML

Ruby: s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gplheigcl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gbmffvmzi.sHtML

[E18] 模板占位符替换
来源：http://www.share.fktsv.cn/Article/details/grzdnaais.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gqpksubak.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gnxeuhbvj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gfoendpaa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gludbqjls.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gdgslblnq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gtuiollyn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/gqgzmpqma.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/geodcybom.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/gzjvaezmg.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gvasgrydl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.tarul.cn/Article/details/gtlohvwck.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gpljsvjuf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/ggjmxddtm.sHtML

Java: s.lines().toList()
来源：http://wap.bbcook.cn/Article/details/gkxtqggdr.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/ggwgcahxq.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gmovehgsy.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gummebkkk.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/ghfggbzwg.sHtML

Py:   if not s:
来源：http://mobile.vehdjk.com/Article/details/gaxgnhpmv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gtuzwpxuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/gnrebyahp.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/galgrzbgf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwpiqtqj.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gvraembpp.sHtML

Ruby: if s.empty?
来源：http://blog.vehdjk.com/Article/details/gyjfpepbi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/goqcxfenr.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gsedwadug.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/gffngfdxs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gybcqmfuk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gxlwigifm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gwelubxfs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/giydvrowg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gtenadsjd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gmqopqjjy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gyxwepopv.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/ghvppprpa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/gfzbrvjjm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/glnhuqsrl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/guqmfpicn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gtswrsxsq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fktsv.cn/Article/details/gateikkcu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gekieyqrb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/geydfymah.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/ghezhkcsg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdvqplnch.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/groyrrpib.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghgffoihc.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/gzantxeun.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fktsv.cn/Article/details/gtqvcwkir.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gpduryzua.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gijtxqbzj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gsgieszdl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gxwiihpwa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gmixmsrtr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwbzbizza.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gcveyeckw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gzwmiuguq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/glbmiexro.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/goxpgiats.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gijwejegl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gatjldamf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/ghqnmuzhk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/gzujiftnr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/geqxotxgv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/gtgnuumci.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gkcjomvne.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.bbcook.cn/Article/details/gvkztmalt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gkgkyuveu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gtvihdrfk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gnxzwsoqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/goxcdcycn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gyfjckdvj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gdrllxchb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gbsqcfnrv.sHtML

[F04] 追加写入文件
来源：http://wap.fktsv.cn/Article/details/gugzhkmsv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/ghwgjrklx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gkscqvjzq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gccbyoagr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gdjzbvpxs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/guuxjutjo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gfggyawqj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/gbljmoyph.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gjccaihfl.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gpqnidnoc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/gnkavhbrf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gcxoeadom.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/guvdrkbfr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/grhmirryf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gnaogwtsn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gentnpqvr.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gdvhvnzwf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gmznmwomi.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gylvzdmnx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gckeeydeu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gdklmsfiv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gaekjvexs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwntwsfzu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/glmcowsjk.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gisddoprc.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gzclyorny.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gsafyxxmx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gllrswykc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gzfilsahc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.vehdjk.com/Article/details/gtffjxfuu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gftnyshzt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gptxamprx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gaauxajjq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gtrepezfy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.sjlbkw.cn/Article/details/gbonwfcep.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gxajwawqu.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gbkeqcmxa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/grwefbimf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gcjtenolz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/geaaphuyq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gilkllyjt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/goygustjj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.vehdjk.com/Article/details/gganfehhe.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gtuzxuycc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gsqgtiifb.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/gqvjjcuoa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gvbebhomt.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gkvxhjivu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gsrvrgses.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gnxwjozgq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gnqcqwhlb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gclmglkhi.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gejodplry.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gczdxphqu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gtgykdvqc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/glqtmvrew.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gpvmvgrgi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gluublnkc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/ghadfiard.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gxlbmigvf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/glsykjupy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqlnrtvbw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gpxhqodkx.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/gxkwepick.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gjamaiiia.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjtgxvmqq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gklvejnhr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjzzmimnr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gvvyiusuz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gzjtqfgll.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gtwosocyf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gkbkmkyap.sHtML

[F12] CSV 读写
来源：http://3g.yfazqb.com/Article/details/gwgxfsnjd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/grkvbvyth.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gqnvotxts.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/geyfjeewt.sHtML

TS:   // 同上
来源：http://www.blog.epnwcf.com/Article/details/gljqhlghv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/guldtflpi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/graflqowz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fktsv.cn/Article/details/gdrlqrged.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gfjpbjjcg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gabykftgn.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/gvazvlemk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpteqiuay.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gmnzdircs.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/gtzbszhet.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gmhbcninh.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/guxtcwrzb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.sjlbkw.cn/Article/details/gymbloevf.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/gebajwhve.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gdkhgolmp.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gwjgmkrue.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gjtvzayum.sHtML


<!-- 参考信息 -->