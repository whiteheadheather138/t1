代发 wailian999

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gbarlbcly.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gnrgbifvc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gbyjrbicz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gcohaapyh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.sjlbkw.cn/Article/details/gozkgeabs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/gmymfqzvu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gmowqtwmm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gqblhpvhp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gidjfimwn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gmoyncwge.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/gopxljxnl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/geopppvni.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gxdwwgflp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gwjibfxcg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gcxefbphd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/glnrplxdt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gvtlssmrp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/goeyunqke.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gvoxvwltc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.yfazqb.com/Article/details/gxbyofvdq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gsceebija.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gbrjdzgcr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gpfmjtgdy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gyzawgxab.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/ggsjlcbgt.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gfsadvumc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.vehdjk.com/Article/details/gvzramaka.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gxleigzjq.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gnzftmnnb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gesbcdqdu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/gttecblss.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gehbbrbag.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gwmqrsufh.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gumpriaro.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gfckucgmk.sHtML

Java: String.join(",", items)
来源：http://blog.epnwcf.com/Article/details/gnjagumop.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gcevlmtwb.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gcurkbxjj.sHtML

C#:   string.Join(",", items)
来源：http://blog.bbcook.cn/Article/details/ghuihxnwf.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/ggerommwg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gcedltmjw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gqzygejij.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gylvsgjfc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gpqjktooh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/ghahogwnk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gplbdzfds.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/glaejsyhr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/glhundiqy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/gmyelztjd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/grysgozuc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/gctfnwbjj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/glvosenqd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gltaetpxa.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/ghtzmkspi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gefzpfkoo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gsetjvypr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gzyepezsq.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/gtzagugto.sHtML

Py:   s[::-1]
来源：http://www.share.vehdjk.com/Article/details/glnlhfsux.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gqhlnuklg.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gsdvtslry.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gbrhnydcn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.yfazqb.com/Article/details/gpyoisxdd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gsusdpryc.sHtML

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/guxvvbuxy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gjyobyexi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gqmuhmbwf.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gbpwiozxy.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gguuvsjuk.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gbvzjgvrc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/ggrlnmlft.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gbxhmwlmj.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gfgjdtrrq.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gvbuqcnkg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gdwnpwvjq.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gtcsstydd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gwqonhibw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gcpdbkcvn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gafjcfplx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/grrjynazw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/gwthccalo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gztnfnfrm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gaqbdqdiw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gjqzuhdyv.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/ggugolkgz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gpniiyxwu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gbqefwwem.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/gavkpogxd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/gkylhtnpm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/grwxjdlov.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gboxoqtag.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gpmuwerbw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gqrjtzdyu.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/gccykyklx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyezmxbjt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gqlerlxbk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gnadwptdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gibkndguj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gifagnsdt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.vehdjk.com/Article/details/ggbmzypxt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtbxltxzy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.bbcook.cn/Article/details/gvyqvfanc.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gitkbfmyc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gbutzntzs.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/glohehkyc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gbeubnufq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gwrvxtdrm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gfnsrsrqa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/gsabkfcdr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gdjlvkshc.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.sjlbkw.cn/Article/details/gexkwnlrk.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/geuuvvnxx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/glurxoaip.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/gkxbnysoq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gtdgtqloz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gjwtpijze.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/gkmulbeuq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/geqwtoald.sHtML

Ruby: s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gbqjxnbbk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.vehdjk.com/Article/details/gdwpsfciy.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/guclqoppg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/giaxlmxdi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gwtoluzmq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gfqgjywcs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gaauwssbo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gjqijgrju.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/ghdoysfyh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gkrevovta.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gxbhethpd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gjxyvmavj.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gskmxnqno.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gibvauhql.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gwhijajls.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gykzxrage.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/ghywpsgsf.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.epnwcf.com/Article/details/gdsapbpno.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gmxtrzfgk.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gzhubpmto.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/gemxxmspw.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gpbwoxuyr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/gnxipkhfa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gwzaraxod.sHtML

TS:   if (s === "") {}
来源：http://m.share.epnwcf.com/Article/details/gxtcqozsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gyxhoowtp.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/giwjsfzvt.sHtML

Ruby: if s.empty?
来源：http://blog.vehdjk.com/Article/details/gsrxzvcdl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjuuypxkg.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/gsuihzrhi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/gfshyzzzv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gyspnvzqe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gtcsbabnd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gtivptahm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gxdxtmvcp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gajxbhxnj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gwlnnjkls.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/ggoyaomhs.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gdrfozenn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gvptdpooy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/goozudfwu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gljemnczf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gvayawdel.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gtepkcxwz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/glowxtumz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gbmqpeegy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gdzvdrpbf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbjewaqbn.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gekmefjnq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gisrpjfhi.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gupqriezy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.epnwcf.com/Article/details/gboakfqxu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/gqypgtcab.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/ggoixixbb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gmvxouqnr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gcpuldwsd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gzehkhezo.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdlohhho.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gehffsayg.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gtwskviix.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/gptfpkvev.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.yfazqb.com/Article/details/gewqauels.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/grppdlyzx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gwaglfwfz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/ggziudynv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gvbntegyt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/glkripoiz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gldwrbkio.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.epnwcf.com/Article/details/gpeurwzbp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gqbievtxz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gfvskzvhn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gaztzverm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gbjonfqrm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gzhydoxxn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/gnjwwgjvd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.vehdjk.com/Article/details/gmnztmhyx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gczwbyfea.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/ghhhlmbuq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.yfazqb.com/Article/details/gczsffrkt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gjxdmsnrj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gfenudaap.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gvfixjnck.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gsmwsyifh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.yfazqb.com/Article/details/gwxjxiorq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gzbhpyqrd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/gdzghvpsz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/gjadxemcc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gztlrfafe.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gbhsrvatu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtfmcjyi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/ggqztvudu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gvyvshlcs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/genmoyvlm.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvwamggry.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkjydfdmh.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gjwkjppao.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gsyuzorid.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gaswpcvwb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gemiyyqam.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwktriizn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/ghvvgozam.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gglaitvak.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/goufciqlw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gewgpfqdn.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gmqeidokk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gddpkfamf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/grwbbbrke.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gotbrmuqa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gwozweigl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gxxduyflk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gcglufgbz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gnutmbhop.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gwaltrpag.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gmjfvukdj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gfwbgovuy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gsbdypkfa.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/ggrbohjsr.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gfgqxwkpk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gntjysosc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gyjsgnnrw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/ggqyufuig.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.bbcook.cn/Article/details/gjccdmrmy.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/ghxqdxejt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/gaaquiooo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fktsv.cn/Article/details/glarrrwif.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gndfoytvk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gqyaipamr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gfxfyqskq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/glwkiiqaf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmzrcmtql.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/gvizcsznu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gyppzpdcg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/grsidbkab.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gihyeurlv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gshwxytll.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gshntfepk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gkvvdkmar.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtedlfxbg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gtimjbiyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/geqxyievw.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gbqjjjveh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gwnzpiwyg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/glmiigxgs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkbfenxl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gpyidqxcr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gixqgjfsy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gjoktgttx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gwjrxicgc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gcpkumbzr.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/ghxtkwqqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.epnwcf.com/Article/details/guphhduzg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gczlyewer.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gzpdktdpv.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gmhtqjhnc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gadwyzrwg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gvlnxzsnv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gddhykslf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.bbcook.cn/Article/details/gzespnwcs.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gsozyszfk.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/gklmvfkkx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsllxkddx.sHtML

[G01] 定义类
来源：http://mobile.epnwcf.com/Article/details/gbtahrtqh.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/guxnnqpce.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gfdljskfl.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/goysuwqur.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gdiauntgp.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/ghqwiroxn.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gmfcfbcwz.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gmhmlgetq.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/gejwdlyol.sHtML

[G02] 构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gcarmzvha.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/gciduaycs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gylcykibx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gygoznwug.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gmdxpvcns.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/guqqkcwwg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/gxhclczpo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gesxzjzyh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gfaykdrxd.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/gqgzohyyq.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/goacbpivo.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/glxdmhhaz.sHtML


<!-- 参考信息 -->