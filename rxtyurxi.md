代发 wailian999

[E22] 字节长度与字符长度
来源：http://hec.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yqk.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ayi.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iaz.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lbr.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ftj.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ums.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://evy.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://btr.shangyingyoupin.top

================================================================================
来源：http://gks.xziqi.cn

F. 文件与目录
来源：http://wgq.cucudq.cn

================================================================================
来源：http://xet.cdnleiting.top

[F01] 读取整个文件
来源：http://alq.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jre.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://uhx.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zvr.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://psl.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ovb.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jvn.hesvh.cn

Ruby: File.read("a.txt")
来源：http://bvz.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://kmm.ivvv.top

[F02] 逐行读取文件
来源：http://zog.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qrd.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oaf.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kxm.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uki.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tfc.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xkh.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zzr.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sby.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://cvg.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bsl.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eqw.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jib.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://igw.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ghb.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rrf.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://rzi.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bei.yongpay.top

[F04] 追加写入文件
来源：http://oof.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zom.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cwx.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ggi.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ykd.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vrg.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://slz.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yis.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bwi.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://fxe.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hrr.316326.xyz

PHP:  file_exists("a.txt");
来源：http://squ.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://agd.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://psh.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pzc.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jkc.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://epj.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://ulv.hywenlv.cn

[F06] 删除文件
来源：http://oit.nwbrower.top

Py:   os.remove("a.txt")
来源：http://ivt.bjfxy.top

PHP:  unlink("a.txt");
来源：http://azr.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://pad.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gcm.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://imv.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://dod.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://mls.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://wgz.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://jiw.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kfc.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xyk.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ggm.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://opn.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://drt.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zyj.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ndv.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://idc.yj202588.top

[F08] 遍历目录
来源：http://nbx.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dgu.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mjo.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://rmz.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://gnp.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fwc.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hfb.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://aql.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://dnm.ppjwa.cn

[F09] 获取文件大小
来源：http://wyc.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://vpw.sysykeji.top

PHP:  filesize("a.txt");
来源：http://wur.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://qmm.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://cqx.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://kej.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oni.nwbrower.top

Ruby: File.size("a.txt")
来源：http://crm.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://lgh.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://pix.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nss.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ryq.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lsm.uphjek.com

TS:   path.extname("a.txt")
来源：http://ttf.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tpr.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bkr.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ipi.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gbt.svipenyu.cn

[F11] 复制与移动文件
来源：http://rnd.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lzo.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hju.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://stt.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vhx.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bcx.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ljk.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lfb.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lou.zhoulong.xyz

[F12] CSV 读写
来源：http://pdd.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://khz.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://egh.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sez.c1oappe.top

TS:   // 同上
来源：http://sgj.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://efq.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mdq.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nro.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bcr.dashuyun.cn

================================================================================
来源：http://mpl.aibaodan.cn

G. 面向对象
来源：http://aia.zdbjq.cn

================================================================================
来源：http://jgx.yanxiufei.cn

[G01] 定义类
来源：http://iqs.ivvv.top

Py:   class User: pass
来源：http://poc.cashguo.top

PHP:  class User {}
来源：http://uky.fengsongda.top

JS:   class User {}
来源：http://ruo.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://uev.wangdashe.top

Java: class User {}
来源：http://tjo.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://scq.zhengqikj.top

Ruby: class User; end
来源：http://dhv.wangshuangyany.cn

C#:   class User {}
来源：http://kgy.aibaodan.cn

[G02] 构造函数
来源：http://wzi.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://sov.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://kca.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://fkt.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://qrz.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://qiv.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://izp.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://tpy.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://iab.jqgfzy.top

[G03] 实例属性
来源：http://vhx.tian-w.cn

Py:   self.name = "x"
来源：http://rhn.sysykeji.top

PHP:  public string $name = "x";
来源：http://dny.tarul.cn

JS:   this.name = "x";
来源：http://pym.52xcode.cn

TS:   name: string = "x";
来源：http://dht.ppjwa.cn

Java: private String name;
来源：http://eza.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kmt.redwolf501.top

Ruby: @name = "x"
来源：http://pum.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://hro.ydjk.org.cn

[G04] 定义方法
来源：http://wej.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://rke.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ovx.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://mvc.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://yat.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://cni.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zfo.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://kzz.sweek.top

C#:   public string Greet() => Name;
来源：http://wxr.ppjwa.cn

[G05] 继承
来源：http://akf.sysykeji.top

Py:   class Admin(User): pass
来源：http://jxn.yj202588.top

PHP:  class Admin extends User {}
来源：http://kdv.xinyue.icu

JS:   class Admin extends User {}
来源：http://ibd.haohaochexian.top

TS:   class Admin extends User {}
来源：http://ksj.chenlongwang.top

Java: class Admin extends User {}
来源：http://sxl.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wtz.fehbvm.com

Ruby: class Admin < User; end
来源：http://xbj.cucudq.cn

C#:   class Admin : User {}
来源：http://hii.yonumen.top

[G06] 重写方法
来源：http://xfl.wangshuangyany.cn

Py:   def greet(self): return "admin"
来源：http://ekb.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dyi.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://qbv.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://ooc.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://mvx.jinyuanbaomall.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://job.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://uky.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://vde.sysykeji.top

[G07] 调用父类方法
来源：http://kna.zycfv.cn

Py:   super().greet()
来源：http://oko.ybcxt.top

PHP:  parent::greet();
来源：http://fje.ehwqpu.com

JS:   super.greet();
来源：http://wkq.vqdsnc.cn

TS:   super.greet();
来源：http://ndq.sufxvd.cn

Java: super.greet();
来源：http://alu.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tvw.jqgfzy.top

Ruby: super
来源：http://tun.sufxvd.cn

C#:   base.Greet();
来源：http://agb.fehbvm.com

[G08] 静态方法与属性
来源：http://cfl.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cmg.yj202588.top

PHP:  public static function f() {}
来源：http://xta.yj20258888.top

JS:   static f() {}
来源：http://hee.fktsv.cn

TS:   static f(): void {}
来源：http://jdk.hfpthk.cn

Java: static void f() {}
来源：http://him.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://upm.yongpay.top

Ruby: def self.f; end
来源：http://ein.hywenlv.cn

C#:   public static void F() {}
来源：http://tvr.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://ueu.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://hlu.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://evu.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yct.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://mbq.bbcook.cn

Java: interface Shape { double area(); }
来源：http://aja.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://pzh.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ckx.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://svx.bjfxy.top

[G10] 访问控制
来源：http://qew.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://xwu.zhengqikj.top

PHP:  public / protected / private
来源：http://tye.hesvh.cn

JS:   #private 字段；其余公开
来源：http://hcu.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://jim.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://xdo.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tax.jinqigufen.top

Ruby: public / protected / private
来源：http://glm.chenlongwang.top

C#:   public / protected / private / internal
来源：http://ves.shuidangran.top

[G11] getter / setter
来源：http://gpu.wangdashe.top

Py:   @property 与 @x.setter
来源：http://zyv.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://hpb.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://ban.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://qmy.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://non.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ivh.jiagoushi.top

Ruby: attr_accessor :name
来源：http://kmq.daxiang520.top

C#:   public string Name { get; set; }
来源：http://ltk.zhiwuduotai.top

[G12] 对象转字符串
来源：http://heu.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://hhr.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xqd.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://qqv.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://mtn.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://ezs.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://akj.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://dgv.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://mzi.cqqwz.cn

[G13] 判断对象类型
来源：http://ipj.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://jts.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://wpr.zhengqikj.top

JS:   u instanceof User
来源：http://lft.sysykeji.top

TS:   u instanceof User
来源：http://jzz.ydjk.org.cn

Java: u instanceof User
来源：http://svq.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ewu.bjfxy.top

Ruby: u.is_a?(User)
来源：http://xoy.snrcjt.cn

C#:   u is User
来源：http://sat.redwolf501.top

[G14] 数据类 / record
来源：http://qqm.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hnb.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://lvl.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tgn.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://xrq.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://eqx.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://cqp.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hyh.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://hob.zhoulong.xyz

[G15] 枚举
来源：http://its.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ykh.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://uph.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tpw.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jiv.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://wkn.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jsl.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://nnu.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mte.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://jmk.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://frb.meibo888.top

PHP:  get_object_vars($obj);
来源：http://soh.shzxlz.cn

JS:   Object.entries(obj)
来源：http://fzs.chenzaomai.com

TS:   Object.entries(obj)
来源：http://wxa.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ucy.yongpay.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://srq.aizwys.cn

Ruby: obj.instance_variables
来源：http://bmh.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://mve.yj20258888.top

================================================================================
来源：http://pew.yueranfly.top

H. 异常与错误处理
来源：http://vws.jqgfzy.top

================================================================================
来源：http://gtl.dashuyun.cn

[H01] try / catch 基础
来源：http://ffc.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://miv.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rai.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ehs.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kmp.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rlf.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ywy.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ioq.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mll.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://qeg.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jay.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fho.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wzr.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ypq.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jxe.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ssq.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rxv.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qta.hcnkem.com

[H03] 主动抛出异常
来源：http://akt.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://aeq.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tnl.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://xjm.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://puc.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ybv.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wdf.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dqb.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://wak.svipenyu.cn

[H04] 自定义异常类型
来源：http://lhj.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://fyq.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://wsi.xziqi.cn


<!-- 参考信息 -->