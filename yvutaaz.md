代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/gxtmehnrh.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gvesdjnrq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxvqnrwa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gkdhzpkxp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gdxvgzflf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/glkjieqnn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gyszrafsw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gabwovslt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gujwpukff.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gqcafpfpe.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gmsmyvepb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/grootxske.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/goufqvcks.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gkddanthu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gpwkcrurs.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/glptmtsth.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gdezdhfxc.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gobtmjuuq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/golwvgdoe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gjyxvppys.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.sjlbkw.cn/Article/details/gqszaemzz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/gfnyobkgb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gwdaxooyt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.vehdjk.com/Article/details/gwaolwfxn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gmdupoije.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.bbcook.cn/Article/details/gelxxsfis.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gwkrlywmq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gyshdxixr.sHtML

[E06] 替换子串
来源：http://m.share.bbcook.cn/Article/details/gotsqmqpu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gswpxvxiu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gmsrheqhj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gvjijlsio.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/glxdnqzjm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gkojmvdqp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/glblhttda.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gleiklwnz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gfdntspnr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.epnwcf.com/Article/details/gwwfanjaf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/gluxnvexd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/gyuzvqmeo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/gibkkfyvi.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gtxodxxni.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/gyfrppmwe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/gurmuoatw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gvsarjmuj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gkxuhqcgz.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fktsv.cn/Article/details/gmqchbmxz.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/geseaueij.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gzttypkbe.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gzezsxcop.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gvuxkhxxw.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gopgcqyxe.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.epnwcf.com/Article/details/gmupguguw.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gaerccqsp.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/gvlfyfzyr.sHtML

[E09] 去除所有空白字符
来源：http://wap.yfazqb.com/Article/details/ggrvtqmyy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/gfcmvlgiz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.yfazqb.com/Article/details/goohgkvbx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/glnhvdqaa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gdisxdqiq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gbaywgfam.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/grjwvxhgx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gyxtkrwna.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/ggeduxwde.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gbsiwbiiq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gmdmuxhvq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gthhkcnhf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gomfzqqsx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gvlgoapia.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gxuxdyuih.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/guqgmhybs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gifpsypwv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.epnwcf.com/Article/details/ggruaoneg.sHtML

[E11] 反转字符串
来源：http://mobile.vehdjk.com/Article/details/gxsrvdoxi.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gkhvcmklq.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/grvrwlras.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gipknuuqi.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gqoxfurrw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gpbszvieg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.vehdjk.com/Article/details/gtcxbfbhg.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gntlmialj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gymnttezu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gslownewf.sHtML

Py:   s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gljlvftha.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/ggjybukdn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gadvzjfcl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gqzqmvilu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/gqartlbsq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gceqikdii.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gsewxmwck.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gxfzjvvtx.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gaovpvrfc.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gxyzcuzbv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gnmzcwonc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gtzekercw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gcczyyaoi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/grzstlozd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/gmhgnyftb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gjdwqxdrx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gptdijgyf.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gmzuppzgz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gyujvunfi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/gkkjtnsdb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gxoymcyfs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gffimhemf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/gbyazcbzt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gcxbqhxul.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gbzbxznvb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.bbcook.cn/Article/details/gizsabsrr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gzpwtboyi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/gjvrvtpgt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gkssnnzqr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/giprireeh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gfsnyntka.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gmgqtwuyj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gcnuuusll.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gkghihbhe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gpoltrukr.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gitfjxxow.sHtML

Py:   f"{1234567:,}"
来源：http://baike.vehdjk.com/Article/details/ggunspyew.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gyiunzzrv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gygkzhcyc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/grmakoqet.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.tarul.cn/Article/details/gamtgixam.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/gpnzyliud.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.sjlbkw.cn/Article/details/ggatcmnhf.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gnmqepnas.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gcqvfujcl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gbpnblyzr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fktsv.cn/Article/details/gaiftkrwc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gsohpwhnc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/ggabghbzi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gwofkkrej.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/gxflnblfu.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gzqvhqqrq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gemeamvqf.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gzlpqvcqf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/gryavhrmu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/grbvhsrfx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gbicsyboy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gfsxnesku.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gcmjlkmiz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gmlfqwzmc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/ghceibxqd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gzkvhilph.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/gdxfpablp.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/gzrcgpmlp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gckizcklc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/giydzslgx.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gxkietiou.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gqqfhiexk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/ggvmbumna.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/guzrxfbyu.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gpzumqssv.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gpnxnxlbp.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gztwfayym.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.vehdjk.com/Article/details/gofuhixbi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.epnwcf.com/Article/details/gemzvbuya.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gchaykqzr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gsexneqdy.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvgabtgel.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gfilyesls.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gribifofs.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gpvgtdlhs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gapfiyonj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gzeufauim.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gruyrjqkd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gswlqzxjq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gjgonqizx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gptdyqhld.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gycjpxrpx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gwcyvpiff.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gtuqvedtt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/gdmsbdpeb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gojckuiub.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gmtpzsrnl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gljpyjbmb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gpmjkgqsn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gsxgempob.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.bbcook.cn/Article/details/gjonjmndb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gvujoibya.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdtljmpkr.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gkpccdrjs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbqnablpn.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gustdgokw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/goeesyiqy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gqzcpftii.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fktsv.cn/Article/details/gtwaypylt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gykfqlkux.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gpqrkzrom.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/glaiomlwc.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdyezptzr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gdnrlkask.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/gspassspb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gcczmavwr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.sjlbkw.cn/Article/details/gwibqgutw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gpalfahdd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gzdggittu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gthvkxfju.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gmxkujfjq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gydnhfsxv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.bbcook.cn/Article/details/gvxgeiaiv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gudmldciz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gkmoyeusg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gbpejzcwh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gvwrjsvrb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gjkelpjqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gczwgxlho.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/gwyagkyrz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gjceibvmj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gcsnixcez.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gjpfnjcyj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gcpochcbn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gepjyycdz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gybsscrfy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gjhjzaxbs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gunloqunx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gkdkmuidy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gkbpfrhhy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/gqawyjwuq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gsvgpdteu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gfiayryfl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/gjqklrzoa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmotkhpgp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gscvcxahs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gpykerqkd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/ggrvxpetd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gwamkbxdz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwsweipyu.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gxndaxzsm.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsazcovnz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdbacqys.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gsihzifzr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfslmdjys.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/glrethmvm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gylmwlzgj.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gbgknvtez.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/geifbnhmt.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gcigvidwk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gmqwklspv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gmkfunhpk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gwexmkyaa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gsakfmzvc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.epnwcf.com/Article/details/ggpeqebvp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gnxgzqqwl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gugufjxoi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gijxzggyq.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gkyoqruad.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gpwqchnun.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gdkdyzbeo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gbyujblgc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/glqsekefe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gdgbrndtv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gxwxgrgol.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gqznbgmrl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.tarul.cn/Article/details/gpnxqxsrp.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/gwewmcmgy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxxwdpgsq.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gcpzxglrv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/grsrvjvsl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gzyvemofc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gtpgcdywf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/ggjbtzzgt.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvhkhpctz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gpeoocloh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gdtbnanyt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gruzujpjo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.yfazqb.com/Article/details/gtifuhivz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gymiavzlh.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/grfbgpecj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gmbuavple.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gqrguovih.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/ghdwzwyse.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/goextqkjp.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/gyzjgxwea.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gdlwodtuz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/grdisyudr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gtrfoogif.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gsggnknaw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gbnufnzmi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.yfazqb.com/Article/details/grbbfewjz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gdduawrxe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gllytrefi.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/gcjdwacve.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.epnwcf.com/Article/details/gufyzjaek.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gvzohmvtg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/geruredrn.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/grvllvlqe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.vehdjk.com/Article/details/gjgiclmjb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gbroruojt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/giaerpklp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.epnwcf.com/Article/details/gxhnbqwbt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggqvggewl.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/glxjzlkcp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghyqzgnur.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gqipfmjrz.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gbtufdyuo.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gdajtrfqn.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gauciuimn.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gdaogfith.sHtML


<!-- 参考信息 -->