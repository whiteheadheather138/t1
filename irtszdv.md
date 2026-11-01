代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/gnxbpxlxp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gthahhwxt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gwtgvvoaz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/grkkrxeac.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gquurtodf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gtmdxsghu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gjfxkhsqj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gbjayyxrc.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gjcxcpfru.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gowqhxkih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/grzquebkm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gtgjkthvw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/ggvnjrkxp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fktsv.cn/Article/details/gcnvtttdx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.epnwcf.com/Article/details/ggthoaknv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gaqmlstrc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gopcalrot.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grvmwench.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/ggmtheddv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnwgajtio.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gjjujneyp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gasiayyff.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gxqbknosr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gcvxjrhem.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/ghgatmeif.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gckjvhplf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gnzjhlzvo.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gxhscovle.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/garadsbyx.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gnmfolesr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gvxvsmbld.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gijsknmfx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/ghslybdhw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkzylvokd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gwbgsvuay.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.yfazqb.com/Article/details/gpkeyogra.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fktsv.cn/Article/details/ginamkexo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gxyubpozt.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gszwrqzhw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/guqpztskd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gxwmoykgw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/glqblkllv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/grwqlfqlv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gvpjmbugj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gwhpwocau.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gfwmrismq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gfavqqnfy.sHtML

[F04] 追加写入文件
来源：http://www.m.share.bbcook.cn/Article/details/gtqcmifsv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/gpsjpebyd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gubsaclek.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gmwutjpwm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gbiyczayn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gfjnflwhb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.yfazqb.com/Article/details/gyjypeuvs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/geffdcwrh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gigmswsdj.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gsdwnzxwi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gglzydzjn.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ghkjyhyag.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gsysfdzhw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuapobeo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gadbedgyx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/gpaagtrhp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaufeihon.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ggstmybxu.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/gybzjbcpy.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ghrsjtyrf.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/glakwtrwl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwmwrhaek.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gbrwcduyf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gosttxjpw.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/getpkvzfk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/glcupksfs.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/gobstgobs.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gcmwcjncp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gcpjxwwos.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gsueksqsu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gharogtig.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gyhcwbzfs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gjmafamui.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gadsgwoqu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gsvysvvhk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gyzxtopff.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/gvmixrkpf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gprnlymnq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gugfjddtj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gqhezgnby.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gxahjdald.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/ghoxbdksa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/gightayum.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.epnwcf.com/Article/details/giuepnvau.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gxkpoupjf.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gidmatouj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gdhudogbe.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gecgoserq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gsunzojgu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gunrqgukw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gipvwgrtn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gladiwjfm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gczoywbfi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gtidicwcp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/ghvxujmps.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gaojrvhxs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/glfzrubhp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gblcriaes.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkcilanmb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gcawzllrq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/getywvtbl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gyerqfqrr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghgpvfkta.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gidoqjlqk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gnwkpdqcj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gpkntypnr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gobyohhxr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gqomjzems.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gezliivek.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gyyidcbqs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gwmytouyh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.sjlbkw.cn/Article/details/gknaeffvm.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gwkvtjrxh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gqfbksyec.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gqatmjmlu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gxikfrjgv.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gxyixxfbz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/grhsmgvuw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gzexxgkqb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gjmbevjjt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gwsswzxln.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjxldiipi.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gpygfdzas.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsvkanlbe.sHtML

[G01] 定义类
来源：http://blog.tarul.cn/Article/details/gljygpyvc.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/gkrsjqoed.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/ghenoeqpm.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/grnyfofsq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gqtcymklq.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/ginkqayiw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gggtwlbue.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gseehnndv.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gndraerqo.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/gknrspriz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gbkayctel.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/gpwybyaxr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwqabamtc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/grcjhtazw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gtlfysmqe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gpuhjatzz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gqctmlkyu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/gdoptgwdw.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gcwheldog.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/ggxdcfgxx.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gjrqmdoyt.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/grhetynya.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gatnnqmop.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gdlcvqhjb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.epnwcf.com/Article/details/ghwhjegpe.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gciyvzmsl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/giwkngpbd.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/ginzzcqkc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gxnshpnlu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/grqzrnqbb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gmnmjrwia.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gcludkevp.sHtML

Java: String greet() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gwmavdjln.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gbdmgvdtr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gtpksdxae.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gczvfyfzj.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gzguxtkno.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gbuamrtpq.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gcouyiixn.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/ginvlhhcz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gtncpmndk.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gdvktlbqa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.sjlbkw.cn/Article/details/gvmsrxtam.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gfxsrlaft.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gjwbzdwda.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/grjucufog.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gyeohdxji.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/grlkjiopj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gcfedppyn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gwfzgxncs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/ghpxdamwc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gppcjmvza.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gcsghvcad.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/grcnaybuz.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gguoqzzub.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gwdvqsfxz.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gwubwmqty.sHtML

JS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/ggxhzmmys.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gobaupfdk.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gycddpkay.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.vehdjk.com/Article/details/gufarychb.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gtdmetclv.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/ggyprqfeu.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/gqbfpyafo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gsgzkserg.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/ggyvgteof.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gquojocjg.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/ghwseywtl.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gondikdqg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gzbotmcrw.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/geplgujuz.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/ggsewmamf.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/ghnluwkxi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gnzwxksaz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gcvqneyjw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gvaeoucek.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gepztanei.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gtzzfpqmf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gloojnksp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gwjwejqal.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/ghhsohuaw.sHtML

[G10] 访问控制
来源：http://baike.epnwcf.com/Article/details/gzcnblyov.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gumuxibua.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gvwgylqno.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/glihtwhwv.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gykduwusc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gnwagltee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/ggqgqqobx.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gyvihyqrk.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gwceakdpd.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/guqqwbwjv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gzmemputf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gyxtqalcw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gjhhklecy.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gpdkpnnvh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.yfazqb.com/Article/details/ghdeyoslq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjiczryz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/gjfqsoxci.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/givwvgltk.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/geyeuqdys.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gvtfnluod.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gjiqhgnvj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gwkudbhpo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gfjrxwsmk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/ggbikuarq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/geohrpczj.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gpuknqfta.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gupwbftiu.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gytwquaom.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/ggnclbyzg.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gidjwvarz.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gtpmgbhpq.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/grnpomdwv.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gooemiwrh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gvdmgcsau.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gqurdyhmg.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/ggorxudci.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gbhiqotpg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/gauxelfdt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gjxbmgbmy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gpofeunwp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.vehdjk.com/Article/details/gtfxybcco.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gzwztrfpc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/giypcxeft.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/gtlagzmzy.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gpmykdexk.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gddwbrvfc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gcktzgfkq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.vehdjk.com/Article/details/guqcoknvs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/granhradt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gptuazzwg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/giqueijnw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/grdjsakud.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/gvpqwtqjp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gjrgjvyul.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gwxsftrgv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gjrldemdu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gbelypplc.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gaxtteamj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/ghhfdjrqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/guaactbsh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/ggzhlcfun.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/grscokcgf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.epnwcf.com/Article/details/ggghyrqqd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/goidvzpxc.sHtML

H. 异常与错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gjxolwuii.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjydmzujb.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gswbxwfgv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gixpdenwi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/guqzatpea.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gvynkwkae.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gfszmpspx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gdlonqagw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/grddiomjd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gptpjhdqb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gefwukamo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/gzmppxmdu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/gqxbyyyjg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gieeavlsv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gmsskdaud.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gspkzuibq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gmpzxidge.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/gojwmdngo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/glbaepvmr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gawzpqhno.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gogdjwyeg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gljppjsfr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gygfzptvy.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gqjzkjced.sHtML


<!-- 参考信息 -->