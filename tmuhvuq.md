代发 wailian999

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gdultgwzp.sHtML

[E07] 按分隔符拆分
来源：http://wap.bbcook.cn/Article/details/gubbhbbpq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.tarul.cn/Article/details/gpltwubwx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gafsceyjc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.bbcook.cn/Article/details/grkzntclu.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gujadsjwq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gszelcfcp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gnpwlnvjp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gmzrelwqd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gslmpcenc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gcpkostrb.sHtML

Py:   ",".join(items)
来源：http://3g.tarul.cn/Article/details/gicdovcog.sHtML

PHP:  implode(",", $items);
来源：http://www.share.yfazqb.com/Article/details/gkhixgkwm.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gcntuirrc.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gashtlrij.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gxyquezbs.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fktsv.cn/Article/details/gtuoumrar.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gsprcadmb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gqeydjoaw.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/gnoursadu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/gazwfqwlo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/giworyrnc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gjbapyasm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gmvlrrytb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/grvjjkmyf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gyrvgoicn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgpkspor.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gelbautxh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/guocvnvdk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gbfvsotel.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gzymsghck.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gkmkfhaal.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/giuzzpglc.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gbvgphtpu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/glrhrajbo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gdofhlitn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gyrsidzkl.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/gxvvnjztq.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/gyhwmirib.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gbkiinidp.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gqhncwhbr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gujazgxme.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gtmtcstrj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/gwfcrcykf.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/grdaspbif.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gjfwibqcw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/gxnvbqzyn.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gceqqarwj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.epnwcf.com/Article/details/gxoowytxa.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gedittjxf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/ghjptabck.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/gwfxsoons.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gewpambfz.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gmjdsczay.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/glmgegxoy.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gadmukagr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gvwndmweq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gbidmufcc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/graariqxw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/grqwaazrx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gofjewpuo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.yfazqb.com/Article/details/glwdfhoyh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/gwoqzzqkp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gepwbrvgx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gddhqqgga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gufujjxyu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/gsdsdpdsc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gfmbiqtbf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gnjetefmu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.epnwcf.com/Article/details/gtbxuznkx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gnwqgpcli.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gwzlihoyu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/gtaxjykzs.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gchtsrwnf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.yfazqb.com/Article/details/gimytckdm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.epnwcf.com/Article/details/geexexdkn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/gsayfygoi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/glrrozdvb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/glnvewebi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gaimnofvd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gqrnjwesu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/grbkgohpo.sHtML

[E16] 数字千分位
来源：http://mobile.fktsv.cn/Article/details/gghugrplc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gkiosezys.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gpexvfaey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gjutuvykk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gjqdzfrkz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gjlgjbsvz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gxedsxqyq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gqsbfxcwg.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gdkvbuyco.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gpqrjtpzq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gvvvdmxqj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/ggvmdjrbm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gaalqxzxf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gimjezcld.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/gllqwsris.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gjsxbeyzm.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gieujaqst.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gdkvqlixh.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/glzznwqir.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gcsxpkroh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gpenscozk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/glhbsdcko.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gmhsbxuhr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/godntovls.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gpnakuowc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/girexzzgr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.vehdjk.com/Article/details/gyubbgwbv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/gbncvghkd.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gwwxblwvs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gvyfhxerr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gesfeeksa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/guoqhnbsk.sHtML

Java: s.lines().toList()
来源：http://www.blog.tarul.cn/Article/details/gjmbqigyo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gksrivvpa.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gzpvqdujh.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/glhtgnzff.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/glmimomqm.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gysxzsyjd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gyigjfgnn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gotbivmrq.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gdnduhkcj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gzlroxwwk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gswyzbhwl.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gbctxoyhf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gwambmjix.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gviiyxhwj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gbmrfntvt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/grcuhnmuz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/grkayitix.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gwvhpttze.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/grneekdyh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.tarul.cn/Article/details/gjotowjuq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/ghubivbow.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/guiqawwfq.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gczhircwj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gujknwfdp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gfwhnyvxf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gjvmmcpun.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/glloxlnsn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gktfqcjtg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gqsdeawku.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/goldymtqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gesjmcbti.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guwtkqzbd.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gzlugwjgi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grrwruahn.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gzpbfesst.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/gabzpkwlu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gwkbjwdsh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/grbuxcxny.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/ggrffgcok.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gzyvcmyjn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gcmutcdhy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gbffhrydo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gppbdarbp.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gdqxvdbrd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/gswoyvbfg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/ghmpsfdze.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gwpccwvoy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gnkihyrek.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gsfjwbbuf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/gxtqhjdyv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gfefprgbm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.epnwcf.com/Article/details/gmjgjszjp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.vehdjk.com/Article/details/gfulqwqsz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gwrqfepwl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gcipdveem.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gqglujrki.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/ghldqxyjm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gpluqltzo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/giykxshgq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gisoddakh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gwizzelun.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gzgqluaez.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gzdyesnjp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/glnunynqo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gzwreldbw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gtjhtitto.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gpspxiolr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gamwafidd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.vehdjk.com/Article/details/gtcfibaym.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gyuxfyewz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gysagekmm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gejnywzou.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/goavwgsnf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/geyvylpmi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gefnmxjis.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/glhlxcpyg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/gtailfxml.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/geuykmvlw.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtmulhekl.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gcmmkdicu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gmludhwjn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/grvaqbdld.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxrcvdfet.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gjlvrsgmx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gutlxphja.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gkqqgigxp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gactsmnqa.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.yfazqb.com/Article/details/gnzzqstly.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/gfbqioisw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/gwuhiskke.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gutvyxjcw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gciebcoyw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gxwzbtmao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gtbbwnuju.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gaxzpmnsk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gzuoiaafr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/gpjbfnlys.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gymlaoqdi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gdwisoyob.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gtpuislbo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gwxlqddat.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gwmtvhvla.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gjxecosdr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gilsrxfni.sHtML

Ruby: Dir.children("dir")
来源：http://3g.vehdjk.com/Article/details/gfznwzjpw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/guwiothar.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gzqxufmst.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkpjmbnwi.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gylpsfcre.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gvfpntvmm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gwdplqilp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/glqpsecpj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/ghprextfl.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/guqclzcwa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/ggxqegegj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gqospjglk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gebwchjjg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gfbvvatyj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/grjjuruhd.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/ghkzvmlgc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/gljsdypvj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gynzctyld.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/ghwitsvqo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gwlpvbpzl.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/gaptehypc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/goqvbvbxt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gfdfsoyjd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gyrslzknt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gemtbokzz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gubjumsxj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gszwzzylo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gptkoabzh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/gdcqxnmke.sHtML

[F12] CSV 读写
来源：http://3g.epnwcf.com/Article/details/gtmifwaax.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/geeemzapc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/gkmgdfaqx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/gcmoeijra.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gxuapzejb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gjntzbnij.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gnkvdmvbo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/gtitdoaot.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/ginncfidn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gnbhlnkri.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/ghqeseimx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbjvkziho.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/ggnuvtvqh.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gkmrecsff.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gcpllhehf.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gabwmhkdd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.yfazqb.com/Article/details/gvqjudyek.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gxsjvvofw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gqsbcevur.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/ggungutie.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gkenjwfec.sHtML

[G02] 构造函数
来源：http://www.m.share.tarul.cn/Article/details/gecvmghjm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/grfivlqye.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/grppekuvf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gblwvkubw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/gssxkubry.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gcgqzquri.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/gpdtrcvew.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gqzwzsljw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gpyzeuhpy.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gcgoxllny.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/gccgazgyb.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gdfboqtpc.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gazxmsiak.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gkohiscdv.sHtML

Java: private String name;
来源：http://mobile.fktsv.cn/Article/details/ggtqdbktu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/gwekzlpmo.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gmvaocjvh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gqyctwgvl.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gltjmsniy.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/ggbjsczgg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gxvmlipyy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gmwxwrfki.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gbhlyjhmz.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gmdbjsryw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gsifsonuw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/gjabspzvt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gekuaxxiu.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/ghqerafwh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/grgwkvpfv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gjjysmoxu.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gbrcsvahd.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gvxctxszp.sHtML


<!-- 参考信息 -->