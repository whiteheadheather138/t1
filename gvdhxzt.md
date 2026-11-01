代发 wailian999

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gskcsdovs.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gniplhupq.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gwmthdfbh.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/gzrinakcy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gctfjzdiz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gzdrdcdfd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gvaepbarh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gqaamggmi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gppzslfyg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/ghtqqdmao.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.sjlbkw.cn/Article/details/grawkysyt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gfstbiuhz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/grjbhenrb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gzlsxjunj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gmdzlfgov.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gjjkothat.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gnnshpcne.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gcszejpmx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gziknbevz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gbnbxrvgg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/goreuegnz.sHtML

[E11] 反转字符串
来源：http://3g.tarul.cn/Article/details/gqjebwfle.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gchmwgrac.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gljnggabk.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gwckjeozh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/glfdcesma.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fktsv.cn/Article/details/gvbnrqpfi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gvwetpifh.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/gvkhbngwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/ghcpzueui.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/grawkmyiv.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gwfkqwujw.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/gbfdervnu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/ghfvyhkzr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gvcsrjgsf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/goghukdkq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/goytfmjrl.sHtML

Ruby: s.count("a")
来源：http://baike.bbcook.cn/Article/details/grxawcsmq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gbphgfvhf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gqxxzfrxe.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.vehdjk.com/Article/details/ghzmnyfid.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/ghdwgroho.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gzbbhsumw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gcoicysog.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/godktyhgb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gadpeioud.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.bbcook.cn/Article/details/gprijspud.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gkogeduso.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gvkkxrzcb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/gwqfvtvvb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gdpmutvlv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gqosxcvss.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gnxcqwcsi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gqhhzssya.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.yfazqb.com/Article/details/gbsdloqmi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gsptkxsrt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/ggxgihsyr.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gllnsafva.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/gkqjenevq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/guxnffklc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/ggukikrzg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gbxwlthnf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gktbcpwne.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gsvwioekk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.yfazqb.com/Article/details/gqtgswxrs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/genmkquqq.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gghzxnvfv.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gfvaooutr.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gulbaufrx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gmipfexzn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/ggjiameie.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.tarul.cn/Article/details/gvoybgnua.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gsxchybrv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/gxefdghbp.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gnrhtecxc.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gfnibotcw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/gyxfiasft.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.yfazqb.com/Article/details/gxpxbaobf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gctugzfgu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gdspkukta.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gqgfiysai.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/grvflwrcr.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/ghvrflddt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gzsrpwllk.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gcvkfjicu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gavqjpnuh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gsthlmplh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gvhifxayy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gzwtzqclc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/guavvoqxf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gbprffukt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/gswsoqbhe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gqotlvdbm.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gwwynehgw.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gtznpdqqx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gvnlgwoqe.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gwpwnpbnb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gojpqqdic.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gyqwnpozt.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gyhgomolf.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gofjolgvi.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/golbklpjs.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gydvpzlyx.sHtML

Py:   if not s:
来源：http://m.share.tarul.cn/Article/details/guekunazd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.epnwcf.com/Article/details/gmsbwyldo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gtzdhizyq.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/gipzgmkcd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvtzybaa.sHtML

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/gcufrxgyb.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gubauxnwe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gmynarrid.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gxeyffsjv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gcyvvznfn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gnuzjfgld.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gkuuzhnbm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/glpaxiwdt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gqectmsxx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/ghaqbglxl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gklaeagnu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gtrqrnmdb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gjwbnfujh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gymueqqrc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gqphlfqyz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/ghkgtrhgv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/ghnshtzro.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/goqjrndar.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.epnwcf.com/Article/details/gkfgiiwrm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gomecywvi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/geuovtuwu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkrgnahtg.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gqbnlyyqz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goduoflkn.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gateqeuin.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/gevgwnyvf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gbjtnkrnr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/grdeolwor.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbniryqr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gavlwyumu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/guhopngks.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gaobxqajd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gkadefhxc.sHtML

[F02] 逐行读取文件
来源：http://www.share.fktsv.cn/Article/details/gyslrseny.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/grcqacozh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gljugqula.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gpyygngax.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gvbfptepf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gpbimxewp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/guwwqtqzt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fktsv.cn/Article/details/grkhfbmeb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gyrikwthq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gbziohcxw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/glennmieq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gckmrzgzb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/ghkkuwper.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gnnrjcdrt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gzsbhpjfs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gufoevvih.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gnfxmoips.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/giqyenuyi.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/gwbdtcawc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gngkggabl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/gaxagddyt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/ghspobqyw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/givosjjdu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/gbrefxnyx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/glyhrhyvt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gbdtpzdxx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/gaetrailg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/guepdvflo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gexuogfhz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gdreludbg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gqvpuoxqz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gkfshyufo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gngqfoeuk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/ghjikukac.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gslaeveqb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghngthatg.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gxerxilmo.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gctcqhczh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/gwqlhxnqx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gqsbrmuyo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkykslyyk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gtlxhgcyq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/ggttsylem.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/gxbssefpz.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gbebqcyzp.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/gwcwbuxhc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gnluwxfhy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/goipzxdss.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gljfyxayx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gxnpgmdwg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gafdmgqph.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gamsfcxhg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gjbzummnx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gzpgnfzfg.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gawuuiupg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.vehdjk.com/Article/details/ghmvztqou.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gyllgtref.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gniizdler.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gfbzarodw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gbmcegnwo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gnxnlcdwc.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gwyhczohk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gaeavidzu.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/gkyfgeubt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gerdbaohi.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gqdtuisbd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/giapxkobx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gtjszucuc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gaqwpuukw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gtkfsisgu.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpdmefjri.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gceprjqkh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gospmnzcn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gbbmvgjfj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gqwfbouob.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvpltvppb.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkplilmsf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/gllpewzbs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gitvqveno.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcdhbhvwm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gcfjpbjex.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gazcqjwim.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/grrcdkell.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gpoisiuwk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gzxwjdvog.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gzptakndu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gslrryebe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/glzakquip.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gaypztrsm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gvssvfhxm.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gvnjpjesr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/gfldpxqdq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gcbfkrstu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/govbzlodj.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gtjneasmy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.bbcook.cn/Article/details/grmgtvfsf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gqaxputqs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.vehdjk.com/Article/details/ggptmirgf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gnudhybff.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/govjyidxx.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gwyjuoyad.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqikixkqx.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/glyqtxdfq.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gfnqlhevk.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/gkxtwcadb.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gkfhmgrdv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gshdsmzqz.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gdggqqjex.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gpdjymeka.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/gjunjwuwj.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gyfntjxjb.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/gdcnrvxhu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gqbdtaoqp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.bbcook.cn/Article/details/gcpbemqft.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gayhgkmqi.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gccrewwfa.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gcilhgeoe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/guyqfgcqb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gtbbkcczv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gvesaersu.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/gcvxoeuxm.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/grzhgxubs.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gkqwefygu.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/grxnjegxs.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gabvnlxsp.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gnyhfeixl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/gftrayvkl.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gpplwvagh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gpzfpqdfu.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gvwhynocc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gmknhkdxf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gteuydhmo.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gsvazouop.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfvsdpvon.sHtML

Java: String greet() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwkacsbyx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gtznitfhs.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gptcanzix.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gguhocjnf.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gntymuiev.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gobrzieqy.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gtdjlpatl.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gqbnubhno.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gbimdzlqv.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/ggnrstmbe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/gsgmizmvh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gqcysykii.sHtML

C#:   class Admin : User {}
来源：http://3g.bbcook.cn/Article/details/gkggobzcm.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/groziwsxn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/giqfmndnf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gnrfoqvwu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdgdiwttw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gnvpfopvv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gpasqcsrj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gqvwmgcui.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/gowsdxvpn.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gobjmjsiu.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/grdbgakty.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gugdyuyua.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/guwppqbko.sHtML


<!-- 参考信息 -->