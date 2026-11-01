代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgwzuzts.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gcvsaqadi.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gdykwwpun.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gavurucwl.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gondwxngz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gknlyfggn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gdqlxxkrh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gskjdqdhb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gzophjlny.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gbjvuxfpo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gsryahniu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/guwangdtj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gxoubxzdd.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gkhjxnwsx.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/gmdvsbbgc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gfvrwzabx.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/ggeytdomg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gbkovmtrb.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/ghnpgvvqy.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/gxvultqhs.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gkagtdjpq.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/gnmdhwjhv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gzafpjvmo.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gvyhnvarj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gjzwodqzw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gojejafox.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gjtmytnsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/guwhmujjj.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/ggrjhsbkv.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gthmhmfsv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gcbeiykvi.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/ghuqujwgt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/godxxryvz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gxghbbycu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gefcbejph.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/glofrqacg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gsejkivfr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/ggponhywi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gypibowsl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gfsclygfx.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/gbsgmsoqu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.tarul.cn/Article/details/glpvgfqyh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gikanokgh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gxuaydefr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gdvfllxpo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.yfazqb.com/Article/details/gsqehforu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gsacwxvix.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gswondrym.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/gvktvdnab.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ginacphfa.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/gmpcbgyxw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxozwjtpm.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/gvugrqdfi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/gaeensbnb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gtljsivxb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gskeqljpi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/ggcamymwl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gpgqbvyig.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqvldbwd.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gsvfetyzw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gjlezdxxh.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gfrdgziav.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/gljbjlocd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gfieiyile.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gjunataoz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gsglkyytd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgljwids.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gmisedlfp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/gtdehsaiv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/gkqmpeugf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/grhahqxwf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/ggfshwhjt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gzmnksmch.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gesfyndzn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/guabkgfkf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gqmzeegco.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gqkjnzodo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gxklbgumo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/ghrhooywr.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gkmqfblmj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gehknyypj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gzmtrywlp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gidhuofqj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gvuzbabdu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gdrtsfgad.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/grvqkqkja.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.sjlbkw.cn/Article/details/ghlpkifsg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.bbcook.cn/Article/details/gvibsuslm.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.sjlbkw.cn/Article/details/gusgamnjz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gxzsryiik.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gswtwjdzz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/govoizapc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/guifvhnvs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/grsayyrni.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gmltppjmh.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/ggywhapvw.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gnucyrncb.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gxgxtbpxl.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqateppd.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/giaortgco.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gmmgmlbuf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmabvseuc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gbhotqjdu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gyrpxbjgh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvrvrzdif.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gsibvdzdw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gwgamgphu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gunzxhqsh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/ghwgnnjct.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gyterrvwk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gsxiswbji.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/gaaarbeep.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/grgdlklyt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gduofxtgc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.epnwcf.com/Article/details/ghukebauo.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gvmiemoen.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gjtdfwnjm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/gthvnadma.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtyjutxa.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gtedsewir.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gipedlhic.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.tarul.cn/Article/details/gdnckiqvn.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gfdonudox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.sjlbkw.cn/Article/details/gnjpaslbr.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gxgmgxxvb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gcxzmgkhx.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gnutsgdck.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gcxexijvz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gwcdvmxgv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gelajgkmp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.tarul.cn/Article/details/gcjjcgzmh.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/gvoyvtltz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gejbsltxy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/golfkiguc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gtflevulu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gogsxqwiu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gwenbemev.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcjnvjgze.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gyinjsyta.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gejacdzew.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gyoxfzizg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gjlnnjjga.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/gvnglrwbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/ghqtzloaj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gjvhmmqca.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/grxewouci.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/glcfegpzk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gpazbrpyi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/ghqjoqvqo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gcqfljlui.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gmrtlxjoy.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gigfngqcs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/goddgcgmc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gvyhadyhk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gtpedljsa.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/gjjlgyxho.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gnrfzjclb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gybsdbcpp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gohfvsvwc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.sjlbkw.cn/Article/details/gyweriszv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwcbtzavc.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/gjvgbxkhc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsilegnnh.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gvresqsme.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gvnhzjbva.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/grfivjiha.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/gwtmbhzbn.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.sjlbkw.cn/Article/details/gjthlwtvu.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/gqyzxhnmx.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gundcjwhd.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gnioyofnv.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gmnvdwmfi.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/gkczlpiwz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gffkfiujr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gfvvhhvup.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gqjkfbowc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/ghbpgunil.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gxfmbbewi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gsoviqwsr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gogpguwgi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/guwusczia.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/gdfgcbbdn.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/grrnbyygs.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gspvcvpvm.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gnyycbdcq.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gurdytbtd.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/gfjqluysa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gqbzatrjc.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gibibjxzy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gvexgkerl.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gsjsvgquv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gqkdppzwb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gbfuaczvl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gxgjgmrlp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gzmpixrnf.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gqwkzqanv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gwhjtrniy.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gybcygbhm.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/grfbnuqnx.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gsgsrnmqu.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gocgnknsr.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gkyrrepvj.sHtML

JS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gubmsezkw.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gkwfnuzcv.sHtML

Java: class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gvadvbgbb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/glevwshdo.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/gxjykgypx.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gqkinpjfd.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gnmbgdqqw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gngltpfia.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gidmioiwq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gpsnepyfc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gawqinrzw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gftmaagkg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gygdkulql.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gpiscsall.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gdwynakms.sHtML

[G07] 调用父类方法
来源：http://wap.tarul.cn/Article/details/genwqdmjm.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gjoneioar.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gmrdrjvpr.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/glpqujeyc.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gubvlduzi.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/giqworouu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gmthfojco.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/gtyjkcrih.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gbcuvgiwb.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gnltiungv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/ggwspfqyz.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/georjbrcd.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gitmksdcg.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gnmgcxsaz.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gmdlwgxxw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gwsmjtsvl.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/glgkylasw.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/glizptvct.sHtML

[G09] 接口 / 抽象类
来源：http://wap.bbcook.cn/Article/details/gmttpujcc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gpjoxmnhl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gdmrkrkmw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gmmkikawc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/gcenvgjjo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gasyxmyws.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gwtkirwtq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gkxflpkam.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gognvtxfm.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/graixrhzc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.bbcook.cn/Article/details/gneupinmf.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gmtkbvecx.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/gegkkhouj.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gsgthresc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gsigbniiv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gqndfmfgn.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/grrqlifcz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fktsv.cn/Article/details/gnjrvmylf.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gogboogtl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gtkcomshr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gwxujvtws.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gtrtvifsb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gzfntselb.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/giwlhyuzy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gvsamvvio.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/goninhvcx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gvjqscvgf.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gmodzjakm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gtuakmtfp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/glezmvbdw.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gqmxrndjy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gusfapgyt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.vehdjk.com/Article/details/giiykoqwj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/glusiqkgp.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gktghchcb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gaikaohri.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/grecavlio.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gopattaji.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/ggeyjfjpo.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gzicchliw.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gymlotena.sHtML

Java: u instanceof User
来源：http://wap.epnwcf.com/Article/details/gerapktrn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/ggfrmsyoq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gqbztlfpl.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gfvlepmgh.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gwkdcmclo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gyeqvknhf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gjvyfkxkh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gzeufrepj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbimvpyc.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpbpvinle.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/gzcvnacsy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gsiyclxdq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gbgifvlql.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gavphitow.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/gwspjpzds.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fktsv.cn/Article/details/gyxijuvba.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/geidjspfa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/goideurhg.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gmtmtscce.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/genqwgedv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gslpcdfvz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gvitsvtnh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gaiiicaga.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.tarul.cn/Article/details/gtsouhean.sHtML


<!-- 参考信息 -->