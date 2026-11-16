代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tsx.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://eif.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://swa.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wjk.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://spf.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ifm.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://lij.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rcp.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://ltl.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://osc.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kbi.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bxn.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jsk.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fyb.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wrq.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qrz.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ued.yj202588.top

[E19] 多行文本按行拆分
来源：http://ndd.birdmap.top

Py:   s.splitlines()
来源：http://vrm.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://crb.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://iij.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://hns.wangdashe.top

Java: s.lines().toList()
来源：http://rep.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://lfn.jinqigufen.top

Ruby: s.lines
来源：http://ykr.jinqigufen.top

C#:   s.Split('\n')
来源：http://azv.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://heq.ydjk.org.cn

Py:   if not s:
来源：http://mpg.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://joc.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gad.52xcode.cn

TS:   if (s === "") {}
来源：http://uol.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://ylg.yvedp.cn

Go:   if s == "" {}
来源：http://ydo.birdmap.top

Ruby: if s.empty?
来源：http://qus.hesvh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://snk.chenlongwang.top

[E21] 超长截断加省略号
来源：http://kxw.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://psl.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hld.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qdq.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://huy.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tra.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://snv.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ebu.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zki.jianghu66.top

[E22] 字节长度与字符长度
来源：http://tyz.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nmw.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gww.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tbi.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zru.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://heb.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kef.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://dvc.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wde.wangdashe.top

================================================================================
来源：http://jfs.chenzaomai.com

F. 文件与目录
来源：http://ann.nanxuanxn.top

================================================================================
来源：http://yyv.hcnkem.com

[F01] 读取整个文件
来源：http://dsp.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qyh.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://hbd.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fdj.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vrj.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dcp.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://evk.epnwcf.com

Ruby: File.read("a.txt")
来源：http://tmz.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://qza.birdmap.top

[F02] 逐行读取文件
来源：http://glb.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gwm.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ggw.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tfo.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gbt.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xte.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dnx.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ozd.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vrx.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://yje.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dwo.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rnn.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dqh.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uvl.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dvm.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fnd.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://oes.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gnp.xuanzx.com

[F04] 追加写入文件
来源：http://bbr.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://plf.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jim.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zre.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufu.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nqb.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tpf.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ges.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xdu.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://ikw.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wcr.yj202588.top

PHP:  file_exists("a.txt");
来源：http://qvi.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://qig.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://mqt.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jms.sysykeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ggx.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://xni.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://bhf.jinqigfzy.top

[F06] 删除文件
来源：http://dyw.andypj.xyz

Py:   os.remove("a.txt")
来源：http://gbm.yuxming.cn

PHP:  unlink("a.txt");
来源：http://ysb.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rik.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://ani.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ine.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://efq.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://fmj.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://yot.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://mfk.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wze.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nnj.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nqe.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://anz.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rle.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://unt.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rrg.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ttz.birdmap.top

[F08] 遍历目录
来源：http://tos.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bdi.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ipi.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://bdy.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://ypd.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qhg.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ohh.fktsv.cn

Ruby: Dir.children("dir")
来源：http://ahg.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://wdp.jinqigfzy.top

[F09] 获取文件大小
来源：http://sab.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://lty.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://bih.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://rpg.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://tng.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uef.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://msi.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://pdm.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://zjv.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://zjn.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ufn.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mja.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sfv.hesvh.cn

TS:   path.extname("a.txt")
来源：http://ybt.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ovu.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xnh.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://snx.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yir.yangfankeji.com

[F11] 复制与移动文件
来源：http://cda.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fcf.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://efz.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://srt.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dgt.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://urw.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lig.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uvc.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://irn.yongpay.top

[F12] CSV 读写
来源：http://bbr.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dlu.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lwo.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wxw.yfazqb.com

TS:   // 同上
来源：http://ldr.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uhk.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ivl.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wat.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cqv.tian-w.cn

================================================================================
来源：http://drz.cucudq.cn

G. 面向对象
来源：http://mqg.xingfuxueyuan.xyz

================================================================================
来源：http://gye.xuetiantiany.cn

[G01] 定义类
来源：http://ocu.mhx1999.top

Py:   class User: pass
来源：http://imq.shzxlz.cn

PHP:  class User {}
来源：http://ajr.yfazqb.com

JS:   class User {}
来源：http://bhg.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://tts.fzhhl.top

Java: class User {}
来源：http://dzb.iojbl.cn

Go:   type User struct { Name string }
来源：http://kqk.ywan-chungtsiang.top

Ruby: class User; end
来源：http://typ.redwolf501.top

C#:   class User {}
来源：http://hfg.jinqigfzy.top

[G02] 构造函数
来源：http://eey.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://xpq.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://klq.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://vib.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://pvb.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://zbr.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fay.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://aqu.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://jhq.quarkkingdee.top

[G03] 实例属性
来源：http://gyw.gotoacloud.top

Py:   self.name = "x"
来源：http://jwn.vehdjk.com

PHP:  public string $name = "x";
来源：http://qye.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://fsw.yj202588.top

TS:   name: string = "x";
来源：http://rmn.fengsongda.top

Java: private String name;
来源：http://cou.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uto.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://kax.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://aaz.guowangkeji.top

[G04] 定义方法
来源：http://dko.andypj.xyz

Py:   def greet(self): return self.name
来源：http://fbi.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://cxw.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://bfb.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://uwb.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://oxw.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ijg.52xcode.cn

Ruby: def greet; @name; end
来源：http://xrj.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://mil.guannengcc.top

[G05] 继承
来源：http://wxz.aibaodan.cn

Py:   class Admin(User): pass
来源：http://tip.fehbvm.com

PHP:  class Admin extends User {}
来源：http://vrt.daria6918.cn

JS:   class Admin extends User {}
来源：http://nyh.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://huf.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://pwh.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://css.tanke756.top

Ruby: class Admin < User; end
来源：http://yfz.fehbvm.com

C#:   class Admin : User {}
来源：http://zqx.hywenlv.cn

[G06] 重写方法
来源：http://qdp.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://ykb.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rpp.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://jiz.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://mon.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://pch.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bqt.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://gpa.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://gtu.quarkkingdee.top

[G07] 调用父类方法
来源：http://wuv.sxryk.cn

Py:   super().greet()
来源：http://nyx.yangfankeji.com

PHP:  parent::greet();
来源：http://kog.epnwcf.com

JS:   super.greet();
来源：http://gnu.zdqjudy.top

TS:   super.greet();
来源：http://ign.fanxiaobao.xyz

Java: super.greet();
来源：http://vgk.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ttd.fengsongda.top

Ruby: super
来源：http://ecy.bbcook.cn

C#:   base.Greet();
来源：http://ags.sufxvd.cn

[G08] 静态方法与属性
来源：http://dta.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cin.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://efr.jinghuilouyu.cn

JS:   static f() {}
来源：http://zvq.jianghu66.top

TS:   static f(): void {}
来源：http://bav.haohaochexian.top

Java: static void f() {}
来源：http://dgx.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://ppf.jlsjyb.cn

Ruby: def self.f; end
来源：http://mjc.jqgfzy.top

C#:   public static void F() {}
来源：http://vhi.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://zwx.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://gol.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://oap.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://art.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://moc.tarul.cn

Java: interface Shape { double area(); }
来源：http://jbo.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://nnq.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fga.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://whn.guowangkeji.top

[G10] 访问控制
来源：http://odc.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://gyh.hysaishi.cn

PHP:  public / protected / private
来源：http://ajn.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://eto.gzhubu.top

TS:   public / protected / private
来源：http://ysq.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://wrk.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zoi.yuxming.cn

Ruby: public / protected / private
来源：http://pvj.nanxinkj.top

C#:   public / protected / private / internal
来源：http://gev.jinqigfzy.top

[G11] getter / setter
来源：http://vha.daxiang520.top

Py:   @property 与 @x.setter
来源：http://crf.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cpw.316326.xyz

JS:   get name() { return this._name; }
来源：http://efp.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://yac.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://bzj.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sxs.zycfv.cn

Ruby: attr_accessor :name
来源：http://lcs.fehbvm.com

C#:   public string Name { get; set; }
来源：http://ngv.zdqjudy.top

[G12] 对象转字符串
来源：http://cqv.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://aro.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cbx.yuxming.cn

JS:   toString() { return this.name; }
来源：http://dfb.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://ltn.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://ciq.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://ijs.mhx1999.top

Ruby: def to_s; @name; end
来源：http://nue.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://zkn.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://jka.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://lgo.aizwys.cn

PHP:  $u instanceof User
来源：http://wii.pengpengdd.cyou

JS:   u instanceof User
来源：http://vfm.fanxiaobao.xyz

TS:   u instanceof User
来源：http://ufc.meibo888.top

Java: u instanceof User
来源：http://noy.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lhc.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://fup.aibaodan.cn

C#:   u is User
来源：http://dkg.yanxiufei.cn

[G14] 数据类 / record
来源：http://xyq.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tny.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://iyt.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://zzb.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://shr.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://cxx.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://iec.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vvd.jqgufenzy.top

C#:   record User(string Name, int Age);
来源：http://xps.ydjk.org.cn

[G15] 枚举
来源：http://mjy.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vhe.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xll.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zqv.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ucg.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://bqu.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aes.zdqjudy.top


<!-- 参考信息 -->