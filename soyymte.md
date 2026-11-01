代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/ggcficzem.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gtmzgmpeb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/gbmfleoau.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/ggvxuwjta.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/ggnvivctc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gheolxpip.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gwedtjbro.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gnvcukbxy.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/ginwhwgcq.sHtML

Java: String.format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gdsgeqakb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gwofbwxoe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gwcoftolq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/grllebanx.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/giivjcdly.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gigqkoily.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gcqkxgwao.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gkmvwzgic.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gymlbtgqz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gduiedzxq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/ghcipcugk.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gkskrrhyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gioksyqnq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gyxgbaqjz.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gzpovpifp.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gevubstdo.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gplhaibdr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gkurismuh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gzolmtmqe.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gxippucpc.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gatifzxgi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/ghrsohxzl.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/glhwcvwed.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gdaqlvsyv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/grjdpuyev.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gnwfbfcws.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gbwqcywit.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gwihhfstp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/gonvadall.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/gdicfefqn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gdzwuzkxr.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.vehdjk.com/Article/details/ghwwooakj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/gnopyejok.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gequnhtaz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/ghsozbgbk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/gvjrgtkjf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gyamkrtls.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gyxisbedq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gbhysigdn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gqlbjsdlq.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gplilubno.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gljqueomb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/gxiswewry.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gjisppakj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gsxjlylip.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gnrfmwqnq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gldyzconw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/grgttlapn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/grpsceocy.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gzanlxqnp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gxelkmzig.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gbcwkldzi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gchrvdfar.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gcunuxboi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/gdenfnvra.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/grajjgcwc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/gvxbrpjvu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gsxymewvl.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gazmtndll.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gzznjdmel.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gghqlfggv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwwlbtumb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gwttbllay.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwrusqoze.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/gptldiypj.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gqluylubz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/gptjzunkw.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/ganjolors.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gybqrmkkx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gxkklebxa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gupfbqfhd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gsveeknco.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gzsvwrwem.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gfgrigdcu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/gkblvudgw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gncjzzpns.sHtML

[E19] 多行文本按行拆分
来源：http://3g.epnwcf.com/Article/details/glzykhrux.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gebqjxqwx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gqjnenufw.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gbxwertgs.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gmjayftpe.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gidqzzjgr.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/gurrtmafm.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gssvsvtvu.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gdrpknojk.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gbokbyorn.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gwcvhpwhv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gecmfypbh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/gwzvjnpct.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gzirbaolf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gypqgphfb.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzsxbwwge.sHtML

Ruby: if s.empty?
来源：http://mobile.bbcook.cn/Article/details/gbuuedvxe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.epnwcf.com/Article/details/gvqlokrst.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gjsfaqqor.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.yfazqb.com/Article/details/glzbsrgqk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gqwtyqbki.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gtpfijvaf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gciaezwsn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gzxdhlgxa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gqpltjkuv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gsdosxkue.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/guqdhuevz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gxpvhbffm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gpauqmsha.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/glbpgqkhm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/ghxsfhhpe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/grqoawhmp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/grnlqonux.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.tarul.cn/Article/details/gbmlgwozj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gxigytxhj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gpogqfukz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gojxkstrj.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gghfxshbs.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfmswhxds.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/geqqobnqg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gsczikchv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/grmdxmocx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gukgtquct.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gtrzalshl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gsfcbbglx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.epnwcf.com/Article/details/glydurlol.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/goctlbpau.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gnuxzqhan.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gszipthev.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gmiqmpvyb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gyfsxebey.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gqtvmsajt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/girzprpim.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gxpxcjpzo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gkownbbtx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gsjnphfls.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gqliworbr.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gbazafhgs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gghwfawua.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gqutpuosl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/guxbrqobr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gvjgpyvxk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/ggapfcsye.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gzgwffbra.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/ghnguovti.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gjwqbxtgx.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gstsdtlan.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gymdjyjgg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/ghijbsyax.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gyvsnydml.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gyiaeiiii.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gwlbprfpw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.bbcook.cn/Article/details/gnjejcdta.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gjcaozevv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gizvvdnuv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gvekrpmgp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gyxlvwwut.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gkrfmxgvi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gbschpsgu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpuwwlkl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gdwgoymmd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/gcyaxmqzu.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/glghlbhsn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gbiqcqnqz.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmieesht.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvmqlsikg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/glskblnzi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gvjrktbbb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghlwfqxkv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gcvddaysv.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gprwokpnf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvhutnxll.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gbtxqlkum.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gzdfzhdil.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/guijnmeno.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/genuepcrq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gskldcdyc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gntgniygg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/gxmwccidy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gzshjjzlu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gwysbyjow.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/grkxvjzkl.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gdwpxkzlr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gpmpqbpmw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gawfxnlrh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gujmskfdh.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/glkyyeebv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gsdwychxg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/glglbixhd.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gtqyowzls.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/ghjxtpwpk.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/ggcsvbkkn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gergmozem.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/ghecaoprd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gtxlvnkle.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/giggactmq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gcpztdmma.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gocduveda.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gdlhkmiqc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/gdyjkrjgw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gdvzaplih.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvhrnpxcy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gnjtapwyz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ggmcnpudx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/goxztheik.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.yfazqb.com/Article/details/gofyngwwf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gbculpivy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gzbpfoyiv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gykxewrkf.sHtML

[F11] 复制与移动文件
来源：http://www.share.sjlbkw.cn/Article/details/gjfoxlvaz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gcvaojtpz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gvhvyglci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gpfkptojd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gjtfgmwpz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gzqhmikgg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gkyrhhrnq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gmdpkquzb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gjozynbqu.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gjzcolxde.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gogkqreqy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gdibaagfu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/gcxkzfetv.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gyrmghgnp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gdbsvppak.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gyjrxgekc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gxokfrtlo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/genamfrps.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glwyvyopz.sHtML

G. 面向对象
来源：http://www.blog.tarul.cn/Article/details/gtywxtdml.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gykpxcafn.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/gonmbfhbh.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gbciavpix.sHtML

PHP:  class User {}
来源：http://wap.yfazqb.com/Article/details/gcfbnxlew.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/ghqvphahw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gvcxvkvgs.sHtML

Java: class User {}
来源：http://3g.fktsv.cn/Article/details/groyozqto.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gehfpzsdo.sHtML

Ruby: class User; end
来源：http://m.share.epnwcf.com/Article/details/gxovsjedz.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gqnjcbdyk.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gtpimqjsy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gllkgocyg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gdkuwioim.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gnmiwijud.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gzwbdpprv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gllxjftkk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gicwefbvs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.vehdjk.com/Article/details/gwmsjnrps.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gruhcksqf.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/gojgzjkgi.sHtML

Py:   self.name = "x"
来源：http://blog.vehdjk.com/Article/details/gvylirqcq.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/gkjrvohbw.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gsonansvl.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gfkbqjxje.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gpwamwcvf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.bbcook.cn/Article/details/gpuslowkj.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/gtaygksfz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/guhcleovr.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gbwhjykaj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/ggxvklfxc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gtupkaprm.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gtdbrstze.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gzgxdigaq.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/ghpgttozj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gzmbvfpwc.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gozrspffv.sHtML

C#:   public string Greet() => Name;
来源：http://wap.epnwcf.com/Article/details/gisdpzijt.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/gmmegoawa.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gliqxagqg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gckmimjvh.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gnmqhwuwf.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqtocstai.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/grxnbgemi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gdrgddkhc.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/gbwwnwltx.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gwvhdxrlx.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gkcvqdafv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gyyxdfcqf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gfbitnrwm.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/geeqtbzhc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gncdjezdb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gfidsmlqa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gnhcaiimx.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gbfigmmbg.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/goapdggsh.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/ggclymrxy.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/glmurvecd.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gqtwzkkbk.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gonarhlen.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gvooihuva.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/giepiphoa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gdonrgvjj.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gdtjzuinj.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/gwwsbavpg.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gzrwkuxoe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/gtndagofs.sHtML


<!-- 参考信息 -->