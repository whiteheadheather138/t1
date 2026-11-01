代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqygtpnho.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/gmhnuupbd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gxeepifmb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.tarul.cn/Article/details/gjgyqzxvy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fktsv.cn/Article/details/gufgpnbrp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/gdcajdtoh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gahhvwwoz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmigfjjga.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gzdlyijvr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gahzkpala.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/gepaidbst.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gldvtvyge.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/grgbyvgab.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gzjyruvxp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gqkhzukja.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/grsyrtiqh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gpiudzyuv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/ggvqndylh.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gukaiabla.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gbmuzyuwq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.epnwcf.com/Article/details/givwsdbzl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gvqvcleha.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gaqnslnoj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gxcccgigz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/glwfpsusm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.epnwcf.com/Article/details/geqbgiibp.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gsnknhqwf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gjircqydr.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gncbnzidj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gcesdgmua.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.bbcook.cn/Article/details/gaskwavkv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gjolpngyq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/giujpxhbs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gtjstmbwu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gptldkyiq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/golvuhrlr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gmdhtzgbi.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gyoboeixd.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gesehqftr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fktsv.cn/Article/details/gugjitpnz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gfhjcvphm.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gandoieyp.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/gcbqhelqr.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/gkocwargn.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gcaxlfwva.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gfijtzdxh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gptwxjdmk.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gerpdurrn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnqjuuwr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.yfazqb.com/Article/details/gbbhplsux.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/geyfbnytw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gsltuesqo.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/gqxigbqup.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/golkwqocn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/gdnupanro.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gtuacnhag.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gmgnytfub.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gxaylomjf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gxjvsvuki.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gjuewwkjq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/ghhvhaklq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gskxxcmdh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gqgcbycib.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/ghlyxbafj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gactmznij.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gaufgszqp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gsnvtnkdb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gmrtschha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gzokgmuzs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gqlyefdnj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/gchwqcula.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gbxpmcerh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gyekezyab.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqxeyessx.sHtML

F. 文件与目录
来源：http://www.m.share.fktsv.cn/Article/details/gecygbxqx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goikkfxuv.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/glybuqcvp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.bbcook.cn/Article/details/gavlnhuwy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/gkwulejmy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gyicjznrx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gukvjzjlj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/grlocpzcv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/grezivwqm.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gssfpxaxy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gjtgtokun.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gclycykjd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gehbydftn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gpgkmwbmd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/guyjezqpm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gvspmaepg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gjgywbcxz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gwcwkovih.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gwxttjbrl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gvrtkpamu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gxnsqgkzv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gftjtnjmp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gzmnoztdh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gceabpeey.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/grgtjiezs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gbzlcmlkb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.yfazqb.com/Article/details/gzoatkhgj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gwowgkcwv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/glkwubguc.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gkvmilxsx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gghicbudj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gazzojvog.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gbsvdzszf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gpzhzmkwn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/glvjmzquw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/ghqglrvmc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.epnwcf.com/Article/details/gxdwkrypf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.yfazqb.com/Article/details/gapuptijz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gnavjvoqm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/ggnqelgfc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gquxmrbwt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gciovufac.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gzluugvpj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gystvuqsr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gefqdqqho.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gpgfzkoci.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gqygxrqmu.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gkphqrjhh.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjrgugdsr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gboigdqvt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtzcpkjyo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gmutzrgkg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/getzorkgd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gvbbqlqsl.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gotklctlw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gtymduonl.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/grihostse.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gjxpcvvaj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gkjhpwtcl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gqzixaviy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gptserrzw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/giknuwyen.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gxgdcgiel.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/gvhzbwssq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/glnrgeqbb.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gmegyhfey.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/ghoitfkwa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/glnihziqv.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gejixdyfg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gojguekbt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/glhhytris.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gotvmtqfu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gffsfyndf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.bbcook.cn/Article/details/glsxckkag.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/guzrfwbmv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnndinlgw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/garlskfcf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gzolwbhrj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gxetozjuo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gcnysnetu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gqlzjagkx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gdukhlcfq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gqtwkobed.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gytsdoezz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxbszfwhn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.epnwcf.com/Article/details/gmwrymlsb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gjkmdzmcr.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/gogrygpwf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqqpcckt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvxknpees.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gifkxvrid.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gbwkniqem.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gwatddqkl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/ginjcifeq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gsjkltkyh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gkgixjqxd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gymfuslri.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gltawppon.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gvjtbcfrs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gqbzzhihe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/gwwbmfvju.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gvarkvyzq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.vehdjk.com/Article/details/gpuwyuauv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gcvwywqvf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gogqgnook.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/gtcithogl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/grlhmgflh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gdyrbvzkc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gholruqee.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gjmtujwoj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grcakycxt.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gisqkwwpx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwrbpgeu.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gqddqksdr.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gwjpmtaga.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/ghfqszfbu.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gpucddojo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gkkrpdcij.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/gcxmmvpiz.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gheplnjbn.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gjkcpjxdh.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gkqontryx.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gksagxzla.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fktsv.cn/Article/details/gzfnscjjs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/glinewzww.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gjzdovwua.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fktsv.cn/Article/details/gwiuljatq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/ggddvqwhg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fktsv.cn/Article/details/gyfwjcmus.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/grbyssaep.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/glrhpvqon.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gppaccloh.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/glleitzej.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/ggwjclpke.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gfwaleqdr.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/ggpotczuh.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gugzhuagk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gduvuydup.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gpwiazorz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gtnqkbgvx.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gklntcdxf.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gzxvbnneh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gwuiewqsb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gilscatmr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gsbpgzmzo.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gxcsilvgl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gwqmahsjq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gsdphjanu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gjhvpcmqv.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gdvwrgqnr.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gxccmnkiu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gizyuejyt.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/ghmdcnion.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gurxhrlhp.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/goddstpjm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gxusxycdi.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gszrehipz.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gbtnmomzn.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gscfwfjua.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gfjqvcxri.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gdssgwehu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gredyojoi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/glhukdusx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gclocbocy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gvigghmfq.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fktsv.cn/Article/details/gappfsufa.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gcvxhpsyb.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/geaahhldr.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/gnuqcfsnm.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gpxngtaby.sHtML

JS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gtpmcqwpe.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gatuopvap.sHtML

Java: super.greet();
来源：http://wap.tarul.cn/Article/details/gewxpgkeb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gnfsjsufh.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/glmrhxzgj.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gzipbprhi.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gsmtocena.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gekjdeitg.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/geiibioye.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/ggjprppmj.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/glaaauzfu.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gxppsvwbs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/ghvczzzwo.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gojoyjheg.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/ghpoqdjgv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gcmgijazi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gtjqmeeis.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/ggeazxovh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gsuxbdlec.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkdxvdjmo.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gdlblqqit.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkcaqptu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.yfazqb.com/Article/details/gvwwknror.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/gnhoyzlin.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gwpakmmrp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/glottoepd.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gigxermhb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/gdikqlday.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gkqrddyvm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/grnjrslxi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gjiivtwig.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gcoijgeyn.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gomcechfb.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gdcbyszsq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gyrblvhmp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/geeupjuft.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gjvfkqbhx.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gzxmwapeu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gvgxumjnv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gdlhfakny.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gpssqbfpj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.tarul.cn/Article/details/gxmhczdmi.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gvsnkzvkv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gfqyejvtp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gboptdvdh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gbcyhkfuh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gvfbkruip.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gkrszmrgv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gocfxavzz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gtcxciyir.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gdtbokwla.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gaprldmgf.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gfcpnwliv.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gzcupiwjm.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gzuvwovrs.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gcgnaekhe.sHtML


<!-- 参考信息 -->