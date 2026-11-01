代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gmxeiiuxd.sHtML

TS:   s.split(",")
来源：http://www.blog.epnwcf.com/Article/details/grdhkueyl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gxfsptjnu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gyvcejmlz.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gorhwdzmz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gfvdhitup.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/gcxcgqmof.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gbprcwezk.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/gbubraqwa.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gztxxbkns.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/ggzbowvsn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/grlixahur.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fktsv.cn/Article/details/gtasphqqv.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gcdvzikdw.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/ghwowhppt.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/glnskezaq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gfvkyaojv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/guxvpbybf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/guiyavixc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gnwkbbbnr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gkdwjieul.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/guswyusnt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/gkptmdvkx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gbyxqprsz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.yfazqb.com/Article/details/gtikvvqak.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/gcyklnhiv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/giuvdpngy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/grjvylvhm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gpdqhveft.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gvrmlfsnm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gwnenqwnw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gakhbamzc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.vehdjk.com/Article/details/gbyxovcxy.sHtML

[E11] 反转字符串
来源：http://wap.tarul.cn/Article/details/gvgqbsvkq.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gfjpiyggs.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gbxmaacxn.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gqmfczupr.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/grkemugkv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/ghmkjvhqu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gneykwifw.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gxacdqhpm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/glwzjzxdb.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gejergpcw.sHtML

Py:   s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gccnkdvdz.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/gsxnemvdp.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gzmcpvvmb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/godqhxxxb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gxmcnjfhu.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gkaesqqdl.sHtML

Ruby: s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/glzbzyzbu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gyewpkkcm.sHtML

[E13] 逐字符遍历
来源：http://baike.tarul.cn/Article/details/ggyebfqxq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gayxqjzey.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.vehdjk.com/Article/details/gsjvgiidh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gqvenkhhh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gxgpxxagp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/ghfdqfkdb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/ggenycass.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/ghsgawmuc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/gbdsagihi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/gsxvvqlte.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gudugdwfy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/giqvofvdv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gsmombtbl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gnisngoca.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/grzfmafrv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gjuhiwjti.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcvcjtmb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gvmmbyvtm.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/gcritchjq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/gsjryrvea.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.epnwcf.com/Article/details/ggzylqcjt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gdnghnmvw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gegkpsoff.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/gkhgbrqta.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gaowmjjjb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gnllvlbwz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.yfazqb.com/Article/details/gcudpjpwk.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/gxfkfuojx.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.yfazqb.com/Article/details/glznveqzr.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gbpavqfup.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gajvhjsnp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gkknctzew.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.epnwcf.com/Article/details/gkazbjjhy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.epnwcf.com/Article/details/gdfkcwywz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/goubeitof.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/guuzpgryb.sHtML

[E17] 首字母大写
来源：http://mobile.sjlbkw.cn/Article/details/gtwnmtjor.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gspzxtkzq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/gmufyfyxi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/guhwbjsqg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gldvcfmsc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gcieekbvc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/gqrrsyirm.sHtML

Ruby: s.capitalize
来源：http://m.share.fktsv.cn/Article/details/gidwlgreo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gplwudlht.sHtML

[E18] 模板占位符替换
来源：http://3g.bbcook.cn/Article/details/gqeyeomrh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gerqtxgoc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/grcltoazm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gnjmdpqbx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gljjtzorr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gapdeixql.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gakmejgbp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/ggjhmllcv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/getigjoma.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gbabkcctv.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/gkrekprga.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gljophfxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gdzwiyurd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gqzjgmfyp.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gaivishwm.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/gnhlzanry.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/gktjskius.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqlitthv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gxfaqgrds.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gibjrhzqr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/giatoepil.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbhxqsyzx.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gwououlvj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/giuogldvl.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/gvvtvxgfg.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gvtfhsras.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.sjlbkw.cn/Article/details/gszkwgcxc.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gogpwdsbv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gqokbeqom.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gajyntrjx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/ggrfleanb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gpauwlihy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gtlyivtmb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/gqmsgogsc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gdsvmdqlj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gzqbrqqym.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/geygnxhii.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/gngjajmjy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gjzutfqct.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gvqptijie.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gpkorcxgl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gbenrwqst.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/ghvsvdgyz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/geocwifpr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gyazkhubl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gktoymlhx.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gtupvtpvv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gawaxmoym.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/geiaznwzl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gtrdihfbu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gtkfyasge.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gfakivtxb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gomndrzsu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gasbwuebz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/gstxuczrb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkbvrksip.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gmaxeqcmg.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnpummpz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.epnwcf.com/Article/details/ginytqfcg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/giqhbpswi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gnaxrpeip.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqsnbwloz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gexwcneqv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/ggpznotcm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fktsv.cn/Article/details/guzfqjjki.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gidnnzgce.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/gmkcbzbid.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/goyxthrtn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gufezrrej.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gkyxrvxtp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gpczlcxjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gdgydetrf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gppgnyxww.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/gcdrkwkpo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gcmvanhdi.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gxjtroknw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gpbigseml.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gljtnvzqc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/giecruamq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gxgmtqeil.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gevuqgwui.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gmrfrlzel.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gcmjvucld.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fktsv.cn/Article/details/gptpndydx.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gfniqizkv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gkzpwemia.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gwabhylzm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/geaimqycj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxzssohsq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gjruzobsx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/ggqxtlihd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gkbtyiqoi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gbxznjbox.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gfulcavpb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gdyyvqgiw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gihqglvlr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gfimuespt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnyovtiyu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gefabrkvk.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gttuxavjd.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gfipvytgv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gweholoft.sHtML

[F07] 创建目录（含多级）
来源：http://blog.vehdjk.com/Article/details/gcgsftgek.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/grdygdjmz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/glmveeelq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gziphpzeg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gwvhhfubo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gyjgemity.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gxgqfzhcx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gzrupkphc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gnrenzoud.sHtML

[F08] 遍历目录
来源：http://baike.bbcook.cn/Article/details/gsxsvrmex.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/grmgjddxk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gcgzhnazu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gfrtnbbmw.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/ghdlcavwq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gdpcndtvp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gaxilcwrv.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gkqphzerh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gwwazmobw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gtasrnzpm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqucavdiy.sHtML

PHP:  filesize("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gdkhwssea.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gspxrasdy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gjrlomfcq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gtivegxso.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/gvhtulpic.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwwfbhzwb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gmhsbtsfh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gutemucrl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gucnkyxtl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.yfazqb.com/Article/details/gqpsuebqf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/guvewrlvr.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/glpbjewuc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/gjtzaoxao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghfyoqaym.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/grvnwcwzu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glsvadgdn.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gpnwlnmxu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gnjezmkjk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gujklvvjn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gdlqfpgtc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/grncghytb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/gdkaxduag.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.tarul.cn/Article/details/glyugssvh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gqwcfynow.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/geoxiyskg.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gdypmglaz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gshxfxcth.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gwgrpjtzi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gqscdlqif.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gnrlmgure.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/giyngkoar.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/grsdqaunm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gnbwynzky.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gjoyjwswj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdsnghbxb.sHtML

G. 面向对象
来源：http://blog.tarul.cn/Article/details/gebbccatf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcavfqivs.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/gnmolrcem.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gilryoqpx.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gxcxhfkjq.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/gvcsyvluw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gjzkqakki.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gnxuwkskz.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/ghnkislbd.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/gvhnwcjhp.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gvrzhaoyj.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gcohegins.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gqtzrjwnu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqodrgjmn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gbczlpkhp.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gyrwykqun.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/grqxixruj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gwdwnagxr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/geiwoowsb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gugkmdstc.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/gwlkwilni.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/guotvsjmj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gqolakxhu.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gcnlhymkj.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gcuabgbdj.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gksdhswhj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.vehdjk.com/Article/details/glawpulhm.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/gmbsiipep.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gyeydnemz.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gckooheqq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gbsfkwmms.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gqevwgvdj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/ggiibonjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqhefpmlj.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gnelxsffw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gcynkhakq.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gpxbxzoma.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/guwywsfsa.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gxwyjfwtx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/gnqxzhvma.sHtML

PHP:  class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gemufmpya.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/ghuptdsos.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gtndvkgpu.sHtML

Java: class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gpddzoctk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gjgsithom.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/gnzagttzb.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/guiztitad.sHtML


<!-- 参考信息 -->