代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gzshxvyie.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gfgmvcsdg.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/goprjpdvv.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gxzrgnwab.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gluyowdzo.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/glginbamj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gpsuaxtqg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gkvbdqtjp.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/gusgqbsoe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gsxursdja.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.vehdjk.com/Article/details/gvkeuocdx.sHtML

Py:   s.count("a")
来源：http://blog.epnwcf.com/Article/details/gdnzpenfs.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/gljnfliyf.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/grqkfjpvu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gykocjhcx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.bbcook.cn/Article/details/gzieepvxk.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/gybicxaep.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gezsgucba.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/gtdpqfqnt.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/gkuwarhks.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gvlgcfzgu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/gcvdmlaav.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gmytdlhfi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/glylrezzn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/geqjqfcph.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/gjfigzjpw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzaytzxh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gftsanyaf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gypocgnmh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gikvejyoi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfdotyvs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gdkwdmeno.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gjgvyaiwv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/guxklkxmc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fktsv.cn/Article/details/gzguxciyn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gvvnczchc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnhfzaim.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/grtiwvser.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gakukdhuy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.epnwcf.com/Article/details/gvwgyjriw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/ggcphyfsa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gucpyngby.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gkikjhbwj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gtrqhansk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/gmiinymmo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gkyawfafn.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gnjcnnidq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gsdoheuot.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gqqnyabsm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/govgduyic.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmzjakai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gqejhkmoh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gwvukznhc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/gomowlwpc.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/gsglpqulb.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gvtnsjfby.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gndcclzay.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/gyorebfkv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/giunnnwlv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gvjgjnnmx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gmyejidfy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gunaiwltd.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gglnhfqvn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gxseaqhbb.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gjxdqretx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/gmyszvqmy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gxcroazrd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gqoyjcvnz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gbqfseamo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gqnuuugwu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.bbcook.cn/Article/details/gdoisdmvj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/gztfienmq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gxbjltesu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gqbewcyvp.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/gvcefcngr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gpyjdgnzj.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gwdbqasik.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gqudbozjd.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gvjlssrbl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gamhomcdb.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjooxcsn.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/gfojmeimc.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gvuglkvzn.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/gefusgftu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gzidpmjst.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gznsladnq.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gfbbxtrfb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gqwdionrx.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gloufxgoq.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gocwedrsw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/ghbhbsjrj.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gthritesy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/gqnlmtncu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gotzoozjt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gffvvgchs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gsclalwtm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gkshgmson.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gisnwnhfj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gayzgpuom.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gcdmgsxqu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gnwlytxno.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.epnwcf.com/Article/details/gpuqjhagr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gmtxmmrix.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gpovfxvsm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gbqjsxhpa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gjgamtvwj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/gqetwumhb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/guwsahpla.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gbpbzazkh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gidlqtsha.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gvxsvtcjw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gptikauim.sHtML

[F01] 读取整个文件
来源：http://wap.fktsv.cn/Article/details/gyfdubkdh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/gtnkfrkfg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gqmoqkqji.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gvvktiiiq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/geykscxvr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/guwivjqcz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.vehdjk.com/Article/details/gucsdujec.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyzbdjcp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/ggkxzijbr.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gawnbojzt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gpackvjbp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gzglobgel.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/ghffsslbn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gtbjjvgnl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gezepakmn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gmwfyujpx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gpwhfrgec.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/gixvjucgt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gxgyfzfmw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gmdqrhfey.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gstwwxjyq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gjaxfupmu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/ghkqezwse.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gawojpxtu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gsbbzzjgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/guqifmnqs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gvjzgwtef.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gcuaqgtcz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gyxklywoe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/grtxagyfj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gdteddzji.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gpffcyarj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gjzbaxffq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gkyyhxufv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gjrxsiccp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/gbjqrbpdi.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.tarul.cn/Article/details/gftymgbid.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gzjjlmngh.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gubymjlbi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gahorwego.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkcnfimyh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/guqqvpcce.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gnpyzbsjj.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gzpzafknx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gokiakkhw.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/gioehbjva.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/glfauzqdz.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/guhlgmsfk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gtdrbcdld.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqabtdkrf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gopudeolh.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gteftxmdr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gpcwoqnxv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gfpjzgzgb.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gxoaifyab.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gcfzuojis.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gtvcukocj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gepcvyndg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gigkczsoe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/ghakqyvao.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gzpofzwuv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/greixmpav.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gipzfadtt.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gcrdcvumg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gvbtrtgbt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gmtjcymyy.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gjxnxlqqn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/guvmpmghp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/goymfbpkx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gztsohsfb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.epnwcf.com/Article/details/gsycjrppz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gtrrmnpuj.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gjtldvton.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gaqmzdwev.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gxhkbrcoq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gvfyniamd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gyznzteav.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gasqvffdv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/getgikzso.sHtML

Ruby: File.size("a.txt")
来源：http://baike.tarul.cn/Article/details/glmovgtif.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gmszxvuax.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gipuzrkoy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gldcbnmct.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gzaycaryg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkpaxeryr.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ggzfcihbd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/garuyelgq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcpuinyck.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gwznuffwg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfsfbkous.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/gmzoffjor.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/grbyrfcjx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/grhmsnvwm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/graaafaft.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gejvtfpib.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gvyqxmtsm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/ggxuekncs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gqxectozg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/giqpgobiu.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/grbcawine.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gotxkzqnf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/geecpmnmr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/geecvpmvd.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gxfxhjsdn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gxnaswqev.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/gkthhbunl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gyhzpqzep.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/glzzvrpva.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtluuanph.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gdbxjmyfs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxjxsuugq.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gdhartpze.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/gdpzylyca.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/geuwtndff.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/gabssrsyz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/glqhevjev.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gyqgwriby.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/gdgybynaj.sHtML

Ruby: class User; end
来源：http://baike.bbcook.cn/Article/details/gbiqvbcbu.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gfklvacnx.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gtbfskzur.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/grkzznuzu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.sjlbkw.cn/Article/details/gqfzyndgl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/grwznhkgs.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gigwtmjjo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gyinyzfvm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.epnwcf.com/Article/details/gccaglzds.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fktsv.cn/Article/details/gxgvzrage.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gmgtwcyef.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gfkygtcpt.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/glmhogecw.sHtML

PHP:  public string $name = "x";
来源：http://wap.fktsv.cn/Article/details/gxrkmvurq.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gojomicut.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/ghbozdmnf.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gajbqkumn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/gyqldnadu.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gbgfipdas.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/geotbjbya.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/gbhncnmyo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gwwavntic.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gzdlxufjr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gdhjzunfr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gndpyinqf.sHtML

Java: String greet() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvvasvxhx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gmyseiksy.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gynoymmhf.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gpzcqxymg.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gtgymungd.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/glltxdyob.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/guigdoajr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdltovvzl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gozzmzuho.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gjjbacnse.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gezdprnju.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/gwumvvlkb.sHtML

C#:   class Admin : User {}
来源：http://blog.vehdjk.com/Article/details/gsnpntfrh.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gpfxfpvmj.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gvpkmwehs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gkpscrtrv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gyezpnzes.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gbkqjvfeg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gfidzmsuy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gpuppdujm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/grgbpkojd.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/griauacmt.sHtML

[G07] 调用父类方法
来源：http://read.share.bbcook.cn/Article/details/gpzqbeylh.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/giejbczec.sHtML

PHP:  parent::greet();
来源：http://read.share.vehdjk.com/Article/details/gcskrrbfg.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gcqvmceyk.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gclywjoxr.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/goemfnmuh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/giohtmolx.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/geeututly.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gctmctjwd.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gfcsnfruc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gjjrunlxo.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/geojzuemx.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gojzpcrqr.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/grdbiywiw.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gpadtjrca.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gwqxfrcul.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gdagqfvmo.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gpuqlhpey.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gazyskssz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gzhjyomsj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/grqdspomc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/gjehdzwch.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gbyekngsn.sHtML


<!-- 参考信息 -->