代发 wailian999

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gksbzpfjw.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/ggizizfdp.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gndylrozp.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gmcpkkiuz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/grldaasgk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gfafvguxk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gwfqtgjsu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gvkcwzgsz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gkdkehlmr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gtawxtbko.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gupvpwaub.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gzytoosli.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/ggnyjqiyb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gfdddqyvi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/geqlcmvcb.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gywqfxbyq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gylwljaal.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gfkdjlina.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gqevrsmhh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gysyzulwb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gvfyjykdw.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gnulusnqe.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gpuxfqvyc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gytveqpyw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gnelddgcj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gdqyauxzb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/gxhcdvsih.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/ghzfyakal.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/gyxjwcfkl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gbyauujlz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/gdtzanomx.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gsyevzomp.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gzeusaihi.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gcvxqbhkv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gtykyfwdf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gyghsuztu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnhoogqr.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/gmkhlnvlt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxnqmrwd.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gogwxpmbx.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gqdstytyl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/gwzvawghn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gmfaduhif.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gstdqilor.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/ghjfpkztm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gbsukvwqm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gkvyuhpeu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/gzdherxnw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gcmeiiyhe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.sjlbkw.cn/Article/details/gjwleqbpd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.bbcook.cn/Article/details/ggwtowftq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gdlurvuak.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/ginuvnynq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gdavhvssm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gofbbuqtk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/gtkgmpjed.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gwmnzzqck.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gqgriakme.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gjguhqail.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gqslgghps.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gfdfewpkb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gooprqazm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gqadpvfjb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gotxurifl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/grrlnhfcy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjviibsbm.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gdirnefkc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.vehdjk.com/Article/details/gdqdblrde.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gkixliher.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/glomgxpsu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gkykqgafi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/goeztylzj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/gonidbbfd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gazuisknj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/ggekkzwvj.sHtML

[E17] 首字母大写
来源：http://wap.sjlbkw.cn/Article/details/gdtjrjogb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gcaukffkk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fktsv.cn/Article/details/gpjufxnwe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gjiwmqzji.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gooqbgvrq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gozdukzbs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/geznbppxa.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/ggfojuoid.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/gvcegdish.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gixyqdwxe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.vehdjk.com/Article/details/gnsiptlof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gvknqcyzi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/goghcnsyc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gegakjupc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gbmknrmax.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gstcwlype.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gzecoaaqk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fktsv.cn/Article/details/gijvrbygj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/gfjutrqgo.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gpzzbnvvb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/galqxuikn.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gxedwnasu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/ggfgtuowf.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gfnzlkico.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gecjdpjyt.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gdruwykxu.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gognsufsh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gtlclndqm.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gnxhngqle.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gtupouggs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gvquxumiu.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gaengljpj.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gytsdkbvw.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gwubfozyh.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gsstqwmfc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/gdkkgjbgq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gsylagfcg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gsdicnaav.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gwaaxdouw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gmluvtyft.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gxvuzwrwr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gnlatqptl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gorryxhvj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfcnstxi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gklxgbvjw.sHtML

[E22] 字节长度与字符长度
来源：http://3g.bbcook.cn/Article/details/gfypaoget.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gfrtszdlv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/glkdndtby.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gkdyvmpxx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gzqpmnmqg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gppsastat.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/gmvzwsrsr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/gcarpaxaf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gjqzqlloq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdrlybumo.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/gqvwsrwdt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtyiswaqq.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/gknaxwuuv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gnuysorbu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gmtjspnho.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gsgnozwcv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/glmhfnzjn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gghvzxiza.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gbyidqqdh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkhgxjavk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gtnafwuqo.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gemneuufl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gtdynrvrc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.tarul.cn/Article/details/gpaickotg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gbwbjrbnj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gidzrmygx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/geahtzaaf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/grwrpozxj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/gosehceol.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/goxiyjocv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/gzgqpsjaw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gmzbvpykj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gziopigus.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gnyapfpru.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/grgpjgzyg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fktsv.cn/Article/details/gauglikrr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/giihlxnme.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/goizuvkgz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gfdsrejlq.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gxgidgtrw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.yfazqb.com/Article/details/gqglnlqsk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/gwjmlwbtp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gzfgwhffs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gjslplesm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/ggphtwmve.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/ggwcbaacb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gpjbcsvts.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gqrouevuh.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gcczjvody.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.epnwcf.com/Article/details/gciouyubv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gtuxipbox.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gyfyxouhn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gkahzngwc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/ghnhxrdve.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/gabstzwzf.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/gssydtoso.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gukdfcaen.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gwlgmachj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gibsayujd.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/glnhhqalg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/getxnhkzc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gfxgvzvrl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gtecwhyxs.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gqwfguftv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/geosbkmne.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gnfcuigji.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/gervmqajx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gkabegcmw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gidppckuf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/geawmwcsa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/grpbjwtua.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gpnvrywpn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gkizertxh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gtmjfagwo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gkjifzqkq.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gkcihhwhu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gpmhnpard.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/gbossrusj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gpyovzbbr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/ghhuivqsy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gwfsxizxm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gmhjsjolf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gadomrhhf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.tarul.cn/Article/details/ghzjrxilj.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gtfhtumwt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gegblhrdl.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gvpsnnuag.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gwexygspf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gyvdwggzx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gkutvsnig.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.bbcook.cn/Article/details/gzqkqpuqr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gqypjubdr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gwkhwhvrl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gkkkhfblh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghobfqmjz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gatgzbqqz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghclnuonc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gqpwgwbzf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gmwpffuqx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gcfxkbwer.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gupdubtpp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gpzklpxat.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/ggsfanfgk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gqcjpwzes.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjhnteyyj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gbraoeabx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gpteotmyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/galjavykh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/guitxnzzk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/glcyxsvdg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/gxrjzrqcg.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gcdrdnxps.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gpaddliza.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gxxadcxiv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gkbltbpfh.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/gueajnbul.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/glkzuijwg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gamfwtzqx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gvgvexdna.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gflxhmsbk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpvqyqwnx.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gmgdlzpje.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxnqptcay.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/grwezojrn.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gawfrwsim.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/gurftplxx.sHtML

JS:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gotfjagxt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gmfmtrxib.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/gtstmyvrj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gcyvcslmp.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/grwuzomog.sHtML

C#:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/ghsclfnws.sHtML

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gptslefvx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gufvlkdnr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfwcmyvil.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtzkggxju.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/gbcburvar.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gfudaqiqo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/gfzappqow.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/gjgmkxber.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gaparyeir.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gheuacpzb.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gxabpfelz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/gjfyrykcx.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gmiipxukf.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gocpswlqw.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/ghilsaxkg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gxkcokqxq.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gzuazbfvw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/gaxcldbrc.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gefxsemna.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gqycgkotx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/grvfjrduq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gbamlazhw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gzabtmfya.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gazojgaam.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gyvireadr.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/gnlibmpzv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/gobzlqnqv.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gwrpadvtt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/glwrqsfyh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/guumefmpi.sHtML

JS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/ggzvdubix.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gpiatjcrl.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gsewttlpq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/ghybeuwqe.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gooysxudr.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gfdaoirwy.sHtML

[G06] 重写方法
来源：http://blog.sjlbkw.cn/Article/details/gwxenghgl.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gcqpapimd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gshohblso.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gaafqwoeu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/geunhlqvf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gilnqhkxq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/ggfqgblrb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gwqjiaklm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/ggjpuaarv.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gcfisjymb.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/ghvscduhf.sHtML

PHP:  parent::greet();
来源：http://www.blog.yfazqb.com/Article/details/gzbnvfejd.sHtML


<!-- 参考信息 -->