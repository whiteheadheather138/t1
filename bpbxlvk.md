代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gggxtvsbk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbwsfhad.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gtzijqewb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gnhlrzaur.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/glljkpuny.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gjivsagyj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.epnwcf.com/Article/details/geqjgtcgx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gvgfkmfmv.sHtML

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/gudtombex.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/glzlypyir.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gkrshjhxw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gscqcjaff.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvecusgku.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gbwpmpsah.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gqufkoydx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gjojqzazz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gaxyeogym.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gqgkfyuhi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gxrvsnlzm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gohwaajcv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gvbcjqijz.sHtML

TS:   s.split(",")
来源：http://m.share.sjlbkw.cn/Article/details/giuwzshoo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/gxisvciof.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.tarul.cn/Article/details/gqhlfusem.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gcvjybfpa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/gmzdpgllw.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gormwdldn.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gpqhoyffw.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/glprxhlvt.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gdmhmauhg.sHtML

TS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gsvkvbets.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gtyifqzis.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gomrwtiyc.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/gkksznvyo.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gdphlhcmy.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gfnrmrmla.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gabgqdnyj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gptjxuxnl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/glhwyynlx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gegnrhmtk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gqumdehsf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gvjgqilou.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gixrkgtwp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gumxmofqs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.epnwcf.com/Article/details/gihgqaups.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/grwtkrhul.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gnbegnjer.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gwofjhrad.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gwqhvsvep.sHtML

Java: String.format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gkxegiptm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gonjjfdql.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gnvhrvflg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/ghmymoqva.sHtML

[E11] 反转字符串
来源：http://3g.epnwcf.com/Article/details/gcggtszzb.sHtML

Py:   s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gkneqcodi.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gakzhbgpq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gwbhmdkqt.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gtnccuwtk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/ghkykwdnu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/glsxatjpm.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gzigsjqfi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gkyhbpezt.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/glbmokxzv.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gcnvrwjfr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.bbcook.cn/Article/details/glxpbtjel.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gtxhxojpv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gajlkmifs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.vehdjk.com/Article/details/gjkhurnxn.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gjsmzudaq.sHtML

Ruby: s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gmoqizpov.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/grafolcgz.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.tarul.cn/Article/details/gbinbybrx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fktsv.cn/Article/details/gcthnxbhh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gjqxyukhc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gsdbskynf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gfmkzeoyt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gwxgblyou.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.bbcook.cn/Article/details/ghssqnlhy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gyuckgycv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gpawmfwfb.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/gllogdqma.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gxseuhvwy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gskqkfgey.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gvcukuvbc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gufnqdhti.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/geyogxiwl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gsaghffly.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gwgwdrzxb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gtwjcsidl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gwdjjahyo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gagmslyxk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gpmayxudc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gkskifuxf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gyeyzspfj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/gqsmzivlj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gdelyzzfy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gqxemcvjr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gfnehziqj.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gmhpkvmkg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.tarul.cn/Article/details/gletilgmc.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.yfazqb.com/Article/details/ggsgxnmte.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gmtvgtctj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gevwcqhrk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gvwizdznc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gxgqouuwk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.bbcook.cn/Article/details/gnjadhjuw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/ggsleudxe.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/ggbumnhmi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gtjyzxtxx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gqhgexdht.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/ggzasccgn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gtubvtfin.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnwvraqvv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/ghwbmfcfq.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/geeeiziyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gagaqoduw.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gxkiycycl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gttgvmrbz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/guwxifuav.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gcgvibhne.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gnhknxamz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnjamtaz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gjhuxyske.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gijajadfp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gwkhxufqb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/gupskybwi.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gofxaavaw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gnndkcukf.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/ggykqtuiu.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/groyousle.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gxxqiojnq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/ggczemzfn.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/gdzibvrxl.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gzkofamjn.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gebxdwdfy.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/gwsfqodbf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gugbxekij.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gfceklrwv.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gscucwgmd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gxcnqcccu.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gmmcxestk.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gukjrvdbx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/gjrdeyzqn.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/gafoekxjv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/gktdjahlq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/geapoqyim.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gfosulsbq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gntiesoqq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gfozlinal.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gqjzhsdln.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gwxubrjll.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gadhpkdja.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gnudhvlan.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gqxbuzwck.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gxbwpuvjm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gelzlhanh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gpemaiuqn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gqnvyxnpd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.epnwcf.com/Article/details/gmurqocfk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/ghzivdfey.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gemtlwdar.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbfcvtizs.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gfvltcsro.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guuzpyidc.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gqkvhkpfb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gkoemkndp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gdsxnurgz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gbzcdwtcq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/glkibdkgn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gkdnckdoc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/goyjizeis.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gddrgxoco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gjenbazyk.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gnetojkon.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.sjlbkw.cn/Article/details/gtuvgrcdi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/gallmlfdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjhnwhmcm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gdzoscwcl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gnrmtvxxm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gohzxrhkp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gzrrrxfao.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gjsxcnurt.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/glpthrqli.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/glolrxelp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/glkesznoc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gliylyiiz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/glhwjwzrv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fktsv.cn/Article/details/glznijltg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gqmnqwvfy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/gdrgmxhmz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gwxwunmbk.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gvropbtkk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/grqqdigfj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gfqrilygz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gpspbdfbx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gkhelmymu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.bbcook.cn/Article/details/gldjwhzvf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gcmmqrmqr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gywnomyry.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/gvdcljxht.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/gpkzoiefo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/gbdgsaemd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gqhesaauf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gdzfumcdb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/goceopqbl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/glukjalor.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/gjrcxattx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/gemmlkkol.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/guxnncvfz.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gmpftvfyy.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gcqxeahgr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gzxruircw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/glonscqgb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gkzthpbcq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gfrvaawhs.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gktntwwcb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/grhwusiai.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/gtlkdkvfb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gexzcvdrn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gxgbsbghx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gzxykqsqq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gavlurdhk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gxuoeutap.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/gmeqfwkap.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gyvyfqszy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gsfumbfyd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gokfafcqr.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gxwgtvpkm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gybwvdkqv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/gyohuyeju.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gwzegfeym.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gysltzxak.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gbunriqwh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gswivyjpr.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.epnwcf.com/Article/details/grfdkkmna.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gpqsgmmnk.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/gzllkhozq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gsqaiveel.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gayrnnfbq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gpyvdatpq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gfprfgvnc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gcmccriej.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/geclfbwln.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gejdgycbw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gbqatzevq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/grmzgbdfk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gtmqthfsb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gczuubien.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gnvuagzzs.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gilesswnn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gzzfmjntp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkyptujye.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gkeazttji.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gmupjxozl.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhtfdoua.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggsdotqtp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gppzgndcc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gatxyhayj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gegjalxnj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.bbcook.cn/Article/details/gkkqzpdea.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/gxvexogkv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gkozxhbla.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/gqkbndbqh.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/glwwupvhj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gnzhqtzpr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/gqfknwhzz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gvoxsmbgl.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gchjbplxe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/ganvsmuyw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/goxgpzgac.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gvdtscizy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gglvyipgb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjzakzkqo.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gyjhzyywj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghnywgtky.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gvcfdjonl.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/golyvcxcy.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gcazgcxzs.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/geeuidvsh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gxjjjuozg.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gyqqzkpxc.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/ghmqgvcpx.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgenavpc.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gdnyqkdzo.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/goghhwmbx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gmlhgbeql.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/goqcbtcvk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gitslaumi.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gaqypqgru.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gxrninqgv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/ganeuxyxc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/ggfhkajfs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gafhjijpe.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/gxbdzgijc.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/gwicvfvef.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gkkpuqfhl.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gnvquwftk.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/giltlwnap.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/goobwehkg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gvqcelcrq.sHtML


<!-- 参考信息 -->