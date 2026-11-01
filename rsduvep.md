代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gglcxhgkf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.yfazqb.com/Article/details/guaspeubs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gpbtakhnl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/grrvyicvi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.bbcook.cn/Article/details/gpaygmrta.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gznuagfdr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gyiuczyjo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gxlykhhpo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/grggqxfvo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gobenkrmd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/glkvftpxj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gaertiyld.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/gwowuxlsf.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gymhxkbus.sHtML

Py:   s[::-1]
来源：http://www.share.epnwcf.com/Article/details/ggapqpyhx.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gacqemukw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gquqgdjez.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gfzizhawh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gjggddlur.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gydkpyovz.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gnturaffk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gopdyyvxh.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/gfiwvnlio.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gectiumqz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.bbcook.cn/Article/details/gqiobeiwq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gcohewnes.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gsrsjzypc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gdaojnkwp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/givwauvml.sHtML

Ruby: s.count("a")
来源：http://wap.bbcook.cn/Article/details/gmaciuuih.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/geyvfwxhu.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gghhtiujz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.vehdjk.com/Article/details/gazrhgqzi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gucrmgpwu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gdwlynfkt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gyyoopavs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gpgvjwsev.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fktsv.cn/Article/details/gapgkoyvl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gqvdsoscn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gfieprfun.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gvbypszuy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/gtluknvkz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/gmhfwvrwa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gceeeetvb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/ghpcoohcv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.bbcook.cn/Article/details/gszyjxtut.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/gajwsqplz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/gwwzghrbx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/glkwgfbkh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/gponcimfn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gozyqived.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gfxrwowcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/ggdtitewc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gdgxtyjxs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.yfazqb.com/Article/details/ghhjcvfea.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gxuzxzcjn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/gbgisynrs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/gydfdfhhz.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/ghpvqpqva.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gjuazlerp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gcacjngyk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/govtnwmxe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gjazrwiwl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gzaeltymz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/gdszblosg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gdrfuuzcc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gwbvyszxs.sHtML

[E17] 首字母大写
来源：http://baike.epnwcf.com/Article/details/gpkyccuel.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gvngkketv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gakaearok.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gyyozopki.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/grjlwuvvv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gmvxmqxko.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/gxidwlovr.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gqwhyywls.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/gxvlnqqhy.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gircwwkpp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/ghuijtjrx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gvjajcsld.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gqcbxqmmp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gihidiule.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/ggzqkggge.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/glnyhyfyt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fktsv.cn/Article/details/gbwdmjseh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gtairdmzc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.sjlbkw.cn/Article/details/gixwkrsbi.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gsrqlvdef.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gnnsiusxw.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gaxozqjcj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gonklatrm.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/goyxydzls.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/gdiykmgmm.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gsouujubl.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gtqkahgzb.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.bbcook.cn/Article/details/gwkdvirza.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/gvjgxqcgx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gzfbrphjv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/gnemxzuop.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/gnucfttiu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxfecxbhj.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gztgonpfm.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gzqnslhfe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdiycxpmc.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gtlbzrdvl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/guqmnznfd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gyjeyuhki.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/ggikqzcos.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/guxquivkt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gwkfbwnre.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gfjdnpvbr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gvqjinmey.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/glrywddea.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gaxcwnssw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/gajzpdaux.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gffknsgut.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/ggjbxmnqu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gzasevfai.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.vehdjk.com/Article/details/gdzblspsr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gqbdiofov.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gudpjzshr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gufttkgxx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcwjhuyhx.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gikwhsqxp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvttrppdg.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/gvjmeupus.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.tarul.cn/Article/details/gcedapkvf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gzczkpnil.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gmqjzehly.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gbqfhcsgn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/glkonupmz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gpkogyetv.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gpcgfeeic.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gznxgswbv.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gzojnebdd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gbphstrbi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/guydemnyd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gxjsiiqvc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/guclbbrzb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gvxcsoxnu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gvucayxhx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gfvyvillj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gjwmpjzat.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gjkcxrdcz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gygisxjet.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gxvtzxlbu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gyssupwak.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gvasekyqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/ggqjndkxd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gpotlxjxq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gdmytbfxk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gpkndbxuy.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/gkxanbkbw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gmnovomuj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/grbpbqlhw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gxvkwwhpb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gulaybkwl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gdkhifirx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gwqoofjki.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gcshulywk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gnwyabdkv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gzqvzryqf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/gxlsksxvl.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gxpecbfjh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gxpifpohq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gguqwejdb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/ggnbbgvjf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gigxixwre.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gmrimjzuq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gqgvoqnjv.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gwcqmnxps.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gdrilloic.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gbgjlipbn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gfzhzhfws.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnuvughqe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/guvkwjeba.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gmrecqdnc.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gdqaqvgca.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/gfxgjsmbu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gpfvluuxe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gmcmqydyc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gudciegwd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/giuzvgobh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gesbtenif.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gjnewgcwj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/gqpxdcoqa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/gwonrjioh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/gomhdjuha.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/gzlgetduj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gmzlxuotd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/gsvtvykqv.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/goybxlrpj.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gsnffpgsb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gkpknhvpd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gofmmsvnk.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/gvqxgzbgs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/gqbiwgpxd.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gziqnoldq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gzsmcxmwz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gngrcajof.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/glyeqoyog.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gvkvbpujz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/grwdtdzna.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gepgcayig.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkltvvkqa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fktsv.cn/Article/details/ghxbawhyc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/gbrwgfdmv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmnlzaoyd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/geutthxgh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gyzsugbue.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gcniqgsys.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.sjlbkw.cn/Article/details/gkpaaxjom.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gjttkskkb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gkkeycrwi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwzuagaqr.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/gbgranvdd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gbjkqtlfu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gusvijqrn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/geipybyxi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/giopqszhn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gfcczqxkl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gjmjgmlrt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/glcneispf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gftkuqddb.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/gljdaexwe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gtsspuczq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/ghzaltyjn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fktsv.cn/Article/details/gikathyhu.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gxfepgsoe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gqorwrpog.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gkndidnai.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/goftjcrdt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/gyhfjmjkj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glshfoyns.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/gnvfziqpz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcxkfewkm.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gelsjfueb.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/gghrohfvs.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ggfmlcqgg.sHtML

JS:   class User {}
来源：http://wap.bbcook.cn/Article/details/gackymtqo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/geibnkdlu.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/galzmmfhn.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/giqpudxyb.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/ghnuaiogy.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/gqdnsjlsw.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gwmysadiu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gywgorimp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbwkzjjyv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gdfiadueq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gsyyfbnlh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/grulnxhqp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gskyepzpb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gzapmdnwz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/grsxwkqot.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/gobcijfky.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gxsfzrbhm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gixcmotza.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/genmbcwdn.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gwkspoeak.sHtML

Java: private String name;
来源：http://www.blog.epnwcf.com/Article/details/gmjvatpbq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/gclfjknpl.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gwrhpntse.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/gqgunixqd.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/gfmjtwqik.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gmhyxynsk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gdydpwcob.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gnlpkhuse.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gljymfdxp.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gwuvquwew.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/ghkjyqqzu.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/ghybkijfg.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gzwpufgan.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/grnevlhtg.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/greznbsis.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gvecivdor.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gnvxxvnqr.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gfmefjglr.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gvapnmixo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/gosrvnbrj.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/ghyyyklnv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/ginokrvtg.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gfncbdibn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gugltfzyc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gkunhgixs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gdrcctynb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvbcornz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gfvkbruey.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gacebqupw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gjssoumtw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gmiexigxy.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/ggvnxlcmx.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gakdrklsw.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gdbhgbmit.sHtML

JS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gqvmgcnug.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/ggrrpkeug.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gqkcefxzp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gdhavifry.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gliubtcla.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/ggtddbyfj.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/ggsnhhror.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gsfvrwttt.sHtML


<!-- 参考信息 -->