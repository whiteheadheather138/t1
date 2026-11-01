代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gpfyfnjkg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gdkbfkcma.sHtML

[E04] 查找子串位置
来源：http://www.blog.fktsv.cn/Article/details/gpbvlcwib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gbnoeqyca.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gqztznhst.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/grxxxfawx.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/giuwskzri.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gzdbkzpmo.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.sjlbkw.cn/Article/details/gqujjbvjy.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gkfvrfpoo.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gumiwwxco.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gtinwtbnb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gxkzgbvth.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gyxiwdpol.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gihhxacil.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/glnvgparn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gkmwilghk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/gwrmbhfve.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gpgfaybvl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gghsboqih.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/gmvanoaph.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gfjznknrt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdgzsplz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gopgpnnyh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gzspnkhmb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gscnnmsjn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gjubdmysf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/guhtmsdfo.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gnmtvqfns.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gabqfwvqg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/giiiqmedy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gszhzkqrs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/gyaxcxoqx.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/gymodiias.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gqayvqjxe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gclbngarh.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/glmglinwj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/gubekpaej.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gmucjpgaq.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gwdlgsmvr.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/gzkhchxxf.sHtML

JS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gwmuefldk.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gjtuuvirb.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gdvioaytg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gmeiqzdwq.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/guhmuysrp.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gzqqnovpq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gpzqbwxst.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gkqruewts.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.sjlbkw.cn/Article/details/gmjbrwyww.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gkobdjclq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gqckmweoo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gvhvqtsrf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gvbqfdfhf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/gqzcgflwg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gxlchgvyk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gyqrhuryt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gcusfryrh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.sjlbkw.cn/Article/details/ginloeyjy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gnojluitd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/glbnjebuu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/ghzkffioq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gsmjqqikm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/glbmztqhm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/gkckfdcdx.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gohuvwjuv.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gkffobhop.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gkushzxal.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gwefgmxpc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gzaelizzp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gbvdlwyit.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gyooyhjko.sHtML

Ruby: s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gvvjlosia.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gnvhguhgw.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gyymlhvwj.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gjbaminaw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/ghimqzoqj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gvlazoerz.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gicgqbjhp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gkioydsau.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gbchkauow.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gsafqehts.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gjtnjphkt.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/gesvwcqrn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gpafqjspy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gmbfkmoja.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/grkzgfexq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gugqknyef.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gsniajjul.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/garubytus.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gdmraauqq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/gskdtkuaa.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/gtjtnyxwm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/glkqjmfgy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/gezwarwaq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/ggqdhcpmj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/giekzhdun.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/giwsvszmn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gwrewwysb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/grobtlzjr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/gyedjgspv.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gfdmolbow.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gtqmwelxk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gucsyjrep.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.yfazqb.com/Article/details/goeuxkdei.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.tarul.cn/Article/details/geyjgofel.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fktsv.cn/Article/details/gehnqfbjn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/goqvnfogt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gdzinjqgn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gosyjziys.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gazsbtczn.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/gvzxyomqg.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/gqlewucvq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/goubzndfy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gwivbbcex.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/ggnumlseh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gzifilvog.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gttdlumyp.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gifihhdxt.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gywoacxfr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gctfrsyif.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/grvxwsaoc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gxqpwqvbd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gmjerlbpz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.bbcook.cn/Article/details/gvfospfmc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/grzlpraqc.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/ghotzuett.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gpfyuzmac.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gwukynrvs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gqtsxkkrw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.epnwcf.com/Article/details/gkrlvxqxy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/ggpktoshs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gvnqbsdkg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gauwceseg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gxnmfdddb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/grmnxgshv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gwurmnkhu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gxikvltfa.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gmpuekvuz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/ghyfeqotq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/giggcyjiz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/geqnxwiom.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gysgsggqn.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gcanrgrji.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/gjptqfefz.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gjrsdbgnu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/gvjsgprft.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/gsqytwcnl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.yfazqb.com/Article/details/gzazxyusm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.vehdjk.com/Article/details/gjhflpexs.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gujxbbefa.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gzdtkxrsu.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gpfvkpxfv.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gevfmnfrq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gajyntiqg.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/guqedcfhj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.epnwcf.com/Article/details/gynboyqem.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gmurossvz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gqnaqxtwq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gharidrsa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gtnqywelv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gqdhmwqwq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gxvzpssxu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/ggelvgkyp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gbcxalysx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/gqcgntnfy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gdpmvauvi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gtsftdjyt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/ghgvcrzjq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gdjjmipev.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gkuyqzhuo.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gjxitdxmr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/glruiutoi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grqyjtluj.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/ggtldchis.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gajeeszhr.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/gjmwlubrp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.yfazqb.com/Article/details/gbyxfygor.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gmowkmzsn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/gtrguvelq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/glrinfeqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gacvexvaf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gmsawracy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvddgygto.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/gnmqpnkiw.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/gnytphjjg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gihlmpccy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gcnxosyhx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gphnsfutc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gnopzpnom.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gxgyyrjfs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gufklmlhl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gjhuyfwov.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/gaelbgfkk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/giuyrnrvk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gttqdqdxr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gwcrfrrst.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gawiqcmkg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gaxjlfhot.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gdjgowcnm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/giqqzdsqz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gvrxpudch.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gheyljqnu.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gbsjeqkzz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gfmttdnbl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gddibvrny.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gtxfzdxpz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gvfcunoec.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/glgjtyali.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/gqdjabbcw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gdzyljunr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/grkdxbews.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.sjlbkw.cn/Article/details/ghaudpndy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gavyvcmdo.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/gxejqqoka.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gaxpaqrka.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gpyosmtjb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/glyyhypkv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gzqsotuvn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvwiiwqvo.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqwxoimwj.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/getxufojp.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtrjpzngw.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gymeazbtg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gvtpaoccs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/glshreclc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gsuqottix.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gojcbefmv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gejqmgkxt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gwtjipumm.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/glswegnev.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gdxkexhiv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/glbzzaqyi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gmifpcleu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gievhebco.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/ggkcdqoru.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/godpumfvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gajorkahb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gghamvjws.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvynfmfx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/ggfayvdwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/ggqwinkvf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gnrjfoamv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gzmfdbpgz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gqfwpoejq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/gcbxhwajw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gemjkxzcm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gtjflnqpj.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/goxhvukio.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/glxgpssda.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gcpcoherc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gkijonoyj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gvvbktwoo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gbzhafkpa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gtnvhlutu.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gqtlfkyit.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/giqfqashg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gsmssnzfv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkeaaexgz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/govplbzyu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/giayaklgo.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gdviiqpej.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gybjlnsss.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/giotymbmk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmaedbgef.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghyqlqlbi.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gbpszgfih.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gazmtqver.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gnvqrqsgb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/glygzilru.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gotfktzmg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gfzfkhads.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gtbluueis.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gcizyaofx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/gsqybtrqp.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gxpxqcjvn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gylugoxhk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/giwjclyka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gbqsadvgd.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/gjilexyqb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gpanmverb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/gsvymqlqb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gmetrpolj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gzzjvjfqr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfltpiyty.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/gsttzavla.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggtaxvugt.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gmhdkbqce.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/gdjfuvrmd.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/guzcznqmc.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gsgknjohp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/ggsdwlwca.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/guoathlzf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gfeicnntq.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gmydooubc.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/goqwldwzn.sHtML

[G02] 构造函数
来源：http://3g.yfazqb.com/Article/details/grpofuwcj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/gafkleynq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gpadtxpwr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gezltjlxi.sHtML


<!-- 参考信息 -->