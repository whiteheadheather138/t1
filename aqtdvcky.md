代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://why.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qpq.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vsq.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://otw.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yhs.hesvh.cn

================================================================================
来源：http://buc.zhongyouzk.top

F. 文件与目录
来源：http://mti.pycfn.com

================================================================================
来源：http://plt.vehdjk.com

[F01] 读取整个文件
来源：http://kqh.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mxp.hongshengwenyu.top

PHP:  file_get_contents("a.txt");
来源：http://fuu.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lmo.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nkq.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tki.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bbe.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://oee.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://wfn.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://cof.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yfq.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://txi.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://its.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixl.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ort.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zom.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qll.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gni.havefunace.top

[F03] 写入文件（覆盖）
来源：http://ikn.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cxf.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kph.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rwk.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://njx.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bys.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dnv.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://tyi.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nlm.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://jyk.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wmn.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nep.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://din.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gne.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hgq.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yuq.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://spc.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oqw.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://fqf.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iuk.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://ynj.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://vdf.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://zao.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://old.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nfl.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://ual.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://iac.vqdsnc.cn

[F06] 删除文件
来源：http://wyx.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://ttc.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://qyq.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://lta.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://aqi.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://odn.cashguo.top

Go:   os.Remove("a.txt")
来源：http://igo.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://kpd.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://efh.xziqi.cn

[F07] 创建目录（含多级）
来源：http://zax.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sce.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ehd.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fvp.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rdh.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lvi.shuidangran.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oig.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://abn.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yay.wangdashe.top

[F08] 遍历目录
来源：http://szj.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zdy.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://trm.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://wlt.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://knd.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abv.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://olc.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://amw.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://yrn.tian-w.cn

[F09] 获取文件大小
来源：http://bpf.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://tsd.guannengcc.top

PHP:  filesize("a.txt");
来源：http://scb.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://hlo.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://cfy.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://xln.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bqo.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://jig.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://qnh.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://fud.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dvs.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ler.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rbn.yvedp.cn

TS:   path.extname("a.txt")
来源：http://nvt.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oyf.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rcp.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xhp.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kmg.guannengcc.top

[F11] 复制与移动文件
来源：http://irg.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://brn.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ifl.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iqj.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iin.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rnk.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tnn.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qhu.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybe.hnxiangtu.top

[F12] CSV 读写
来源：http://vhy.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vqe.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kge.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wsw.yvedp.cn

TS:   // 同上
来源：http://wac.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ujs.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lyo.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ekr.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kri.ydjk.org.cn

================================================================================
来源：http://ace.pengpengdd.cyou

G. 面向对象
来源：http://xsx.cashguo.top

================================================================================
来源：http://yhv.yanxiufei.cn

[G01] 定义类
来源：http://ofp.shangyingyoupin.top

Py:   class User: pass
来源：http://dlo.fanxiaobao.xyz

PHP:  class User {}
来源：http://tcm.cashguo.top

JS:   class User {}
来源：http://pnb.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://leh.guannengcc.top

Java: class User {}
来源：http://vdw.mhx1999.top

Go:   type User struct { Name string }
来源：http://mzy.zhiwuduotai.top

Ruby: class User; end
来源：http://feg.cqqwz.cn

C#:   class User {}
来源：http://lqy.zhixingplan.top

[G02] 构造函数
来源：http://hgs.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://xgq.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://zje.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://mga.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://dgg.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://qlf.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gld.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://mzv.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://izl.pycfn.com

[G03] 实例属性
来源：http://dau.uphjek.com

Py:   self.name = "x"
来源：http://juv.chenlongwang.top

PHP:  public string $name = "x";
来源：http://fuy.shzxlz.cn

JS:   this.name = "x";
来源：http://asb.bjfxy.top

TS:   name: string = "x";
来源：http://hpz.gogol.net.cn

Java: private String name;
来源：http://tue.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zgn.pycfn.com

Ruby: @name = "x"
来源：http://zrv.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://eut.dashuyun.cn

[G04] 定义方法
来源：http://nbq.epnwcf.com

Py:   def greet(self): return self.name
来源：http://ehu.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gyb.tian-w.cn

JS:   greet() { return this.name; }
来源：http://fgg.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://trf.haohaochexian.top

Java: String greet() { return name; }
来源：http://emm.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hpm.jinqigufen.top

Ruby: def greet; @name; end
来源：http://xda.bjfxy.top

C#:   public string Greet() => Name;
来源：http://wjq.zhixingplan.top

[G05] 继承
来源：http://utc.zhengqikj.top

Py:   class Admin(User): pass
来源：http://qfo.cashguo.top

PHP:  class Admin extends User {}
来源：http://yrl.hesvh.cn

JS:   class Admin extends User {}
来源：http://sfe.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://qlz.tarul.cn

Java: class Admin extends User {}
来源：http://wiq.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lgf.yonumen.top

Ruby: class Admin < User; end
来源：http://nse.nwbrower.top

C#:   class Admin : User {}
来源：http://ymn.hysaishi.cn

[G06] 重写方法
来源：http://qom.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://wbi.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://uue.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://tkq.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://xfu.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://xdg.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yds.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://vhe.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://ymx.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://kuy.tarul.cn

Py:   super().greet()
来源：http://xxe.fzhhl.top

PHP:  parent::greet();
来源：http://hjp.yj20258.top

JS:   super.greet();
来源：http://nwd.cdnleiting.top

TS:   super.greet();
来源：http://agl.bjfxy.top

Java: super.greet();
来源：http://sur.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ggb.ywan-chungtsiang.top

Ruby: super
来源：http://jrv.chenzaomai.com

C#:   base.Greet();
来源：http://hvg.52xcode.cn

[G08] 静态方法与属性
来源：http://pjh.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kjy.jinqigufen.top

PHP:  public static function f() {}
来源：http://xyy.fktsv.cn

JS:   static f() {}
来源：http://mjs.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://gwz.hywenlv.cn

Java: static void f() {}
来源：http://ljk.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ebc.zhijiandao.cn

Ruby: def self.f; end
来源：http://fqt.cucudq.cn

C#:   public static void F() {}
来源：http://yzh.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://vzy.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://vye.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://xre.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rzm.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://sey.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://pcy.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://qyt.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fza.sweek.top

C#:   interface IShape { double Area(); }
来源：http://ugd.andypj.xyz

[G10] 访问控制
来源：http://hwo.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://dee.ivvv.top

PHP:  public / protected / private
来源：http://cqp.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://mwo.jyoumei.cn

TS:   public / protected / private
来源：http://uak.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://jwe.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kfz.ppjwa.cn

Ruby: public / protected / private
来源：http://zjn.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://cqh.hcnkem.com

[G11] getter / setter
来源：http://aab.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://fdq.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yrd.pycfn.com

JS:   get name() { return this._name; }
来源：http://oxy.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://ekl.nanxinkj.top

Java: public String getName() { return name; }
来源：http://wmn.wangdashe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ikg.hcnkem.com

Ruby: attr_accessor :name
来源：http://arn.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://wgl.zhoulong.xyz

[G12] 对象转字符串
来源：http://cnr.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://kil.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://amq.andypj.xyz

JS:   toString() { return this.name; }
来源：http://hxe.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://mli.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://hfa.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://wlw.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://fzx.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://gbk.ehwqpu.com

[G13] 判断对象类型
来源：http://wgp.gzhubu.top

Py:   isinstance(u, User)
来源：http://lqj.cashguo.top

PHP:  $u instanceof User
来源：http://xfp.cheryme.top

JS:   u instanceof User
来源：http://zmh.jlsjyb.cn

TS:   u instanceof User
来源：http://rja.yangfankeji.com

Java: u instanceof User
来源：http://hzr.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hxs.bjfxy.top

Ruby: u.is_a?(User)
来源：http://ctv.hysaishi.cn

C#:   u is User
来源：http://vpa.haohaochexian.top

[G14] 数据类 / record
来源：http://pib.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tfj.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://xco.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xak.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://syq.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://zyd.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://unq.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pem.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://gug.zhiwuduotai.top

[G15] 枚举
来源：http://lxr.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jwp.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gjw.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wpp.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ive.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://bhx.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gnc.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://lux.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bpv.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://gzt.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eme.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://umr.redwolf501.top

JS:   Object.entries(obj)
来源：http://rbr.birdmap.top

TS:   Object.entries(obj)
来源：http://zjg.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://krj.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dzo.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://xus.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://xyb.hesvh.cn

================================================================================
来源：http://vgk.zhongyouzk.top

H. 异常与错误处理
来源：http://tfo.ppjwa.cn

================================================================================
来源：http://whg.ehwqpu.com

[H01] try / catch 基础
来源：http://pof.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jma.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ktp.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://umu.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jkx.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jtf.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cja.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vfb.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://puf.c1oappe.top

[H02] finally / ensure 收尾
来源：http://tfo.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://rzy.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zgv.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ymr.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wyb.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mik.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://zqv.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://glq.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zig.fktsv.cn

[H03] 主动抛出异常
来源：http://hro.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://who.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yst.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://low.yj202588.top

TS:   throw new Error("错误信息");
来源：http://gzq.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wnr.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rlr.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jfi.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://uml.sufxvd.cn

[H04] 自定义异常类型
来源：http://rtk.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://dpa.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://txq.epnwcf.com

JS:   class MyError extends Error {}
来源：http://bvq.yj20258.top

TS:   class MyError extends Error {}
来源：http://fjs.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://jle.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gze.ywan-chungtsiang.top


<!-- 参考信息 -->