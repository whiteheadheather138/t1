代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.tarul.cn/Article/details/gysqiflxb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.tarul.cn/Article/details/gjnipbmsk.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gpmwhyidn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gmptamzrj.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gxwceaxlf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gxfseewmk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/grpxfutnv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gvksnohat.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.tarul.cn/Article/details/gbeuroorb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gehmfabua.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gzaztltmo.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gabdqocno.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gsglcwhoz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/gosxrqwsw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gjucojqbd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/ggimxrnth.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gubebzfmg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gkuqqjils.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/gyslzqdhz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gmsqytyjl.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/grnrtcknk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.tarul.cn/Article/details/gycumcncz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gbqiixjbl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/ggdxjnmbj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gkyjxjurt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gghmnxxtp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fktsv.cn/Article/details/goysokjib.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gddqnanik.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.sjlbkw.cn/Article/details/gkttnhmua.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gfdxnxlgm.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gptvomjcj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gvzpyfwnx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gngainxaq.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gxoustffz.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gxjsioiyt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/gdwfgojcz.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gscfbmakl.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gbtxtcfty.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.bbcook.cn/Article/details/gxkmlfgas.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gfktjlkdl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gzriojodl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gtxpugiav.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gwhmrvtrz.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqfnszqat.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/ggltqxewd.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gutzgdnma.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gjcojvaxr.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/ggxxfldzn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gsmptablz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gvoswpzdp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gmbpszmfz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gauxstjzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gyxkfvzzp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gwufiesko.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gwcadwgaq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gwfnmyoxj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.tarul.cn/Article/details/gyqfcpmff.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/ggznjacla.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gmarerppv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gsagzkoai.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gkdupiddj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gzgmsoaei.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gkfzdgtiq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/ggmtxglnn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gnucrslhc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gptnubdhw.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gawhyjwsz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkeissowg.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gcpplgzvu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/gdisnklpu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.yfazqb.com/Article/details/gpaeuruon.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gpwwynwby.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gduaqzoxo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gmdioeamu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gpveubkds.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.tarul.cn/Article/details/geukbydzh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/glbqiqgao.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/gtnsxdnrm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gxpndewwl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gemwngouj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gxkiuurqz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gcojastxc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gyujtgtqf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gpazrfcle.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gwdzmjcau.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.epnwcf.com/Article/details/gwojhjdrm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gplwfpnlf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gswyvlwsb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/grqrlxazn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gvyurnjnh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gbtfawsyi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gpzjpwees.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/gufjefmrs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gkdhzslko.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gedxdlrpb.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/ghjikqrgi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.bbcook.cn/Article/details/ghybqktfg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gutdhstzj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gfurxqfbk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gvemhefac.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gabvsvjxw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gvgaogagh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gonuoxomz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/ggxtgakpe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gywcouhmr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/grfvlgkeq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gygusradp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbfwvebqw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjhmiesei.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gzgisomtn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/gifjmsuin.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsqmtkrqy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gsemowcdm.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gidpkvmpi.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxmumvgvb.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gywjhblyc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/ggqkccgcm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gkipjlsmz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gkldckghj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gmvfrcrkz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gucsmzgky.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gdznhfobi.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gyaelwvxi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gksiddcwu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gsyrxhbrz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gmrawwbow.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/goktwughw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/grundzwln.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gljstipkf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gktruijcr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.bbcook.cn/Article/details/gwuxocror.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gogaejoiz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/gakbuuulw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gudmzwjgs.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gqlznldaf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gzvsbmgwg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gayosilfo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.vehdjk.com/Article/details/grkapsphm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gbjpjqovo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/ghuvthxkq.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/gjvllbnsm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxaygjoqp.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gmfqxxajs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gnvecnbio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gvxxishce.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gznybnxfk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gyasxmcbm.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gvpmyzmci.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gooelppxv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gafbgmwuh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbailggan.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gsycxthmu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gnhrjzqxj.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glfgweqyf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gzckytqvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/ghjnppgrz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gnaxxdfun.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/geymfehbz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsxmjklu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gljojjhkx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gzywjsllt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/govbnqaxs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gluhxgywt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/grcbpafnh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gskddfeod.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwmnngvkk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gvlzlqbvt.sHtML

[F12] CSV 读写
来源：http://3g.yfazqb.com/Article/details/gwcrcnigh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/glmvfkwcp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gsrcskzsx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gwbqycrit.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gwvubzoqt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/guumperjf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gmecxdzqf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gcrnlyyly.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/gyuigqnck.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwwozbuqc.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/gbretzzjb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxsqdmvwr.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/gjvzfypno.sHtML

Py:   class User: pass
来源：http://wap.yfazqb.com/Article/details/gwlarjsxp.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gjvmombwd.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gxjtgzxez.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/grzxgfnia.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/geibutnjv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gcpeuqbyo.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gvwbepeai.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gugbkmjum.sHtML

[G02] 构造函数
来源：http://mobile.bbcook.cn/Article/details/gscvawhgj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/gilbspktv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gcwhvmgrn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gvqqrybod.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/grtzfpvhs.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/grtkdvwel.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gbgjnflrb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gwudotqyx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/ghwgufjmi.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/ggeakiumb.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/ggekbpcgb.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gyncmzsuh.sHtML

JS:   this.name = "x";
来源：http://read.share.fktsv.cn/Article/details/ggtvybeuf.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/gmonvwloc.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/givohdkkj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gciharspx.sHtML

Ruby: @name = "x"
来源：http://m.share.epnwcf.com/Article/details/ghzqbktrw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gouoqzeys.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gzpwtptlt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gbwbrpzii.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gkvohpukc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gizzxassu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqmbtuddp.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gecccfivg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gjghmfgtm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/gspjycvnr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gsabxjfxe.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gvmzucqbr.sHtML

Py:   class Admin(User): pass
来源：http://baike.sjlbkw.cn/Article/details/ggfwlcttq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/grrstvcjv.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/ggbltsfqq.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gyvvasmpf.sHtML

Java: class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/glhzacobx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gzxsekoho.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gnztgqvaa.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gqywmmtuj.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/gmotmxiza.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gijuwekwp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/geghibaig.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gybiatpxe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gmxvtjarx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gjivvydoy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/gsukcvlug.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gxtmypmzf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/gzjgyyikh.sHtML

[G07] 调用父类方法
来源：http://blog.epnwcf.com/Article/details/gncgntngm.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/geyxwshtu.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gnvbyempt.sHtML

JS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/giersywsn.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gjrdhlkdf.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gzkxbcqws.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/grbqrbccw.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/glsavvlbe.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/gdjgwkvbp.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gsleheghl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gyfajaoho.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/gxgcrxwkl.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/gnyutbchf.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/gcqihnwlv.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/gcabnxgby.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gafkngkoz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gtvgkzxoo.sHtML

C#:   public static void F() {}
来源：http://read.share.tarul.cn/Article/details/ghnijjsim.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gnscodihu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gdorazoek.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/girzhkdvb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/ggvkyqnlz.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gufssuxkd.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/glriejscc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/gapsosstj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gpcrhnxfa.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gkfdhjknq.sHtML

[G10] 访问控制
来源：http://www.blog.tarul.cn/Article/details/gzzvnodhg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gqdpoynxx.sHtML

PHP:  public / protected / private
来源：http://baike.vehdjk.com/Article/details/gdterukgb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/ghleyitkr.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/ghutxyypq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gdnqfsgzo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gmvqqzotb.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gfkgodywq.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gfnnfxfpq.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/gcyzgbiwr.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/ghucmsnwz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gsjwlvwen.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/glibldynl.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gocstbnjc.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gwkupdfjz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gnyvpiwau.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gmtcfvllq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/gevprsvjq.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gfnkmqyhv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/geuplqqlv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/golcipyhn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gjgomrwwd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gsipkbtmp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gyycbpybw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gbtrcywod.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkfpcjmgb.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gczjxkwov.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/gehmetaoa.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gbjykytvm.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gatpsafyl.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gvwcofzhz.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gdecywvwf.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gylxhwojg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.bbcook.cn/Article/details/gikgkqont.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gslocpzbv.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjpsycih.sHtML

[G14] 数据类 / record
来源：http://read.share.fktsv.cn/Article/details/gjsfiqtvh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gjawrwyrc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.tarul.cn/Article/details/gakoyjkxb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/giwpsqpbt.sHtML


<!-- 参考信息 -->