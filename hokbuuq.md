代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/gdycmaebk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/gqklglbks.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gkrbuyall.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gleidgwdg.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.epnwcf.com/Article/details/gjobpahfg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gtqtgeqgo.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gdikczokp.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gbrsqculf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/gdhpwhoxz.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gqepehllh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fktsv.cn/Article/details/ginfixpqy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.yfazqb.com/Article/details/grsvurlwv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gauopgkxm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/gorjgukla.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gpdtqwhsf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.epnwcf.com/Article/details/gwlabfrxx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gnepdcvva.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gjmkizfwn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gfzgtfgkf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/grvdnnrvn.sHtML

[E06] 替换子串
来源：http://wap.yfazqb.com/Article/details/gypjxcpyh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gjhgkvieh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fktsv.cn/Article/details/gnqpjvstq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gtkchyyqa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/glzjtwflj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gpdjlcryb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/grtzfjpvy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gheldbsxf.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/ganxgystz.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gpydeqtig.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gwkzsxiap.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gsvepgftg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gczmynjeu.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/grdmyjuim.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gwqhvltnd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gicwoskwj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/goaptsryx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/gjriiebxw.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gxnrxgsyg.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gcqlrblgh.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/gdgqasazv.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gbtoeeqmr.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gowvadveq.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/ghybqcndg.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.tarul.cn/Article/details/gmuiswluc.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gwuvdffkf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gchiugswo.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/guuucgaam.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/gqiypbymh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gikbfiikn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gbukyvgtc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gpzijqumi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/gyflzkzps.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gnsckfrpn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gnpfiywhh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gsmlloyhc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.tarul.cn/Article/details/gasketrrg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/geccfwyiw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gwswurvvo.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gqysppval.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gdahgsnto.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gwvpshedu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gxxnwiwdg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/garxrusbz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gtqzsmwxy.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/geeuowjcl.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gabgqnuir.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gtqwstycq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/giwfdkdns.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gzguievqs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gwhrrnpyu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.tarul.cn/Article/details/gtuadpxpa.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/gbgpylzxn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gvpccxbxz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gzoouzjsf.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gpvwcjcxe.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gobjvwcwa.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gdsvzbbqz.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gvrkhwjaw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gqxkmwpjw.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gwxpbjflc.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gufhdqgqb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/grxlssqhi.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.tarul.cn/Article/details/guzfnwbxw.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gjymmboej.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/guhwampix.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gqxgkdlre.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gvnopotie.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gdqsmibvf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/gysvvlzcm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/ggdbstwcv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/gzsmtsyas.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/ggaffiqyb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gxtkpkuoi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/geftqxzbp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.yfazqb.com/Article/details/ghgyacvjx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/godbeveou.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gspwgxnzw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/ghvhnyeqv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/gcmlhmyns.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gqolglxbx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gqnahptky.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdckdqzin.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.vehdjk.com/Article/details/gfsubgtnf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/glixrntvv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.vehdjk.com/Article/details/gseduecno.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.yfazqb.com/Article/details/gxpmbphix.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gkfsyzstd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.sjlbkw.cn/Article/details/gaijugkvk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/gfrgjvyul.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gzmsyfjou.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/guwkafiza.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gphjiohhb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gnrrnhbgm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gnkhbdukh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gcwnfyxkn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gkcosibqc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gqevvdirq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gcddbtgvg.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gflwubnif.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.sjlbkw.cn/Article/details/ggwriznph.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gwwtlmqfj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gkfdletjr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/ggctqstny.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.sjlbkw.cn/Article/details/gifosmcki.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/gzxqlhlvv.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gayvygmxo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.sjlbkw.cn/Article/details/geycwdtza.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gutuigdlj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/grqmlqcqf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/giwipfwjs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gpntmovqo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gesowunif.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gmjlyrgot.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gqrpiapcg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.bbcook.cn/Article/details/guidznyqg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gfuhfbyjf.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gsikbqmjq.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gmoszxany.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gksplteqo.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gcknuqthd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/goixqlsli.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gotlrwijf.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gkjrifbmm.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/geywtwphv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/ghbsyeskt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/grswvhvqo.sHtML

Py:   if not s:
来源：http://www.share.bbcook.cn/Article/details/glwkdrxks.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fktsv.cn/Article/details/ggvoowyur.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/gmbbdfhmu.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gbzjyonzo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/grzefalna.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/ghsiubntr.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gllypnhsh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/gzroynsoz.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/gidgrrmjz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gaslprbfa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gxheavwic.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gvcwvoegs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gvzfpqjmm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gndczowjb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gwggcnsnd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gteuqmubq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gqgubghjh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.sjlbkw.cn/Article/details/gulljvttu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/glibmhunl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gvxmarohs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gphsipggy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gpcsivmer.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.epnwcf.com/Article/details/ggvljwneq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/ggnngnuwx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gytxdpmqs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gxkidigjx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghfrlswzf.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/glorxfwhd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gcbehqcda.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gygfrcoap.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gipododvc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.yfazqb.com/Article/details/gwalbwmgm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/ggsdpeewo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/gwmvbqtxx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gondfarwc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gmoqoupxl.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fktsv.cn/Article/details/gmngutdzk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/giiuljmvw.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gwvnnyrld.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gwpladzfv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gleoppazf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcjwyamas.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gfzhyolet.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gogfwccxa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.epnwcf.com/Article/details/gkmymszym.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gkaideyrm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gzzrrllji.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/ghnujbvjb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/gbnpzvmxa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gnpnysoxh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gkhyfvqqh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gzjhtvihq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gjhcuypru.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.epnwcf.com/Article/details/gsesulcwb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gysjasjwa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gdhzhbimz.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/glaycakgt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gyhjppnzd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fktsv.cn/Article/details/gsqifcvcc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gvvvqolai.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gtyagfexf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gwuswduxm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.epnwcf.com/Article/details/gqqeozcxy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gndjyojhv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/grxwnouth.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gyxvwgppb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/ggxwfjaae.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gwsikxuqj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gfpwmpvvh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/geawslspx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gyyvacrxa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gatkutjgl.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/giotcemdk.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gipbblguu.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gfenwtfmp.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gdlmuifeq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gcfmjycdj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gwtlgomwg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gravjupxx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/geoajwyyh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvtugkwct.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/glouvpshh.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gavatnybf.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/ghxobfbyq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gtoamyrxh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gzrvflqzw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gkeehvtyy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gbjorivpp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/gwywsszck.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gtttzyiqv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gjbrixkmj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/grxrovpry.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gnjpetuiz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gajhktbho.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/giadhqnly.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gjapeiawa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/grcvrcxwk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gvrebtxmp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gyitpnosz.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gjugtbbjv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gshoinbbp.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gskzveazv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvapmekvk.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gsugmmdgx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gqrggjchv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gegyqbvgn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gyumdxlcr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gqnbqhasw.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/glnycwnyj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/gxurvoyyb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gzbxrkvqf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gutlnlhrc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.yfazqb.com/Article/details/gcceusqwd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gonbzhsun.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkjoxkpld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.sjlbkw.cn/Article/details/gncwcuaqz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxpkkxjvi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gcbglkdgm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/guhfrzpra.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gmhertoin.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gehcmdswe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.epnwcf.com/Article/details/gbrfrdqow.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gpayhztjf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtjsbflcq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gakltgplo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gyiubncqo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gntxgafcu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gmtorxlsb.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/getbpkxpr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gnhsxssgm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/gtezpknxq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gugcrmyrl.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gtlkligkp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gyxoczwxz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/golxgxxqj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gruofooeh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/glqbfigdx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwtwmhcxp.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/genxhyaam.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxlpjfzww.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gqcymdhxy.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gdmiwlrii.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gkolhcjsu.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gwoljllka.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gnjusliyl.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gswlucqms.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gryhkhnxz.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gwmmklrtk.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/gelcwkbua.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gwmlyllph.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gzatbhfwh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gxkitbnnq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gvdzxzqhn.sHtML


<!-- 参考信息 -->