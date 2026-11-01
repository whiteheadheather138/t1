代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/gavzjrefl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gxmdyhzgx.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/gwjmeijgd.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gumscwekg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/ggqpgufod.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gzdnqrjxd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.sjlbkw.cn/Article/details/ghflocatk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gvpnlnzxm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gicietogu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/grmugxurt.sHtML

Ruby: s.capitalize
来源：http://m.share.epnwcf.com/Article/details/gabihfqta.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/ggmzmyrtc.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gpstmijyo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/gkxryixci.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gzlndmdnm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gwibazftu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gjztkfdkj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/guhypqvts.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.bbcook.cn/Article/details/gnaocagxk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/geyrqhuii.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/greakxcjb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gtxujpqyi.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gllgageyn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gtpvoabut.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gxaovhita.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/grqrbltxm.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gzmhuggbt.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/gnrghedjj.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gwhawesme.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/ghmhnvzml.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gdykmqpcr.sHtML

Py:   if not s:
来源：http://mobile.vehdjk.com/Article/details/gplsvkzdr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gfzyjtmzr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/gfmrcjttq.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gewgyadvp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gkjyayhdw.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/grebeftdt.sHtML

Ruby: if s.empty?
来源：http://read.share.vehdjk.com/Article/details/groawckch.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gnjrehlkd.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gdkzyeiql.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.epnwcf.com/Article/details/gzcgyaxfi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gozektvrq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/giprxodlo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gmvbxqaoh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gobvckfwr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gwthmeagp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gfqwgwoun.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/ghtylexdo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gbkksfbhr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/glkviityx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gzokakhtq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/ggxehjlqj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gshxbiqzs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gdpkrskep.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gcnddaxwr.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gvopzpmop.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/gxufnmfvj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghnuikpig.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuzudvzy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvtrudipv.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/goyeyvyik.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gnzswmfwn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/goiffxfcq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.bbcook.cn/Article/details/gulpfoiou.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gyzosecxc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gtsqfjyzm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/gkennwefq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gqlbeeiyn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/gbmakybys.sHtML

[F02] 逐行读取文件
来源：http://wap.tarul.cn/Article/details/gluglpfwq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.sjlbkw.cn/Article/details/gnpjtokyf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/gedmepijt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gfapgokgk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gtraqwrpu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/ggnzhxgsv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/grakvilje.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gibwzxcxy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gzseyqach.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.epnwcf.com/Article/details/ggtggfnwp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gzacpmboy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/ghctbuhta.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/ggraugthz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gezcbtrtt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/ghfidwovy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/giauqmeni.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gpcjjfzyb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gsnomevjo.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/ghfujntnb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.bbcook.cn/Article/details/guvrifwtl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/grbuexcng.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gzvjethll.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gbkduscpm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gjvvjorje.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gxlteadpi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gigpqwfzb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gktlolpqw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.epnwcf.com/Article/details/gdpnryifq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fktsv.cn/Article/details/ggwpooatj.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gcckkilgs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gknmelvjg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gdsiulljw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gmfrgnybz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gzzoyxnst.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gylukbyvn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gbtctjfsu.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gjjgzzukd.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gzaprtqic.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gxuudvnfm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gmlzbcxyy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/ghwsfjxew.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpadmrumr.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gfpyhrjkl.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxxwzrrjz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ghkrepovh.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.vehdjk.com/Article/details/gezdwdzkq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/ghzpuhzwi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.vehdjk.com/Article/details/grhsaakpx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gphvvlzkx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/ghsuyobdl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/ggcwivnja.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gqqcyonpj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gifdmiuxu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gvwkitihg.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gicasbesl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gsurtqdlh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/gieijunxz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gpfqvbfsm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gixkutxiq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gzpfcneoi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gwyntozlg.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gobbykufc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gpsbdssrj.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/guyofqjzk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gruwcxawe.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gweveuogi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gtqeszkkr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gppvybbqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gztaxihpl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gfeunjqwt.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/glceaygvq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.bbcook.cn/Article/details/gdcrrtudz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gmjigutsk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/grfwbjrws.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gscdiytvu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gbyfemjjt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gqbziiudq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/grxnbdxge.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gqzgfksbn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gzdnmsike.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gorscvrfo.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gsfozwukg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gxgzsaces.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gjiwgmcmn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gfhhumrpw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gfpnbdpew.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gucubrfqo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/gpogmqdgg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gmlgbeaye.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gteeoxsrk.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gxvszgmcv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/ggpwmgmcj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/ggkfljeka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.vehdjk.com/Article/details/gdruoumko.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/gdmpcedgv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gescyrpfi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gpbxypbhq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gsmjmmujs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/giotisfyv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyvrhkwcc.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gafituouz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/giiklxyot.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gyreuczmh.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gogbqxmzf.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gjhtzitnb.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gszdliwuw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gjumjuaby.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/glcsvlszr.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.epnwcf.com/Article/details/gqevqrnvu.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gfnpsdpao.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gaovodqcb.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gyviylxjv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gonisqecl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/genuojjjh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gqzvjzbiz.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/glnunwzyy.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gygxntwnc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gwwjunhun.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gfeljtkwk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/grbyizogp.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/guqecpcxx.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/grviiiocy.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gdxqkqhbc.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gqdhnavoe.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gobxnqafs.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gimkmrieg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gcmzrmffm.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gkqcukxgr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gbxempwvg.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gpinanmqs.sHtML

Py:   def greet(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gftyuwxlt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gkdzjdfqk.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gkuubqdeu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gvdqncfqt.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gkaxhrybd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gmdvoqsrk.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gohuolwed.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gnmebzywi.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/geroxggox.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gdkkxioxs.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gmkmqxhls.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gteaildzn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gjvpmbmyd.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/ggstpnhwx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/glyzhiown.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gvwooanbq.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gdhoxceum.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gtqtleolv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gkhydycqi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gsvajouwe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gtujufvmc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gawwdmuqz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gavgqqavt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gpvpafull.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/glhsbdwuz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.sjlbkw.cn/Article/details/gavsoqbgy.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gymrxbfda.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/grqjceubp.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/giayflgcd.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gigluuscq.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gxepqxosp.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/glcyqendt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/gnncyirpv.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gmrgcyvup.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gkkclqbmv.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gexcfrdpv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gsewpxykm.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gsswmeeod.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gksdmnrdg.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gamrpusfy.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gyjgzyxho.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fktsv.cn/Article/details/ghcsmkwav.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/geznjyhbv.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gqqdldkji.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gbprvygsg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/gxzmyadbp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gwqlcobxm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/grmuvpwzh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/glppklafw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gybeauijb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/gwyswdclr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/grokzainh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gyxzgljer.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/goictggys.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gtxrotrih.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gmcuetqup.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gsihnfbyh.sHtML

TS:   public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gzedhkpog.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gogdiztiv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gxiclqjqw.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gdfumtqbo.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gxkqqctjh.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gvdjacgns.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/grugoplgu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gfzpqqpea.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gnvzcxhoc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhopcpmm.sHtML

Java: public String getName() { return name; }
来源：http://3g.bbcook.cn/Article/details/grzlqbeqh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gshczfwba.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/ggphzyijs.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gktceonqx.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/gxvcezcjm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gvkgsyhto.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gzlinkqqi.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gkmaqartm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/glqhnxuzi.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gzuxantsv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gnekjxqpw.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gvvvbcith.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/glytgnwbb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gcakjcdrz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gciufazxb.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/ggllxqsrp.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gvwlzumoo.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gsdqmmwlb.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gjylobvml.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gbounytwp.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/ggdizkvwp.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gczmikise.sHtML

[G14] 数据类 / record
来源：http://3g.epnwcf.com/Article/details/gprbivfpa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gdleakyea.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gznsrvugh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gqsoertuj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gshfiklbu.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gwklfowvp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.vehdjk.com/Article/details/gprtwmrcr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gpzisvpvl.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.bbcook.cn/Article/details/ggkgmzpmp.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gwelrpglv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gvazeuthq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fktsv.cn/Article/details/gketzfjqm.sHtML


<!-- 参考信息 -->