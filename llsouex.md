代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.epnwcf.com/Article/details/gpodpadut.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/goclxbpjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gcbmrhxdy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gwebrtdlc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gixuhdtvv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gyyxkadya.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gyotwzyey.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fktsv.cn/Article/details/gheborhxo.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gwlnvgege.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gitplfbal.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/geymslwpu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/galyufbwg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.epnwcf.com/Article/details/gqazzdxmo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.tarul.cn/Article/details/gaolkykim.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/gjabvziho.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gnblxktjv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gglgdnosi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/geoyjfnwh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gcaoyedij.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gdmbxpdwt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.bbcook.cn/Article/details/gmavqkolc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gkbkncgec.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gdudgllft.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gczvqavxa.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/guevgdfuy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/gypgyoawh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gtmvkrdye.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gzjyxwtsd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/ghtoxuawn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/guwdvbmbx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gthrgnccz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmhkofee.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gowoyeanw.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gzynvxiwu.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/gkwulujji.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gtfzrzeib.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaqokkdq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjybgvqvd.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gpdkgkhvk.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/glijvlzgl.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/guqdqcdqr.sHtML

C#:   s.Split('\n')
来源：http://wap.bbcook.cn/Article/details/gyceuvvbc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/grmxihedo.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/glimhdvki.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.tarul.cn/Article/details/grzufjoxp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fktsv.cn/Article/details/gtbqggbah.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gyxvlumpm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/geddsqojm.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/gqrkrgsmh.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/guhokaayo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gpusystjy.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/gplevsank.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/guvangnda.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gkytaenud.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gezicrdah.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gqowddxll.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gqrikdqwl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gnjvlxrdo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gjjqznknq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gthxzluik.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/gcdlcdcwm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gfqoegwvo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gobbilxku.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/grwvzkmww.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gpoajlwjt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gmbhwsgxs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/geqynddov.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gfflqquzc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gnrjiwqhn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwnhkndlk.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gmutohkxc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glcplrnol.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gyseeocdi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gsyoasuyi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gsyczrlwt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gxrmtqigs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/grrqidlak.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gnhxplkse.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gswysocce.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwcplezwu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gweffkkna.sHtML

[F02] 逐行读取文件
来源：http://blog.fktsv.cn/Article/details/givemvaft.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fktsv.cn/Article/details/gfwjkujeu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gkurwpusi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gmhiqbjgp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gwbscrvgj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gfegfdgza.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/gamrmbhls.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gzvtxlooa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.vehdjk.com/Article/details/gqcbmkxfw.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/gervzitpd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gqqwuwlcj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/ghszdjueo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gqeolxjtj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gpceqygdm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gvpzkgbrd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gszmcvgkc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.vehdjk.com/Article/details/gndseqcfy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gkvkmongv.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gojfecgxk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gppygvmen.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.yfazqb.com/Article/details/gttfvggkl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gbmmmkpvi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gywnifygf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/ghkcaujgu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gzqzsbefj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gattkmpex.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.bbcook.cn/Article/details/gjxdcxtig.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/ghfisughn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/gauoehgcd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.yfazqb.com/Article/details/givncgael.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ginfstjrh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gvcwvisuw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gtrmxrbgy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/gkoqzlcbv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gkvpmgsss.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdhvidzxx.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gktkzvolj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcscwgoza.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gsyykbmzc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdgavzaza.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gyofvxtyt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/ghcoxlafr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gpzlkanzg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcbznlzba.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gnhjamoti.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gcqjuufav.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gctyriegj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.sjlbkw.cn/Article/details/gdfkiqxvf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/goungxeft.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gngbygwgl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/ghxbarzvz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/gxrmmakhi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gakqzbntx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/goqwatfdv.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gziftekga.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/grvfpvezv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/gkutpaoid.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gmcgzwyyk.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/grhbcxnrg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gndtzrenz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gdekdiyfh.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/guixbmczb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gcfsfknte.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gkhdshkoa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/glklwovpb.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gfulyfsxl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gpljqkexy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gmkvdpksg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gpaknsuhx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/ggdsutpik.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gxesftbhn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/gihjnoqdj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/grxylxben.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gpsslwkvh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gafelataz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/grnzqzfzm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/goirkfatj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/gvkbmowfk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjlcvnpwd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/glgxnphea.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyfwjpwfa.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gtspdmrev.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvqckzunz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmejafkta.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gsclscofi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/glosrskqf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/ghygsyrqw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.tarul.cn/Article/details/gvrbuszdq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqpievuua.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gltjdjdor.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gbtgbgwez.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.bbcook.cn/Article/details/gxpetdubl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/ghogozlzg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gnzqsysbd.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gaheyzzzi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/gvdfsrtog.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gyaebuliq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gifwywvoj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gnvnvhgla.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gaofgbqfa.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/girrowzdj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtizkzkmi.sHtML

[G01] 定义类
来源：http://3g.fktsv.cn/Article/details/gkeactolo.sHtML

Py:   class User: pass
来源：http://wap.yfazqb.com/Article/details/gwfdvfybn.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/geuxolfut.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gospafgpu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gnvxwjltw.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gnivwhisq.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gmjhbcjhz.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gssvlqmwr.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gendkziyn.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/guaygaluo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gadqxzljw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/guragxpqd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gpxrckhzx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gffijdhhj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/grgbrhrmt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gsxxjnmge.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/glxntgggn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gapszkgaw.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/ghpufrrgs.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gjfdxlanm.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fktsv.cn/Article/details/gukoruoco.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/ghknypxwz.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/groqixdzj.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gujlauocu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/ghqjzxogd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/giyghfcrk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/ggouprkmg.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gwyffnple.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gmewvoesd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/grrmaqllv.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gazdufhgj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gppwgyqgj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gjraugzui.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gwqcfzeoh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gwtyvgewh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gditzaukf.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/guwqrjjpe.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gjilfrsqn.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gvmavaxlf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gdlonqyur.sHtML

TS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gnssddnoe.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/grtcdtfsg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gcrjjqaaz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gcidouipr.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gfvligfmo.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gyxciabfn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gsmlrxrwt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gopmkyadw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guxppxvbh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/ggtplwwlu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gzgiqbpju.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gqiuazkoo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/ghuvvivgf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gptzhxfad.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/ggnctauvt.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/gwaiqxwxm.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gaoowyysb.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/grtjnnxty.sHtML

TS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/goqbcliqi.sHtML

Java: super.greet();
来源：http://m.share.tarul.cn/Article/details/gpliocmex.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gukoqrvsx.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/gvymaltdv.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/gilkvhzos.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/ggyzveuqp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gmwphaizk.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/glhkljang.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/guhvghmih.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gnzxijqoi.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/glrhmjcyt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gabmgyijq.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/guutmxxlp.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/giwdbowoi.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gcmwstzsb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gsloyipdl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gbgeqcdey.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gwnrhljdh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/gwhqescxz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gbxlvzouk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/glgnifhbf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.tarul.cn/Article/details/gppitywid.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gjtxfcoxi.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gdwksxsmg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gzgkczcfv.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gvlmxqdwu.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.bbcook.cn/Article/details/gbdpkrrka.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gcfmczgir.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/grcvaglsz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/gobsfrtcu.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/gbqjljefg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gczudcmlr.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/gxwfliuuk.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/gktadrimt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/geewnnhfk.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gbggqcbhk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gynqrwxgw.sHtML

Java: public String getName() { return name; }
来源：http://wap.fktsv.cn/Article/details/gsfwvdfir.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gejejoesg.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gpaerfzuo.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gqrigbstz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoigqxcg.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gwirbdivz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gamourunt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gsaenuafg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gqyxbmsmx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gitfkhudv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gyftgtsrd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/ghozpqbyz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.epnwcf.com/Article/details/gdeuazssm.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/gvzpratwh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.bbcook.cn/Article/details/gpydrgump.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gyvbsnbja.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gehwcgnyd.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gcpapqrqb.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gmkpweqpi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/guphlkgra.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gijzwhyrn.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gbcexikfu.sHtML


<!-- 参考信息 -->