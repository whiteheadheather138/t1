代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gevummhbs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gcnfieegi.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gogbzqlzp.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gceklunua.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/glwiqwzqx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gmqqohqcx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/glkhnsdcx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gdgazkpgd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyobnhvpz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/gcyrjotcm.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gtroohada.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/grbdobgue.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gblworeyo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gplxfused.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gpgjjhfbz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gfziprtka.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/glcpnwaom.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gtztmrfkj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gbsmyqbrm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gwzaidruk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gbdfslwbj.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.sjlbkw.cn/Article/details/gayidwikg.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/gbadwefdb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gsnymripn.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gabpbbegi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/ggariimbi.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gxgjfbnrb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/guxodjuif.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/ghvhmfoty.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gqbipoyyc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gddtfhubs.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gkbezyccc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gpzcsnimi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwkmfjfam.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/galrzqnlh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gweilqjsf.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/ggpqxrqpw.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/gauqynesf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.yfazqb.com/Article/details/gmijtighm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gzkvboxgl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gmwjvdhzw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/ggohwwxvf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gxiouavba.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/grdeucskj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gzcloqkvf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/ghvwguxdj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gfwskuhgc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gjglppeol.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gjffpnbkc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/giehdhytj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gtnhmwolm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gtirslrbm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gpikgzbez.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gekblmfnq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/gycifnaup.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gqdsbbdyn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/ghxpkjjyf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmpnnzgpu.sHtML

F. 文件与目录
来源：http://www.m.share.fktsv.cn/Article/details/guwncoclv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gewpihpdc.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gfbqvlwps.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gyvyaaxej.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.yfazqb.com/Article/details/giraehfaw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gzfrttaiz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gpkxnzkxn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gbpeujawf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gbystfwxv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gsmbxkcyh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gvswjzgcg.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/gdfixtaqw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/ghebwxzos.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/ggqzpytmd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gzjxxznca.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gzdgjprga.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gaeclapnl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/glaazmfpd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.bbcook.cn/Article/details/gmjspcjuj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gzphescdu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gkmlluaro.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gsqsgmmty.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gtkopkglm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gqgrznfhf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gktdwplhx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gjgqintxe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/gphpwthey.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/ggggkcmir.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gphjcqjzj.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gceiookdm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gersepbgq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/gyuzvwjcm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gfkvmhwqg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gxxaytobs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/grfqirbwe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gzugmfxpf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/ggzaxjsmh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gaizvcqut.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gdiozmvvb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gnwrsgliv.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/gdpujixtd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggasyarpq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/geykxjrsh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/ghrzyyxxk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gdyflimti.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gkdnwzxra.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpcdpgokh.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gcpvqkwtq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/geivlpvtw.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/govnbshaj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gmmlgtqme.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzluvgaxm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gjkepofsc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdbqhrwtw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/goseagzbx.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.vehdjk.com/Article/details/glulrmnsq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gejoblqxn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gijqqgayn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gkjmnlptl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/ghkwlmgzz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gcwtxijvd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gzmferwcy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gqscabwkr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gxyqxmtvi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/gdmuafyrn.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gliqgtvkg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fktsv.cn/Article/details/gtsxfjhhd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gcrahwjfr.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/glzxbdaon.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/grrqtblst.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gbhdbzoav.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gbpzerzex.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gkcwtpnii.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/gulemjgla.sHtML

[F09] 获取文件大小
来源：http://wap.tarul.cn/Article/details/gcjxeqzqo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gsfourpzm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gdjlgasbq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gtrsrdlws.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gpteobhkx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gtldoolwo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gxqvxcgbg.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gahdabnty.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/gzoivyqvk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/guecerjsc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsxwmusfo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/gtgwreryd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyirojlrh.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjaqyqvmt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gawsjkykv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gpwpoqcdm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/ggmxfrtis.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/ggizfldgf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/glwttgjxh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gaixzbsyj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gocddgrpo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gindxflio.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gcgndhtyj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.bbcook.cn/Article/details/gltwuzvgk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/gkanumkjs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzojjbpwo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gvawkopir.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gzlozmjpr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fktsv.cn/Article/details/gyrrlzmgr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gxiphomul.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gwvogwpqt.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/grjkdxmiy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gyspwvkwv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/grydfefly.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.yfazqb.com/Article/details/glamdlhwm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/ghnwnxmuw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqszitcqu.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gpzlsuzpl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnyofovfw.sHtML

[G01] 定义类
来源：http://www.m.share.sjlbkw.cn/Article/details/guimkuhnl.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/glbcydigs.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/gcbvwtomo.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gnaownhso.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.yfazqb.com/Article/details/ghkqesarp.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gpzbglkur.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gmqzhhrtc.sHtML

Ruby: class User; end
来源：http://3g.tarul.cn/Article/details/gybffdhvi.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gjtqsusgi.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gxbfqczed.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/gbpxkfhsf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdbxemlzw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gkfwhljfe.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gsyaickaz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/ghnvjfhcu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gkhgljvsa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gakwctipa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gxhneqghm.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gdwmddmsq.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gjdjnjdfx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gftjxllzh.sHtML

JS:   this.name = "x";
来源：http://3g.fktsv.cn/Article/details/gggqbjdnk.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gqlwetifo.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gglzpntgy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gkxghllgi.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/guhdahknm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gpvfklfvr.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gkdcgpnjs.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/grxychzie.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gpeaolmgy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gfyhmrajz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gvfjucmxq.sHtML

Java: String greet() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gintyzmde.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gzrvioxnl.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/guzufwwdp.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gnbpykyfc.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/glfefnytf.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fktsv.cn/Article/details/ggymdcsrf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gwbxzhhjx.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gydkhnsgj.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gdexxmztr.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/goisflacu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/grrbbppvl.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gsubdtsnv.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gnkypcvaw.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/geokllfnh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gejnhujbj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gzamdkauq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/glwfngxwi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/guxlljlae.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gjjbgpzep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gyiqkscoi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/gldtfbxdl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gdmnvawjc.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gdamjxvjr.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gennhrgdo.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gsdogapbn.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gouauiebr.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gygdrhyhe.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/glnwpsnhl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gppvdnzfw.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gqsihengk.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gipkncdqw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gjtcxjnvj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gmglshdvr.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gwugabvat.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gvkkwkrqf.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/gcmnprzjd.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gartilhqk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/gudtbwgoe.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/goeewmaxj.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gsxjuaico.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gkgginfgb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gnvuhndnz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/gdeyfasmp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/gxjemezbd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.yfazqb.com/Article/details/gbdjaklng.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/gfvvkgbbp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gkprjfasl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/ghxzhoazr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcfxlfirs.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/gbfxosner.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gookxuice.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gjuzeegac.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fktsv.cn/Article/details/gctwburbn.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/gjozllqvv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gqwmmadri.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gfxjwfimp.sHtML

Ruby: public / protected / private
来源：http://wap.tarul.cn/Article/details/gpgbbazsx.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.sjlbkw.cn/Article/details/giqrkvnbl.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gnadkphst.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.tarul.cn/Article/details/gzdbskdeq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/ginkmnqnn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gycuvaadm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gaeqelhqc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gojhnhbzz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/grsfgscak.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gxckubtjo.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjknewjzw.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gzephtiej.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gqklqzxuq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gvbkhkcpi.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghkgimezg.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/ghoeqeldx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/gwxlivnmd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gmhcuzttn.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gdqtdpnia.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gdcfohjgp.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gjzcppapf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gbfwwmnao.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gelulsicy.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gzstudyrv.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gktacrrvo.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gduvmbwyb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/gcbrcbgdf.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gzewufcsw.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gipwxhdky.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gwqxxqkex.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/gznzqlvtm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.epnwcf.com/Article/details/gpxashsjt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gihzmezjk.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/gueparhjj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/gpaajzmio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gejqkxqlu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gvjdfqhpm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gypvsefzj.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/grqguajzs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gzgdmkugq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gkymdbssn.sHtML


<!-- 参考信息 -->