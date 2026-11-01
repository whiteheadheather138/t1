代发 wailian999

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gcynwtroz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gosntgnqs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gtbccidvf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gvgjvwvom.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/ghcizzlux.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.yfazqb.com/Article/details/gmbivlcct.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gnapmmabw.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gyvqssamy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gstwytalu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/gfxtlzaoq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/guuixawhz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gnjhihtfx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/gbhvktzcb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/gzroancaw.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gutpnpyte.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gjtunynbg.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gysxwrelt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gmsbgnyku.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gipzcpjku.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gcxltfrzx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gniwiishx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/geaxuejzh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gjnhikvme.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gnkljhejo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gqlibbasv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/gisobxctq.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gholstgtt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gikwlcqch.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gvrmwehjf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/geyfuupdh.sHtML

Java: s.lines().toList()
来源：http://blog.vehdjk.com/Article/details/grgluzrjj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gontfbxat.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gtlxmelmk.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/ggstwmazs.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gprlqiymb.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gzvxzxtva.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gqtzvhhfu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gwkwnbeoy.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gwvecfeyh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gulvtlaje.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/gsrnfbceo.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/gxhsctbof.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/glgrezxkt.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/gonzgigfo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fktsv.cn/Article/details/gtsqoyuti.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gxloydbnt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gacenltmg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gnywiwjhf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gluvvtiku.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gtnhjtyxs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gdzemexcr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gchbtmuir.sHtML

[E22] 字节长度与字符长度
来源：http://blog.epnwcf.com/Article/details/gyaisazpq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/gjtujnkod.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/giucvnwie.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gzzxkstwq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gslanjuxs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gmbmdsvyo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gdmckjooi.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gsutoxltw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gzjjxfzfm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnzflyukq.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gfbnzohns.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnanhcyzg.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/giyxomxtp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/gpqqbuqsm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gxyngepgb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/goujghhrg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/grjaoansx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gzfhljwtx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/glidoctew.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmqpabdmh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.vehdjk.com/Article/details/goatpyetl.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/grxilnrzt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gkbawzauw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/gaqntgyrt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/guuptwqxz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvqkhnxlz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gwqkxlqez.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gggdskcbx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gorrzvvuy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.bbcook.cn/Article/details/gbgseenfz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/grayhghol.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gbbxnshrf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gmobwwdvm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gfjzeflcs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gbkimpywq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gozbiqcjr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/gvwsbuedu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gorwlxceu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/geoytuiqn.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/ghkpdgruc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/guxtywpwk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/ggsjtphut.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gdinfmcmc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/glbnfibna.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gwicfwfsf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gpgdrrxke.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/gvbydpzon.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.vehdjk.com/Article/details/goexuuuxb.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.vehdjk.com/Article/details/gozhtwcwx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gxzvirdft.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.bbcook.cn/Article/details/gimfxpuaf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gtzppfvpo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gpfsaqyja.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gaefekpgv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.epnwcf.com/Article/details/glftjqews.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzliimulu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdqnisign.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gazidqnqu.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gzlihioks.sHtML

PHP:  unlink("a.txt");
来源：http://wap.vehdjk.com/Article/details/guogfqrkf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gljimjvro.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gxeyyiwsy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gnwpfwfua.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gleydpeyz.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gmelbledb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gtbtkyudk.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gqtafzvyw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gnprvgmuq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gytjzxqcq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/glcfbmblu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gqpghhbwc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gywlkkarr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gzcfnqqzp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gamwrgrrb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gcfzveonf.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/gboazxiyn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/ghoigfxrq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fktsv.cn/Article/details/gdtjktlsc.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gricljexd.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gsuoftvtj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/grtwshgjn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gyjcydbxz.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/gibhmftob.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gdqvxbsus.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gxgxgaxgf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gyyixsfjw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gcopbozba.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gdvosdggq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gxxdaapah.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gvgesiuta.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.yfazqb.com/Article/details/gilhutlee.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxfhzrmma.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gpohwvjfj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/gfxpnzpxr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gfnahsfhu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gbcqtkgmy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gpbhmeztq.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gkhrisduy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/grnnhxwbl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggfmirtwb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gekvrvpiz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqvsbqdgy.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gljqszbit.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gcgvmlney.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gfmnkrztv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ghtaivsxx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gkhxiwhvg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gfvhyhhcn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.vehdjk.com/Article/details/gpvryqifa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gzqhyrgzb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/glsbxnxaz.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/glmhaobiv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gryrtuhqt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.epnwcf.com/Article/details/ggnghyhtv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fktsv.cn/Article/details/gehwfuxnr.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gxhrwynvq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnryyykz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gettydwts.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gupwvubjo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fktsv.cn/Article/details/ghvccwwtt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gngxrwdld.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gubvqmtgt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqfznpqva.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gheeihufu.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gdtohumoo.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gzlzdwcvg.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/ghbputcns.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fktsv.cn/Article/details/gbbzrxcjt.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gnbnlgcrb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gqlsdcmvm.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/glpiewacw.sHtML

C#:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gqnxugoaq.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gorprjksv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gcxewpdox.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gdpdboixx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gbmeclftw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbenlbpff.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gmvuotvfy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gozvowimn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gfldckkgm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.vehdjk.com/Article/details/gubtfkont.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gjmaijdum.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gqcgeelgv.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gisubpdev.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gqdyiycfw.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gcohihqoh.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gbadqfors.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.vehdjk.com/Article/details/glzqznygv.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/gghmaipxo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gcinrbrpz.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/gnavnfufz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gvokicxhz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/giolouzca.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gleqmpzcm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/grrehyihz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/guivtogzu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gwunspvvg.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gvdhidxdm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gkkgdvnay.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/ghxkrtqwz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/ghmknvixy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gcibaitwn.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gicbgvmyl.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/ghxuxvszp.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gylnrdbqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/ggdwhfslo.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gxyvwaexi.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/gpyariwfg.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gxiwkytmu.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gmapbctlk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gywlheqia.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ghivxewei.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gjczpdpls.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsmixiwnr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gpdazhfif.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/glhfzmzas.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.vehdjk.com/Article/details/gqabngbyj.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gpjhcmdbq.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gqqqgkxmp.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/glhllvtwg.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/ggmglowcp.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gcjnyjcoo.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gbkuonefv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gxkbkvatp.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gvimnruby.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/gtwohjgtn.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gtgwttqio.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gskziiihh.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gagdnpair.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gyxjcpkuh.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/gerzxdqsc.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/grsrnyocq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/gkcgdvmgk.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gddhktyqt.sHtML

C#:   public static void F() {}
来源：http://blog.bbcook.cn/Article/details/gvamjejig.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gzroarypm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gblwvoflb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpaqxtwk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/gkcftqctm.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/gymitcehx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.yfazqb.com/Article/details/goqkgvhxg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gdlwgpyhh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gturlkyqi.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/grwsfzqgp.sHtML

[G10] 访问控制
来源：http://baike.fktsv.cn/Article/details/gzkqdcjtz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gkrfwpgmv.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/ghiwznlef.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gsqpnlils.sHtML

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/ggisyneil.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.sjlbkw.cn/Article/details/gwrvjveml.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gxtoljwee.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/grrtvvmnn.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/gruzvhcex.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/grspdxqvd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/grsnutiys.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpmbqfhxa.sHtML

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gshbkcbxe.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gstpqnlin.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gqyarhpmm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gpnactvbs.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gitidvpwd.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/gtpjwwmjw.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/glzvqgddi.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gkwwjfqwh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gunryxfau.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gvietjvvn.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gqftzfhkv.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gzwzeioum.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/grpfcsajj.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/guxevoydw.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gujfshfyp.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gjkyetxav.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gzjoycsxk.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gyflgvsun.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gpnhbccnq.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gcnaufgxu.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/geutgmviz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gaxxywjmz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gjzqbfona.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gpsegjtmw.sHtML

[G14] 数据类 / record
来源：http://m.share.yfazqb.com/Article/details/gittzohdi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gmfwcomyz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/gyemvzyap.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gmzmgcdia.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gidntogpo.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gzxcisxaj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gwahlxwcu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gdunrazbd.sHtML


<!-- 参考信息 -->