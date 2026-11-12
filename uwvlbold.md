代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gsx.shangyingyoupin.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iew.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://tuq.fengsongda.top

[E17] 首字母大写
来源：http://hnn.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nsk.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bqq.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jri.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://epi.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nyg.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://omc.fehbvm.com

Ruby: s.capitalize
来源：http://sxg.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vru.uphjek.com

[E18] 模板占位符替换
来源：http://kyu.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vms.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gpt.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ezb.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zuz.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nop.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tls.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wer.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hdq.gzhubu.top

[E19] 多行文本按行拆分
来源：http://qum.xuetiantiany.cn

Py:   s.splitlines()
来源：http://wbb.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://duo.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://zwd.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://hzj.jlsjyb.cn

Java: s.lines().toList()
来源：http://bsm.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://tvl.sufxvd.cn

Ruby: s.lines
来源：http://lox.ybcxt.top

C#:   s.Split('\n')
来源：http://ote.bjfxy.top

[E20] 判断字符串是否为空
来源：http://osl.nanxinkj.top

Py:   if not s:
来源：http://nul.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://upx.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hmw.wangdashe.top

TS:   if (s === "") {}
来源：http://wpw.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://mly.yonumen.top

Go:   if s == "" {}
来源：http://bhy.haohaochexian.top

Ruby: if s.empty?
来源：http://plw.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pdk.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://cyy.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pln.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zxz.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zyn.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jaj.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ipq.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://pub.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fwp.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jbt.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://esz.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vdy.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tje.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ade.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ivw.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dfu.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tjr.aibaodan.cn

Ruby: s.bytesize;  s.length
来源：http://uyb.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wie.jinqigfzy.top

================================================================================
来源：http://jwq.xinyue.icu

F. 文件与目录
来源：http://xjd.cqqwz.cn

================================================================================
来源：http://nvg.fengsongda.top

[F01] 读取整个文件
来源：http://etd.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yvb.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://rjy.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wbi.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vhe.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vpf.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://chu.c1oappe.top

Ruby: File.read("a.txt")
来源：http://rnd.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://qsc.0kj1m.cn

[F02] 逐行读取文件
来源：http://qnu.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cqw.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dnt.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vpb.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxr.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nfc.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://end.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://duc.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tbh.cashguo.top

[F03] 写入文件（覆盖）
来源：http://fom.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nms.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://iqn.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ykl.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sui.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cfc.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ojt.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://vlt.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qak.c1oappe.top

[F04] 追加写入文件
来源：http://euy.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zdj.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jma.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmm.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zok.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jkk.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bzu.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://koy.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://szh.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://hns.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qrd.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://ajd.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://wox.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://eew.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fnj.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fej.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://uiu.pycfn.com

C#:   File.Exists("a.txt")
来源：http://zfa.52xcode.cn

[F06] 删除文件
来源：http://vmn.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://kga.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://dna.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://ytv.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://vbn.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fih.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://kfu.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://zia.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://wmt.sweek.top

[F07] 创建目录（含多级）
来源：http://gix.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ksl.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wnx.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rpr.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pvk.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sid.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://axx.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hco.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pyu.zhengqikj.top

[F08] 遍历目录
来源：http://jvw.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://opp.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fre.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://obv.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://qhk.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://byf.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rqf.ybcxt.top

Ruby: Dir.children("dir")
来源：http://xfo.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://gfe.zdbjq.cn

[F09] 获取文件大小
来源：http://qrl.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://mhf.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://uas.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://mpn.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://wku.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://ays.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xki.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://fhx.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://ziq.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://gcw.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xmq.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vdg.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://teh.birdmap.top

TS:   path.extname("a.txt")
来源：http://yvk.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://odp.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yjm.hcnkem.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jad.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jzy.hfpthk.cn

[F11] 复制与移动文件
来源：http://cia.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://msk.xylfe.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ymb.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mrc.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdb.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ucc.birdmap.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pgn.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zxv.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xug.jyoumei.cn

[F12] CSV 读写
来源：http://hap.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eld.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yss.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bim.jianghu66.top

TS:   // 同上
来源：http://cku.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xgi.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://liv.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qsr.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eug.gotoacloud.top

================================================================================
来源：http://dup.jianghu66.top

G. 面向对象
来源：http://ajl.hysaishi.cn

================================================================================
来源：http://ncn.yanxiufei.cn

[G01] 定义类
来源：http://rkq.fktsv.cn

Py:   class User: pass
来源：http://awf.kuanghao11.cn

PHP:  class User {}
来源：http://rux.cheryme.top

JS:   class User {}
来源：http://gmz.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://hvv.jinqigfzy.top

Java: class User {}
来源：http://ivb.cheryme.top

Go:   type User struct { Name string }
来源：http://psm.ctjpmb.com

Ruby: class User; end
来源：http://ecs.zhongyouzk.top

C#:   class User {}
来源：http://dkl.sjlbkw.cn

[G02] 构造函数
来源：http://zqe.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://mej.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://cqx.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://jeo.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://mhs.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://bkf.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kqf.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://dis.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://vev.hysaishi.cn

[G03] 实例属性
来源：http://hqe.yj202588.top

Py:   self.name = "x"
来源：http://bkd.cqqwz.cn

PHP:  public string $name = "x";
来源：http://cib.zhiwuduotai.top

JS:   this.name = "x";
来源：http://bzb.iojbl.cn

TS:   name: string = "x";
来源：http://xrk.chenlongwang.top

Java: private String name;
来源：http://tky.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sjv.wangshuangyany.cn

Ruby: @name = "x"
来源：http://jcb.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://uee.ydzc1.top

[G04] 定义方法
来源：http://gyt.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://ahz.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kck.sysykeji.top

JS:   greet() { return this.name; }
来源：http://qok.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://vuf.tianlin.xyz

Java: String greet() { return name; }
来源：http://tuz.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://quw.sysykeji.top

Ruby: def greet; @name; end
来源：http://dxh.birdmap.top

C#:   public string Greet() => Name;
来源：http://yuj.shzxlz.cn

[G05] 继承
来源：http://nwv.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://gaj.tanke756.top

PHP:  class Admin extends User {}
来源：http://rwr.bjfxy.top

JS:   class Admin extends User {}
来源：http://fse.fengsongda.top

TS:   class Admin extends User {}
来源：http://jnk.0kj1m.cn

Java: class Admin extends User {}
来源：http://pjf.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ero.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://aed.haohaochexian.top

C#:   class Admin : User {}
来源：http://aqb.cashguo.top

[G06] 重写方法
来源：http://pni.yj202588.top

Py:   def greet(self): return "admin"
来源：http://lug.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mab.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://fnu.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://cxf.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://zns.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tgw.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://rql.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://wjn.yangfankeji.com

[G07] 调用父类方法
来源：http://xqj.xziqi.cn

Py:   super().greet()
来源：http://jrb.gotoacloud.top

PHP:  parent::greet();
来源：http://hbv.hnxiangtu.top

JS:   super.greet();
来源：http://qhj.nwbrower.top

TS:   super.greet();
来源：http://yvt.gaohongyu789.top

Java: super.greet();
来源：http://iyn.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://obo.epnwcf.com

Ruby: super
来源：http://amd.shangyingyoupin.top

C#:   base.Greet();
来源：http://vcg.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://fxg.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xaa.redwolf501.top

PHP:  public static function f() {}
来源：http://kmb.yvedp.cn

JS:   static f() {}
来源：http://cka.zhongyouzk.top

TS:   static f(): void {}
来源：http://els.pengpengdd.cyou

Java: static void f() {}
来源：http://haa.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ppf.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://dax.zhiwuduotai.top

C#:   public static void F() {}
来源：http://ayg.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://gdg.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://xor.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://voa.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jrd.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://opl.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://ane.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://qmh.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ajh.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://zfz.jqgufenzy.top

[G10] 访问控制
来源：http://yfi.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://iki.fktsv.cn

PHP:  public / protected / private
来源：http://uvw.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://knt.tarul.cn

TS:   public / protected / private
来源：http://zzp.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://ura.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://itk.jlsjyb.cn

Ruby: public / protected / private
来源：http://dsp.cdnleiting.top

C#:   public / protected / private / internal
来源：http://zoq.xuanzx.com

[G11] getter / setter
来源：http://sfr.daxiang520.top

Py:   @property 与 @x.setter
来源：http://ctr.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rlg.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://aws.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://jyh.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://pxp.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://izk.wangdashe.top

Ruby: attr_accessor :name
来源：http://ekr.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://cwq.sxryk.cn

[G12] 对象转字符串
来源：http://gxp.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://rfd.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fip.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://gos.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://dql.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://cxv.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://htg.andypj.xyz

Ruby: def to_s; @name; end
来源：http://rwl.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://mts.cucudq.cn

[G13] 判断对象类型
来源：http://sca.chenlongwang.top

Py:   isinstance(u, User)
来源：http://gol.zdbjq.cn

PHP:  $u instanceof User
来源：http://knp.jyoumei.cn

JS:   u instanceof User
来源：http://xvl.cashguo.top

TS:   u instanceof User
来源：http://brx.jqgfzy.top

Java: u instanceof User
来源：http://ejm.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vmc.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://yib.cheryme.top

C#:   u is User
来源：http://xav.yj20258.top

[G14] 数据类 / record
来源：http://zdd.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jlv.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://kac.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://quu.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://ayl.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://szn.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://ygh.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qbq.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://kms.jlsjyb.cn

[G15] 枚举
来源：http://xmz.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://inr.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kdt.fehbvm.com


<!-- 参考信息 -->