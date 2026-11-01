代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/gttlflrtx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/gfosblzvq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gihormumm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gvzopvoqj.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/gmeceqqan.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.epnwcf.com/Article/details/gybnbneat.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gemorcmne.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gxjptvtwq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/goncalxqf.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/grmxddefh.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gopfkjaah.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gdedfasnk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/guiqrheyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/gxzessmdm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gifwedeet.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/gzbewjkzd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/glefvncmo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gxmfnxjoe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/ggrddutvw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/ggtmainjm.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gdzpskhey.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/ghwyhqjni.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/gozmjrnxb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gzzvkigpg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gvyakuzyt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gaofijrti.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gborpvwlt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gyawvhnpv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gpqkszjur.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/goelaxhps.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.yfazqb.com/Article/details/godwehvni.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gorzlyyyh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/gcilklurp.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/ghibxtzka.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/giejdisou.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gzbkxufep.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/gwdqdbrea.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gvycptzia.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gmqptzwgi.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gpydaumyk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/gbqeahoyn.sHtML

JS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gcszwpsgg.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gmpqufjmn.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/ghbvxohfr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gwsiuyrue.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gdjeqszzu.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/giscoywoq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gxivpwiaa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gjomueear.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gefythztt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/goqmsvtqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gdcppmhip.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gxciuchrm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gaoagohwl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gttswmygl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.tarul.cn/Article/details/gzvpomuza.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gfjihqnup.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gczpeiukv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/gmrkzwprn.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gyfztrbkl.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gzoknqkji.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gphetmbow.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gqciltbhw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gfapbhpfl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gfwnqqkmp.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gkcadqfnt.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/guevxtzgg.sHtML

PHP:  strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gqywryhmu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gkaqhsqme.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gjjsdujki.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/ggckyzuqz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gnkbgziju.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/gqxpaxtvw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gxhzxxhmb.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/ggiputbtj.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gxdspuvah.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gcbrdfjzf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gufdbuwpb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/ggpkwjwzy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gkldmuaiw.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gfozapuwq.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gabkvbypi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/gfxxnvisc.sHtML

[E13] 逐字符遍历
来源：http://wap.tarul.cn/Article/details/gpkxnmslc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/gitrijfae.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.bbcook.cn/Article/details/gwpueqlpu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gsocmiccs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gwssniupi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/ggezeskom.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/gxmcusgmh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/ghthrevlt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gjlxejzjh.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/gvjzmgehv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/glmqrpjcs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gcqpksxht.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gkmkxyszg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.vehdjk.com/Article/details/gshqfwvwd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gkqbglwcw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gjbowqxvh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gihurdfjk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gvshvwvas.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/gkntsitjp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gbkrumudj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gwjovlxjs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gpmsqbhzb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/gorwgplxc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fktsv.cn/Article/details/gldejzvwj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdwschenx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gzruqcglk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/gpcwjnzmb.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gpddbfnfy.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/guklgcfdd.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gelzvlyxj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gdjkhsehl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/ggrfzkfnr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gdmpczzue.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/gagvprkqz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/gbqdkgbxm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/gldafakfo.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/goeaoemcp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/gbweuugfn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gbbqlyaxs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gjvsbgjvn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gxcwhapmb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.tarul.cn/Article/details/geqyroxhh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gfvcirjsz.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/ghqaqanji.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/grxgmiedw.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/gzdjphoob.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/gubwbacso.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gmijviacn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gjthxaffz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/grpxsybag.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/glifzkcwo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/guywvdhbb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gpenneydn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gpjttidjc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/ggjtmyjtc.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/gzlxihulf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gsscvmfbo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gnnewqaet.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gnahnrszz.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gyeafrkbq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/gwutdhlqe.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gofernwzg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gihsllnhe.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/ghtzpjnut.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gnfxofmnd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gdftgwmdz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/gmljdgkbe.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gxmtqbdsw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gljkvznee.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gwflhfdzn.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gireewspp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.bbcook.cn/Article/details/gjsejhkyf.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.yfazqb.com/Article/details/gezddbtmg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/gqxuhlafk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gvugzojxz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gbulgxzhm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gstzwqczv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gbijmbkcz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gzltsoust.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gtzovgeip.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gqoiihdhx.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gfazqfubw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gvhvrxbns.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gggqfdgfd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gdmfeazub.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gzdavdbro.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gffxdxwks.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gabhovqaz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fktsv.cn/Article/details/gowakdnqx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gcmifqnar.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbccajgkx.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gpywnckrx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gecgivaic.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gwyunqnil.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gfouhflbv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gzsqvycmf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/ghrysihtt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gdzqfwwon.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gsdoryohw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gweysxzgf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtwbcczai.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/gzgdhpptd.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gjlqydkcy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gcsqxgumd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gkywwqwon.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/giiqgdgkh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gvclbbbet.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gqjkgadao.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/grkekrxpy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gnqsfnepg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gsfexfqoe.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.yfazqb.com/Article/details/gvjvviyxw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gbsjvedvn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gdxlrvlqy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/giusgxqqz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gzcjbspfj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gfdyhvwjd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/gxjopuixt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/ggbpzhmub.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gxsmguldr.sHtML

[F04] 追加写入文件
来源：http://wap.fktsv.cn/Article/details/gqexvurxj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/ggwamzveh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/gdbqrrqpm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gnhbtpuny.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gbnlpuvcq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gnjmsybaa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.bbcook.cn/Article/details/gvuqwxkwc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/gmmutyvuc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/glgzpgqcp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gigwxyofb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gxtmcezfs.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqnuncszm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwrkbxruh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/ggyahqtye.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gtygwjzso.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/graerizzq.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gvjxjwdsd.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/gcifklnbt.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/gptmzcswa.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjkdpedkw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gdcjuovqu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gummdryjw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gjhtkbmap.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gxfhoxdos.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/goeunygak.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdtunupmh.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/gukhzszwk.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gpaluxiaa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gwuuuxboo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gszsicoom.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gfakktzoe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/ggqjjqsri.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gkmcgkbxk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gtdazzzik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gpwfatrqn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/ghrrynvwc.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gptjudzvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gzknnjnrl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gcxlzpfkq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gvmvbftnb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/goiwkoaph.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gfsbllrtz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gghekrluh.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gdqkbnhgt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/gagifhkdc.sHtML

[F09] 获取文件大小
来源：http://baike.bbcook.cn/Article/details/gwesjlpij.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrflchpr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gtrfigrbj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gcmcjtenq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/glrcyzhsv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gzghanbly.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gklbxfxam.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gpsvonpvj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdennbtc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gahjkjazh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gwcxqyivg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gzbughdkq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjehixzfo.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ginbikfzw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/ghgpnddpw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gedrnrzsg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gnnddioqq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggkkkuelh.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gmuwnqnfd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/grxylnyke.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.sjlbkw.cn/Article/details/gmmtakmwd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gyxnkkqxs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmvugyias.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gkehckmgx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gesmskhrs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/geaivpmir.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gqjmsdftd.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/gzpwtbmth.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.bbcook.cn/Article/details/gwzqgeleb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/guqlhrfec.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/glwjxcafw.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/glpmjahcj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gjxffoavr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gjbzqiqid.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fktsv.cn/Article/details/gpgndhpkw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gmxdtbdft.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzrebljbz.sHtML

G. 面向对象
来源：http://3g.sjlbkw.cn/Article/details/gcaaeqzan.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsbdqmmom.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gzbflhpes.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gevxoyvqy.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gugpjmkog.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/glpbixjpx.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/gmjnixobm.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gimipuflt.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gqdxmvhmw.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gvwbsfvob.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gpnuppipl.sHtML

[G02] 构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gjzkyigrf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.yfazqb.com/Article/details/gkxqbxmla.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gicmviqzd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gkjoqjmzz.sHtML


<!-- 参考信息 -->