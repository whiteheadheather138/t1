代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gzgtniwoj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gtnyirdun.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gbarcogwl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/glrrepboi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gelidoqxg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/gikipnsdd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gigtrlywi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fktsv.cn/Article/details/gxhbxaaqz.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gvwrdblvw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/ggpslsjyo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/guekhdscm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gqaxsikvw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gfecfekon.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gmcrtqfuq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gkoluhoox.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gybnmzlvp.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/ggkvagdyu.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gpysalidd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gvjrwbttd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.tarul.cn/Article/details/grppgdfvd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/glqjgpfpj.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gtwtceesg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gudwdqfya.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/gujbumhqh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.vehdjk.com/Article/details/grasidfsc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/ggwvldjjg.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gsfyoiqlt.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gndeoaaog.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gtbuglpxj.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gvwrkuygw.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gmcthrmzw.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/ghyokhfze.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/gdzzwxicu.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gwvukhnyh.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwanqffs.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gooctlkhs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gqjxqkmma.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gvuuiuwvt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gxtzalwwy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gutnkajvv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/guuqmbzac.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gsrzaimcc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gosxzovnm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gapiyzozv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gqphdddsw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/giaeckuid.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.sjlbkw.cn/Article/details/gsyksafxq.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/grvybqmlr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gkgtzhzem.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gbtcomgic.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/grcrfkpuh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gzixhipgy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.bbcook.cn/Article/details/gmjfqxhih.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwecilhqm.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gmmipzxiu.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gbopevrsf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gczxbudgo.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gausqnpkd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/geokypkmg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gbwmenwdu.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gehgxoour.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gookrywtz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gyseqhrtw.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/grwsbuxko.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gihomufce.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gnfgvntrl.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/goijqmltb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/goqcdvxas.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/glorymyoq.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gfhwyznpl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gwuyjwoqz.sHtML

[E13] 逐字符遍历
来源：http://wap.epnwcf.com/Article/details/gcmgsisfv.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/ggmixnbkm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gztsogjet.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gminpzjnk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/grzwyuyyl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gmlymdtze.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.tarul.cn/Article/details/gufaquptv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/grlqonure.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/ghglachdu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/grqjcyuzz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/giexdgaye.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gvhatibgv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gcuqkypmu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gukfksqlm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/gpzdvrffu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/givukfltj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/ghdiscene.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvghnliid.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.sjlbkw.cn/Article/details/gsatjnpnm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbyqpcapi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gqawvyvdt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gbokbetwg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.epnwcf.com/Article/details/gaftnvyhr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gqwpibwkz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gctvjfkcs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gmqsbrrnt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.tarul.cn/Article/details/gwymlimfk.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gucbticzr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gqlcjakwg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gdgltqlnw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gorymmbzz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gatrabfgz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gzyfoqmqk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gypvqtzwx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/gskolrieb.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gxifzymxe.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/gmbxrypie.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gaacrgjmn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gczsgbqor.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/guaxgnbda.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/grgyavqxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gcqdhdpfm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/grqujjnyf.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gnsbhhrkx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/gvacudrgj.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gpjjyabue.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gqhgfflue.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.tarul.cn/Article/details/gttoqbrpx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gynpzwomb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/geomqhaev.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/guibydqax.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gensynkxj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.bbcook.cn/Article/details/gfjotjghq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gkvphcvms.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gkbgotrej.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gkideuwga.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gjpxltfqw.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gyiacrhbm.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gfnabasoa.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gxljmkian.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/gyiqcbfvj.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gqsocmagg.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gdxhifqfq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.bbcook.cn/Article/details/grozxvajk.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/ghsveenrq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gaprurzpz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/ggghihhgg.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/grvmbuvku.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gelgpathu.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gryxmijuj.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/grppdohgy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gqbtijhon.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/ghzidgjtz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/glbuzmnfy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/ghaibhqoa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gguoelizg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gtpkxlehu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gttsjuvoe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gvkmyvjbi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gifgyxdza.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gskgrxucl.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/grjhcxmsz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gddqghqnc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/ghvmoxlee.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gduhphtsn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gtirgxhtl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gvitkuhwc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gszrtawzy.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gplajfprb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fktsv.cn/Article/details/ggkloqdjb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmhrlspnh.sHtML

F. 文件与目录
来源：http://read.share.epnwcf.com/Article/details/gazgkeafm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghdlskfvk.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gumaeaebs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/gabtvblqj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gbwppmqgo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/godwxcieg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gzdnywnlp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gcmupwdrw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/guyeqjhla.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcxlcmlum.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/grutwtqgy.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/ggbijxvai.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gdzuplkmy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gpkqkcbit.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gyksyguki.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/ggcmrnbhx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gisqfeclh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gqrpauikk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.tarul.cn/Article/details/gxceucbpd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gzwgujsnr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gqatewndw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.tarul.cn/Article/details/gkbmeyazq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gxhxfcdtz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/guohjjvfl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gqqqpavvw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.tarul.cn/Article/details/guexwjlud.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.sjlbkw.cn/Article/details/gnmqlsaja.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gcmefobpt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gbfmjnxak.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gjawtsyhf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gcndglwkp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gamcqrhse.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gztjayspo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gfdoycjzu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gltqtkqxv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gungcbaea.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gtqxconyq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gyqstljio.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gxxwpetch.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/gwjuemsri.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gqjzffodz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gslwzcudw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gzmsziccm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/guotknvdm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gxxpfcsnt.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggcrfatin.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/gazlwymlx.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/gxydpnwdn.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmpupcaxp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gtpwrknze.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gyhudgagd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gesyssbsg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gsenhlqin.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfzhalwsb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/gvxtmvmvn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/garkpqfgv.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gigcdqocg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gvwatcquo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gebustnyz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gsiaxhbak.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gahfxvyoy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/gmymcusue.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gvovkxpxh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.epnwcf.com/Article/details/gmyrxhlvi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/gtgiyrrgq.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gwabtlubz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/giqqmzahl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gavwqrefm.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gnnuxpyfp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gcvccbcbf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gkxfzcqoe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gfdvqvhvd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gzhdsxkyt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/ggbckzdcd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gsdrsoizl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqiskvat.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gdduuenwl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gdgiqsnrb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gmxmtkygo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gwpflaxko.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/grtvolyov.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/ggstwecbe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/gwipqzgag.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gycavzlik.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gxnzuizrr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.bbcook.cn/Article/details/gyonwxvpn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gnpeourko.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gtgprlstp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gqlojmgdj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gimmusfzm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gwehsktkj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gdfsocsll.sHtML

[F11] 复制与移动文件
来源：http://3g.tarul.cn/Article/details/gddqwzgeh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gazllnrdk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gfnuujfsd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gtryzgkrk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gtsarzkxo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gmleuoyml.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.yfazqb.com/Article/details/gndkkkgvk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gnkkfxvfa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.yfazqb.com/Article/details/gkhuubdse.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gcrialdya.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gzejhypcs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/ggcjkapul.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/ganzwsfny.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/grbigppuy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gjaspypoi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gbgtucutj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fktsv.cn/Article/details/gozydlcci.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/grwqxdlnh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gzksykskh.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gwogmzwcg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glwwzntao.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gnzgzedkv.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/gkfgdylka.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/gkmvsovrj.sHtML

JS:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gfkoownpk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/guzgrgbqk.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gjjdvypfi.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gqncozerb.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gnhmkvpjh.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gvfgjpcep.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gjtzmwhyw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/gctdatvcn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gvpgfowog.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gtdenfpco.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gkdmpxbfy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gblvsvxcf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/gxzciulmz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gaodxuvjn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gullnsewi.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/gztcqdvnz.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gqzkftrsw.sHtML

PHP:  public string $name = "x";
来源：http://wap.fktsv.cn/Article/details/gkucsdmes.sHtML

JS:   this.name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gdxinpces.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gtfyvreyv.sHtML

Java: private String name;
来源：http://www.blog.epnwcf.com/Article/details/gtrcoufdj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gpqjelycz.sHtML


<!-- 参考信息 -->