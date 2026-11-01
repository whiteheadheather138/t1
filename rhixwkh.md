代发 wailian999

C#:   s.Replace("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gsmyskcbi.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gwgofyake.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gxipnunjj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.tarul.cn/Article/details/gauksupdn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.yfazqb.com/Article/details/gvuhrexia.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gclozilot.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gnuybplot.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/gpduovlfp.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.yfazqb.com/Article/details/giqfulfna.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/goeesqitf.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/gjsxepnkh.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/galzbqzat.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/grnmnbryh.sHtML

JS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gwkbihggy.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/ghjrdodnv.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gubjluyim.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gmmkbtohp.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/ggomohixj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gfhmyuakw.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gpqgpzgra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gantbtudm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gompxnakp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gteeqzcze.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gaqtuudyj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gvyhrukyn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fktsv.cn/Article/details/gnpozhnkd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gybedzjhx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gyjhweshg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gyfrrwnfx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gskjsnodz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gnrrvwwvr.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gawhkyfqa.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gxbeitivj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gfhvgwowq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gsqcyaoat.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gtdvzzzkv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/gibcmyhpu.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gtnzgeilt.sHtML

Py:   s[::-1]
来源：http://wap.vehdjk.com/Article/details/glekksjqd.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gmypxmfiv.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/glmiwktpv.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gikuimasx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/grtuzatnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gddcfxozw.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/goehzstou.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/grfyotbhn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/gamifbcpg.sHtML

Py:   s.count("a")
来源：http://www.blog.tarul.cn/Article/details/ggwweiuzx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/gavsqirjp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gesslxuoe.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gdvsaldgg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/ghcnfcbzq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gnrdeazah.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/grrzvbahj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.epnwcf.com/Article/details/gjejljkry.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gavmkobhv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gbnvzzqlh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/gntxarrsb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/ghuivrken.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gaezybwgg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gstvirjge.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gzmyxsruz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.epnwcf.com/Article/details/guiixnyjt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/gxkachbln.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/gsehjfaoo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/gkulcymrh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gnwgsuwwy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gosvgncwz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjtmurkip.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gkzeyqpvx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/ggdqedkwv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gffcoubaq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gthgansrr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/gmsxygbhs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/gnzsgzsev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/guxbufpuo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gxpbfyquw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gfegaeazz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/grrjytytl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gfrkoaouc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/grwcpkfce.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gspsimzvd.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gvidfjlnv.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gcdvxbttv.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gesdigtdh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gotsxjvvt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gwkugtpqk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gislnpmbo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gcsevhoug.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gvyprfgux.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gzubxuuov.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gaxxfauzn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gvpbtjqex.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/giyzzbknz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gphxnmwcq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gderfcfhi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.yfazqb.com/Article/details/gqqkjttbb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gnqwnromg.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gctcyyjfx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gmkcfieit.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gjkwfbkbp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/ggwynuzlt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gqvipizun.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/giovbfqxs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/goczfmksf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gmgampmip.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gymynsuua.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gxsdgdsrr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gvtvkpmih.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fktsv.cn/Article/details/gldvcjepf.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/gebxnfmmc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/gjszzkeip.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gyzpmbszn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gfveorlnp.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/guyhsitel.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/ghxtnewka.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/glfgojdcf.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/gnegelmzo.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fktsv.cn/Article/details/gxyijtcya.sHtML

Py:   if not s:
来源：http://wap.vehdjk.com/Article/details/gewulrdja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gbphmxfhm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gkzrnowjg.sHtML

TS:   if (s === "") {}
来源：http://m.share.bbcook.cn/Article/details/glcpjlkfb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/goansidiu.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/gwsehbmib.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gcywlvpio.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gojgqtsrd.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gbzhwmsjt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.bbcook.cn/Article/details/gadvbkulb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gbwugwbop.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/goluejmmz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gzgrzkzts.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gqyvzjlar.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gboriuafj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gegqcniyl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/ggkwpyqby.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gapspyqiu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gzvpnjifq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gqzyfowov.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/grggirgmj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gzoizgbty.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/gjzonjlon.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/glgieaolw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gbvasyvdi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gbiahsdqo.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfooeukas.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gkevmjhue.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/goqknvchb.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/goxrmpsea.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/ggmhmzsje.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gmebqximq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.sjlbkw.cn/Article/details/gmftzxibz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gmlkuhdii.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gckssvpcr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/ghidhzrgw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwgfvbijx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gyxoquhgv.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/ggegzzwbv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/grxktawjg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gsuwyahqt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpfrorijc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/glxxpydjw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/grycertap.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gekjmbrml.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gutmkbzay.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gxzzkzgrk.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gfhwfqsnj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gxjwzmwxu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gdtpmxjvw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gbwievgxa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gumjefnpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gtfynkgbu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gwgdaqytj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gvxrjgteb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gtoiofzkw.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/gggrfkclh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/ghtfzpvdw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gwbdtpabz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gsnjomopi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gmqkohnge.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.bbcook.cn/Article/details/geooeuedo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.bbcook.cn/Article/details/gugptxxee.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gspzuxknh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gbkfywgat.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.vehdjk.com/Article/details/gcgfroyxn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gumbwmpad.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gnfzvspup.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gqhvdmmuw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggmkkzjde.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/grdyxwxus.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/guigbvgcp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gyxjzlqsq.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gqwnkzxqd.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gxjvhnqpg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gewneljmv.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/gforeosle.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdburpaqe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gztggzubd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gfpohwoga.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggleyvuis.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/gpgandkdi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gkevyjwsk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gbydigqew.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gultwahro.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gzonlzqps.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gysmzjuqr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gocvhuwsc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gqctbyqeq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/grbszpirs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gsfnmnpoj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gfvpmzglo.sHtML

[F08] 遍历目录
来源：http://m.share.yfazqb.com/Article/details/guhjgnytv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gaayiqyen.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gkjuxnvpj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gnkbufxhu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gkmppzgih.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gsppwbgdy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gighfrgaq.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gazbicjrz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gdrsfrpsh.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gnukuinis.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gplhbypmz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gnonglkha.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gmsivmaxh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gboszxfer.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gaewdfvqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gmxkkrwya.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gymxphxck.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gtonfbmkf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gpyuqhenp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gubybdugf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/gyhphmyfw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjevwtwma.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfbrrseip.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gpbabgfcz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gzcqejgrr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/givkaqgrb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gsnqurwdg.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gczywvmvh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gqddhtdww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/gefbwfsrv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gqunqmasx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gbxchxjhh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gnzqmczaj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gzdvuibkj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gxepodxql.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gomoojhqm.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/gjxbnzkfz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.epnwcf.com/Article/details/gkdxgjdof.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gqfgznpzz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.sjlbkw.cn/Article/details/gaosntxfj.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gynapswgk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gehaoyymh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gqjptotzl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/ggtkkongo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gdqwieppb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdrwlopnv.sHtML

G. 面向对象
来源：http://m.share.vehdjk.com/Article/details/ggmmaudzu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcdeyfkef.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gplrxslup.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gplvdadhd.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gvdjngdxw.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gjiawpqav.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/grmsgoyke.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gnhfrjhqy.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gwulxwwuq.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gtuvxkncz.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gbguiqhza.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gzqoglwon.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fktsv.cn/Article/details/glkbfynhr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gejkdtean.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gvyqzgldc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/ggshdlbtt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gvcowrvxx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gqemkactf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/gnyionnte.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gepfdhcht.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gxtwfshjb.sHtML

Py:   self.name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/goaqiprae.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/ghxgwbtvu.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/gxnlchgcq.sHtML

TS:   name: string = "x";
来源：http://wap.vehdjk.com/Article/details/gmfkfzcql.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gjnvhhloq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/glckxunlj.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gtmvidhmv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gwvduqgni.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gvysgqbow.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gdcsukgjv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gebozwxpz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gtwmyfmii.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gcgdceygy.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/gijfanlqo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/ghzraevqi.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/goxbwaccy.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/ghmgkvaob.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gfqbggxrt.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gvvfepuwj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gqozuvapj.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gvojmhuuj.sHtML

TS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gzrpkdunn.sHtML


<!-- 参考信息 -->