代发 wailian999

Ruby: s.reverse
来源：http://3g.sjlbkw.cn/Article/details/ghrdxawbt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gxvtpvngr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gwqoavgfk.sHtML

Py:   s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gluiqrjwc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gjyiuqagn.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gyinhamwh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gbanffcdi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gllegfusw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/grhsgagld.sHtML

Ruby: s.count("a")
来源：http://baike.fktsv.cn/Article/details/gmgkldeym.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gyffihstt.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/gdtzzhosd.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.yfazqb.com/Article/details/guemqngtj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/gcroprmld.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gjwhmwmox.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gerbkmxik.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gvhcpfyvo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gpypmpcmr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.sjlbkw.cn/Article/details/gkarmpgxz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gezgkkhpa.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gerlezqxw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/gtldsycsc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gnphqryyo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gduhnxcap.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gevyrysbv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gwidxnzen.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gkrkvkyzg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/gssohcmql.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/gzxknqctx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/genacecsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gtbplrhsk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gbgeyeozg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gebhvinxp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gyspkzxfj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gkqlxmxsj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fktsv.cn/Article/details/gyhwbaglw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/grhxyhyhi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/ghdzknibw.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gunewfpol.sHtML

Py:   f"{1234567:,}"
来源：http://blog.sjlbkw.cn/Article/details/gkfqwpbwk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gofcujnap.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/ghwcfpfmj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gynoyswxi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gognvduas.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gryhonwak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/gctldcklz.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/giarbfuey.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gacfuliga.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/gutykdzet.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/ggmigjkft.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gxfgqfsov.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/geruneyde.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/ggodqxhyz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/ghhqddthc.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gssoowxac.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gbpivwfue.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/gjdvunjae.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gzutelvhg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/gdowiydxv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gzzmauwfo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gcrgvsloi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gncxflhjh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnihkjhsz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/gjootswux.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/gtwnixpca.sHtML

[E19] 多行文本按行拆分
来源：http://baike.sjlbkw.cn/Article/details/gkvyqlwgj.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gbwpidloo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/gyzvihbfs.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gewmpskwl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gtlouavbf.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/gytmhtycw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/glhixtfbn.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gmuhsymmf.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gsqnsbzqv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gygojxami.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gemqwhvrz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gyshavgjo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gjyfkribb.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gcqbfkokq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/ggtenbgxc.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gbxgndntd.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/goktceptd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.epnwcf.com/Article/details/gohmwdiam.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/guxowaxki.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gyrvsonuq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gtprxifjg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gjvizrglv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gipzdqqge.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/ghhsraevv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/ggrxekoky.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gwczhtsmv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gnystewgm.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gzgsgbpvh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gcustqwvt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gijlqttdz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gfzwfdbpf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gbamqjscq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gmclqetie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gyuhjovyw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gecalrqkm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gfafcpuak.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grcsyieab.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/gaeovpwyv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwvsrrrnk.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gsadazutt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/glcshmgxv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fktsv.cn/Article/details/gbqxracyd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gbvcsyowk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gyvbiujja.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/golwrkxzl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/goancuyqc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqpyophyn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gaafpbcvv.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/goxbujaff.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gqpeoxihf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gyeevkuic.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gyhtfyprw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gkkrzciml.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gfsktsktc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/ggnxvbmfi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gkcvpaylw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gduodfvjl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gisiitdun.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxypfdoa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gtvvuqjnu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gbtoygrck.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gsnxwkvad.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gdvtlipqh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gngfqnnen.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gkierxeba.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/ghasozhbt.sHtML

[F04] 追加写入文件
来源：http://blog.sjlbkw.cn/Article/details/gttegutka.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.epnwcf.com/Article/details/gfrzyncaw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gpbrhawao.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gdcwumolu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gmarwqemm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.vehdjk.com/Article/details/gpvvhsgxw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gwurtnwih.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/goxmxgzzb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gwmmreqtt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/gdgungcsa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gemhrgvoc.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gdknozcax.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gbhccmuyi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkkmzheyt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/ggbxtrgaq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gtkmxhkil.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghbittjpz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwxuxxctm.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/gzcgnmhdz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghtrwtuxf.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gozecnfiq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/guxdrofaf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtjpjjunx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gdkwzizcj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gswjsgavd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvckpgdnn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gjyfhyjuy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.epnwcf.com/Article/details/ggtrspxfg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gcyqdaoce.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gncchrpla.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/ghapsxfuv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gryriduue.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gdglgngkm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/ggbqcedif.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gijnhxyqg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/ggteynghc.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gaaktcchr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/geiyqpgtj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gibtawvud.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/ggxuiznwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gidindgxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/guzebscxv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gzeeaizkf.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gfecaosrn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gufolparn.sHtML

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/gatfghuoi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzmqajvvd.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gticgcrnn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gdagijyaq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gjlrzouza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gmmyctshk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gcnlwchik.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gfltttybs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gxxugwruj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gnfdtockv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdrddxfod.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/guzuabqau.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gosdmrbyc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/guiiyscgu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fktsv.cn/Article/details/ggoashgcl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwedlaxqi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/glonoxxqs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gknehdglg.sHtML

[F11] 复制与移动文件
来源：http://blog.tarul.cn/Article/details/gllkylwix.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/galdbishj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/geolwkaeg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gohzbfevf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gnvouehag.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/ggjvxbtxi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/gufvjacck.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxiowvdww.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/grtrhpqqm.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gzjugnoet.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gbftagevg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fktsv.cn/Article/details/gedlcqghm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gfwobnvam.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gzopuloua.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gvyybavgh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gytvfthht.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gauzyvomy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/gahzehhab.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjsjyyddm.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/geckoqcxu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggpfwwako.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gjvufjgon.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gappolrns.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gpaxtuxkw.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gkspdvbpu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/ghzvztsah.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gnrwouadf.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/gpnqgicfp.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gupywcvtx.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gctjnfxkh.sHtML

[G02] 构造函数
来源：http://mobile.epnwcf.com/Article/details/gcojhzxfm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.vehdjk.com/Article/details/gfzqctrks.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gazmpkxaq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/guedexfzb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/gttczfnob.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/giusziwjd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gqpmuvyty.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gfubaabez.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gnhxzrckf.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/gejfjvksy.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmfvqaus.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gxlhyjaug.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gvfgxhxtw.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gioiwhndv.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gezycmaoe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.tarul.cn/Article/details/gwbhczemx.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/goitmqfhx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gapgrwpgl.sHtML

[G04] 定义方法
来源：http://3g.fktsv.cn/Article/details/grenyywkh.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gviygjslf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gbtddbofv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gzgmqfikw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gchbigrek.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gvkfvztln.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gineaxnto.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/gltunijay.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/grufwxfbk.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/gksefdpcq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/gvlyjqtwq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/grxrqmcms.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gmxjrcsql.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/ggbhstvbh.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gkrmojakn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gxvkgezvq.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/gdobsybiv.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gfwtjnjuu.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/glmfwbdky.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gkyjixwmm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gtdckyobi.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gpkybdhov.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/ghjyofnzw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/guubpxlsi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/giwedyjfb.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gsgxhtrsj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/glynahirv.sHtML

[G07] 调用父类方法
来源：http://3g.epnwcf.com/Article/details/goiqeajnp.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gmtdlzjuo.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gjdeoswia.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gmrwhxefg.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gdbycmalk.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/grriuqgbd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/geikhjmap.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/gknnlxscq.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gzvwzvwwr.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gyzzpkqyf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gsahesixn.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gwvjbpooc.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gquoyafgt.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxjbolfa.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gxpbwzaph.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.epnwcf.com/Article/details/grxkmmilj.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/ghujtdhiy.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/guvzqusyw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gepfvpzhf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/gngvpegjk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.vehdjk.com/Article/details/gttvsvgqy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.yfazqb.com/Article/details/gqhacvucu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gbhuxqrxy.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/gddhaxfum.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/glhbkntpc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gowgdziff.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gxbibmmxs.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/ghcwhggzk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gbpjivyeq.sHtML

PHP:  public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gupffljfx.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/glvolwmpp.sHtML


<!-- 参考信息 -->