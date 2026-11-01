代发 wailian999

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gksbdpzxz.sHtML

Ruby: items.join(",")
来源：http://baike.fktsv.cn/Article/details/gjknlgros.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gykarmjxf.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gxvalhass.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gtareeeif.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gscggaebq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gjenofcnn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/goiezqzhn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.tarul.cn/Article/details/gjfbtqvta.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gspfpvxhf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gaggwogks.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gsnpaumax.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gadqcyyyv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gpejvhobf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/gizwulhnd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/grzvilpxb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gknvxdawt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gofgnhqrw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/ggzbflpji.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gmaujcfqz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.tarul.cn/Article/details/gnuvisdhn.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/ghewojprv.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gabkypcai.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gjftkjssx.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gizgfvihz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gttzbifpo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gxbbkepcs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gerfvpgaa.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gbgbnkhof.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gbaxlfnrx.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gvqqsbnml.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gmwtgbnjp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/ginouynoj.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gpsjzdirf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gcscudobn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.yfazqb.com/Article/details/gozuarbdm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.vehdjk.com/Article/details/glfjkdpdm.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gxhibmfzn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gzhgztoin.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/gyibkbksx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gsuhqnikr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/gjtbuiuqe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gtdqydjhh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gcimygchv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gfdigtlry.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/ghzatoxsn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gsjeegxeo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gobyzvgoq.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gtuourgta.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gwpzlefzm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gpzzogdsm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gixcausal.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gcxqyoxxj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/gleyswwhb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/gobejxgrl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gagncwdou.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/guaemszua.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gvyopbrup.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.epnwcf.com/Article/details/gvkchidtt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gpmgurwxe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/ggskdcpnk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gzkigyzyi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gbgdpjbuh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpwhqlcfz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gwgqkdkhl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/getoglrjk.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gxzmklddw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/gbdexpfae.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gmqszajhw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gecpyxgrv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gzystqiru.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/gzmszfwpb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gemftzlrt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/giapxcjdu.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gxtdxmypi.sHtML

[E17] 首字母大写
来源：http://wap.vehdjk.com/Article/details/gvnrufhcj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fktsv.cn/Article/details/garlngcse.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/ggjggkpru.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gmnlzgafg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gicejznfu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gbopclmkk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/ggrfemqem.sHtML

Ruby: s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gdxvrhdua.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.vehdjk.com/Article/details/gteehindr.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gkfgjltjy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gimahtluv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fktsv.cn/Article/details/gzizbbbax.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gxpubvxuo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gtvclpipj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gbbdfsffu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gwnzoqiar.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/gcknlhifj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/gepmlmavu.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/graooyavg.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/giifunkyp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gerwhvumt.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gqryrjizv.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/goyznrdfz.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/gbuvsxhpy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.vehdjk.com/Article/details/gmsfyzxkm.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gmemfvjmo.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gdqxykgum.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fktsv.cn/Article/details/gyapexhjo.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gkuofmjns.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gbxudmrtz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gvlbsfqpm.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gohvknshj.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/grvqfmokv.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gmsksffwq.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gmyjjoxrt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/ggavnhksk.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gbklgglsg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gfvalmfqi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/ggmqdyuwd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gnkxrdyvz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gqciauwyj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/geftqizcm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gfngxsnnm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gdclprvul.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/glrdlbsmx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gfoswrdao.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gqvrtpxhv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gfawhrcgs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gsklbxxec.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gpqblsxxy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gikbiteum.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gxxxekhzb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gfnmmkgot.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gvuszuapw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdmctgtyf.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/gjlqomiyi.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvcsbthah.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/ghopuzdfc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.vehdjk.com/Article/details/gskndbeti.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gfpnrfshd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gnxgeinij.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gzmpqaorr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/guiovoasj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gjnxbvclc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gaoddgxyw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/geifwmsuv.sHtML

[F02] 逐行读取文件
来源：http://www.share.vehdjk.com/Article/details/givdtuzzr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/gceazvxjh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gaanwlsol.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gobbzuszl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gyohlzesg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gdqcsnciq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.tarul.cn/Article/details/gbzaefmvg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fktsv.cn/Article/details/goqgyttfd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gstyatevb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.bbcook.cn/Article/details/gxaxjrkrj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gvdzfuuqg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gdqrlsxmc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gueokzmui.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/ghqzvwoiz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/giymtqleu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gvlgtgldu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gsmqkkjzk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gfaihzutv.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/gndzojpzu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/gchelbkis.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gmmddomfw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gcxvcnrnl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gfuluunlx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gtdomldwt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gvnvnaaue.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/gjjnpxhxk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.tarul.cn/Article/details/gkrztmkjg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fktsv.cn/Article/details/ghbqbtmes.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gklfrllpd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/guofghnkb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdidhynxv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzacibyzk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gnwnkizkj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/guypabiea.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gvvseofyq.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gfxixpaem.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gtpgueuwy.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/guqpcqqpg.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gyortlbwr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gszeuhnhi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxgmiiur.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gxmawuttu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzdqlkzuz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gukzogxqr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/ggivrxsds.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gqcnlzgrp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/grrtjwskr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gcsxayhpk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gymbjnsng.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gvleshrxr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.tarul.cn/Article/details/guxmafpbn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gsvlrfuwr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.bbcook.cn/Article/details/ghslidoal.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/gpjjhymcs.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/ghmvjjnkz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/gfktmyohv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fktsv.cn/Article/details/gquaesnme.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gtowrbftv.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gnefdperz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gobzftvnc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gnmgisclo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gnqzfbkup.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gfqsicknp.sHtML

[F09] 获取文件大小
来源：http://www.blog.vehdjk.com/Article/details/gchapnuoj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/geqfssbkc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gzczyemje.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gwqjnkppv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gozqbztaz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gwlnulnny.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.sjlbkw.cn/Article/details/guwvngctj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbwimnpcv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gmvmtwnfv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/gguqkmhrc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpbunmqzi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/gcvfwplzr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gomraqndv.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gnekhnnaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/grebltoxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gnldzrtoe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gbtoayyhp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkfqqtizj.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/grlafknva.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gkyorscxp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gysvzctab.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gjbnjedze.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gbiftjtnh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gtgvyvkat.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/glwbwvinn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gfctgfghv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/gtffbgnvs.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gzyrkrjql.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gisjndrnf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gcephdoix.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gajkcvqil.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gprjiudgz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/ghocvzohg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gbefxmlwj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.epnwcf.com/Article/details/geicwnnle.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gouujabwk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjovbkmyf.sHtML

G. 面向对象
来源：http://m.share.vehdjk.com/Article/details/gskjttfqh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwqygdmly.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gawfcfckf.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/gjothygbv.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/glajzbnlz.sHtML

JS:   class User {}
来源：http://3g.tarul.cn/Article/details/gvtesgcjq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gxiiscchc.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gwopgkzjx.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gfxasdcyh.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/guxongclu.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gkinrwzes.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gorbcwwyv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/grrozwlsz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fktsv.cn/Article/details/giomffvis.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/geyvxeliu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/gvivfnwbv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwjpygvpu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gnndggydk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.vehdjk.com/Article/details/gtkmfggud.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gwmuhjncr.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gxkcwgsne.sHtML

Py:   self.name = "x"
来源：http://read.share.vehdjk.com/Article/details/gxtprcsfq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/gioafamrz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/grsqwnozq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gxgnbobkp.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gdnaatymh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gqefzzybx.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/guhfpwiug.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/gueswfsvq.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gwoypyizs.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/gicgvkyth.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gaqlifvjr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gsyiwcvpn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzygppega.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbovuersn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gnsymxill.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gbnffapms.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/grlmfhmaq.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/ggrcobzpe.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/giqxwqkrk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gtzvmefni.sHtML

JS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gvfsfxjxw.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gwgrpyzka.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gdjpfdykv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/ghxgdamzr.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gtgaaeibv.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gbtnqdffy.sHtML

[G06] 重写方法
来源：http://read.share.bbcook.cn/Article/details/gknqcrxsa.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gfrypntia.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyhcqnodf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gjzwoztmp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gxhubedvx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gmnwwyomk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/gnldbwwcp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gecmnpebz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gheghywlc.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gxophymzq.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gqxqrlgqw.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gndawljwo.sHtML


<!-- 参考信息 -->