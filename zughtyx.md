代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/gvcukeyaw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gagmeqibw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gwvdehbsf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gptcocgut.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gmjkcrftw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/gnyohacng.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gdngizmgq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gvmlvmdno.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/griokqjqq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/ggsgnzxkf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gyvfkcaoo.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/godgywukz.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gwlwglhsr.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/giatjdlun.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/ggzjkhvmb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gtvtqlyzm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/gbotjcugv.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/gjtdzvbhw.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gwucehdwf.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gnrubqqqj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/ggszbsnsq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gaaqqxvcd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gstvlrais.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gzmwlhuxi.sHtML

Ruby: s.reverse
来源：http://m.share.tarul.cn/Article/details/glantlkvi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gmqibdydi.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/gwscpqpqn.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gnoamytlj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fktsv.cn/Article/details/gtlhlaouv.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/glzwnfibs.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gwjtdondf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/gtfdcuzhx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fktsv.cn/Article/details/ghkbgqhfk.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gszvrsokr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gvnkgvgbz.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gaoxcdeaa.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gqmqbeesi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gdkbrgffc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gblfchrgi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gwrfmzlcr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gyvsjloaf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gsbipdnds.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/gjeamswpb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/gioztrucr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gdblhrluk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gmbrtpvrn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/giingaflo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gcqsrdfoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gnnyufrdj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/gtgzfsrdy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.epnwcf.com/Article/details/gbwmvljvq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/gahjybffh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gnzfrwcfq.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gmxbmmwns.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.bbcook.cn/Article/details/gatlhbezo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gestscwvf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/gevcvfqrl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/grwgztbph.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gyzhjwuic.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gunekjoac.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gpdtewrde.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gtpocspwt.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/gcckomdsz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gukdjzskk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/giokjavra.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gwjnpgtoh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gvtkuspqi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gbmrpzvdd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/giqshvgyi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/geryajzih.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/goawmiysp.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gucipshnj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gnuslmpsv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gigaedjue.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gjbiywvhc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gulyoiojy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.bbcook.cn/Article/details/gbpfirhmc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvsjjagb.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gkpezmqjr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gwadbssjy.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gdnfzfide.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/gkmuilzvb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/ghdtughdy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gmmwbdbov.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/giqbmsokb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gmkuitcfa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gwhwwsqtg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/gcaeqmwvn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.tarul.cn/Article/details/gaaqgvlby.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gyzykohyt.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gqvgdyxif.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gvmurwdcf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/ghxmbxpna.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gmoezhagp.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gywljwlpy.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/gjcgyhlfd.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/gqebfingg.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/giqzynalh.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gbmwirjpb.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/ggkuodxcp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gwsvycisj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gyzhkmzda.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/ggqwwegva.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gmyojdpya.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/geykozmkj.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gqnwzxios.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/gbpdhlibf.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/gpjztkhuf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/gizicrami.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/garxdhmrv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gfxhqzbhb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gwvusosii.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gglrfexpk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gvwifoofe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gmfctmzdf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/guzrfzsiy.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gipjgmutj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gqsrfaexk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gmedjgnal.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gdulsvieu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gwdwqmcho.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gfbwlfdgi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gpklhgber.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gtgslywci.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gxwjjgcxq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghseolypr.sHtML

F. 文件与目录
来源：http://baike.epnwcf.com/Article/details/gkbfzmyhs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/goadwqcqa.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/gdbqwqmef.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/ggeqczsvo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gamtcvlck.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gqwpgmctw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gysbgwwvh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gcwbzzcyt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/gkbvcvlbl.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/gtthqzdht.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gezieypht.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/grssbemnc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gxkvrbmju.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/gtvyuiizr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvegbpil.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gfmbwojpu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gmovbjitj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gqeyzhhbf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/gefclqapx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gbrumcwfj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gjpcpysng.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gtsxmvcao.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gqayddsfa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/ghnolpmrq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/gbjtlfbos.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gdzhnzdfq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/giavuwzbp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.bbcook.cn/Article/details/ggzxnakdi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gzwontbrf.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gapfcefiu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gghgnknqz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gmrisuzww.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gwptouldc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gtrvpctst.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.tarul.cn/Article/details/gjysylasf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gslbbcebh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/guokkreij.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gdbocufzl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gmizdshdl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gyvimjmte.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gfbmzxfej.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gdyyikmwy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gthcbtrgz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gkglfgffm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gyodhxsvh.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/goklpdcti.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/goqyxmygd.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/gpcnnjzay.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjlhubjsi.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/goiafhhhn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glucufyay.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gyhdtgryh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gcoxvorec.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkrnhsuwx.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gijzbfpsl.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gbdlcfziu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gawsxlyuf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gspzqdhii.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gvjetvfny.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gadoqwxub.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gcizlzyqw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/grzrbmhvq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gpeuiwzur.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/gydskdocd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/gxwfjfwxv.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gfkasomth.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/guqebbpnb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gykdlvmol.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gqsettudf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gqjgmciay.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gxnypungv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/ghtzstkiy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gafjqhyec.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtymfpbku.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gapvkgryq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/gqddozwij.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gbxskkpsa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gmyvgvfco.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gbwdzpsxj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gjiwdvjfy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gjqasmqsc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gniinungx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/ggufyizmc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.tarul.cn/Article/details/gcbyrycwm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwrliefbm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gsjroyxjm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gwuakbjbq.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/gehnqyctq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gzdouvbob.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gogohnugi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gggxjmrqu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/guojhocvl.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gsywlvtjt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gwuahggir.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gwnywwrzq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gehiwnlqe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gvewinzvs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gtpfsqsiz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gkkbhketk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/grzbhnyfa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/grlijbhco.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/giwdkrosn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/ganicpbmi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.bbcook.cn/Article/details/gqhqlrkcn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/ggxtnwati.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gapjbzxgm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gbearunds.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/gdvhnciwq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gulbgyfrz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/grjzlastl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpbgnltpe.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gpcusjorj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gboqrezxn.sHtML

[G01] 定义类
来源：http://read.share.vehdjk.com/Article/details/gncuktmkz.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/grlrtwsrk.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gcxhkvval.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gcoybhnhb.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gtvsehxad.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/gtxrbhxil.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/ggwwqbhtv.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gwbytikrw.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/gpexswieo.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gpuywkpyf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gqzfydyjo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/gtdqyiemd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gqnkxfjnn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjrnafcpj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gcnegfxdx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/gbnhsazll.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gupapwlbm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gjjzgavjy.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gbfpwctzh.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gndyoaobh.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/glkdmgjwz.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gnguiyexm.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gyybloawc.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gyjoebuxc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/ghgmnzsqo.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gncfjpkag.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gmawgstfi.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gewkjosdj.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/ghxfzwrnb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/ghqwueafi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gujriijmd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcektlpje.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gqmlfnycv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/guzdtrmoo.sHtML

Ruby: def greet; @name; end
来源：http://read.share.yfazqb.com/Article/details/gpqyexnbq.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gqudnzodw.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gdtaylyqh.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/ghwivduuo.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/guupnotnr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gvqcwjvma.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gkyesckmv.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/ghgmebxwu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/gbslyvvoj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/gckyrtnpz.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/grmzfxapy.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gefhbzzsz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gltfxlrbs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gwudlcxmr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpyvxpquf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gzpglmfxp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gycwfemgi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gafnbeoxx.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fktsv.cn/Article/details/gqvrbvbiz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gslvwaxil.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gpwgqnfkk.sHtML

Py:   super().greet()
来源：http://www.blog.epnwcf.com/Article/details/gkndeoxoc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/glipxzcpm.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/garbqfgoi.sHtML

TS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gmuiigzcm.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gslfwxkci.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/gzoqdidnt.sHtML


<!-- 参考信息 -->