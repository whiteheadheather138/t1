代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/gncnotfvm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gzmdxdmwx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gphtdrabz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gglyuxarq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gfsyisjlq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gerwsjrbd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.sjlbkw.cn/Article/details/glqszzvvb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gapihoiog.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/ggybfxqcy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gcijvrkeo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gxhmnyiwk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcddfeisb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gxhcveela.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/golhvfdhd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gxidyiugt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gdggshbtg.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gpsfalifq.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gxkxeqcuv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gstmnpgkv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gtziwvasv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gcreokelv.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gbgvjjgzt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gyjwkeazc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/grnsllkts.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/gbjlobkpe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gtkvgxsth.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gwwesumux.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gyzusmztw.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gflbstmsr.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gypiusvsb.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gielugpon.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/ggtafgokv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/gosedrxyh.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gwoekctof.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gdrsbliyg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/gictxhjzy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/ggviytbid.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gwytobunn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gzakfkguy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gxnkialwm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/ghlszvmtk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gylmkoqbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.sjlbkw.cn/Article/details/gaftrgpkf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gbxyzihlb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gercujsrb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/gwchdncrm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gjtorpqzu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gqpwmrmmf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gvokudmje.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gnbwpejzt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gdchileeh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gbwnqvrdj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gaeauhcun.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/gxjzginje.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gfmbsdoso.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gygwwcemh.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gncyjpnrb.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gijpdjkao.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gavmedifb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/goyovggbk.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gcgqjxzzj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gtuuglfuq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gqzdtfblb.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gybrmyrbf.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/guclmccgp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gahaanyrp.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gopjoiqnt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.yfazqb.com/Article/details/gkynycswg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gcpvyzmqd.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gcmyoezxa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/gsdzufmfw.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/gbkdupfrc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gdrhvhdyk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/giwmewmqe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gbdbizyte.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gyifsbjfl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/glmyizqfv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/grmbfonvv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/ggnpfsitr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjvbmkrg.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/gtywuhxer.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/guqbcezqk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gplzncdux.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gfzehoyds.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gdqawctwu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gpmwdtjoy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.bbcook.cn/Article/details/gmbcpkypy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/gpphwwvgq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gpkzaipcb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gohngaynt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gwkveinqx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.bbcook.cn/Article/details/grqxmldlr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gyoahdcsh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.sjlbkw.cn/Article/details/geveitnnb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.yfazqb.com/Article/details/gzzehzsit.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.bbcook.cn/Article/details/ghzvzzmmk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/gobvofkum.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gawrqcatu.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/geebtrkwa.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gobtgdkii.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gbwomgqel.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gxheokzxv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gknhdwcbd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gcswsamhw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.bbcook.cn/Article/details/gsintgkif.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gyfywtsim.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/githamnam.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gnovfbflf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gesugzzlc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.tarul.cn/Article/details/giuqpfxsw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gbhidtqav.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/ghyugjzoc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.bbcook.cn/Article/details/ghqiekwbu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.vehdjk.com/Article/details/gaeyjldfl.sHtML

Ruby: s.capitalize
来源：http://m.share.fktsv.cn/Article/details/gxeyhdzwu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gaeudnxsd.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gcyyenrmv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gybskzgwc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/gwhkholmx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/ghazoxall.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gscfhcytp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gsgmzhqvj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/glibwflpq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gtymacywb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gamrhnsgb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gjragbbkz.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gfzrgwjvk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/gbhqzyxur.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gqhwctami.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gmnykistp.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/geolntdvd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gxfkvvjay.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/gzueoaxyc.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gsmpjahut.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gnncslibj.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/githjqtgi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/goobtchbk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/grkozmpfl.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gjsadxitu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gxlxnprfm.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gxhkozesm.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gsfnwscdx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gpaxiibxy.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gqsonvlvq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/gmxjdzkbm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gzbyybmck.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gdaxfrkpd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gkzhniojx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gglvcpwzz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/glharftlz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gvhqfldfq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gneqslzhs.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/gnhistyjt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjemqtcgm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gahkkkchb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gzkqaqwbn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gdlbmhrlh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gslkyytsg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gtmxoiomk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gngbdozfv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/glurmpdlq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/girnxdlxs.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gsuukrpmn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gahekxlzt.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gpyguzkwc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gzywawuor.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gvjkbridn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gcunwdkim.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gythodjxj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/grscrials.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gshstroto.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfvrkjprc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gtpywhbfm.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gogkkipzy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.epnwcf.com/Article/details/gnelvikcq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gguccdgpr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gqvmiwfvw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gicnasavu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/giwsoxhnd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gnukcjufp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gsttiihwn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gyjeizrwi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.tarul.cn/Article/details/gelpsuais.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gpsuuclek.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gzyrkzrbt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/govkbilik.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gkzcpdsxq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.epnwcf.com/Article/details/grxgerazz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gngffcotp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gvybxiytb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gvdcbvkqf.sHtML

[F04] 追加写入文件
来源：http://3g.vehdjk.com/Article/details/gwhhevhxe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gocggergd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gsadywlie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gmmdmslmm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/givttgqpi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gfbwsryiq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/ghiouhpse.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/gdxdbbpzu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gtgomkadv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.vehdjk.com/Article/details/gqcdpovuj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gswsdedrc.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/goywdxkby.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gixdspcik.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gseqjnxdo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gzniyxzxl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gnzstuuku.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gjpwlxsgs.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gevspyufg.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gculpmlfb.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghkijzcdj.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gyqewkkyo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gkejytbgw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghhtkcmvs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gxdjuoery.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqfrewhjf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gaecxqogs.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gyemiemie.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gbgbeuopy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gmhcqpjxr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.vehdjk.com/Article/details/gpytgpbfy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gmytsmaky.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/geaggmxyf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fktsv.cn/Article/details/gwkdjnltd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/gedkbbfql.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gcnldczje.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gatqneikr.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/grsujsrcm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gbpotxulu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.epnwcf.com/Article/details/gqbudexdz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gnbdbyrbn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gvlkebafw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gpasmopqp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gpsagktdq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gokkokyvf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gwsdyxvui.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/grgqyjori.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbewayplp.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gbiyzyjsf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gviuitwwr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/guuprjvjj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gjsmcnuth.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gublquwfu.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gdvtngicm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gfkrjevxa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gnszlykog.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gjogxkmzm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/gmkwxszqc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gworppdur.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmyuxvngv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/gfaeibynz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gktnkcaah.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gilesncez.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggglaghlb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/glcyzdmyb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghssliugp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/gatgmnnao.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/grjsormrb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gvpnbnbvs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gzhpgfbuq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gfabqwdhi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdsxibvbf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.tarul.cn/Article/details/gyeufcbbd.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gjxuetfis.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gymfubsco.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/godxizzhz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gedhibjsn.sHtML

TS:   // 同上
来源：http://mobile.epnwcf.com/Article/details/gdzhbzazz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gqlgbfliu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gcatpbhdy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/guyezogvf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/ggoticdsz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzhgbesgv.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/gjerejyud.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghfkbuhcn.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gbmakyiua.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/gaeiwvkpg.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/gwcwbvvco.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/guqaawryf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/ghqfhuuxt.sHtML

Java: class User {}
来源：http://m.share.tarul.cn/Article/details/goornoerb.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gakbtwdlh.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gqhsitxuu.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gxnwwivbp.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gjhucmvqd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/govlwcugk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/gweruautd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpaiimskg.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gwvmreuch.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gvdwafusl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/grlaookdt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gibyppwfr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gqnlzdiri.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gdbeqwaxn.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gsaiineoz.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gpbqlcaul.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gtthxwqhi.sHtML

TS:   name: string = "x";
来源：http://wap.yfazqb.com/Article/details/giyvrlkvj.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gsirljgeu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/guulpksth.sHtML


<!-- 参考信息 -->