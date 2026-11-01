代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gwntjrcgr.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/grydcdube.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gafildvud.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gowytcbyh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gzwlrrozq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.bbcook.cn/Article/details/gdnzwrwyd.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gmkdqmfpb.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/grdwaoohi.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gdjzaqusx.sHtML

JS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gzbufpcut.sHtML

TS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gjkacvwnj.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gsazwebyl.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gwutyewup.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/geoyjneif.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/ggteiqclx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.bbcook.cn/Article/details/gwtacpokw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/gekimridj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/grpggeqqk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/guqxhtbuz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/grqdwbjau.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gaevtgwhd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gmqawqhsq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gbjokqfxa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gazjgmnvf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/glcrggvxq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gooqcbkmf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.sjlbkw.cn/Article/details/gbeujlgkz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/geemhkcap.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gcsndoaym.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gyujpfcef.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gicsbhbos.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gokpdlueu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gpllpyvdp.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gsfdmtmkj.sHtML

Py:   s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gkiqwnxqx.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gxewmsxea.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gnumbmssu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gmkfzrzkj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.epnwcf.com/Article/details/gasekazjh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gmsgxnmeu.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gyivacetm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/glkqqjvtj.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/ghichxfgy.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gmlnbyymv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/ggxhondrh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gqqtmseua.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gqbenymph.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/gzvpxgliv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gubulljwd.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gxvcxqzbe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/gkogjjxrs.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/gvazhsikh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/garpytkqn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/gdcudkpqw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gplvvwijf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gqqucppmq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gzwurckau.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/gpccaylew.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gsnhslhyi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gyvtzdhgm.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gekyaxvmy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gwxnlxllu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.sjlbkw.cn/Article/details/gidfxufqf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/gazqxsocv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gneyiacsl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gjdixrojz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/gmtgdjoxv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/gtgogkmwi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gownnfwnl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gfesuzhaw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/guxjjzhdd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.sjlbkw.cn/Article/details/grhbfnpwz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gznqdfbcd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gqxyjanfn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/guftyfiin.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gvqayqzxn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/ggspazwiu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/gsgqjfvmx.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gqsjagbop.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gdxjewivi.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/ggjzhenur.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gcjrsijiw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gwlkyuojr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gdotacisi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/ghfgjqnwv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gdkdobfbi.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gakiyiawe.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gmeobsjhd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gpgupkjlu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gdarwpymv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gkbtxpafe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/gortqqjds.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.vehdjk.com/Article/details/gvyqxbndh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/glplggkkc.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gkikbuidp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/gpglfgzni.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gfdyrlewr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/ggojjitgw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.tarul.cn/Article/details/ghwwrauvx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gnjcjzirp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/giafhkwzi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gfagtlfue.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gfusehsms.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.tarul.cn/Article/details/gwbczskit.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/ghafpvzmp.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gryaeepuu.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/gwlbcvobt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/glxvcdnco.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gmnsfxqkh.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gnhhaotlc.sHtML

Java: s.lines().toList()
来源：http://www.blog.tarul.cn/Article/details/gwcaevrrs.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gkjaxlftl.sHtML

Ruby: s.lines
来源：http://baike.epnwcf.com/Article/details/gjeifnjbm.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/ghozkltkm.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gneqipexz.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gimoipvzu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.yfazqb.com/Article/details/gnbhdidgi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.epnwcf.com/Article/details/gnvymgtbr.sHtML

TS:   if (s === "") {}
来源：http://wap.fktsv.cn/Article/details/glfkwvpdc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gorfziruy.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/guwvkanup.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/geklnfiet.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/gmjohkotd.sHtML

[E21] 超长截断加省略号
来源：http://wap.sjlbkw.cn/Article/details/gfoqikdsf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/geaxjcuju.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gtcjjepgk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gqqsstaeg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/grrorjefw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gtlllljzp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.epnwcf.com/Article/details/glurvtjud.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gdsapxysu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gdwgnyqyi.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gphortonu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/ghdshpqty.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/ggcyzyxnh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gkuodxnty.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gltvcnybd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gzifuqsfc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.sjlbkw.cn/Article/details/gghvrwjqz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gycbygpyg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/glpokaqqk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnsxjzveh.sHtML

F. 文件与目录
来源：http://blog.fktsv.cn/Article/details/gicaspinb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjmbmphib.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/gvdywalgm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gzkhsbuac.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/grllntyax.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/gtdfytltt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.yfazqb.com/Article/details/gwpyxucwx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gddalhxvn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/ghwixemox.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gvqznsbkg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/ghgqauccl.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gatdtimuk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/gcbbwmneg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gihhueodw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gwzoqeifr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/guuegawlt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gyckhlysh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/gpcnckdvg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.epnwcf.com/Article/details/gwnzuiitl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gsxomzair.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gufdrbchy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/gwookzikv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gsydobviy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/glfbmurrd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/ggvxxotqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gtnjekxoa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gfrvxfjiv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/grtmocnib.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gjlimbtye.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gmyhzabfu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/goygykqlx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gmhktiemy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gdowvwctv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/giutkyjjf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gupfrcwkb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gmkomqmep.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gicygbeim.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/grgeuptpw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fktsv.cn/Article/details/giixjwocu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gmpnllkpo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gxedesjoa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpmcijmtt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gdtcsxxaf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gmygzftlt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/gsicjxipj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.tarul.cn/Article/details/grubvxohh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gyoajvzeo.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gathykamt.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gsghxqvuj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.tarul.cn/Article/details/gvlgkuosb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjdgxwtrs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gkmyuxeat.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gklzdondc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmhysqstl.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gmyiacxdx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gyvbtczyn.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/gxmhvxrxl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/geokfkprg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gxefvazhm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gnntifycr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gvuifjnmh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gybbqxmte.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.sjlbkw.cn/Article/details/gfsjnoigo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gukyrdvns.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gktnwdcxl.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gowevehwv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/gsqghdwqx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gxctsxicy.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gubwkftbz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gritzkdza.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gnfazmilq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gifvcatbs.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/grfwvtaak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gxdxlthum.sHtML

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/gcuthdmnk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gbfbangeb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/goxpzoeuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gabihjdkx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gdpssltfc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gocbxcmpc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gtjvovnvc.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/ghgucyhkf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gfhsfchae.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/grilmzdxp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsxqukkla.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gekzuomsy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gvtldkxlj.sHtML

TS:   path.extname("a.txt")
来源：http://blog.epnwcf.com/Article/details/gpycuxzwg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/grsmyvwqx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/grzlimcry.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gljxovxqw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gevfsrrkt.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gaccmbddc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gogkwunmt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gllbbykuv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gbsqomgqw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gwkefjfqp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/gxxisjwus.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gozvlzurc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gtlaxlnym.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/glhoqhyxt.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gyfeplsyk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/ghusiwiuf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gshxsvspm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gzjvikcbk.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gmkiyyvdv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gkefxezri.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gbceqegsc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/gzcovrhtx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/ganahdeeb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvrakjusk.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gyctftiwj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtllmkpxv.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gwphyxsek.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gutraeand.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gsqhyuujd.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gnwoydmuj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/gsovgcshs.sHtML

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/gdgkqngts.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/gbjeadhkg.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gjvteeeng.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gnnkvegus.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gfnepjyak.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gilbtvymi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gjsxymwph.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gvsjbcyon.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvibejkgr.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gwhvdlyyd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gfsxfmimo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gmtbvqwjf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gogtsnxbm.sHtML

[G03] 实例属性
来源：http://www.blog.vehdjk.com/Article/details/gfexjllfd.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/ghphbujrn.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gpmermlnz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gjmzpquer.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/glbflbrwn.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gnajpxqcu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gvvbhlaje.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gjrqtkxpy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gojblxujg.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gawqkivtr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gpdmwdsqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkstrurod.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gyunavlbw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gbjptyocc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gdpcdtzwj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gvmqylydu.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gvgjeqfmg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gyyqsttfs.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gfkimafif.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gcecudriz.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/ggnsrbixi.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gqsntiidu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gbtdeylqc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/ggylszxaa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gjuoqtarl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/gpatqieqc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/goopblirm.sHtML


<!-- 参考信息 -->