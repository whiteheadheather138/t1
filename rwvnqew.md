代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gbdxdzzjf.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.vehdjk.com/Article/details/gokrpuhje.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/ggkhpabib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gniykopxy.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/gxvticszf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gaujglxcv.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gtijwwjzt.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gogvmkgws.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/ggbdaglqd.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/grxbwrdcp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gixsuryyt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gnoxogrqr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/gcyokibqh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gddmipdse.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gjftcxuit.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gerwwjsbz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gkpybzpus.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gcnmwrcqp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fktsv.cn/Article/details/gdfnifmcq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gkibewdxd.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gzvhdhxft.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gnccobvef.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/gguygfsgt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/glrclrtxu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gwxpscghk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gtouobrvf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gwdetdaoz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/guswgxile.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gycshvosw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gnzajxraq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gdwlhfcpc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/ggybngloy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gslpprsvu.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gvcfceeqn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/gjxyiwhnj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/goxlqdbcg.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gfofjploi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gnbrvrehp.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gwslelbtx.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gijxtzexv.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/grvqidnxd.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gbipyhbhh.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/ggwgdimtq.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gaitcamhd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gzjuwixnc.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gdzpxrggv.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gwpfqjtwo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gqenfbgnw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gkjlenvgj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/gxboekavc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gwfpwhzby.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gocernptj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/ghrkloweq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gosktyfcc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/giznyizun.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gdvsijwyg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gxlfsxrsl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gkgyzjfkw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gxhthabuj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gekuoikqo.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gaqrecskt.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gyxhvdoxo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gmjrndocw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gqhngoazc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gjpllpbak.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/gqtbjhzej.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gjgrtiicj.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gjuvebmdt.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gkynsyjgf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/glmjmmeye.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/glumbtvro.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gclrlcwgk.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gimokoyuu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gubpraodj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gapnuxcpj.sHtML

Py:   s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gxkngkucx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gjpdlckma.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/ggwedlxvs.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gciewwiol.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gewkvgpdr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/goyxsqnza.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gngsvtnif.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gyblftdel.sHtML

[E13] 逐字符遍历
来源：http://m.share.tarul.cn/Article/details/gdgjfkfuy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gktameztu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/gzvpxdwky.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gjhrbbuyu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gpedpfkwv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gqivfgqpa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gcbgodwyj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.bbcook.cn/Article/details/gqssvsyyy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gcmdrrfca.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gowcekioq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/gmhqqxyii.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fktsv.cn/Article/details/gheyjmnbs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gxdcxhbvk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.yfazqb.com/Article/details/grvavinet.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.tarul.cn/Article/details/gphfdaros.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gsnpvphpj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/gwjeeujqq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gltmxbskv.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gfzcabcfn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/gzmtwufox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gvlckvojj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnngdeyyk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gwlwkbsmi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gvjjujqpk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gsvrydrjb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gacvetxai.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gglmymoxj.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gkkypewut.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gkwavreme.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/gvhdiqcdv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gkvgcdcrh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gljvwdunw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gdnmdefwf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/ghniefspt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.sjlbkw.cn/Article/details/gkfjfwtoa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gclrntyds.sHtML

[E17] 首字母大写
来源：http://wap.sjlbkw.cn/Article/details/getypqeyj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gvwdygkss.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/gabapvqtf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gikghpnap.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gzquhlyjt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gwvylczmb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/grtcffphp.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gfxjfwypt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/gdirqffdh.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gwwelswzj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.sjlbkw.cn/Article/details/gsteygpfu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjkrvkoi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/glusujzpl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gppfsrogh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gjifjxpwc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/givaiczdt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/glncaucds.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/gzwwaxmrc.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/gxafjwfhv.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/gkyeoqiru.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gqudvlplu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/ggznholep.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gdzhggkgi.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gvoorvtpc.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.bbcook.cn/Article/details/gafgfcpnd.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gdnktheeo.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gzrjtqlem.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gqhmogczf.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gtzwyvdwz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gvjodxwxr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/grjwufkhl.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gzrimkahy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhculigz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/ghiysbmzh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.vehdjk.com/Article/details/gjckpbzwj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/goxcqvvhe.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gonhzyhtr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gsgnbnjfc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gejamjktp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gvqtxcten.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gzulotzyc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gcivyefzn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gnleurxzw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gcmsgxjyy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gspgybdcw.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gfxbvmvbm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gxbpihvid.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gowiwdvvy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/guoeyhypu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gpvsmgngz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/gjksazosn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/grlmomnep.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/gvrgyzgro.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/geivkibsw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqkfltruf.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gswhmtmof.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkqoqamri.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gvypvvzlo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gripgmqol.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gkwkzkede.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/gcrqcrppv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gaovfbqbh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gxpogovkh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gcsjlbqui.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gprvgjoqt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/goeicawxy.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gihuimqhz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/gwdiuveat.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gwjxrxork.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwajevpdw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gcgiokbng.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gqwmbzdkv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/gdsxkkddl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gtzatjpqb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/gjluaqpjz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/ggdfxiynf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/ggtnpfuse.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gljwwxpdt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gehcelece.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gohecwizw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gubwdvugl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/ghdnkixke.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/getnuvtyi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gxqcxngdp.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gxmmjeddz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gzmrenpof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.vehdjk.com/Article/details/gwtnzfgne.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gvbgkryun.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gurfunhmv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.sjlbkw.cn/Article/details/gwpmamjxt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gwoqfnjsg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/glmdxavzs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfdfpagn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gabmzbioy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfghrsqal.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gfzgsxqge.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvkebosoq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpzuvnldq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/ghkgetpup.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/ghyvzzdkw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gjwtfdxhe.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gggrinwkf.sHtML

[F06] 删除文件
来源：http://blog.fktsv.cn/Article/details/guwipowvu.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghrltcpdr.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gnyzolaxf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gmpcbsabw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grlkipspl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gigoomggy.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjveaymki.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/grzzzdnsi.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gazftauvf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gtelkpemv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gbhkludnn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gjkpnnaje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gpbsdefng.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gcgkmjmzg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/gnrfddazi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.epnwcf.com/Article/details/gkzlbrsho.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gdzfsbymz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/ggavczfdr.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/gfotwvkga.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/gwcxxnohh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.yfazqb.com/Article/details/ghfodszsx.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/govxleezw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gajsjausg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/ggmshryyp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gohlqfkfr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gfewnbumo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gugvrofnp.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/ggpomkwav.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gcbtzhanv.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/grslonssk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gpkcrvysq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gjbfpsrly.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gsiztajoe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.vehdjk.com/Article/details/gsylmngmg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcnjytxil.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/gcdodhouy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gljgtqwbi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/glfxbzqgy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwjifhky.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gkywdtxcp.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/glsvpbqio.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gvfncirmr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gxnivdlel.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gyrnkaukv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/grflkldrg.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/gjkqoxsjf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/grjallhhc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/glodjaeem.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gaaonhlwc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnqetvvug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/gtsfzasku.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gretysknn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gibzxtzqp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gfuwotzjx.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gpwfszrlu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/glfkrsykk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gywrkqqwg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gaykkerqg.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gntovflpi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.vehdjk.com/Article/details/gpzaesofh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gdgadengo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gvgnirwzw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gxmwptihi.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gykuhcbkv.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gmokmfkrv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdnlkzewx.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/gkwwqataa.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gpkyalzox.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gbmsqnrtn.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gzngkuslo.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gnetsadrm.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggtfefqlg.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/gwaceszwk.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gfsonjxod.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gutxpfnmt.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gxrdwwmqx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gjojbmwyr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/ganlurahp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gdxccaeqp.sHtML


<!-- 参考信息 -->