代发 wailian999

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gudyxrhrx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/geaipkeus.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gzzcxndxp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/guudfmfpx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gkquxptmj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/gstcwaudc.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gzwtvzqmy.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/ghtdnmhmd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gypidiqfk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gdgjutufh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gjsrnzxnq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/glubsdydi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gmxifvmql.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gqytbpsam.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gnisyhwhm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/gvofqqjqu.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gypuvbqnj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gdlpfqbll.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gtgwnfdbn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gjlfitwaz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gcjrlbdbw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gditfyvrz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.tarul.cn/Article/details/gliwkdtla.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gbewopwls.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.sjlbkw.cn/Article/details/ggoaxeqkh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gfqnhxwpg.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gdfhvzfps.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/gkpvuxynh.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gtagvlmsy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gqqjbysjc.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gyqtanydh.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/ghdzvfprp.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gtsextojz.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gngpddzdp.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/gumixadyg.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/ghcgkybwo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/goscnansl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.bbcook.cn/Article/details/gqvcgkouk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.epnwcf.com/Article/details/grdtvvcok.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gyocpcxlk.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/grignbnib.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/gejadwrun.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gorffjqha.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/ghnpzwstu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gpknqscla.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gsbcxlioa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gitxbzhpb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gmhxjhhdw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gevdzlpbl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.vehdjk.com/Article/details/gexrzhadg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gvtcqzvag.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gwmvmscyf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/gruuluhld.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gqpvgxgon.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gyjthxhda.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gdlhbhbro.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gpxeufeon.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gmxosgdyu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/ggxjeglra.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gaifyabwh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gtzjidald.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjctepskn.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gqheqkgcr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkvgipmhh.sHtML

[F01] 读取整个文件
来源：http://blog.bbcook.cn/Article/details/gfmbicyxo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gmazcirhe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/gpwjxztlv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gvunpnzlx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/grghsxuwx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gjkobavlm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gujpofhqw.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/giatavlzu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gacbndomp.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gdvjcetmz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/gpuecrwgu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gknvowrbp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/glljexcyd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gwhxqfvli.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/glcrvispr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gghazupja.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gtxcihszw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gbltkymgj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gxxewcrnj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gequfdvvs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gzkhpoduq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/greeblbbu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/grcpxaegv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/glihfymft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gvtddweho.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gobqvngck.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gddaqtnjm.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/giltriayn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gpiazmwsx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gnpafbkbf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gbsmlsjbh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gbjahkmor.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gtjybpdkk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gxzgjworp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.bbcook.cn/Article/details/gwytqlmdz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gywyueuar.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gaggvglqv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.epnwcf.com/Article/details/gdqffethj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gextsfzrj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gnnoztrfj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gtgksgceh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gcqjmnfbb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.bbcook.cn/Article/details/gihfmesse.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gytfpfgnb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/gwareeddk.sHtML

[F06] 删除文件
来源：http://wap.yfazqb.com/Article/details/ggdmzsstg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkjumwrlo.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/gkczequdo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggxmhfbpe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grzfzjbjy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gafayfjzj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gavqbvnba.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/grnucenah.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/ghksipqwb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gghnxsran.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gqlncrmkb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/gbhqnbffh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gpllfqpjj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gadlnyioy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gjiutrrfb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gmycqlkwl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gaqqyieya.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/gzkkrnswc.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/glljgdnvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gxeeofmzn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/gxthvhyjq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/glcqmfrbi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gkwnobsvo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gvuwzehed.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/getevdaav.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/gybemhjse.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/gyyoqckim.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gnbkblrhf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/goqzylxme.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/giaskwtez.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/grmjemgau.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gflzgpajj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gwvvlkdvi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gbuhrhtzo.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gwwsyifti.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gmrqllgxi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpwzssci.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grwmjkofm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjgrmkdlf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwlryxsme.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gchyyfczi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gjjutofbm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gdkvlutbo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghfigioem.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gjiwenztv.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/glntzccmt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gcvpsnqfn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/guzjrqcli.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkdytzhbk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gycjlcbqt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gathqabkv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gtxnvgiew.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gzqemltsk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gihcgowpj.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gwilecmao.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gmmonaskj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gsrgmvqbr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/glaoeldpk.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/grjcdrcur.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gezvkapuc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gbbkwhbpy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gcksexovf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gbdsjpahf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmmewlcbl.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/grzkunyqh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbgetuktz.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/gnagdncud.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/gnpelnrgd.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/guaowkpjf.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gzowgyxnp.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gtcpneagw.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gyzcpurbn.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fktsv.cn/Article/details/gacuosjhc.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeqwicwl.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/gjlmpdrlc.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gsirqyxez.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gdoqnlsyx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gbkazppql.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gjcnecdrm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gqflqiqdl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gddciwwgi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/gnbsubrxm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/gwfecngri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/ggygdhmfg.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gseukposg.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/genqwlwdr.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/gacebftij.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/grffddbde.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gyirmtwuc.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gjrrpcxyx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/gtfsrukuc.sHtML

Ruby: @name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gkrmsfhba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/gdbujrpla.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gebjmeutt.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gwpxrzwdw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gpqveelyw.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/grylmkisd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzwmgsznk.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/gufvmwmdg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gosuwzggt.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gerfowiwg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gnalawmsd.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gijsoffhx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gxuypmqtg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gmppvsjho.sHtML

JS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gqzcoxjls.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/guepqlrhx.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gobbssefo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gdwzxbqxe.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gyvqpjiwo.sHtML

C#:   class Admin : User {}
来源：http://m.share.tarul.cn/Article/details/gsrxswxvq.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/gngbzweuf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/gkbcxqatm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gewwpttdb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gsosduaei.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gcpvimfai.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gmazpdfck.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/gpgrjjton.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gxiwmrnpx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/glballygo.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gguutccsk.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gfdvzjmlx.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gakbhyqrq.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gqclgmbos.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gjximzkjy.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/glmdlpiyl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gufgcvavm.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gyjsldncm.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gqbkctxsh.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gyrvlrxng.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gwhvqwtww.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/giqvpktzb.sHtML

JS:   static f() {}
来源：http://wap.epnwcf.com/Article/details/gwaukldah.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/guopcdsio.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gxoctejnn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gahnrcgmv.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gynvunwtn.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gawqqnpzw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gwpntvmgk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/grgwkptug.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gqfazadai.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.bbcook.cn/Article/details/getmngmof.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gvdprietb.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gjgtwuxgf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gkjiliamn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gqzgesuwa.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gbejebvsp.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gepkyunoa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gkpfelqrl.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gpeccrcey.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gqmmiplnm.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gtiriyuij.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/glufzsuxy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.tarul.cn/Article/details/gxnikjuff.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gjdvygqds.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/grmeokrkg.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gjfixdnsy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gkvkjkagb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gtjlpsmyc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/ggpnbboly.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gorsccfdo.sHtML

Java: public String getName() { return name; }
来源：http://mobile.bbcook.cn/Article/details/ggocrcwuj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gqceiuuli.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/gbvsqpceh.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gjklgihub.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gvgzmpkoc.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gpgwqdejm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gntlcodaq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/ggcvkiune.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gqwfwudos.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gjxhvylht.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gpensexpz.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gbbefjuad.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/golonyksi.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/gmskkxyuv.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gwxngihhq.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gqdqsgusd.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gtnwodrkv.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/grgkamrbu.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gtrkojamj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/gjzccydic.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gigzgnfvp.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gutoehqqc.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gxqlaiiwy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/gsrwepmsy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fktsv.cn/Article/details/gumgxenpx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gpdpearge.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gerntshah.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gqlgcrpyf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/gcgyesbyt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/gvtubxiir.sHtML


<!-- 参考信息 -->