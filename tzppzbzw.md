代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jxr.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ads.jyoumei.cn

Ruby: s.capitalize
来源：http://krw.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kpv.nanxuanxn.top

[E18] 模板占位符替换
来源：http://bqk.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zeq.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mkl.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xzs.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://btm.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tbn.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kmg.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lwz.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ose.fzhhl.top

[E19] 多行文本按行拆分
来源：http://dky.yj20258888.top

Py:   s.splitlines()
来源：http://poc.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mhn.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://mzf.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://sis.wangshuangyany.cn

Java: s.lines().toList()
来源：http://pvw.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://sqx.snrcjt.cn

Ruby: s.lines
来源：http://dqo.dianchejie.cn

C#:   s.Split('\n')
来源：http://xhv.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://lwx.nwbrower.top

Py:   if not s:
来源：http://kyr.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hyu.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kjt.yanxiufei.cn

TS:   if (s === "") {}
来源：http://ffj.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://wwv.wangshuangyany.cn

Go:   if s == "" {}
来源：http://zyn.sufxvd.cn

Ruby: if s.empty?
来源：http://ico.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vye.jiagoushi.top

[E21] 超长截断加省略号
来源：http://ipi.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lth.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ckp.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://brx.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vxa.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nng.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://pqs.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hmt.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xtx.fehbvm.com

[E22] 字节长度与字符长度
来源：http://cwu.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gzs.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zps.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aag.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fsm.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rlp.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ppd.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://xan.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ian.hnxiangtu.top

================================================================================
来源：http://gkv.gaohongyu789.top

F. 文件与目录
来源：http://kzb.tian-w.cn

================================================================================
来源：http://olx.cdnleiting.top

[F01] 读取整个文件
来源：http://nbc.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wqd.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://mhq.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pgm.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fag.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://cob.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://moh.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://mfm.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://yvo.ydjk.org.cn

[F02] 逐行读取文件
来源：http://fov.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vbg.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ijw.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sfq.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hrv.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lur.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gai.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ljf.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mio.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://grm.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ekt.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://smm.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ohx.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://szw.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hfm.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://upe.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://kge.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rbh.chenzaomai.com

[F04] 追加写入文件
来源：http://dai.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yll.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sdy.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ubp.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ujm.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rwt.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xuc.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zuz.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://enz.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://slm.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vpe.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://unp.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://acj.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://foj.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fcw.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ofp.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://vjx.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://wmb.hesvh.cn

[F06] 删除文件
来源：http://ulr.cashguo.top

Py:   os.remove("a.txt")
来源：http://fvf.yongpay.top

PHP:  unlink("a.txt");
来源：http://eji.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://plg.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://eoa.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gct.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://gze.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://wzv.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://lnz.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://htf.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://huo.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://six.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bvc.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eon.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nbd.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://etf.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tks.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pmj.birdmap.top

[F08] 遍历目录
来源：http://fvr.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://llh.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kjw.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://qnd.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://nek.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zhk.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uvz.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://sdh.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://hgu.cashguo.top

[F09] 获取文件大小
来源：http://drd.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://xki.mhx1999.top

PHP:  filesize("a.txt");
来源：http://qcv.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://ngv.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://cao.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://hzg.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sek.xuanzx.com

Ruby: File.size("a.txt")
来源：http://gui.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://hoy.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://xpl.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tws.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://woq.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zhk.fktsv.cn

TS:   path.extname("a.txt")
来源：http://cvz.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://udi.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xhm.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yhn.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://snd.sxryk.cn

[F11] 复制与移动文件
来源：http://hnz.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kkl.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bal.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://irc.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hgh.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lbz.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rka.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lkc.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://klt.c1oappe.top

[F12] CSV 读写
来源：http://pjk.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kny.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uab.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fjx.vehdjk.com

TS:   // 同上
来源：http://ljt.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://csi.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://olc.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vcj.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://szh.mhx1999.top

================================================================================
来源：http://lql.xingfuxueyuan.xyz

G. 面向对象
来源：http://uam.ybcxt.top

================================================================================
来源：http://rlr.daria6918.cn

[G01] 定义类
来源：http://xwg.cheryme.top

Py:   class User: pass
来源：http://jpy.zycfv.cn

PHP:  class User {}
来源：http://jsv.tian-w.cn

JS:   class User {}
来源：http://xsq.uphjek.com

TS:   class User { name: string = ""; }
来源：http://lqw.guannengcc.top

Java: class User {}
来源：http://qlz.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://xid.ehwqpu.com

Ruby: class User; end
来源：http://wod.shanyushiyangtech.top

C#:   class User {}
来源：http://qhn.ybcxt.top

[G02] 构造函数
来源：http://lzf.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://nlf.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://qai.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://ewi.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://pkd.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://hiv.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vim.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://wyq.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://sxe.yj20258888.top

[G03] 实例属性
来源：http://rbg.cheryme.top

Py:   self.name = "x"
来源：http://mbp.bbcook.cn

PHP:  public string $name = "x";
来源：http://xlq.daria6918.cn

JS:   this.name = "x";
来源：http://dmj.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://jsm.yj202588.top

Java: private String name;
来源：http://zqf.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wbt.xinyue.icu

Ruby: @name = "x"
来源：http://won.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://nhw.jqgufenzy.top

[G04] 定义方法
来源：http://fpx.yonumen.top

Py:   def greet(self): return self.name
来源：http://nne.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pxr.hcnkem.com

JS:   greet() { return this.name; }
来源：http://awq.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://jlm.fzhhl.top

Java: String greet() { return name; }
来源：http://yns.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zgf.cheryme.top

Ruby: def greet; @name; end
来源：http://wiz.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://krz.yvedp.cn

[G05] 继承
来源：http://ady.xziqi.cn

Py:   class Admin(User): pass
来源：http://fmh.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://efu.fehbvm.com

JS:   class Admin extends User {}
来源：http://bjp.hywenlv.cn

TS:   class Admin extends User {}
来源：http://pvv.yuxming.cn

Java: class Admin extends User {}
来源：http://twe.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gdj.cheryme.top

Ruby: class Admin < User; end
来源：http://tix.ehwqpu.com

C#:   class Admin : User {}
来源：http://ytn.jlsjyb.cn

[G06] 重写方法
来源：http://yhp.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://aku.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zzm.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://jxz.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://jel.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://hsu.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dex.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://wvn.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://tla.tarul.cn

[G07] 调用父类方法
来源：http://jsi.feifeiyinyue.top

Py:   super().greet()
来源：http://bva.pengpengdd.cyou

PHP:  parent::greet();
来源：http://vfw.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://ozf.uphjek.com

TS:   super.greet();
来源：http://lin.smart0.xyz

Java: super.greet();
来源：http://bay.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ujp.zhiwuduotai.top

Ruby: super
来源：http://ydj.jinghuilouyu.cn

C#:   base.Greet();
来源：http://xmd.jyoumei.cn

[G08] 静态方法与属性
来源：http://ade.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uzn.andypj.xyz

PHP:  public static function f() {}
来源：http://nal.yvedp.cn

JS:   static f() {}
来源：http://skj.fengsongda.top

TS:   static f(): void {}
来源：http://cfn.yanxiufei.cn

Java: static void f() {}
来源：http://sfq.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bzr.chenlongwang.top

Ruby: def self.f; end
来源：http://mxf.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://qox.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://xbp.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://fmy.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zec.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zgo.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://vth.yonumen.top

Java: interface Shape { double area(); }
来源：http://ldt.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://gek.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sdl.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://neo.zhiwuduotai.top

[G10] 访问控制
来源：http://ptm.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://tzq.feifeiyinyue.top

PHP:  public / protected / private
来源：http://rdw.shuidangran.top

JS:   #private 字段；其余公开
来源：http://vcz.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://rde.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://aeo.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://lbp.xuetiantiany.cn

Ruby: public / protected / private
来源：http://qwm.cucudq.cn

C#:   public / protected / private / internal
来源：http://wrv.yvedp.cn

[G11] getter / setter
来源：http://foi.yuxming.cn

Py:   @property 与 @x.setter
来源：http://yar.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eqb.fzhhl.top

JS:   get name() { return this._name; }
来源：http://oox.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://dml.hywenlv.cn

Java: public String getName() { return name; }
来源：http://qxc.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qpo.ivvv.top

Ruby: attr_accessor :name
来源：http://mmi.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://ixh.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://gpa.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://sbf.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://heo.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://mea.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://mde.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://wsx.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yle.yj20258888.top

Ruby: def to_s; @name; end
来源：http://ano.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://xen.zhiwuduotai.top

[G13] 判断对象类型
来源：http://nyh.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://rxs.tanke756.top

PHP:  $u instanceof User
来源：http://yqr.chenlongwang.top

JS:   u instanceof User
来源：http://eag.yj20258888.top

TS:   u instanceof User
来源：http://kjj.fzhhl.top

Java: u instanceof User
来源：http://mvx.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qxm.xinyue.icu

Ruby: u.is_a?(User)
来源：http://qvf.gogol.net.cn

C#:   u is User
来源：http://opl.vehdjk.com

[G14] 数据类 / record
来源：http://tau.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cqu.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://mpy.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://qfb.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://del.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://qrh.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://gcv.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nnu.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://fgv.andypj.xyz

[G15] 枚举
来源：http://hww.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nkb.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ssz.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jhu.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tjx.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://rgu.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qgp.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://kir.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gvc.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://tuv.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kdb.aibaodan.cn


<!-- 参考信息 -->