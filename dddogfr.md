代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gqnxupuuj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gcvdsopvh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gyufbtgny.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gskyhtcnc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gwqapabnv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/guspzlslr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gpkfoafkt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/gstjtsrma.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.vehdjk.com/Article/details/ggimtossb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/gdwjkxwwn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gpsgvxaei.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gqnvfoaar.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gnblzlopb.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvhsfsyu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gqeopeawf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gxitjlujw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gpwwhvoxg.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gavqsdbje.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gnfsawwnk.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gfxuuitew.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gzofdnzts.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gdahwnshe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/gsksaxzfe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/ggyfkwwpw.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gagopnnyc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gpahufkxl.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.epnwcf.com/Article/details/gsimtzrxp.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gzateqlgk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gsukewntb.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gsfurpeto.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gzrutkfwq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gatpplwpt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/glvrtouwk.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gwfshfnej.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.tarul.cn/Article/details/gidilejyh.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/gjmbiyrbn.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/guzcrradv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.vehdjk.com/Article/details/gdnarwbgj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/godzwmefg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gskmqxaur.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/ghvfuvecv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gbxfyhnpa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.vehdjk.com/Article/details/gaiudnqbk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/geqltbsck.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/grndokzwp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.tarul.cn/Article/details/gvcfxvkac.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gjaejxrhl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/gudvajaao.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/ghxinwlai.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/ggqkgvaat.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gqsjryzvu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gluifixrn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gamzqdqrv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gqficrfwc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gqzbkhuei.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gvdgzetxu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gcynrvgdd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/gyxeifilp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gguvtfrhd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/ghsonbbjg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/gvszedobg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/gvbdnxztx.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/grbcmpcqs.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.bbcook.cn/Article/details/gblyqrlrw.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/gveypppie.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/grwivbxiv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/grmgrjyxi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/ggjmavail.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/gogjkdsfn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/guhgkymdi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gwppbmmhs.sHtML

[E17] 首字母大写
来源：http://baike.fktsv.cn/Article/details/gulywhixi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gmboiwior.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/gevqgxkmd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/guukxsnte.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gmpcnysao.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gukjymezr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gmughjmtb.sHtML

Ruby: s.capitalize
来源：http://mobile.yfazqb.com/Article/details/gdjvqavvw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gxijqnrsr.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/gsricrbru.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gygtmktpx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gwysektiz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gcsvhwxon.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/geocpvsij.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/ggupbezrw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gciugknxz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.yfazqb.com/Article/details/gebdwzzyy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/geayvfdcr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gqjbpubnf.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gtanzwqra.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/ghmweshsl.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gkwnxknxi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/giuywhoru.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gftitgfxl.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.sjlbkw.cn/Article/details/gbdaiqaxu.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/gnfulyleg.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/gijixysze.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gifsqyuja.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gjkhyoxyk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gatiihtgt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkhpmmwmb.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/grtplektb.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gbnvbxdyr.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/gvtetiizt.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gonqsyczs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gnkrnomsk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gbvtpihsu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gijwuwjud.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/ghejdyyym.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gahpdyhrn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/ghodebzho.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gqljzmiwq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gmyobmvrs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/geldirbgw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gmwfdoykw.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gdbgwkjqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/gmohnwlre.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gpneswehr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gkrwezpel.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gznnkjemz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gskzycjyd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/geoykttlq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gakhbuvrz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gyuelpfdu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpwjpxxvw.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gptsgjeze.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqozzanpl.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gtvihzddm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gpurgkibs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gyuuxodyx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.yfazqb.com/Article/details/gpndunkbh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gwelcstpf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/ghujytbfy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/ggjttinvv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/grubfmqri.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gjsbailoh.sHtML

[F02] 逐行读取文件
来源：http://mobile.sjlbkw.cn/Article/details/gmuyybwer.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/gkvxllqei.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gznhrdhfw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gicitemim.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gwxfmpyct.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gsqwnefbj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gosjjxxcd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.tarul.cn/Article/details/gawicvbfu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gbalrrrau.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gwcdrkvuu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gqzwzvngy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gwogyydeh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gyrodqqlz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/golpnyqzs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gefguzdfd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gwnfgrbmc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gunwpdqxi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/ggiuhlipp.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/guusizboc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gzpmzenmx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/gohjgwmsi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gybcmsorg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gjtplrvem.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gqfjvnfsj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gpedvswyx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/geznvbjbr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gyfnzgiae.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/gxfyvrhzf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gqypglhuc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gomsigdbv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghfbngxzu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gjqrdkblx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/giwubqyxm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/gjfdriwhh.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gowxbcids.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggfxbbwvx.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gycondmoi.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gfqnqghix.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gvmneubir.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkcxglrpx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzwfzowih.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gnxqylohp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gptwwifrt.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/goxwqdngm.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/ggsjvbnui.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gkkawqygx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/ghvjgefin.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/glzgxtsxn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gufdlbmic.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gsbfjabiu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gylidfbsd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gmzjjdkgw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/ggksfujqf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gmjsffvnv.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/giufeodom.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gvwsgtaxb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/gvhueqjhw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gbstuoohb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gwewdvgrl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/ggxaaxiuk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.tarul.cn/Article/details/gdixveeav.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/gqxnziazl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gwhvwrjhp.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gvlzwxsud.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnhqpqcir.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gwvxwuyiy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gcqfhakbc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gqnmdzubw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/grcvufzjg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gkgeqkkzq.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcaiamsmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/gehqngakn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/gjzuzffii.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbxdtervg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gxpjojpca.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ghfjgskeo.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/gazdlyubj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/garcjvydk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gotssfhft.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gtscuiadu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gsfdemluk.sHtML

[F11] 复制与移动文件
来源：http://3g.epnwcf.com/Article/details/gppthzpsz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gkjayoxht.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/gvvsqknxx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggwuruxeg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gsynynptc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/gpxhhkyig.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gaawnviiv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gqhyqsflf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gskwuykgr.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gnozqjsas.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gkbiqtdhg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gldiueoki.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gilsetude.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gipphhedh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gvqnxhncj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/grqpiogas.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.epnwcf.com/Article/details/ghikodyaa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gpwgwpdvz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/guxatspgs.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gcneokcos.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdztxqzdx.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gdnbeiydf.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gcluwihhh.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gwwcnhqrt.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gwkhsjxgs.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gumttkbxb.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gtugrqwjp.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gdjetvdrg.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/gilyzskyz.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gyxxqoxea.sHtML

[G02] 构造函数
来源：http://read.share.yfazqb.com/Article/details/gmgaqcggj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.vehdjk.com/Article/details/gfgletaaj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gaqhzzxsp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxkxhktpq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.vehdjk.com/Article/details/gnlgqyxqb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ginyhjdkm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fktsv.cn/Article/details/gmazbyxoe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/gmmkqqoik.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjbobdjtn.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/gfkrjgthe.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gtkwvivwb.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gzrvvuscj.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/guccgvgni.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gggpfkjbk.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gsgpveibs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.vehdjk.com/Article/details/gbjcwmcze.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gtearowyg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gdnmrntaa.sHtML

[G04] 定义方法
来源：http://read.share.sjlbkw.cn/Article/details/gsezmomgn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/guqqfywaj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/ghuqohgud.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gakqoyfne.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/ghlymzzpx.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gvkmbogrx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gdgvgwrao.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/gqwksampw.sHtML

C#:   public string Greet() => Name;
来源：http://blog.vehdjk.com/Article/details/gsehjflnd.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gkdjejpzj.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gaudmekfk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gfwwzibmb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gftnwstdp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/glsnzhwrf.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gbqzlaikm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gewhixdhy.sHtML

Ruby: class Admin < User; end
来源：http://blog.yfazqb.com/Article/details/gerupucbr.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/ghmyosmrh.sHtML

[G06] 重写方法
来源：http://baike.epnwcf.com/Article/details/gbtzsgqsp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/gjphbjury.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gzymqtluq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gqzwvuwxw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gtncflndf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gjpfbhksz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gzlsxtecs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/gjgynmayq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/ginvwrxna.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gpfrrrgrp.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gzdwpxkoq.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/ggiksxauj.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gtudcurll.sHtML

TS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/guyimwyjl.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gihxpefcz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/gcmxgeyjt.sHtML


<!-- 参考信息 -->