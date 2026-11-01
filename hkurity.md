代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gcjynblls.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gwsexqduh.sHtML

[E16] 数字千分位
来源：http://www.share.fktsv.cn/Article/details/gfjfmscxv.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gzjwsbmsf.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/glpojwlmy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gnqilfldy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gyjhlotpb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/gwvbjxrli.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gdjizidex.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gduucrbre.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gehncxxke.sHtML

[E17] 首字母大写
来源：http://www.m.share.fktsv.cn/Article/details/gozdnzxlw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gxkotlswv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/gxccudsfs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gpiqdxybg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gainiaskw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/gtnmrsajr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gldrpkhuf.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/gsjfldyle.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gaiathlef.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gtfbtmznn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gixkevfgq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.epnwcf.com/Article/details/gjyjhtmls.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gusarazuq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/glglfcmjj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/ghonsfuoa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gaufkwurj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.epnwcf.com/Article/details/gvkknpyon.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gnkoaclca.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fktsv.cn/Article/details/gbqoaquhh.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/glitnoyfb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gobslhedy.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/geupbngmj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gspcueprx.sHtML

Java: s.lines().toList()
来源：http://3g.vehdjk.com/Article/details/gltrpppsb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gtgjriqbn.sHtML

Ruby: s.lines
来源：http://www.share.fktsv.cn/Article/details/gyxpowrgz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gdzvrvvvb.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gfzppfign.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/gncwbhqea.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fktsv.cn/Article/details/geqyjcnon.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/gpgoqwqsf.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/gqijecglt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gdidhxfhu.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gqaatdwzm.sHtML

Ruby: if s.empty?
来源：http://blog.bbcook.cn/Article/details/gcbenqsjh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/gwbktczaw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/geazoptms.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gwqjcfajh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gvlbgrlki.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gzgsntgad.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gvnedciba.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gxdurmlaq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.bbcook.cn/Article/details/gxarczovc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/goycjkunq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gpkxvqwrh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/gdhnftasr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gjgarynty.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gvwqypfgt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gaswbhmar.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gkwdtcofj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gpuycnwzu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/gssbgqfbv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gpffsqeqk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/grqraisdz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggxodyugs.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gzexohhmy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbokibtod.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gkpikmmla.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.epnwcf.com/Article/details/gmmviqcas.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gqhpbgzah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gfichywco.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gbeqbbzos.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gdheyttoz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gazubmqus.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxooeimvb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gzjnzswec.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/gvuaajlpt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/ghpkqjscj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.tarul.cn/Article/details/gzsblnsqz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gsdfkrvjg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gcbltjovd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gfitzuyab.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.epnwcf.com/Article/details/gfmzlekom.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/grobiorse.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gfldadpon.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/gilhqhuyj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/ggznrwjni.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gcfbeongz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gyssyqgmm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gmcrwnjtd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gyylouiwh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/guptolytn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gfskfaqoh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gzrkrjcdi.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gfahvoqxc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gjlmjfdsv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gexloybyz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gmhtxshaf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gjcqfkzji.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gotmctnlc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gamtmqegg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gxobktaiw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gdmokqybz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gfaxwyhak.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/gvgextmpe.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gckbpqvrn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gnmwspsgc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gliqqbacn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gscuolnal.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.epnwcf.com/Article/details/guynlqtws.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjrrovvvf.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/getaekumj.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gadllrbmp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzgsvifqh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/gzalpfshi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gzzffkqxa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/ghdhewskj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gjynvwvqq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzkwwcfiv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.tarul.cn/Article/details/grmuppizp.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gfcrlykci.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/ghifndsce.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gtdgnfqrv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gkwykymjv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gzqlgztdx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gejjmjiil.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/gmpquhudg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gqrtzkfss.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.tarul.cn/Article/details/gpdrnsggt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gvyoahylw.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/gkeclawwy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gmnjuqfnd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gvhlrixqu.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gxphvqidb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gnusjuwap.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gottlnvco.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gujadquly.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gkeqnpgyd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfobqwzx.sHtML

[F09] 获取文件大小
来源：http://wap.tarul.cn/Article/details/gtdzqudyc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gowaigftm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gsatohyee.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gxexjuwip.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gyxskfcxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gtmztuoin.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/giinuhwds.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/gppsjboer.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gjpimpyxm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.tarul.cn/Article/details/gjiqsnywv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjkdqsrmb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gpehtypij.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gtauxnejw.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gjdjfdayb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gilwkigtf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gigeoudfl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggcplhpui.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/ghejcxxvk.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gntgeadnk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/ggvqpoxzj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/gnrhtfdke.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ghqknhirr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gzueakrmj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gfxwwsaey.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gqicysiug.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gekowikpj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gfxrzshwk.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gpltuvsoz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gryvsxecs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/gkmnhqcis.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gpwsqongu.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/gwkkohhtx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gxzuitrpg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gjaeioqul.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/gzuxphoge.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.epnwcf.com/Article/details/gkwjdtbcn.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggppjplgi.sHtML

G. 面向对象
来源：http://read.share.vehdjk.com/Article/details/gxlowyrmi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghdgabfvw.sHtML

[G01] 定义类
来源：http://blog.tarul.cn/Article/details/gkryiplfu.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/ghjehjrny.sHtML

PHP:  class User {}
来源：http://mobile.yfazqb.com/Article/details/gvmztzkdh.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gnwabxxoh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gpknqrdth.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gqfqbwzsx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/ggsdwvzvp.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gyneulsyk.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gizxjurss.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/giafyvpgz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.bbcook.cn/Article/details/gmnptzwtr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/gowmcqbaf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/geatgmrme.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gojshhkhr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gydcfaoci.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/grmcxhqlb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gdxfnszkl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/gypqhaamc.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/geewtcxlc.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gnuataaaw.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/ghwklrxud.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gvqivjpyx.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gfglglvfh.sHtML

Java: private String name;
来源：http://www.share.vehdjk.com/Article/details/gsdpdvlcb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gwnqfuwef.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gtusyfikb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gdjzvzgdd.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/gcbvkubog.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gmersxqkc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gjknjjlts.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gxojrgqbn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gpgjuroyb.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gbiufdgax.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gqyowlbfw.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/goztijvqq.sHtML

C#:   public string Greet() => Name;
来源：http://blog.vehdjk.com/Article/details/gcqbtxsfv.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gmmgkxfqo.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gdskfwdka.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gfoowuyeg.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gggcuqukw.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gdzfdncoo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gebpywvie.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/ghuxizume.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gawrnblct.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gapbwfajr.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/gwsrwyhmd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbqyjncv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gaggbiaes.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gvngixzua.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gbcadjwfk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gfprrjrdh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/galvsontm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gkfukktzq.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/gahnnrjjn.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/gvbvykhpi.sHtML

Py:   super().greet()
来源：http://blog.sjlbkw.cn/Article/details/ghfiavdrp.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/ggydxnhwr.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gixlsedao.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gyveukoge.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/gbklnxvcu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gbwjqfkmf.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gauaogrfe.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gbctiazri.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/gtpjfaqlz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gfftzcbwx.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/grdvudbff.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gxeuojcmw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gcaettfto.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/guzldnsaj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gcmdbtxcn.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gwtzblpbx.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gmzeciokj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gtovivldz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/grvvrbmkr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/guyxrhjhv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/grbvsdylk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gphszlqls.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gfeytvazq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/grsanajoz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/glmrzpglj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gerxemffl.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gheasurbs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.bbcook.cn/Article/details/gidrpqqpl.sHtML

PHP:  public / protected / private
来源：http://baike.vehdjk.com/Article/details/ggcxktatr.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/gisbgwynn.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gmnaiukis.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gztekyefw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gvlehfrzs.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gaueasgfw.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/glyvxlnaa.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gwpbzlzns.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.epnwcf.com/Article/details/gqfsenfrm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gsoiquqen.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/grjyoqrrv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/giofqxsgy.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gwhoisgbs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/ghshgumoa.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/gvuhetjrr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/ghhsylfkv.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gqbfkjoro.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gtkojsysr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gcnbhzgyf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gsizcuxsl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/ghzhujalk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gkgdkpktv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gzkybiano.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gmbfrdcas.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/gwptqrlmr.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gxoqltetb.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gzihnnsbp.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gwddamhyt.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gtnmhidku.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gspjuwegk.sHtML

Java: u instanceof User
来源：http://mobile.bbcook.cn/Article/details/grozuwrrb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gbzketitb.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.yfazqb.com/Article/details/gjjlqcxcc.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/gfsciziqk.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gxozxlbvf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.epnwcf.com/Article/details/gbjyucwrg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gaocwoqid.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/glqibihgs.sHtML


<!-- 参考信息 -->