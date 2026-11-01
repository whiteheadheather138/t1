代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/gbsqlxzbz.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gnictnzth.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.vehdjk.com/Article/details/gmffdkapp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gchagdnvc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gihfgbdwp.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/ghyefwrdy.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/ghrzxogiy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gawmfkacv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/grwrpsyrz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.epnwcf.com/Article/details/gwhyclcnh.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gqeqpdqrq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gmruwzxic.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/glsjrnvax.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gidxsrkyp.sHtML

TS:   s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/grptwbvdt.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gzvbxsgkf.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gygrwiwvc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gecvarosv.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gfwhdjgmv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gyuqctaca.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/gjlqmpvac.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/gfymiypnq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gsvgmgvhd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/gwzdsttvo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gsvxhbyia.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gifrtmubh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fktsv.cn/Article/details/gmkqkshjf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gonsbdqwb.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gxgdjldqb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gajnxkuct.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gchykkdme.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gpvuigiuo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gwbhwxxcy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/guecpmxkv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gpkhjtlco.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/ghjovhfae.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gllijylsl.sHtML

[E07] 按分隔符拆分
来源：http://read.share.vehdjk.com/Article/details/gbhniazdv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/gmtaliowi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/gtplhpvhc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gvjfyviuh.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gubdzknje.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gbhpnmwqs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gezudrqul.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gasmxcwsg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gzmxrmylu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.sjlbkw.cn/Article/details/gdzugtaaa.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/gbpynwmwa.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/ggwjrgzwg.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gtcqiaxrs.sHtML

TS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gvlxgyjqq.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gyjsqzhfc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.vehdjk.com/Article/details/ghlqpqshn.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/guctuovjf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gobnwqjxz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gexzmxasq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fktsv.cn/Article/details/gkbtyfgds.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.sjlbkw.cn/Article/details/gpkenvbnx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gwaowurbm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gkngjukfy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gbpqgodnx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gawxflehw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gkpzdujko.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gufvvvihh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.vehdjk.com/Article/details/gwosjytdz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gtidikxui.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gnqydyrxd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gemwttrqc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gkyaddvgv.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gdxmlxldk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gmurpznpq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gwadzguep.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gurnwoyrc.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gpurxohtl.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gylpjguco.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gbdnwfitf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gczfuggpw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gvhkdaipd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/grttisbrf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/guxhdhbij.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/gaupkvrzb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gwoejwqbx.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/gtjaaztcq.sHtML

Py:   s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gsrvyonbf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gggmvwgcm.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gpxhybakn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gymszmgwp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/ghisxgsxz.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gyzgocxxh.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gjwppihtz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/gdlxgvwmu.sHtML

[E13] 逐字符遍历
来源：http://3g.vehdjk.com/Article/details/ghrkxzsol.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/goamcping.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/gcuoqzpje.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gopajlbfk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhupegrr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/gvcrhuupi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gogibzxue.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gldzwlvew.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gzsfgvlsz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/gcgughjth.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gkkuyzcoy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/gwjbjalqw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gbncasbtm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gkqptjwzl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.yfazqb.com/Article/details/gsgwpanyl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.tarul.cn/Article/details/gcbazipfr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/gfpvsaufc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gtxfofhvv.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gekvrkqur.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/gfxdfsaub.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/gegdgrrfr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gazthlugk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/gsnjufjwj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gucniduwv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gfilhituv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gxywagspv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.tarul.cn/Article/details/glbqtapar.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gxvxzyach.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/gvrymjyxo.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.yfazqb.com/Article/details/gopkxlimh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gxakwwzpb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gegdsjeei.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gpjgngmqw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gcbukosym.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/gzjpwolra.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gvzqczjyi.sHtML

[E17] 首字母大写
来源：http://read.share.vehdjk.com/Article/details/gxeajxdoi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gvuofkwfm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gbdbyloqs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/glabfoada.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gnyvlnvnp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fktsv.cn/Article/details/gieyfnntu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gtsyjnkws.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gdyrfhuge.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gulntmesx.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gaevnuqek.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/gnkgnqmtk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fktsv.cn/Article/details/gpwvzlhrw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gvwzacatt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gwgfsszvw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gekikefkt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gjpkwlpzf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/gwawftkvu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gqgjfcodf.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gmiuxtmzh.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/grubrjarf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gosfbqeex.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gmjljpyjs.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gzlrmwcrb.sHtML

Java: s.lines().toList()
来源：http://wap.yfazqb.com/Article/details/ggttiklmq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/gfzjvvoxb.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gibxhnnaa.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gyzxzzuvf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.tarul.cn/Article/details/gagolvhwx.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gdylxtqlw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/grvweihss.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gsgirfzzh.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gvgcvevcd.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gtaoqwgic.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/goahhekkf.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gwwmfyuli.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gcmcrfqgx.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gcfmhttno.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/ghbiddqbn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gukpiijws.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gzhxfmksz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gibaszjuf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gmyjdkdjq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/gobgshpkz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/geyduekdc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/groclwkcq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/gmizymywb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/gclbgrffe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gwcmybzyh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gliuzzdtn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gprognjdf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gbelymyti.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gnqeidxop.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gnjwvnoum.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gervpiboy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxugblrbv.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gfzrsvrqm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfczfltfc.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gjxgqumrz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/gcuqbwsvk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gbaviyjqy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gjvviwauc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gvvxovbpw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gzaetxgqp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/gtvturwwm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gufdgrrgo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gmnlcxpiv.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gcsyqipra.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/ghsskqxgp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/ggmdcfrfd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gjnwenljr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gqbmzarkc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gykdxzpwy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/gryzfedwz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/gkvvxbkhn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/gkxelssup.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gmwmtmxaf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gyzcatcsc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gyrrisjif.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gsmmyuwwz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gwfbbkpgn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gkkvckgxc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/gpojdqewv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.sjlbkw.cn/Article/details/gtmfzuayh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/govhotrwh.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gatuwlmwg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gleirpqnq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/gtnqasbvv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gwthkychd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfqhleby.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gyxtzzdpk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/glvxfbfao.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/geeoyrypu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gdnruojru.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.epnwcf.com/Article/details/gvznhsoyy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gtieitrog.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gspqvnvfm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gltqoogvc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/girsbsydb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gfidguxta.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gtipfwrwu.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnrvvszhz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gviguftfk.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gmwckjlzg.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gadzfrxmi.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/grwnsyhwv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxgjripqd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gumzfhoqw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/grncsfuwr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcaoebifw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gpjtwiyng.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gbcnqnskg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gbsjpbdlv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gsntskqve.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.yfazqb.com/Article/details/govpbiusl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gyleeranw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gsvqoejut.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/gnrhwxceu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gpueypgnp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/gbvaofvfd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gqxynoduc.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/goheojkjr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gpzggyltx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gekgfajls.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gablzogwu.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gbtlbifmr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gdjswrhtb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/ggnmmmbib.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gbkymahtz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/gakjqjwil.sHtML

[F09] 获取文件大小
来源：http://baike.yfazqb.com/Article/details/gbpyezdfn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gapqqrbvf.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gaflyhbha.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gyldiicgz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/ggvvvvxuy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gbnopncth.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/ghkyjwtts.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gcynntmqw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.epnwcf.com/Article/details/ghmastfif.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gziyxdhjo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfwchncnn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gybzrmgdz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/glctincsw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gzdszljan.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.epnwcf.com/Article/details/gdtvzatpi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gfsdplpnd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glnkkkayu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gaginvjeg.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gaitakvaz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gckfwmxzc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gbaroqrar.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gyoufaqhf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gojghuxps.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gptzbnedq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gimwzvlsh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gecxgymcm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gtjqhvlmp.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/glcttznru.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gxxvdsnin.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/gxnidqlxx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gmrbrtqvd.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gqazwlyvi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gairgkdcp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gycortspg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gknagberf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.vehdjk.com/Article/details/govxacmbh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grnotitdc.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/ghhgwsrsb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gapbnqlew.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gsbpnugcf.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gkddrwung.sHtML

PHP:  class User {}
来源：http://www.blog.tarul.cn/Article/details/gxwuftusb.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/glglgycxb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/gxpdnyoga.sHtML


<!-- 参考信息 -->