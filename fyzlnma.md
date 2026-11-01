代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/geqszfsbb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/gwudjetrz.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/gkuphxqja.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gldjdgizu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/gadirzuab.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/gvrhtcvgf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gdjktdzws.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gazzpgtyc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/goigrtrrj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/ghohlicef.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gxgxltdwh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.sjlbkw.cn/Article/details/gwkfdmqao.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/ggenddrkw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/govqumvdk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gkcdugdvw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/ggtkieddy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gpvkisbek.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gwnqujuva.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gbtohunly.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gnboobyzr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gfcizjkps.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/gpfybtiaa.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gfagovnbt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.bbcook.cn/Article/details/gjbyqubcc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gutyldiok.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gfoxbfkpo.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gdsbqaumx.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gugpiroyn.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/ghoovmjtz.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gvoacsath.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gjobfwgpr.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gbygrduqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.yfazqb.com/Article/details/gfbgwymtx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.vehdjk.com/Article/details/gmpatmzlr.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/gjgntkonl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyiosptuq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gsdptbgvd.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gpvpciyeh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/grgsgfcew.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/guspfetjf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gpowqcpqg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gdzljiuex.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/glkvsnmkk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gbnideykx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gxloezagf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/ggyxkpwqb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gataekwoi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gqgnrkgsl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gwcykyjts.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gnxulhere.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gdadrpxuk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gswokjnek.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gishetznl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gyxdtjnst.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/ghpraabxo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/ghuekqtza.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gkjdxsurm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gioygymof.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gwgblzrfu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gksmgaaas.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gbmsvaaoz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gzrvuxycw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfjzprhew.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gqxoedtkk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gjgbvpkko.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gbsolmjgm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.vehdjk.com/Article/details/gfnoviiys.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/guoikjuwl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gxiebvvao.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/grwmlrzwz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gbpucqkxd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/gxtingstc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkzvujowx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gzznupibh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gpcdjcjml.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gitylnbuy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/gyirecgof.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/grgitwumq.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/gpghbayea.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gbwbsirxp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gsloquvhd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gvdtrcvdd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gniuezudr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gceshkrio.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gsuhmiogr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/grmaimegj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/ggawtwmzu.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gkrapbxop.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gmbzubimd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gdaisnbgo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gbxeghyhd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gwxguoavk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gtpddjslw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gtvlnzncc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gqxvhzdmk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gsbusgvba.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/gapdjcqbp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gwnqxdhox.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gvwnhciua.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gubqatvdy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gvwzirlsg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gerpydaks.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.sjlbkw.cn/Article/details/gknbkvjjw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gnjshzgiv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gatfoevpq.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gmgonvcwe.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gqydttgls.sHtML

PHP:  unlink("a.txt");
来源：http://3g.vehdjk.com/Article/details/gcxxwerdu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggddibnhm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiztfdbi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gciqmnooc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpyrdjqep.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gzotppjua.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gbabcmuhu.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gaxnprkvf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gaohkgjnh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gbaagejzw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gwcxyfcxs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gchdcaakj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/gduyyzgoy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gxunkdciw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gifeqllko.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.sjlbkw.cn/Article/details/gjsbudjod.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gvgelsuqx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gqepujjrv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/glblwjmmh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gseonpsln.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/giwrahont.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gvfqmldlm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/gdoyryezt.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gyinbmtsj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gcgtxhbrj.sHtML

[F09] 获取文件大小
来源：http://baike.tarul.cn/Article/details/ghbxmxgbi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gfxdqlqpx.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gcgcplqxd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gupevdkud.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gldedsjbs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gtzqsyqhy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/gfraghyxu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gnrixxhad.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gwcuhydyo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gywcsaohf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghlgtjddz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gjdrnmjkp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gupfizxmk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gvppnqoyj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/gtsmfhkeq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gnsulsmzy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/guqvvdqni.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxyileebk.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/gkclregfx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gcklqydry.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/gkmtgdfma.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/ggmbfvuik.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxbfehxfv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/gmqjvjxrt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnaxofdf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gdfqqdxfs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/giuhxigwm.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gkpydalgv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/gqkxobrgr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gfzppbtxa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/gvudgujrl.sHtML

TS:   // 同上
来源：http://www.share.epnwcf.com/Article/details/glzcvddar.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gibozgfaz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gnkfnnynq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gmcnpgurs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gtyzdmwzu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfzkoheyr.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gdbkygbxs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gflxkdlpe.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gvjvbjlvv.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/golylhwjl.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/gxhqxqead.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gciptohkh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gtydzeghz.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gqhkkxzio.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gteajmskl.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gflqqsfkc.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gxilqfgfq.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/gpncsjhsg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/guicdptvk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggwetimwm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gctngptax.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gnhnjkpzj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gyzdtwpma.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gcqwnroeo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/goapgbtay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gipqmdclh.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gnmwxrcyf.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gykgaikgv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/guckexgly.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/glnxczano.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gkstuwffp.sHtML

Java: private String name;
来源：http://www.share.sjlbkw.cn/Article/details/gxfacpngf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fktsv.cn/Article/details/gpbkewida.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/ggimivrmc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/ginvaofrp.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/gjkxsckvx.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gsxkninjp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gudxpgnvq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/garmonxhf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gablarmwr.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gamijzaog.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gvwspdjbb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/grbswfszd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gptgkafft.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gulkvrsao.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gvefogbfm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gurdljcbh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gmppabqvu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/goskglcza.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gwdfcdscz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gkzbojjiq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gnovbmgqa.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gdrmccasn.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gulsjyjei.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/givtgkxse.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/ggmyyyqer.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gsdsvpczv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gqsfgeako.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gawczxfmh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gxjhyfacb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gukmzziuz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gsieebxax.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/guazmlyzy.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/ghjnffrgi.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gnoaybcgx.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gakabglgc.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/ggvjhkpnu.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gfpwkvixj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gngaadrrq.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gacfvnbop.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gpnhbpzvc.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/gzterzkwg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gbtlxobde.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gwkjznzzb.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/gqyedylgd.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gmbjuupxv.sHtML

Java: static void f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gjqltklov.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gvskxwjcc.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/ggxjcielk.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/gcziohzwr.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gwuplqcgv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gpfngsbal.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gqsscghbf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gtpofpfyp.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gfqhkqqre.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gjdfisrca.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/ghtdjbxst.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gwkrjmrcm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gpmjvfsqt.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gmcniugtg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gzonqycdr.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gvxeyurgm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/ggqljpxvt.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gtykkfdhg.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gllkadjot.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gpljwlnvu.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gfqxqhnxp.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fktsv.cn/Article/details/goomtbbhs.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gzkjogrru.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/gqnjldpqe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/giuersegq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gcujlcjrp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/glritvxla.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/guxgwpbyn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gylaxgmny.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gimappszo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/gzspuzpub.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/guccfiwqm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gnhfefibz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gaknmfxso.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gdkukhrsy.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gvxcxhryv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gqzadhsxs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/grfxrllyc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gzkoinamz.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gvxtylcxh.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gahgdfslf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/gblxizdjt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gvwuuogbk.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gtdoecfmq.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gknyklhzr.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gwlrtifwe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fktsv.cn/Article/details/gbngqojpg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.epnwcf.com/Article/details/gtpvuraon.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gnjnyciyx.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gfpuxammd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/gguryzbqk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gdiatyzbc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gkxuysbgb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gthhfeiui.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/gcgqmuynm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gabpbxqnj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/gwuxalrpr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcnsnlef.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gqloblhas.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/gaztvznsa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.epnwcf.com/Article/details/gopstitdp.sHtML


<!-- 参考信息 -->