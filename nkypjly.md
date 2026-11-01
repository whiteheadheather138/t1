代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gsfncpohf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.vehdjk.com/Article/details/gdclsohbh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/gadarvkvp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gpqlvidpe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/glcaflpna.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gshtwidfi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fktsv.cn/Article/details/gdtzydxep.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gnzhhqdyc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfscpemxu.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gexwhxrfe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gykykeljp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/glrocjvgp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.sjlbkw.cn/Article/details/gltirubdt.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gnxyvusqa.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/givxrzhiw.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/guibcyhgn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gcimbtkis.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gstbuftkg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/gnpxjtfra.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gbsijqynh.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/grwoijqof.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/ghoajkrie.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gmxcwidmo.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gpzatowrx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gmyymzeni.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gwpzjiojp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gpcrumfja.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gklqyebkg.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/gbragrtjj.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/gzajyeiaa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gdhiwmnqn.sHtML

[E13] 逐字符遍历
来源：http://mobile.bbcook.cn/Article/details/ggywntyir.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gxsvaxyqe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gwpclskzl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/ghpweqlbd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gutjlfhrw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.vehdjk.com/Article/details/gmrfxvbmj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gfqtgxhjs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.sjlbkw.cn/Article/details/grazdcbaz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gjrrpsfgh.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/gtawvwpwa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/gxisufssy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gsnhuljnk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gonghouzi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkjgecyml.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.bbcook.cn/Article/details/gjfxlfljr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gvzraxuup.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/galxtjpiw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gdsivaxiz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/gjfagdick.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gpsuihlie.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gveuktkuj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gsewpbriy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/ghenggjea.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/guqghaqhv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gmlvgmdhm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gzztfasup.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gkxtstzfz.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gwwkvqlnt.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqfhrftu.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/gpitssudh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gnphqloor.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gkblbscpv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gqbzlwtcb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gzebvdxdt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gjsfhkahj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gcretdohu.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gkyuxitxo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gvrvcuxas.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/gnupqdpsi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gxrrixymn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/givxcfhht.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.bbcook.cn/Article/details/gixvrpkog.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gayngmtax.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gmbuubkip.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gwyextpki.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gnogxvxqy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gbcylbnhh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gsmlzpcee.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/ghjxmbrrj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gwomniqnz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gdqtsihue.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gpkzchbxl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gxetqmpir.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gdcyrgygr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gwiddseqw.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/ghrpwdhpk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gdefyroer.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gezbrhsgi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gfonrnxwb.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gdtmfqbhk.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gzwpixoji.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/gnsaebuan.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gbgwlnilo.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gcmqatxxv.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gzfukigpe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.tarul.cn/Article/details/gyydhclkz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gwxagedfv.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gmjrbmiab.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gnutzxawn.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gzudngcxr.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/ghukfkfqj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/gsnwnvjcg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gwurddevf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gubnfswip.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gcaxrrsds.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gapihxklb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gqojfbjdc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gttmpourg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gfzcbxxhu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gebzvevtz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/guhqtnegw.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/ggkhqtdxp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gsvxileit.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gkrxuqlgk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gjrerfbys.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gclldlbox.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gujebihre.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gjdoebvor.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gszhhmesk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.tarul.cn/Article/details/gezhruigh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqfdffzeg.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/grdcniruf.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gotxydgeb.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gxyloyaod.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gmuuimsvj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gclpdicai.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gywvkhfds.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gcxfoqmza.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gieeriqfm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/gpawotkyy.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/glbzdkome.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gqekggkrw.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gkqksatij.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gfkwdicwz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gjdenfsfi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gutbpvjfx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gyrwulhgy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/geekwcmpf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/gbxccvqif.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gpwbdgccq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gldrwbdzr.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gntaywich.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gltbmfclp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gfdlkdifp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/ghdnrgdak.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gcpdrrhrf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gdlmvnpfm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gflqqkbra.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gvoyurvjs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gmftzdbvi.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gpgbhaeid.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gcedrfhug.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gyzgxdcwp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gdrkawtml.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/guugaahey.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gkzhvwtpw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gnyjqfzsn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gkinohvgf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gvicfpvwv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gadtmryqf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/glqxdkpgs.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gtymflvrk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/giwyqxvjo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gnnxwdjpg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gxtofafck.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.bbcook.cn/Article/details/gpkgfkzxx.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gbsobcjgy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gtwjvvswy.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/glkxtbmag.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gyvcbeohw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gbiepnpbi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjgqeyzab.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grknwxtmg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gstktpwal.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gxgegoyki.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gitkddoky.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gbowddbto.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.yfazqb.com/Article/details/gkbnfodpk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/glvrchsln.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/glqdlchkw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/geffbvcvh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/ghuludqvz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/ghubcrdtd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gvfugqwwh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gppebzpat.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/gneigtohv.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/grhkzkpvv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/gxlissdab.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gtnedruyl.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gjratxpby.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/ggknptuhu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/guivbzcpn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gzmlkhurb.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/glriwhorb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gakiolyes.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/glzqqyjer.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gzaqwkbbv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gqqlqdsjh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/ghocxpkhy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gcmrjmver.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gliazwery.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gydyglqvn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.yfazqb.com/Article/details/gptikahky.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/gulxnbisu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/gkjprhala.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/giksnefxs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gbztlrfie.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gyadmgfov.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/geqgsiusj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/gkapfonjy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/guwltnlim.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gomfkydpw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gixmjvepf.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/gryufbiib.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gsqekgelq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gjrxyerpa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gjxfmvrqb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gvsopandu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gamfykpot.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gopbvwifr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gnxkgptud.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/goktudfsa.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/ggmqetvmw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gtouyanny.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/geeerybrw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gdzjvgryw.sHtML

TS:   // 同上
来源：http://www.blog.yfazqb.com/Article/details/grfriftno.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/gzjremnkd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/grxjpeirb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gxwlzqjfy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gwctctjge.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gekzwaisi.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/gmppxtwqd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdqxatpik.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gbcshlafn.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gbbhpfrnn.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gxqoqmqqt.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gnalatvhl.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/ggjpzeqdq.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gngoqkhjm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/gakzdsxqa.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gziwdginz.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwrtnmtbz.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/gjjjvpkow.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fktsv.cn/Article/details/ggtqtcmye.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gpatkhuia.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gidytnham.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/gdpejkjix.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvtbnzgte.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/ggzherpep.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gvfmvaepk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.vehdjk.com/Article/details/gwhomxqfk.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/grrnyntdr.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gcqncarat.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gkwsigwmc.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gyadiilup.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/gulmqxyev.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/grplpcrai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gpndmxamc.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gkasubtud.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gmqprkpkf.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gzubmfuev.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gijwxudcn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gcizsrshq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gahqmoriw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/grbbxqjlb.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gwinnvxga.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gcadblqbi.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/grdigvdmj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/ghgykuvbk.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gnwpcqgfh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gyffjuqgd.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gygvkwjfg.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gqzgnynyk.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gcdgvddxg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghyiuidir.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gbzmaqsen.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/gatqerbkx.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/graggfbyw.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/gkckkyayp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gtwkmmorn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gyvyolqnd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdldkbwtb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gnmhdugrj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/glwdesoxc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gfgjutgin.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/galnlysnj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gsrjsvoch.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gutduvywx.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gixtrrbnh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/geghgbbzb.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/grvjivsre.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gzhzruhut.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gcgdfxgbt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/ghbbycpuo.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/ggpmfeypr.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gtbgmelpl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.vehdjk.com/Article/details/giobeamil.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gdhnqexsu.sHtML


<!-- 参考信息 -->