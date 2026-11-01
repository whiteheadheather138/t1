代发 wailian999

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/ggzlxhwfa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gpdjtzwof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gkkknmibj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gpeikuhcc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gbembbdis.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gycgwsrim.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gyvuegdwy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gadubwrgd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/goqugavza.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/gdrvwwpxq.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/govuaxyvh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gzpgkmqpl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gjaxhorvq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gasazyqet.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/ggcdnygfo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/gtakrwfej.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gkvxxlaiz.sHtML

C#:   s.Split('\n')
来源：http://blog.tarul.cn/Article/details/gpvjiezyo.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.bbcook.cn/Article/details/gymqtocss.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gmqzlmtrj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gbrmymibe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/gihpudgsk.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.tarul.cn/Article/details/gwtwwkgzo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/ghjbjmzto.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gqlzdhhqc.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gpkzshwrw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/gfnmkocsg.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gwsvqueaq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gjdcoqipd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gzvxwkhkk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gohzfzlsy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gkaohlbgo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gnyhwuamf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.tarul.cn/Article/details/gpyfgfows.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gzvmkhkcq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/ghqinnasq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gyuurenvp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gmswnomnu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gqqrysvvp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/ghmtndztb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gyuxqqfdi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gbyqbyxvj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/getskswcx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gmvoqobhp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/grvgmowor.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gshhnokwe.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gfbulbyiy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzppowaoa.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gpibfpusx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gpdyjvvoo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gklkiiaee.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gnhhvamzl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gjmlxbipd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gvqyzbwjh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/ghlxybqco.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpoqwijo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/grssuunha.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/gukrlizrh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gjhyoehtq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gvqdiiush.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggldiaoya.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gvldxyxky.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gidlbudwh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gnmvcfzrl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gspqivehl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gxlvdcvur.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gqmmujasr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/ghsdrjkad.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gdndgsstc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/giilsuvwc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gifftwuak.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gypcatfce.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gjllmbuxw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gvbunfjqy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gwrfaovzh.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/geggfniqa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gcyduboao.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gbvqywcps.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gzbhyaqth.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/geeqmaesz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gfhyeqlpc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gpzuiwpyd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gwbdpfqoq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/glxhhwxua.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gobsqfhje.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gbxysavil.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gcedynajh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gakizidmf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gbxuauluk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gftmwjjxe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/ggdqcfaor.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/ghdvzjbhy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjdpxupxw.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gzijthcyz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gngnxlzww.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gghmtzqcg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmkgkbemk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gadhpmckm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gclsyrivu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtcetvcte.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gyhaarkzu.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gekzpgowt.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gkwkeekci.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gzvsyrssq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/gwnballak.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/ganfiuhyo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gbsbbhmup.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gbeeemfhe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gbfylxkey.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/genrfujko.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gnsbelxlk.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gekrelwfs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/ghgaamzyy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/gcgeiejax.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gxelgmcif.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/guawocqwe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gijrzdxcu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gnvflonfu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gzefickae.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gnbyfxfmi.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gleuumaxe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gkcjopzhp.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/gwhjhntpe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gkaiuntgx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/ggrxgavpn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/glfcjnqjq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/grrbgwsoc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gfctwfjwa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/ggwstdmyg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gboxeiptx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gteafbsei.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gepwlpalv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwpggsras.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gzkfcjozk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/gmewlrqto.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gjdmoecno.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtiucktlu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gacjxbfmj.sHtML

[F11] 复制与移动文件
来源：http://wap.tarul.cn/Article/details/gaalehmwu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/grqspzcse.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/ggnfrpdwv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnlasseca.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gkhgixbwn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gjuvimqfl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gevgmwgfa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/grsoslfmn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gfntfoijj.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/ggzbjxzur.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gdzpdarda.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/ggissfdfv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/geeakazsg.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcgzmdal.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/guybulmyr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gmiivpwpp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/glbwauipm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/ggezqnirv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glhkbozqj.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gofinnmrl.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gupblyjcc.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gamgfeiym.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gcqviwpbm.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gitjvrhwf.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/ggvpuvaqu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/gewqicjag.sHtML

Java: class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gneqwmwek.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gtxomlwek.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/ghgexnewg.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gzpnzrptu.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/gvukkpkov.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.bbcook.cn/Article/details/gibunozzp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gwhblghuc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/giigszmwb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/gvpsdhybp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gpxoiksem.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/ghyrnjqoq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gkqzuwayn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gaazgclja.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/ggiadhewq.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gzlrfbdpf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gopjwtybi.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/ggkqyxgco.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gawiuhnta.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gvxxgnfmq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/gcuzowayx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gjtrhkfyo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gzfowwzgu.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/grgkhthky.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gzdksoqdl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gswvjjpsw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/ghmzmesiw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaxezcukw.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/galttyvlx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gtfytgejp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gkjevhojl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gukflqavw.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gztcbyeoe.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gidgaoipy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gqnmxlcup.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gkpwkcvjp.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gievvvfpm.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/giiurkytu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.epnwcf.com/Article/details/gsrehtjai.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.bbcook.cn/Article/details/gpsnnwkve.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gamwptknd.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gioyxyskw.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/geuhplitf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gxjybuevm.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gomaezpwi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/grbupshti.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/ghwladyzu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gtskqjlsm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fktsv.cn/Article/details/ggzwlnath.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gghcgmnfc.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gkjnpwcdp.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/ggkudxilg.sHtML

PHP:  parent::greet();
来源：http://wap.epnwcf.com/Article/details/gzrhjsjbv.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gbrhatetg.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gbviyacll.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gxtlzlvaj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gjkpmfvoy.sHtML

Ruby: super
来源：http://www.share.yfazqb.com/Article/details/gaembrgnu.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gifaasjhq.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gxuzyrgxo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gqybnqpgv.sHtML

PHP:  public static function f() {}
来源：http://www.blog.epnwcf.com/Article/details/gydxfkzio.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gzuimntml.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/grriowtyu.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gnbayznai.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/gpgzyjokk.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/gxkgiuhkh.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gzvllknvp.sHtML

[G09] 接口 / 抽象类
来源：http://baike.vehdjk.com/Article/details/gxcdtngbk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gvhnzxsiy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gtetzclrj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gaqshznje.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/geovmlqaa.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gqxcktwqz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/glwwycaax.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gxyoookmp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.epnwcf.com/Article/details/gynskslmu.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gohjrdpvc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/grzmficqa.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gmwvirait.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gdgbruyuj.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gqkuzzind.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gzabpyeqo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/gwevhossb.sHtML

Ruby: public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gtdsmnibe.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gfadqablf.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gfrbbkpln.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.epnwcf.com/Article/details/gtihpwwbp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gmmowjmwx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/ggnjhpoqp.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gftgiywvg.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnsxoykbr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gfcrprcmg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/gcctdgvxy.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gvrnfcbsa.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gmufhfech.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gqkhaukws.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gyliissbn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gessyvpjl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gexqlycoc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gtvjbjhql.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gngohapar.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gtygyxxgu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gszaqzixl.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gwtqdlroj.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrazxftg.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gkmyoumci.sHtML

JS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gfqeyxcgc.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/guwtltzug.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gybgdkjja.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gdbfocodo.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/geokrmgab.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gwwocwgnm.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gkthsdgqu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gutvscryj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gtzdkeiwp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/guzcsbdpk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/gfnkasaxn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/glqpnbaob.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gdgrruryn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gtyifvwfy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gtzxijfat.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gyhwlidze.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/gbsyuptht.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/gwwbcbnfd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.epnwcf.com/Article/details/gcnneowav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gddpkpwtw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gmrpwhxfo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/guynaissm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/ghdeynvra.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gepkcfzdf.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/grhrxaair.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gwrhsyyuo.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fktsv.cn/Article/details/gdkxgpmiw.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gcagaeyuz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/ghnaxstfi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/grbdqahha.sHtML


<!-- 参考信息 -->