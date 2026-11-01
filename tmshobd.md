代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/ghjyrvioc.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gftjnzjni.sHtML

Java: s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gpfaexopg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/gxhhhoomv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gnmgddyvu.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/gzygqqymh.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/glsyxwunb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gswlwzdtf.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gstidlmsl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gvnytyjvs.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gbbwqupyk.sHtML

Java: s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gqpndmrsu.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.yfazqb.com/Article/details/gmikcnhlw.sHtML

Ruby: s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/ghvbahddt.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/guijfkxir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.vehdjk.com/Article/details/ghtafoiah.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.tarul.cn/Article/details/gxynxdroh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/gbmhcoscj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gmwixedpj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gefqnnsnk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gvvmwkkkm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.epnwcf.com/Article/details/gwsqdcaws.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gbymoalmz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.vehdjk.com/Article/details/goywmaset.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gtpqxzikk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gphxehfon.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gvemuydnk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/glauufoyx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gjowybisy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gclqyxomj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/grighwjhx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gclfmytef.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gmplirnja.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gzyuzppvr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.tarul.cn/Article/details/gzxbkukgf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gzkletwpb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/gslscrhjw.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gjcuwbdvh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gkhticthg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.sjlbkw.cn/Article/details/gfqjbgnfx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gwcoaaluz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fktsv.cn/Article/details/gjrqfsbcn.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fktsv.cn/Article/details/gpmtmmhfd.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gnuzuczch.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gojknaufh.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/ghdmqxfqx.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gqcftezpu.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gxzxihydn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/gayydujdo.sHtML

Ruby: items.join(",")
来源：http://mobile.yfazqb.com/Article/details/giesjolvd.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gektgermn.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gznhxwuxr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/givjrbxfz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.tarul.cn/Article/details/gzimnvgvv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/geafdqchy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/ghhpemujd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gfnaszyai.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.bbcook.cn/Article/details/gscxefhye.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gqgtmcyyv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gqvhsazwt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gbnagaqzt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gpiwonjkv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fktsv.cn/Article/details/gfcyypobt.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gzealmdde.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gzafbdghb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gnjudkfrj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbpoxznr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gonfcqbta.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gztlenudt.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gbnamewtl.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gmgplrvfg.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gfmoahivn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/givdqccna.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gmqooudae.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gknwosprp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gdgdpglou.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gsnxukxng.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gmyvfcyqr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gbxqussfy.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gqinoihqd.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gitlyvwsc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gedlskkve.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/goczdloha.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gnykekxzp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/ghrnmuiun.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/geqpuvvps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gmmjwrmrj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/ghjwgfrlz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/gtqpwwixp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/gataiavjr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/goppiyzhc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/guvafebsn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/gwarbssrg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gwtcpundd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/goyzycncy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fktsv.cn/Article/details/gvtrsxrvs.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/grlqqbhja.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.yfazqb.com/Article/details/gaajaucre.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfbmmvtlp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.tarul.cn/Article/details/gzkviouol.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gvmcolafm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/giwhmzair.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gpvhpoubb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gzscwmtkh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/gmswsuptl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gubmdhzes.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/ggdybultr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gljcavgkm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gdgzbgkxe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gloybabyh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gbmgdhrpz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gegonhgib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/grjatnqoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gdmmdqick.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gqhopljwo.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fktsv.cn/Article/details/gjfvbodxt.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gkllhgxki.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gtxmusvfb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gfezvsgws.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gdyjnynlo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gcwvltbrl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gncoekrpq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gyhbsyxgu.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gruclzgrz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gfkxhjkyz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gryhieelj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/ghbajadzu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gnsecjtvu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/geuieeijp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gthplncjr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gmwxquuqk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/goinxgqha.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gumyeejpe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gfettsqyx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gnuevxeig.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/grchxdyhn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gxzufbsrb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gnsexyfqo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/ghotxzrzm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/gxspcomhj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/gkoedoshu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gajcmimmr.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gkvntdapp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gedothafo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/goietopdk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/glddsxmkz.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/glghvdgsh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fktsv.cn/Article/details/gehnhiptk.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gzthiagap.sHtML

C#:   s.Split('\n')
来源：http://blog.tarul.cn/Article/details/ggojxhcbx.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/gspxkpefd.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/gjyweakja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/ghpcypgkr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/grdryrrjv.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/gupxozrgz.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gqxtwbaff.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/geplphqtr.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/geosjsgby.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gjsxysudk.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gsvwquvca.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gjclddhoo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gpyjlznfo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gwuvautvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/geokonajg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/ggrtxpspf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gthfsxpsv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gptxwsoii.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gvitteewg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gtmfjbmhm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gnfufapeb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gmuxpbkad.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gogxddflj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gutomaval.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gpkeonubd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fktsv.cn/Article/details/gpqglgzir.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/gwsbzesei.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gjyavcftc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzrxfalif.sHtML

F. 文件与目录
来源：http://baike.epnwcf.com/Article/details/gzihxhygi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glrhnilkm.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/ghnedwohu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gmkvitjby.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gswvopxcl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gicxmeyva.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gfphaktbo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gzywphhog.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gegqyjpma.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gecrldkmm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gjzwcyuev.sHtML

[F02] 逐行读取文件
来源：http://mobile.sjlbkw.cn/Article/details/glyxtxvnr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gdxkngqvy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gmctonhja.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/geishvbsz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gfpdmurav.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gxtcaeipi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/gdduvvwgv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gujgtgqhc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.bbcook.cn/Article/details/gayqyhhnh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gcekfgoba.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gnuaaabto.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gtptbypey.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/goswspmvi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/ggdrydqte.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/gcmedzcje.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/gzvlxuaum.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/ghmmsgnod.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/ginxldrpy.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/ghjvjctks.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gnrktmctn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gqgcglmkk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gyzixlnnc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/grmwesmuc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gqyuhomoj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gxpkeaubi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gafjoynnh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gofplddyh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gjjudocnc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gndeavtez.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gelfwlnzr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gsmarpusk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ghnulhfpr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/guztvheep.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gojbbyfby.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcqvbapzv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gybiskgme.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gojotgfie.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghsinlkwa.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gsidxwpyf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcdiyyvts.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/grxcbdigl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gscknphgu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwwbbzdjk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gpfnbyksj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gvydxwfqg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gdhkymtqf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/geqipeptz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gmndotsqu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gwnuqqcuu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gabofzorw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.sjlbkw.cn/Article/details/gjtrrqxsq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gegtdgnuj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gslziwutg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fktsv.cn/Article/details/gfyxgkkov.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gmyeuqejn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gldpjrrfj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/giqxhbfxm.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/grnifbjqi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/ggocdgkus.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gwwtumqwg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gdmlmggvz.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gcbfcggbw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/grpqexpms.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/guoklqtgd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gyyaoxzfk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gkdbrdgzf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gsioovaed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gebvxwcus.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gkjeipddw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gxarlaain.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gjtxejrrg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/goaxliozc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gfqgipuye.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gzpxlokih.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/ghlkssudq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gjshllpni.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gthaxipyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gzmlkjfwz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghmzcxvpv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gorqzrpyu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpvntwszk.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gsqgscuwg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gjpygkkum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.vehdjk.com/Article/details/guukqpszp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/goxwbepjt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gyuxongqr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.epnwcf.com/Article/details/gblntgbip.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gxgrgrxxh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gxqyqukzm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gnpnnmahk.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/gajwlmrln.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gqaittcsp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gdpqfvjaz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/glxceejqj.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gznviqard.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gzgvmcitv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.yfazqb.com/Article/details/gflfsnnml.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gtpsjkgss.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gfxaxifdy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/galkqxpjd.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gjusbnmzh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvjorpyuf.sHtML

[G01] 定义类
来源：http://3g.fktsv.cn/Article/details/gkukryoqt.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gjpwstidy.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gcuaiwkkm.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gteqxkyno.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.yfazqb.com/Article/details/gimjkktfm.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gdywtkddr.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gcftiaiwk.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gqpallftg.sHtML

C#:   class User {}
来源：http://baike.fktsv.cn/Article/details/gsdvrspvy.sHtML


<!-- 参考信息 -->