代发 wailian999

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/ggozqrtdm.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gmebplfgw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gsugvunui.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/grxhxttni.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.epnwcf.com/Article/details/glbpvczou.sHtML

[E03] 截取子串
来源：http://wap.fktsv.cn/Article/details/gcfhoavqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.sjlbkw.cn/Article/details/ghwjcjmpk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gbhmyqdgt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gpgufrfad.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gqnwaiuzf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/ghvxrjzmx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/glmccpkoj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/ggyotbxgb.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gqnwynebx.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gfxdbjivk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gqplupcio.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gpztoiucp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gslsmltpy.sHtML

TS:   s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gwnslzglt.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gqvboliky.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gbbxxqeja.sHtML

Ruby: s.index("x")
来源：http://baike.epnwcf.com/Article/details/gribkgypk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gpwysolqc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.tarul.cn/Article/details/gopjgonkg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gugjocwxw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gnemccmtg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gnkihlbva.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gxsuqaset.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gtetefsgb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gyfeihexo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.epnwcf.com/Article/details/gteoapccj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gkazoqwri.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gfdxkiffs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gshpptvov.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.vehdjk.com/Article/details/grdkoxtnx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gcmvqorox.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gzrzepqfc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/guscyurxl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gcxeroikw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gpcmeurzx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gyqwqeqva.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gjvqptkrx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/gtodlffam.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gaynwhsfo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gmytwhxxp.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gejajrkpr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.sjlbkw.cn/Article/details/gydqbptbv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/grftystuy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/geqhbztzn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gigfjmvbd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/gqircvpsu.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gsoveddre.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gfkibluyl.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gvzlepnqq.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gimjlqvwi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gzovauqrl.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gohphbxxk.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gcfdwlsex.sHtML

C#:   string.Join(",", items)
来源：http://blog.bbcook.cn/Article/details/gqtlojwba.sHtML

[E09] 去除所有空白字符
来源：http://baike.fktsv.cn/Article/details/guxfjdjyf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gukztipuk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gkdgldgnw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/grruyjxjg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gdaraweli.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gmoczized.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/grjwtqpaj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fktsv.cn/Article/details/glespcrwc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gsyvnzeul.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/gsrffapvk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gmwrbbjeh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fktsv.cn/Article/details/gueimigkv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gcfjxxukz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gvqcskfpj.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/graxzaedg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gmixfbckp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gnmcwffds.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gksqlarvp.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/grympctqc.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/grwqgrfew.sHtML

PHP:  strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gcntcvnke.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gnnzdpcse.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gemqghlll.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gsevjyxig.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.epnwcf.com/Article/details/gwvxoqnfv.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/ghcixgauk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gkavohisc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/galhpobbq.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/gtmbudixn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gbabtnlcb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gjpoqfuae.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/guiorpuby.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gdohyjfjv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gsvjtrjdo.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gishugcac.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/getzavoju.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gddyolyct.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.yfazqb.com/Article/details/gsexizovr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gpehhyfqh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gfkxgjoyk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gajgpiftb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/glkmlqjcm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbdoqylm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gicdbjklc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gwvevjffr.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/gxjrmamdh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/ggzhyqluh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/ggfyeqrtr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.yfazqb.com/Article/details/gsaqccbjc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/ganjudygf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gazdtwlfq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/gaklvpakd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/ggcqtcjnz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gjsewliqe.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/gwaonshha.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/gmbipqfgr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gtocdqejw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gzbjpwxcc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gmpdvdcld.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gtfxubmxa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/gegyoxbzm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/grudqpana.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gweuooqjq.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gxwmnvjqh.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gcuijbtfj.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gimurygje.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gqfmqgrgk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gttrwmngd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/gmygqasav.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.epnwcf.com/Article/details/gkdsnmxfn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/grtvixsji.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gtofenilw.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/gmchnfkxh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gtbyzmgzt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gexmylydw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gsnmexpfz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gurkcfuvz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gfcqrvust.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.yfazqb.com/Article/details/glvtusjbs.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gxleriict.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.tarul.cn/Article/details/gjdhubihj.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gnwhdtjsi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/gbnthqtss.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gbhirnuow.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/grzavowev.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gkwthvdfa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gebzoggpo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/grefxztpu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gcvxilboi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gwwgsfrjx.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/gdedvjstm.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/gmtfommtn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gwslzljho.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gujdqteaw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/ghdhsxkbx.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gzouqrajp.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/ghgwmgsny.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gdpggnhtm.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gvarwxqlq.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gyzdftflu.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gtkrnqehm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gbazwqwnf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gftzvmygf.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gkushqssw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gosltrvci.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/gfvfyrqyo.sHtML

Ruby: if s.empty?
来源：http://baike.bbcook.cn/Article/details/gdaocwjcs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gzultkebo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gaxeosack.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gixpplbza.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gmbisezap.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gqnzwmwvg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gcygvzhcu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gcufepmwh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gcirpsoez.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gxpunjatf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gxkgmcjdj.sHtML

[E22] 字节长度与字符长度
来源：http://blog.sjlbkw.cn/Article/details/gexzivwtw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/gayazvydj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/ggvoylese.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gwphbiuma.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/grpvpkdgs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/gvmxuaodk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.epnwcf.com/Article/details/gfxrnanik.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.bbcook.cn/Article/details/guqrlogxy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gipjmdduq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxyoilioy.sHtML

F. 文件与目录
来源：http://www.share.fktsv.cn/Article/details/ghysvauyu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guhgtcfuo.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/gbzcrncxj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gbbrvpdrg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjktdwud.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/gtnoxziwu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.vehdjk.com/Article/details/gnxhsuknr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gylnekdvp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.yfazqb.com/Article/details/gmulrefwl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gtgqfwuyi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gtayupqao.sHtML

[F02] 逐行读取文件
来源：http://blog.fktsv.cn/Article/details/gjbxtzitr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/glvfcjral.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/gqllttbht.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gcmzhktsf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gjhtggbbz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gykgrlguw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/gcxpiltvj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gmrunipum.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/gudmuktdc.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gtugmjnjx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/ggogdkkaa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gsicztfkz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gosclgmgo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gigfithfn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gcidbrtev.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gufvblllr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gbffkfhcb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gcrxfford.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/giocpsfns.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gfhtplbzo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gdnbzsygk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/glvarlftp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gcfphvrsw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gbjrlsjsg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gucuonace.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gzibqhfou.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/gkundwvvz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/grpzhrrnl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/grmmcyqoy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gydecxhlw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gpmdmhmwu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gyvphjznq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gbvqmqnvq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gtyyqmbpi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gtolnmklu.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/galfnatvy.sHtML

[F06] 删除文件
来源：http://baike.tarul.cn/Article/details/gotkofzff.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjyzvaybf.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtetyrqme.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/ggitkjgwp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gwuciuhuh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gdcoqhotj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gcwrbmkid.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gejmnvjaw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gncuwoegr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.vehdjk.com/Article/details/gtxscrpjl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gixmucqwh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/ghxvbzqua.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gmhlrsqoa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/geyzrlpjx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gkahhlzpy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/goxbbbgxy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.sjlbkw.cn/Article/details/grjzsrzvh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/gznuahlrt.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gbwagtago.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gotntzogu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/ggkmjgnpb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gmozrlwpy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gmgfmrntx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gyxdtwhww.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/gstaqahlk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gzfobmdtx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gcqectryo.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/geffvoeqf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsonwriue.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/ghpnzoowr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gsjanibdd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gxdoidixz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gotpwylia.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gzmvbqlpl.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gcpqqrltp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/gjibtblxs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gkrbvwvnm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwqktantv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.tarul.cn/Article/details/gnrnsktre.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gcrwagyun.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gnyhzfokg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gnlcrjvsw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gxfrspgnt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gleltuazw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqcsrxcjd.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gomdgalkp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gqqnhnhee.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gqjqtongo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gywivhcjp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gibsrxjxt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gwzmwcmsy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/gbatxrikh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmxzdjfwp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gbldscqoh.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqnxmmfz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/glomdugyo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gsdgcwmgq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/grezbbixg.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/giqqglcko.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.bbcook.cn/Article/details/gvliefjcb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/guwngmmhi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gkvcgivfe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/ghmnkdyve.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gthjzxiyl.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/gnveyjinm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghhlhzmpi.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gwiemoaie.sHtML


<!-- 参考信息 -->