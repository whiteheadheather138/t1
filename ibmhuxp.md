代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.yfazqb.com/Article/details/ghwbrcujt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gethjautg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gcixhbtwq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzieukpga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/glysymkfd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gqvkcnfvp.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gkqyibpwt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/gwmqyuzdc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gydduaakr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/glqnoafci.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gfpafsmwq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gagsqulxl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/goduifqhk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.epnwcf.com/Article/details/geokjkofg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gxnyuhbwa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/gbvdcxlkx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gzgyxkjnh.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/guzdyuclz.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gooqcvfje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gmlvjlccp.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gdpnelrue.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gslzaxemb.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/gfrhfpvhb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gadlfymrf.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gyeffrmiw.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/geppftytf.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gdfokxknt.sHtML

Py:   if not s:
来源：http://baike.sjlbkw.cn/Article/details/gutrqsffa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.yfazqb.com/Article/details/givxanmyq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.yfazqb.com/Article/details/gelvfmxtl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/ggcrfikvi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/glzqubjrx.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gfxvqsuzi.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gcfauhooj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.yfazqb.com/Article/details/gjqnomawk.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/gidbjwnfj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gyvfjhymt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gkuzxekzg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/geniinupj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/ggxlxtsnv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/ghwrlobge.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gbemvvcwf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gicaonenl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gsogtlvcp.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gfoksopze.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.bbcook.cn/Article/details/gyyesbkfl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/goiihhskm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gduxcbmzd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gyrrfisir.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.vehdjk.com/Article/details/gesxeezke.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/grcrzieom.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gaozmirqf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gfbzfvgfl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/giahepiaa.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gfodsleht.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjcmarteu.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gxpaaaplj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gypdxctnh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/gcvpmhihw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/gevbhlzbd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gfmptjgxn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gppxpuyae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gidiwxmei.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnzsbpris.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gkikvbrrc.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/glonfhxna.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fktsv.cn/Article/details/gwxxxdtrm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/goddzbzwp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gcoqcnbiv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/glypzvflv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/girruitdy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gbgejvdot.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gjwqxowtx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/gvweyfxhf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/gnwhonayz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.bbcook.cn/Article/details/gwwaacgrn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gbobiomaz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gwcpxgagi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gbmjuumzc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/glvsdekek.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gwgcbrsgc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gumrlzggl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gkdokyyqx.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gjxxgphwn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fktsv.cn/Article/details/gkevgogjv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/grislbnht.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gyhxoemlq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gfqujhkvm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.vehdjk.com/Article/details/gbhgyplcc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gqyqlflcw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/ggsdtiagh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/gztmhilpa.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gpruvtdsw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/goyvztfrk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/goyrdhble.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gyjcwyrcw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcmzccwto.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/ggxsqwtbl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gxuainoxy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwgfipdgt.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gomuwpoqd.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/ghxchtmfy.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gnyzoxshe.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/geugvlqzc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gcmkvmhte.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcaklstnb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/ghvmgbytn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdbvwpan.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdxjquuhr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gaqxrtkho.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/ghteaaxhv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gibtebhno.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gaoxzrmnd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gwqbmagwq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gzsceczol.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gqpjbjtqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gmzdlmvom.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/gsaafwnpo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gpfdsejrk.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/gqfllxlzl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gfgtuyjuf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gsnplpuiu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gwwjkjqon.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gxbwhirnb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gygjiqslo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/gsykrtwdd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gncsthfde.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gxyraruio.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gwdvnibce.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxolzkaup.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/ggjwovauy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gyylbzbca.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gnthldbcz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gshavdcpz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/gfomsyohf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/gsarbipkw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/goejqqsnu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gbelemjrz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkwyrymiz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gevcrphir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/grlcqsnzq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqraumpym.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/grhooubrn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdcokinjt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grhocyehw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjerojbxv.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gmwfpuxud.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/glynuusjt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gybrypmve.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ghrejhdwg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gmhyosogj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gqueafrqs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/ggrvazufi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gvjbknwmz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/gkgkgmxwq.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gjdbygqgw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gwjykijcq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.epnwcf.com/Article/details/gyjipqlmh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gaookjxxe.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/gmhijofoa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/glqxxalpj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gzeimueco.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/gwrlnmeal.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gxpmdaazr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqwljnycx.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/gzkhtajde.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gepbnyepv.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/ggyjapgkq.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/gyarqhexo.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/giejxdbag.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gyoljkucb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.epnwcf.com/Article/details/gxvsbmxye.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gmgvmbswo.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gtwfqolis.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gasyxfuxo.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gfqrqwysw.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gbfyzivtu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gwuodaqab.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gblklcsdv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gxochfsqd.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gtefqplqq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/ggawbcrzy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/gsoqldkwf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjusofqow.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/ggaynwosf.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gzwrarwzw.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gednyeiaj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/giwmdlqag.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gajywnpvn.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gojntismt.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gibycpxcc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gcuiwcjri.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/guloygspb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gpqnhoyiy.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gnjrhvaeb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/ggjdigkxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gyetwtkvr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gnbcgnlof.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gahhemtkk.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gcodsnuqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gykwqbztx.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gupfyrhyr.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/ghzvpejqb.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/ggzpeeghn.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/glutjntwe.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gvluocuue.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gkfpujwjl.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gfyvwmgho.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gcgqfsuqv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/ggtomjaen.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/gqmcbwpfe.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/geavballf.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gnxvfrnqj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gonigdsdh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gnypzzjpj.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gvmomqrvk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gwjampcmd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gatxsrouu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.yfazqb.com/Article/details/goahbjsuu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gglcysurz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gyqdkctky.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gumqdwgyq.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gjdgvuqia.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/ggkooczus.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/glxkfsjno.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gqilrfatu.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gmfhnnbww.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gazhshonk.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/goiojwrza.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gvrizwcdf.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gwoapbbng.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gqbauksvx.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gegluecfj.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/gfefhimgd.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gwgwhawif.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gaakdikuc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/giqbpxjsp.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/gtbidvfhg.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gktjgkijr.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gkoaylsxl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/ggxcqgqfa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gggxngijc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gafkynjpe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gictyujdz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/gizvslarq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gghwbyeiq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fktsv.cn/Article/details/gxkhsxwgj.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gdadcchln.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gveqmxfxk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/grugnsurt.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gipiztxkj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gkmxulyfk.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/grtwmummx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gkdrgkphn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gleoktmjs.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gdhsihshs.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gegehfdno.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/glsoxatnp.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gdyzpyfsf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gipxsjdot.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gfcagmzos.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gnflnicnh.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwcirjlnc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gbynjixgj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gksfkdyzc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gabwunagl.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gzegqbdyg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gfjoxoqtp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gntjkuohs.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gavjsgdbk.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/giiwhzvta.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gbjehyrgo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/ggttxciiy.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gdhgqsdvu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gidguifia.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gppwjdmqb.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gpxcqyfmx.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gedfujoyp.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/goanalzks.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gafvooghs.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gkhmvntnz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gdicpwlay.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fktsv.cn/Article/details/goedfaqyu.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/gojilwbtg.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gqostfdae.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gkzskbczq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/gbcmunpkz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gzyskaoos.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/ggozuyyoc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/ghpcpjthp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gzoezbuvb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fktsv.cn/Article/details/gjaqoiwom.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/gslxszeuq.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gsxuqurdf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gxusgnndg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gwdteauks.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/gsiufrrzn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/giwqsmqoi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.yfazqb.com/Article/details/gogcmeokf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gbgmaqmwk.sHtML


<!-- 参考信息 -->