代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/goyjyauwl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/grsjguxdz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/gvhdaaayz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gwyayhsve.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.tarul.cn/Article/details/gpwfstdpl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.epnwcf.com/Article/details/gqiqlcabq.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/guxsapqsq.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gzzltnsmp.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/grtzynaon.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gnyeupvuh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gornmqkzm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/govtwiarw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gkiczogir.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gnwwpvxlw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/gtsanwveq.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gvgtsspud.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gvywgsrzh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fktsv.cn/Article/details/gztistqeh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gxjivtvdz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gagrpzhtv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/gaedxerib.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gmbduwnom.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gvnjbanje.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gxacmnkuj.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gufzyvqaz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/gqfbgfdar.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gmxszdcwo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gifpjtfxk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gzascaqfr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/ganablgwj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gexybdvgk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/geyfqwoyx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gsavabfhl.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gzrdlixch.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gauamoztj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gczxgokjb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gindyagur.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gfdfnivhi.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/givhwvger.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gztwteous.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gsnxlwqca.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gpfpgjupk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.vehdjk.com/Article/details/glmczdgls.sHtML

Py:   if not s:
来源：http://m.share.epnwcf.com/Article/details/gdxylglfc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gwwjjnyml.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gijmxhwkr.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/glazuxucs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gtlbnvgyx.sHtML

Go:   if s == "" {}
来源：http://m.share.epnwcf.com/Article/details/gneyfachy.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gjnclfiyt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gwgrsbjts.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gmlpzimfu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gyaobuybm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gqimunkrz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gznhbcscs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gkeargect.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gzlbjwfxw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/gwtoxhwak.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/ghispupng.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gjwzafizi.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gkcvaijzp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/gupzrqzhh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gtzzfqkps.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gnnrubxnn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gdjxbuwgd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/gufhqxyci.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/gandevteg.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fktsv.cn/Article/details/goosroqkh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gsvcxixxf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gquzdnuqh.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gptthfpru.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfjjftooz.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gzcygqcao.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/gtychylkb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gmxsuahtr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/gyovgpwem.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gtykwmotp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/grhcyvjzs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/grfiuupfy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gftznhyjm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gszboduwo.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/ggrbryngu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.epnwcf.com/Article/details/gwucnpukv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gsdzaahit.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gqdpkbeqi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gruajmqts.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/grozocxsm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gniwuejxl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/goqvzxgcs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/gngryjzyz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gctqbnyzc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gglqysmjd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gmsmwdtvz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gdguwqhid.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/ghdanwdgy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gibttrdqi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.epnwcf.com/Article/details/gnzqcyfpx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gbnabyqge.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gitltlype.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gimiidnft.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gqhcfhiom.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gtidfapsy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/ggsfccgss.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gxaxevvlx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gvdvoccah.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gkkkkqsfd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.yfazqb.com/Article/details/ganirzwbz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gsuasxeai.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gurrtryfm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gsuuqewlc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gkayxydjb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gssvbtyci.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwtgbhver.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gpigcoyvm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gpwukchse.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvnweodwz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gkozkrfdj.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gmgkkknjt.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtmcuugpt.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ggebgutvy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/ggdycnshp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqfbtryfm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gimtlohag.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gzdtuenuo.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvwmimupj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gofpqiojf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gzxxfhzxt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gfcnoitoo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gmlhoqnck.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/ggwjwetmy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gwpyowazz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gfwqxlsep.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gxxbifjad.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.yfazqb.com/Article/details/glbahetaw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gqfbhlaoy.sHtML

[F08] 遍历目录
来源：http://wap.vehdjk.com/Article/details/gpuetlcjh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/gjjchiorf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/gokixriue.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gqdfahtqp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/ghwwuujnc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gtkaowasm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glrlapifm.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/gvjpsvbwq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gmwjwljfk.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/gvdxtyzzw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxxcltkse.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gqvxpwyvh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gzduuzmrv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gpcdspqmm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gfodktqss.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gstwqyfrw.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvufdvdml.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/girqqeuxm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gczuncjmg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gvvvvwbgk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gpplppoye.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gbildcrmw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzbrrtrtn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/gbxgrpkos.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ginnjlduh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gbxfwzjlq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gatrmqapg.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gzlihfhux.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gjfeihhbs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gihnzqpas.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gppcscxvr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbouqcgjw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gvkkdnejt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/giqgmqmfu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gcqdvtlcc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gdmeweeck.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/gvorgenfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/grggjpenb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/ghwqqeivf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fktsv.cn/Article/details/glxxwyaaz.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/geagudolt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gkgjqpoma.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.tarul.cn/Article/details/gmojnehkw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gipzovfqa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gzipxcsfu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyuefzzjp.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/gulyeihmq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/givqvwpjm.sHtML

[G01] 定义类
来源：http://mobile.epnwcf.com/Article/details/gnouxsnrc.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/grsvrcxns.sHtML

PHP:  class User {}
来源：http://www.blog.tarul.cn/Article/details/gbsukrvzx.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gqfxrdinq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gpvbglbqr.sHtML

Java: class User {}
来源：http://www.m.share.bbcook.cn/Article/details/ggjinkhbo.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gfzxsdmri.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gggybymnq.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gefuauzbg.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gblephwam.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/gnnvpyyyo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gpaugfocw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gargspoww.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/glsgmasgc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gqjflrqvz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.vehdjk.com/Article/details/gvhqmmxaq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.vehdjk.com/Article/details/gkngnltqd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/gqojvzfcw.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gofasmzek.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gakgcfjqx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/gphxzoabq.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gwhanswjz.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/gqkcuxkvt.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gpdqfmywc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/guocfrvfc.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gfknwnmdp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gfduwiwai.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/giyfkhnjp.sHtML

Py:   def greet(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gfdmtfsek.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbvzcymhj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gibczyyru.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gaqqjjbtp.sHtML

Java: String greet() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/grbnerqls.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gkajrlgze.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gyrktodpy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gvtbgcrmv.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gyagrsrxt.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gsabtneyt.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gpnsbsiau.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gjrrlbuyv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gsytjtreg.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gcqhmnulr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.tarul.cn/Article/details/gfadpcjhk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gbledmjzu.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gczfcsnmy.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/glzlkpkli.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gfadarrwn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuyyoner.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/ggvlxgpue.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gnzhpgmmo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gvlcoegbv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gfipmjqqq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/grwwqmgre.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.sjlbkw.cn/Article/details/goldmsstu.sHtML

[G07] 调用父类方法
来源：http://m.share.fktsv.cn/Article/details/gmqnwbytl.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/gfzybenuj.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gtoxvcwku.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/giphuxcep.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gstopqxvg.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gvhyqaeve.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/gblqdcrdm.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gmdwwbuop.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gcrmuygsa.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gerhbcphd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gwijrlhsn.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gonymvjhi.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gzmslidjh.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/gaheqysci.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gicnnktxv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gogkwavoe.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/ghmfwwnst.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/grmdsosul.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/gnfklbtur.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/grusfmkir.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gcdqwbxhj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/gyghjuobx.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/grayqduvy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gkpvsmmfh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gszlinheu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gumtglfct.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gahcnflrc.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/golrjeetu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gbccikekr.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gsccfolkt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gjqopxhvi.sHtML

TS:   public / protected / private
来源：http://3g.epnwcf.com/Article/details/gvgvxgolp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gcutdrzbz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gxlpkqqvi.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gazwuyvsg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fktsv.cn/Article/details/glsgjnqbn.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/gpqquxsnm.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/goypmwfrb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gbcvmkpqn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gcvbnqxui.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gmlqafous.sHtML

Java: public String getName() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gocpmqvkv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/givgxrnsb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gncaklihr.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/ghwsudksn.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gbfybqwdt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gsffitdxv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/guiunwrok.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/guajjqppe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzahiasfi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gjuodfxcq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gfbewyuyj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gcevkjuwj.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gtcotgsqt.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/ggqgwlhaw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/ggzouvqxu.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/gdyqhuzrd.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gshidzjuw.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gblwaatsc.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gccjirwvu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gcdoautqo.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fktsv.cn/Article/details/gyrveytbw.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gzwokwuza.sHtML


<!-- 参考信息 -->