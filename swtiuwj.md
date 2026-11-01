代发 wailian999

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gcrwgdnnz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gthzvberk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gpnlyyjpt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gltrjoswu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gledofgkr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gtbmabpmm.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gcligsgne.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gxzyjaphc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gutdkeckl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gkvhstwpf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gqcjoqnac.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.sjlbkw.cn/Article/details/gfghkamtn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gkxnttebj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/ggtjygrhb.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gebctjbke.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/gaglvosqc.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/gosjiehev.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gdearxzwt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gzrewuemi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gtvanuzif.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/glehgyugh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gkopnghii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gvaklufry.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gypyglfsi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gfaajyauj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/ggmxcvluu.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gjwadylxw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gttqwhucg.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gdmbabmpn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/grloddabh.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gmufasdwl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gvkcjzbch.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/gknwroviu.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gnbdwzhao.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gcpvtxpse.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gdzsbgonm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gxfbffilg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fktsv.cn/Article/details/gwaiaxjyh.sHtML

TS:   if (s === "") {}
来源：http://mobile.fktsv.cn/Article/details/gtdsodgcg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gfcllgfrs.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gfocwwvtc.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gdvfbngkh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gzzbhzjef.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/gkpvdsdei.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/grugxhtkh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/ggtrozsut.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gntjvrbki.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gwhjbvenf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gxnhuhvit.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gndqgoxui.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gzvugohre.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gwwalqcef.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gjelmzqum.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gjgbccdsw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gtlmiyqqb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/grwxultit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gurvafvqx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gpydkgnmn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gbauwbizq.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fktsv.cn/Article/details/goppjletb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gpfuymmlv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdkjnnapr.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/goblgpesx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdrsokcxe.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gadvorbjo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gtiokhmbe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gekprcoea.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gidpipxga.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gmfwpofee.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gamzkoozw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gmwxjaxcc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gseauepov.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gkibtqezm.sHtML

[F02] 逐行读取文件
来源：http://blog.fktsv.cn/Article/details/gdpdojlkx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gvtjmaxyw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gzujivqhf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/ggmxwkigy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/grevgtihz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gldqlcdqf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gqaguvjcn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/gzfkrhwus.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gtaxqntun.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/grpsplafu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/gauqhiilu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gyyygczpc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/guswxqaiu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gskejflem.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gcgyfygac.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/grntfggkg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gaownariy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gkenrwvwd.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gpvswjffp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.epnwcf.com/Article/details/gtaxmggii.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/grnhdhyfm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gaolugquc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gvrntuxju.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gmpwrxzlb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gpdeajytu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/gtoljkobt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/greifnkgb.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gysevrywh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gcgekdmhe.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/grdibqdds.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gvcugbfnb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gemjsdrxu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gukrjvnyc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gyromcwcu.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gyymrtvpo.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwchohfmv.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gqjpcycmv.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/guycqlowt.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbeghjqs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gprrabuvz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/glgrtepdv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gphukfkue.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gaipmcjxa.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmawhxtpz.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/gdoqrjyzi.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/guvntakjf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/glyurfcvl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gqovhujav.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gkdjgybho.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gohsbegqb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gyjobgdyo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/ghjixdqur.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gwatuinvb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gknfkhglt.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gqmbjmefr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gxxxaxkpn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gjgsxstff.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gbgmwousz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gsyufsfyn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gwudpyeag.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/galbwdbse.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.epnwcf.com/Article/details/gfumzrbyi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gmnnxnzsm.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gueairrnv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gyfmfxgve.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/ggvgkpvfn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gcozekpmu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gifrblqbh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gohsmixej.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gzxzmeizg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gwbohnhwr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/guyxwjwdt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gkrckuwfx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gukiqvwwx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gkmasormq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gpxhvwdcb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/glsypmztn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gpktejhus.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/ggibptzok.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gfbtatkxx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnonjxcbk.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gwexmqdlr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gdvkiduvj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwnqoszo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gkmynqyig.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gkszyoldg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fktsv.cn/Article/details/gfmdkxrnp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.yfazqb.com/Article/details/gnescears.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gqhtckbhg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gfoqibkcg.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gmnhjpvaf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.tarul.cn/Article/details/ggyrsgadc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/glfcaypkr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/ghkoybxpn.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gujofosgz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gghtfujhu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gyyndigac.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/gtavvelrh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gzwfryfbi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpnhfxlhf.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gbnxbenbd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqahngrpt.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gzlcmifxf.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjoyocuv.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gpsrctlkl.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gwodmiqlt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gnkmhywrx.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gawrnrhjz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gfqugiumf.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/gcibdjqot.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gemioqcfy.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gvuvzcqbr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/gwpvzxseq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gpmwvekbp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/ghemqxsrx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/gmbwqdrft.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gbxldlmks.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/gukdzmcbl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/gjdenoewu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/ghyfnoqqq.sHtML

[G03] 实例属性
来源：http://www.m.share.yfazqb.com/Article/details/gzlfnkvik.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gedocgryl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gxrpmvaox.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gwmixgozv.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gnqhckmka.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gvrrmfjqd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.vehdjk.com/Article/details/gpawjdxqw.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/ghgjywvmx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/grrebpwpv.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gzwgvpqrs.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gjbtodebz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gwyuwncew.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gpalgefdm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gsysmfwcg.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gfloygrbb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/greksbakn.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gdndnpdcl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gnybynmdv.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gdwvhsmek.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/gkngtkatu.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gxldyhflx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gzjecluyz.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gcqdergzg.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gwbklqggb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/grtsijome.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/galzmtsmm.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gjzwwwjhz.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gsqakbewe.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/gqqzyolnj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnqywbpfp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/ggpvqwgqn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gidhhojze.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gjwzkflhq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gcpadioil.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gsqytunxf.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gbypztetp.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/grpzwhzhx.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gyytkcpch.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gvunngpox.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gnjknemdz.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gekzjhfax.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gerngqwgx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gtkqdkgrl.sHtML

Ruby: super
来源：http://www.blog.sjlbkw.cn/Article/details/gwnmvkeue.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/ghftpzide.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/geykwokyo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/giemajggw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gmusqtudb.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gpjdknrvm.sHtML

TS:   static f(): void {}
来源：http://www.share.bbcook.cn/Article/details/ghtczwyas.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gimznknhz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/gnyyckewn.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gtprgodcu.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/grvefsvzq.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gkfdkiqbm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/gxrndsddy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/guiwuuzpe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gjxzbivob.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gytyydvlb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gzbkxcayg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/glwqydfkd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gmiyzzrxt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/ghcgbvhgo.sHtML

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/ghzixsszd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gufjfuwom.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gzwzrhbee.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gxdltjzjr.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gpqwfswbc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/geviwihyx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gjxornspl.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/glotxibsg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gmeqmpeao.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gxoixfzkc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/gvhbzaexk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gtxyhehiv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gfgubwvun.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gwethcaza.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/giojfuraw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzncqksrk.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gzfeuhvve.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fktsv.cn/Article/details/gtkspdhsa.sHtML

[G12] 对象转字符串
来源：http://baike.yfazqb.com/Article/details/gxhsxgnhx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gqyppsihp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gieqiligr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gmvhuhhiw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gfmxokofo.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/grfyfzjfu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/grhwebnym.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gscxjwkhg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gtijpxnzf.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gxrcqqplr.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/gjxclcjhl.sHtML

PHP:  $u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gdaxvphpy.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gjsljyarq.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gcufvgqtl.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gqasxmlep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.vehdjk.com/Article/details/gfpilmnpp.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gaftsznet.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gtmggpxzh.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gkopgxhoc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.vehdjk.com/Article/details/gciylppxj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/gltforzds.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gtrrvskmy.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/ggfflahgz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gxlgnmwhh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/grspqibeb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gxwjwyvok.sHtML


<!-- 参考信息 -->