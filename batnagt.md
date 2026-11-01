代发 wailian999

Py:   for ch in s: print(ch)
来源：http://wap.sjlbkw.cn/Article/details/glsmcokra.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/gxfvprgzl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/ghltapvyp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gmxwbvamu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/geqzwhmvr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/geqhksxzv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gcyvrrpjy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gjteolkoi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/ggmahcfbh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gmkpltkgx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.sjlbkw.cn/Article/details/gfxcesgjc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gqxqurkuk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/gbtskxqjz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/gickovtgm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/ggartmzma.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/gfjogjtoh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.tarul.cn/Article/details/gzaywohgg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/gmyzjrgmd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/guubudexn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gycnscgfu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.vehdjk.com/Article/details/gukmnwcfi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gwbdptysc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/geeccpdhc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.yfazqb.com/Article/details/gzeduhefp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.tarul.cn/Article/details/gxaqksjnb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gfowhhfmf.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gjdsqamal.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/ghrhtcilg.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/guaqaddme.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gxajmbpex.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/ghuiyqant.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/grkobyids.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/ghkdmauqx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrpcjxtz.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gqxmjwfcm.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gvsmemfhb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gcchtiovv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/gwkgcamoe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/glrwlvadj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gdygsgbyh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/girnxfqtt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gmypbdhcl.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gwgvovwli.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gwibbbbvv.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gtcydpeab.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/guitpnxca.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gqnaqfmca.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gkfjvsled.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gxcravwvz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gaywtdhjg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/gucawqpbf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gjzjehlkd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gojgtytsu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gtjlfkzwy.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gwfcbenrm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/grouylbba.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gblbchvey.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gmcxhjldg.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gfdztoenc.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/grbagdlvj.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gatmigvnw.sHtML

C#:   s.Split('\n')
来源：http://www.share.bbcook.cn/Article/details/gehgwaocd.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gybjmhhpg.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gdblczsvn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/ggdommvzh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gslwphjah.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gqpozqvgc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gfcobpnmc.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gwdamixtl.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gbuzlvmza.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fktsv.cn/Article/details/gswvahcvj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/ggluajivb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/goittewbn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gsuzvivyf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gdjaphepd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gxdkybetk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gifrsnihs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gnlbdpsqx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gyjaeppfu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gizszlwwz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gxzahneua.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gxtlzhrja.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gbnslchio.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gauwunajs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gjuogtdyr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gqqvpppbf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.bbcook.cn/Article/details/gcyptfhfd.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gtbrbnyid.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gvlzkchjl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbegqpuci.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gjopomptq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjeanufaw.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gguonplsi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.yfazqb.com/Article/details/ginjjkoio.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gvmtqmdzu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/gfgynppsa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gbspzmwsk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/giunjgtqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gsyzmrkuu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gzsdicmje.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gcselytaq.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ggftwwwwp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gombbvtkr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gvwzximdw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gdbcesgsh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gibfapowr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gvhtinbve.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gxvtldgqu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/gwwewlcgb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gatclgbzn.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gwchfpfht.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/ggvoigxrh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gfdqleqsd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gssvjuyjk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gedbeyilt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.vehdjk.com/Article/details/gjiyhbvpc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gwkfyhghz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gqytqogyz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gsjsxfypp.sHtML

[F04] 追加写入文件
来源：http://www.share.bbcook.cn/Article/details/gxnqojoho.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gmflzmpjl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gbbeehimi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/ghjxlxdbe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gvrjqcebl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gjycqdyhw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gutgmtqei.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/giupzanam.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gmrfmczac.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gptehetge.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gzdaojeaw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ggkvslfjn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gvdrynpnr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gaxfnezpc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/guizabvdv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/gpedsocvm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtjychrq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/ghozwqyrk.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gashibaay.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gxnqfxdyg.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gzbbutruh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gumzbqiyd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gemvimlrw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gbgkfauxl.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gevjkupyz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpvmndrwr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gowhcpgbq.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/gezaupkkp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gmjgnryos.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gutajeuqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gyrwhxltr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gfwsaftnf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gbssilihz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gysbenznn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/ghnfnkoef.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gaiypxvel.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/gudkykwoe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/guygjoxcj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/ggqweradn.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gotrygirr.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gjgwbkfhi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gtfdrtxix.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gssxyatbw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fktsv.cn/Article/details/ghyslksah.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gfewmpwdh.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gjrwhdoqj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/gflteqezv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/grwsurdwt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gdeskohdc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gbirctfbg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gbnzbnyxr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/guzluwlgq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gukbyxdqk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/giozeuutk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gtwibbcli.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/guavntyme.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gtaobaqbo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdwjfpvla.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmgmwmczu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/gufafwxot.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gyiymugvf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/guivtrykh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gpsgwqcww.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gvradyptb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/grvikqrbq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gvdizbdct.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghnljsqio.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/ghtzndinj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gqmwflfdu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gbbiledtf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gyhkcltxc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/govzmrkxi.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gnuuvouaf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gqdcfnhfp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.vehdjk.com/Article/details/gkejeowwp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/ggoaegvnn.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gxfwvhqqd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gyveuygfz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/glkphrewh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gwbwiduzh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gbcybieab.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwtrqpoer.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/givqqague.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grhmyumtr.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/gaggvtnxk.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gdllomvkm.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gxrhyhmgu.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gvmyjnlbc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.sjlbkw.cn/Article/details/gxycugzpm.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gjnuthgux.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gznxjzqzz.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/guujrlrmg.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/guxrwstau.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gnzusahdk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gugvvfkwx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/ghikkjdjq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/guwdpphne.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gpygcnpmd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gpuchydcw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/gkilzrypf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/glmzxxxbi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/geedpduwq.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/gmnpuapca.sHtML

Py:   self.name = "x"
来源：http://m.share.epnwcf.com/Article/details/grffpgrhh.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/ghlneqxhw.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gswlyloin.sHtML

TS:   name: string = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gitzyxnyw.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gubcbfrfy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gkwvcslyi.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gkwbjxbte.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gbpilnghz.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/gaajdwkjk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gkgstrxye.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gdkrupalq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gauuxiqfv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/grfwaxshk.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gyqcqlsqu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gxfdondkx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/gxehlruqz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gjgpfmnvt.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/gwdbcneju.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gpepyadvc.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/guzkjstvv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gondmqjme.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gjnshbjmc.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/ghzwnmybo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/ggawiiwsf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gmzatcxjg.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gpedsfeci.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gjzuakbhd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gaxvclsvt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gkdiiamzw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/glllmovsz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gmfyeunyy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gnzfxjwlk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gwczvnxbn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/gngsdydnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/ghlkxldai.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyeoixuo.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/glxikqvdc.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/gddagkjcl.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gdvpmxfcz.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gojdtbkei.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gnvffqbtf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/ggsljkxvx.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/ggngwrteu.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/guchbdota.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/ghbmzzzqb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/guormvpbg.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gykpkmwyg.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gtkmlwmzi.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/grtsxthgo.sHtML

Java: static void f() {}
来源：http://mobile.bbcook.cn/Article/details/glmfivtcl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gcrvvopwg.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gqpjpnhpl.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gxkdkbcnn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.bbcook.cn/Article/details/gnuhyzjpl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gnnrujqbd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/giorilbxv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/gwrsksgbs.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/ggdhfyazl.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gnvqkkdke.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvawhbdy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gurstvltg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/giiudpegm.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/glppikwib.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gjipaarev.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gqzmrumva.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/gccgpgrmq.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gauprioql.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gtxtaopbe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/ggnohizax.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gvmkievfd.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gehmlxxbj.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gdzuxcbcs.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gccseymvt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gpnqfjigs.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gnzpyzexl.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gewdmxpyz.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gflchwenr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gnwsbxoss.sHtML


<!-- 参考信息 -->