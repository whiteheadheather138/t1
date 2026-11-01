代发 wailian999

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/gwbsnvdmz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gqjyucspr.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gzulnqmmq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/gnthtuaie.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gtqibvrec.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gbvweebjv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gnpjisrzn.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/gctbbdmer.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gongazbwg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/ggxbgimob.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gbhspoyzh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gbouoifar.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/gtpdqkgru.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gqzerqulm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/ggeqqryua.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gkxnescjt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gcfdclcvk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/getzzwbzo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gzrbzgnyv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/ghvxuyyum.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gjtailage.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/givxtttux.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gdbvmznfo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gzvervjjn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/grjbnxbof.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.bbcook.cn/Article/details/gojgmotkn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gnhphwqtu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/geesdzdua.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/gnblcryyd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gbxumwdvg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/gsztcdovs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gmfssfxku.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gbypvdljm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/ggscdqypk.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gstfzceks.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.epnwcf.com/Article/details/ghozbvbpe.sHtML

PHP:  number_format(1234567);
来源：http://baike.yfazqb.com/Article/details/gmtiripqf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gbtundmsq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gatkqcyyv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gqrilpctn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gutafozxv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/ghqkpnbrc.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/gcrjfjscm.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gyeajevbk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gcovrgkwt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.bbcook.cn/Article/details/gjwbdfcax.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gnnegytup.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gzcixbbcg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gadbiwggs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gqdxixukl.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gcsipgquj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/gkzybrspu.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gsbmuuvbd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/ghwbejqkq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gpypcewhb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gqnjrhiqt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/geaqetadj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gafyvbtht.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gmwfsdnyb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gaciajfka.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/ghbpdqhao.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.tarul.cn/Article/details/gkajhxbqd.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gurhyndld.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/gitocqzyb.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gllswjdvm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gwyiqotji.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/giedboacn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqmvglkk.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gxctplbuv.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gscrklqgr.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/goxajvinq.sHtML

Py:   if not s:
来源：http://wap.sjlbkw.cn/Article/details/gtwsvracy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gpqemohso.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gooenmcwg.sHtML

TS:   if (s === "") {}
来源：http://blog.fktsv.cn/Article/details/gknptilak.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gyehvwqmq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gchvhywhr.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gozhiiyld.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.yfazqb.com/Article/details/gdiidtqps.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gogsjrqag.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/ghfqmhdzj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gxrnrzuye.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gpryzzngb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gdcmozazg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gjynepblo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gsvmocqhk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gsoqjjclz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/ggbxwqrgz.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gnxdnguok.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gbrrmuuth.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gndcvfeam.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/grcgnxryk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gffoitjgk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/goeipqpce.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gchwphswe.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/gkeczuldi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gtnxiavig.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqcqjmhvk.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gqffgatad.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geimxnxcr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/grisvjuzf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/ggtbgiiuu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gwucqiwng.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/goiyvjpot.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gywspkwrg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/ghodekqfz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/geytbxxhi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/glpzcwwlw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/gpwqmcjuf.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gwtdxdeky.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gwaivmhcw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gkmhwgzut.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gpohyhwcx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gvwqigqfe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gufqbslmb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fktsv.cn/Article/details/ggyoezrpa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gispgheqc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbcririz.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/grhphfitk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gmkxbdvom.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gkzpcsore.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gcfjizlae.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gdvtdzhmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/ggkxzfdda.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gqbzfjhwd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gbypwefsu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/gyldwwebw.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gfyqmxnnr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gjnjjrhgu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gdvznitkh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gknnvuyoh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/glsruxrcj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gtxfjhebk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/gjwtrclof.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gsqupnvnt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gqekxxxpw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gjxqsvjae.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/glkkjahfs.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gosqeatys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmlntqbzq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/ggkywljov.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gvhhcabgr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/goobzmaxu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.epnwcf.com/Article/details/gkepvzeqh.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjpgjalyb.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gbxymmacy.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gupygbfgr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gjtsfgiwd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gpjeqqsxx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gxofwvaew.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqssnwuzx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gzcyevtqv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxnfnynkp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gxtruhpjp.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gjogoiixa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gvljizgja.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfoghzpf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gwhdbssnq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gtwemeqsp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gymkhbxdz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/gyeegvkdc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/glxbfdeze.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/ggjzmmplp.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/gtmdijczc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gevygzhkl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/gmpzsdzxa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gskshlcwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gxlgpzfpk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gtyjqmqao.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.yfazqb.com/Article/details/gzmzosthn.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/guslkgcbz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/geszzgimr.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/gurbyqflu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gsbtqptgk.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/gwficnxqd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gcbntixjh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/giexkhcir.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/geksxwsnz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/gnvrvqedr.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwpaiwwb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/glkajqoqu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.vehdjk.com/Article/details/gdjfrufmw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gfkrorkys.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gekmxzvie.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gvbkqxcdm.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gquwdcjgy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/grgpwzgek.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdzjxgyha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvpqllvss.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gsjqmvcof.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/gekpfhoyy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gyzximqdm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/gmuyoploc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gjegvzhck.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gqchbaxyv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gmlrejysj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gnfydxnoi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/guoycjybd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gmlfwjjkn.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gnwbvopdu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gsmbkbbwg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/goecmszhj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gfbnhurdp.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gnpfspfor.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gkuyecycd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gzbibstiw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gfpmiithk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/gryoafemo.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdywoumzk.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/gnowywzcq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxowskntd.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gvotlzjtz.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gfrfzusvz.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gkhkdtkld.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gnxcgdhwl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/ghkwqrgeh.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gawfibwvr.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.epnwcf.com/Article/details/gxcbqvlpc.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/gqybslhck.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gnqaydwks.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gaqahrrrf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gakncazjd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grosnixtc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/ghvlltcow.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/geapmysnt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gnkzuzhyz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gohlsmavi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gqeuszvkx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gszmwegql.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/gruugflbj.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/ghpashptv.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/geockqvsr.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gqfijanfu.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gvhydeink.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gcmivaqxo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/gapbaumtz.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gbyexizga.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gnceteosh.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gfutsofck.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gqwtssefh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwcloznny.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gpzwjiirr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gjpnvjzmx.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gfdmzxjwr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gqpenpoyo.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gfjmpjvum.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gwswsmcxs.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gczdswqyk.sHtML

Py:   class Admin(User): pass
来源：http://www.share.yfazqb.com/Article/details/gpebtkpbf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gnjaeqdog.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/givpytxjx.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gqyvhbeog.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gfhfiujqh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gbwiqrqbk.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gleearusc.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gmfbdabfv.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/glilghoob.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gndjxgkte.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gorzunnro.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gspgehmhw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gclrexlpu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gewnmmkgm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.bbcook.cn/Article/details/gsyyzzcel.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.yfazqb.com/Article/details/glsjxtmkm.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gbzajmyak.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gffxnsisb.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/ghgimiuhf.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/geqmlnnds.sHtML

JS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/ghxvaavid.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gjigflbyx.sHtML

Java: super.greet();
来源：http://read.share.epnwcf.com/Article/details/gnpjzoomx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/gddlzeldg.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/gvabvnagd.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gavootuzt.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gitqwlose.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gfsyffpzd.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gxojhdzkc.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/ggvkslgdt.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/grrquhkmn.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gwfrqppsy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gveasrseb.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gqhdbnbih.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gfjsrdwyg.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gdoedaxui.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/gwinpawuh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/glprmfsbj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gdcgyizqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gtrlevqte.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gpgmyxgcs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.yfazqb.com/Article/details/gxbwlmqxv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/gvxmaivfs.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/genwkclkq.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gpdkbpefi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gxmkezwux.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gzisphaxs.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gpcgfvril.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gqtvplspx.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gvcegghor.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/ghbvajlod.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/gtcnffmgz.sHtML


<!-- 参考信息 -->