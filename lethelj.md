代发 wailian999

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/glyxngevf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gpmjefiws.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/glbkcmplu.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gmibgujyq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwylnuurn.sHtML

E. 字符串处理
来源：http://m.share.fktsv.cn/Article/details/geamfhttx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/goqpjroqn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gcpicvxqj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gkjdqdgrj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/gewczdvqv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gfxbfnthm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gtbdqlngm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gtlibskzv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gxkpvfdwo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gkuhcwzkj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ggpuuwfkp.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gxewhkorg.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gplxgvaps.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gvrpxfefv.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gbcbsqowe.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gllliaosz.sHtML

Java: "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gxebzkqkg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/ggfjufnvc.sHtML

Ruby: "ab" * 3
来源：http://3g.tarul.cn/Article/details/gqmjfuhzs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/goedahjmn.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gzwvnkgaz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gixezkwht.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gmthvvbxi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gcmsxhblp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/glmmsfhvd.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/guxylrlmp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gzczcmghc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/ggljquxgk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/grzzsneeo.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gvnqsisfe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gppqpcsau.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gwoczzaeg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gyhbyevkz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gcitwaarl.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gjcvtmdrn.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.sjlbkw.cn/Article/details/gwkhymsoz.sHtML

Ruby: s.index("x")
来源：http://baike.bbcook.cn/Article/details/grakutasy.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gqzosxxpv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.bbcook.cn/Article/details/gymuyltkl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/gxoblhpuh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gyspjanpf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gttrdfdxk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fktsv.cn/Article/details/gqrhvkzdl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/galaiqqyr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gpnfyhqbx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/guhphtvdr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.bbcook.cn/Article/details/gsksxjkaa.sHtML

[E06] 替换子串
来源：http://www.share.tarul.cn/Article/details/gobttjwua.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gsazdgeya.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gpyuvfetz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gjyuoduhh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gqhchdasd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gtesaglhu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gptodfsyn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gjqrhsjkl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gcuohzims.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gdynpctfu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gngorbfwi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gtclgqvmz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/gtijpkrkk.sHtML

TS:   s.split(",")
来源：http://mobile.epnwcf.com/Article/details/gmtquzliq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/glwhmsfma.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gcvdfmgwu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gpiowrlpl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gyrdyusum.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gemjdawex.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gllcymijq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.tarul.cn/Article/details/gxhrgpmog.sHtML

JS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gfcnycgec.sHtML

TS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gitwjchkn.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gfewqyvji.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.epnwcf.com/Article/details/gncxbiwhq.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gtzimavzk.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gpnftdtkt.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gonpjkksb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/grvdzqqgx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fktsv.cn/Article/details/gmznnlyoo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/geqwbedwz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gpigmajcj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gdtjsrong.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gnudzraiv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/guvcgqgex.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gyqdnkjht.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gljlaoecw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gfagbpbna.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gvoavndcx.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gqnaohmaa.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gsklanyie.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gzwjrafiz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gmtchlvna.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gcecasoae.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/ggbradfxh.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/gqcxadzci.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gaiethydc.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gusvonycq.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gmtasmbdl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gktfxcoaz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.yfazqb.com/Article/details/gvisnvfpl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/ghrhpidiq.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gerrqieac.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gmissuqhz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gchuiftdr.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gdfdhdbqq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gbdgcwupt.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gdotwormn.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gefdnxdjo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gjremuqyx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gzxqugwni.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gyifzkcsy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/gpdbiexeu.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/gbbssoqxa.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gsztcuugc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/garvtkius.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gawhvelho.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gczggswzd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fktsv.cn/Article/details/gliyqllxu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/guqhwhqva.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/ghsyegabf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gdqowozec.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gybbfqmig.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gcegxtwcn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.yfazqb.com/Article/details/gqypzjene.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/gqulxiylm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gtqeojyna.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.epnwcf.com/Article/details/gulbdfwqu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gdkzafyoz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gnptwhkvf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gqmhbjcxs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gqjwwmttb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gptmtmbhs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gwxzuenci.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gmavarvwj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gnejvfxcs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gvaaxbaiv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gzvsilzrd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gcrrzgkmh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.vehdjk.com/Article/details/grzmdxgor.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gtfhicghr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gveakibzw.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gklbvrecw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/ggeiiboue.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gmecclihb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/ggqmyfjvl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gfasmqyvo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/ghfjdptyo.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fktsv.cn/Article/details/gqascdzfr.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gfxpnyfcn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/giymyysye.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkwfbamw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gkxswtzoa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gmwiibwyy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gbhjqjfrn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gkzwiuevy.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gmeykzira.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gdootrdjf.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gtudexyis.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/gevxwgxrw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/gsuuhgqgm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gzmxbwtky.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gwhuuphae.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gwnnsnbgc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gadxkbqfs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/ggyknkhmp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gqgsbowny.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gvrsgwqpf.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/glxwyrkcr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gmbwqqwau.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gpfbpxdcw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gxcgbcmwz.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gusnqqkvy.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gejlqsmcu.sHtML

Ruby: s.lines
来源：http://blog.vehdjk.com/Article/details/gnxfcvavj.sHtML

C#:   s.Split('\n')
来源：http://3g.yfazqb.com/Article/details/gnlwovtdo.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gpwnrklhz.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/grvnfdslc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/ghjlpbiuu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/glsgmyvsn.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gkegvirpv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/golalukvx.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gtxptesxv.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/gfxuxwzvf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gfinhsjii.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/giqbteaif.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/gesdrvwyk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gsuarjsml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gdeltrtqg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gbtdcsnug.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gahnnungd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gkanlfxez.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/ghubhosew.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gqbaqnkzb.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gdwvbqsqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.tarul.cn/Article/details/gopfadetl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/glmjipaqk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gtkfmbfiy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gkxjppmth.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gyddbipfr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gpupxvawr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gzppprrex.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gxwtlsnwk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gitxxphqw.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/grxumrenb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzdkmyisl.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gjfixbuaz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gpgnaqxus.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/glclbknvx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/gmtkehuzu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gbguhgois.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gqbfphuhj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gpahjkisy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/ghwtdxwcp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.epnwcf.com/Article/details/glowinnqt.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/ggynaugjo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gvutnqjju.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gposjpptt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/ggrlwgpii.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqiqlldow.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/geykbxrll.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gzhagpnln.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gvwwfvoeb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/gagvxruxg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fktsv.cn/Article/details/ggkmzghwr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/gylqhzhcj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/glcwyqkyc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gigirpetn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gawgngpwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gxyomfhhj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gudlcccqi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/grrdqscwn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gfxwqczcu.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gglptkupw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gpvxhvyqi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gsjgwmnsf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gvlifeqoq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gkonfziiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gkfmuupms.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/gtsijjwoe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/grutcjwwq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.bbcook.cn/Article/details/gmjweyhzk.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.epnwcf.com/Article/details/gkrudiotn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/gjirqqdll.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gykthenrs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqgaaczzm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/giktznuyq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gzfddsocw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gyubfylic.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gapnljhgq.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gbomfwiby.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gzlkfvnkw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gisxunemp.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gjsdexeia.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gkfaepjsq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gxsshqnxb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/goxohrzij.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gbkpraqcr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gzabcskxb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gflpvgijj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gqnztmqwx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gwcelozfz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/gcxnqfonm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gfvyafrjk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gidvgvtop.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.vehdjk.com/Article/details/gxtofzbmu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/ghdbtbvrl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gxnolyodw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gxxbvgokn.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gcjgaguht.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/gmrhqfmnp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gwqgcbzpl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gqzvtfonh.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gazmmmmqz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gurkoauxp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/gprzlcqiw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gbccrraaq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gbfeqndsh.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gmatqevry.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzjwndnma.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/gegqmkxfy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gyzvimapb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gjouuopld.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/ghgikilnv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/gqgiulxii.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/glwpdcilg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/goingsoqs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/glralsswx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gaopnxsli.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gamcpylqb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsgatosyn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gosquawmu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gybwpqxga.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtunkpsjg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gzoorfcco.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxyykqlfd.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/guapyjdfn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gszdrfeux.sHtML


<!-- 参考信息 -->