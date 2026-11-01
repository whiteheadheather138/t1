代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gohriegte.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gyouhuvjg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/guelkrvpy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gmyynkmta.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gdvfmzyib.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gefuvpixv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fktsv.cn/Article/details/guvursnhy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gicfuvlzd.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/giafrjztw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gpbwhnhfo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gcclflzix.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gyovywwod.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/giudzmiin.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gdkicnhgk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gtdrnvvfj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gkpshemlz.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/glmhlnujh.sHtML

[E07] 按分隔符拆分
来源：http://3g.sjlbkw.cn/Article/details/gnyrstaff.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gblrgeqrc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.tarul.cn/Article/details/gnfcxnwqs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.yfazqb.com/Article/details/glbcbkqrp.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/ghtytkmnh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gmebdetkr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/goimyodar.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/guluweuzo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/guzvlpsll.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/ghaboeoim.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gnubikszc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.yfazqb.com/Article/details/grqwvcdnr.sHtML

JS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gotxabhmz.sHtML

TS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gjwoojsaf.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/ghautsucv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.bbcook.cn/Article/details/grslbzjev.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gppvvzjor.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gryzpznyt.sHtML

[E09] 去除所有空白字符
来源：http://blog.fktsv.cn/Article/details/gzptnyhfa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gaqjfniys.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/greofuazq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gywiuoodh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/grizyvmwe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/glubzxepw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/ggomoihzv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/gnfafettl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gxvlerfnv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/geepxjtfy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.yfazqb.com/Article/details/ggijqjutu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/giwxqgntj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gupkjuvvz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gwloaylen.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/grqoplawg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gabuaheyl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gekazfxaa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/grnqeadeh.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/gcwqniedb.sHtML

Py:   s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gtprkzwhl.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/ggarznzlr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gfwsdtfou.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/glnsjvzct.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gmtznowbu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gphqjolrh.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gopjkyqmk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gwamlpgit.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/ghsbdlzol.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/ggpkartka.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/ginrwbgbn.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmgniypb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gbawwmneu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gptcvprtr.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gvptiycqc.sHtML

Ruby: s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gvkenejhm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/grjjhteel.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/guqtdjlzc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gguwqfogo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/gjoglsufn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gifivaruz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gutcmcldz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gafghupwk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gcodbishh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gwacwmryt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/gybwzxfnf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gransyvwj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/grfdgnavh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gencffvoy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gkyadzfaf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/glpvjpkov.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/ghxgqikru.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gvmjujvts.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.yfazqb.com/Article/details/gsxbamnly.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gbovstlzz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gcndnkuur.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gbwinbrem.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gagtqghsc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/gaktgwsup.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gsfqpwyer.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/gxhwwxdcd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gbrnipmps.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gynwbddko.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gzscaztft.sHtML

[E16] 数字千分位
来源：http://baike.tarul.cn/Article/details/gnhumbklb.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fktsv.cn/Article/details/gwbskszzk.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gdzjjkdzm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gwysusyvv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gqizpbvje.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gjxrpmwrv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlzubqwt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gspjinjqd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/geyjffwdr.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gtismsszh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gueilsqci.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gitrtamti.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gkckihdot.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gheeikekv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gdppxggxk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gomwobdkr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gcxyrgpsq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gjukhrjtf.sHtML

[E18] 模板占位符替换
来源：http://mobile.yfazqb.com/Article/details/geadlrjky.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/guxxrqinh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gybkedtov.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/ggabagqzo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/ghtoinovw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/glthcrrmu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gtcmyepwd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gnephtwan.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gbxeybqku.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/gxetastcq.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gsbekkumi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gnhgiuwgh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/ghhboltbj.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/glqpiumyn.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/gigamflvh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/golxklksp.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gallzngrh.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/gxsqblonz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gtyrajwwh.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gecovgfxy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/gcqrdblmo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/geuqufppd.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gtvasjglf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwarbsloh.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gsjlssqzr.sHtML

Ruby: if s.empty?
来源：http://mobile.vehdjk.com/Article/details/gdwclsech.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fktsv.cn/Article/details/gczxlarnd.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gzwatqkrl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/ggcpszbnr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gjtunvbxi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/giiipgnnv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gehdhwmvb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gxonznelk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gakgtlrfb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gaeeoptpm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gymdoyqby.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gmxbelack.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gjfiqnmub.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/glwivjntq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gokrfeaoq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/ghnssffah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.yfazqb.com/Article/details/gomlaculr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.bbcook.cn/Article/details/gjbmshlyh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/guxbimbel.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gvnwahlcx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzyyhynaq.sHtML

F. 文件与目录
来源：http://www.share.epnwcf.com/Article/details/gjlfoweir.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmsdszsxl.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gmwmsdxjq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.bbcook.cn/Article/details/gjsbwuzza.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gcwaenmnc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gmlrccxas.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/geyxaqhbx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gtelnsoof.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gfbkeakjb.sHtML

Ruby: File.read("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbvskzhpe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gpajrgbzi.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gcobsefcc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gfsqkgokr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/gxpesmgfe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gvtctarsk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/glhojbqzg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gtciyjuaj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gtuirrpwn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/ggtgwxnfd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gzywlqdwv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/guldhvzgt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/gzoqwhhhq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gfgmjfzke.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gewosbsfs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gqxlvqswo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gusdjqxme.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gsmwcvbwp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gblwcvhrr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gwmxsykab.sHtML

[F04] 追加写入文件
来源：http://3g.vehdjk.com/Article/details/gcmzbwitl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gpzthbpzs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gnyofhvij.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gqxqhvusp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/glxqomwmd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gsakpclyz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gqiqgocyq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/gzvicjbko.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/gqnlzjgil.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gwraalhwk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gkalidhwl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gqhmmtdak.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gkcnedian.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gpabrnnnm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gjcbigova.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gteytosrg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzrclrruo.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/grkrzclgi.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gufuxagmm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gdsknswrg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gcwoetwdi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gtybprwyc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnjyvwpge.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/grcqypqhj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gonadxvya.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqindvpho.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gnepturhf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/geepvwold.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/givvixupr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gezlrwciy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gxviojhew.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gqtnjfina.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gzhfhwbuc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/gpldvrkjj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgkafztb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gopvclqjx.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/goknsbthp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/ghvkbvuko.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gzkyoupfy.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/golxpaygv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gormsknlz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gipbrxqej.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/giqpuqhaq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/gvwwnzrir.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gxtkjkczc.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gqwtrkzrf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gyhplcfkq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gboeesbct.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gjctpecxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gbomtzawb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gelkqqzwd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/ghokzclou.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmxhbqrcs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gnejagbxj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/gloumjxdp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghcthnrex.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/ghbysgutv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghslwvdlh.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gevhhighf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fktsv.cn/Article/details/gxcdjyntc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gydejvrwb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/grdvmtgfu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gqzfluonu.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gtexuxpkw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gkmeuvnuw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gxlzrvvyo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gyipdywzo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gsrcpkows.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fktsv.cn/Article/details/gevxdxzht.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gvdaxgzgo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gzmfuzpji.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/gzinainba.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/gdzzcsugs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.sjlbkw.cn/Article/details/gfbteoqhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gclbucosf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gmermeusj.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/guxwqanhg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gizbrgbkm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gyshfszev.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gyxucykre.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fktsv.cn/Article/details/gdlmxbyez.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghiowkryb.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/ghhtkbrex.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/greskajne.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gybkvpvym.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/gbnowivgy.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gqmihueeo.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gmaooqgbo.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/ghyzasvdt.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gmrfcwhmh.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/gwxnefytl.sHtML

Ruby: class User; end
来源：http://3g.tarul.cn/Article/details/gtudqbedb.sHtML

C#:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuvdayiq.sHtML

[G02] 构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gndsoyzhv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/givztexij.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/gjthctequ.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzboascjx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/ggprfmbvg.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gwrczagmv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gdahrgetn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gwyrhwgql.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gzfwlaebx.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/ghfnxaxwv.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/gcoeksqag.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/griwiaujg.sHtML

JS:   this.name = "x";
来源：http://wap.yfazqb.com/Article/details/gbqvrunvr.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gswivdtqq.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gpkzyuxzg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gooyqiztj.sHtML


<!-- 参考信息 -->