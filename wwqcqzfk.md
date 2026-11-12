代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xaa.nanxinkj.top

================================================================================
来源：http://crv.jinyuanbaomall.cn

F. 文件与目录
来源：http://ljt.hcnkem.com

================================================================================
来源：http://zma.cdnleiting.top

[F01] 读取整个文件
来源：http://elv.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oso.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://jfh.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rtu.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bkl.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://khm.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ahw.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://qxg.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://lwb.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://fnh.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nne.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hhu.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vhf.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nwe.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gzu.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mgu.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ocb.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://szs.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://mlz.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://idn.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://mma.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bwj.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fqu.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://for.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dnv.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://lng.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://coh.hfpthk.cn

[F04] 追加写入文件
来源：http://xxb.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lzg.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ksk.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umc.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mkq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vtw.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://chh.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qrh.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jgm.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://zsw.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xqk.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://dou.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://mpk.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://lbs.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://skd.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vsf.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://pvm.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://xqp.hnxiangtu.top

[F06] 删除文件
来源：http://fcw.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://wmd.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://kzw.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://uki.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://bsm.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mec.316326.xyz

Go:   os.Remove("a.txt")
来源：http://rms.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://ycb.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://exp.fktsv.cn

[F07] 创建目录（含多级）
来源：http://axr.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mfn.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blu.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cmx.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aum.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sah.epnwcf.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iiv.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wke.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yfs.gaohongyu789.top

[F08] 遍历目录
来源：http://yom.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tgu.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qep.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://cjy.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://rzk.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blb.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://juc.yongpay.top

Ruby: Dir.children("dir")
来源：http://xmr.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://alv.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://dqp.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://fvw.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://gar.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://zsm.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://wcd.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gwz.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ibf.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://klm.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://svt.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://xwg.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://weh.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qjf.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://shy.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://pdj.feifeiyinyue.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eea.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qdp.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zge.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kxk.shzxlz.cn

[F11] 复制与移动文件
来源：http://zwi.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bpo.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nmx.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mvk.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://exh.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xym.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ytt.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://usa.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jmx.jqgufenzy.top

[F12] CSV 读写
来源：http://jbq.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://axy.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qaw.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pgw.hongshengwenyu.top

TS:   // 同上
来源：http://zlf.gzhubu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rpr.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nyi.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wld.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jxy.yj20258888.top

================================================================================
来源：http://ytj.hammf.cn

G. 面向对象
来源：http://krc.guowangkeji.top

================================================================================
来源：http://mlp.jiagoushi.top

[G01] 定义类
来源：http://dnv.birdmap.top

Py:   class User: pass
来源：http://zyb.jqgfzy.top

PHP:  class User {}
来源：http://glm.aibaodan.cn

JS:   class User {}
来源：http://pow.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://hdk.shangyingyoupin.top

Java: class User {}
来源：http://xtq.yfazqb.com

Go:   type User struct { Name string }
来源：http://tga.meibo888.top

Ruby: class User; end
来源：http://lcg.jqgfzy.top

C#:   class User {}
来源：http://pvo.shuidangran.top

[G02] 构造函数
来源：http://jkc.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://qgx.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://pre.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://ksf.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://klc.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://hth.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lpr.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://irf.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://slv.ivvv.top

[G03] 实例属性
来源：http://wvs.yongpay.top

Py:   self.name = "x"
来源：http://rpl.tanke756.top

PHP:  public string $name = "x";
来源：http://ayl.ydzc1.top

JS:   this.name = "x";
来源：http://uon.daxiang520.top

TS:   name: string = "x";
来源：http://umx.jinqigufen.top

Java: private String name;
来源：http://bsb.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bao.zhengqikj.top

Ruby: @name = "x"
来源：http://uvm.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://zxg.ppjwa.cn

[G04] 定义方法
来源：http://nze.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://wip.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://thv.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://slr.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://lqu.xziqi.cn

Java: String greet() { return name; }
来源：http://dbb.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jyu.yangfankeji.com

Ruby: def greet; @name; end
来源：http://rps.hesvh.cn

C#:   public string Greet() => Name;
来源：http://dhz.yvedp.cn

[G05] 继承
来源：http://vpx.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://ppu.sxryk.cn

PHP:  class Admin extends User {}
来源：http://vab.fktsv.cn

JS:   class Admin extends User {}
来源：http://cjt.jianghu66.top

TS:   class Admin extends User {}
来源：http://tnw.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://bww.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jzl.sysykeji.top

Ruby: class Admin < User; end
来源：http://fwi.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://ysr.ctjpmb.com

[G06] 重写方法
来源：http://jba.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://nxp.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gqe.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://rvv.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://bat.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://erc.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wtp.havefunace.top

Ruby: def greet; "admin"; end
来源：http://pyv.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://qya.fktsv.cn

[G07] 调用父类方法
来源：http://wcd.haohaochexian.top

Py:   super().greet()
来源：http://waa.haohaochexian.top

PHP:  parent::greet();
来源：http://gjl.chenjidiqi.icu

JS:   super.greet();
来源：http://zpf.hcnkem.com

TS:   super.greet();
来源：http://ydb.sjlbkw.cn

Java: super.greet();
来源：http://qmi.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nol.ydzc1.top

Ruby: super
来源：http://xpo.hammf.cn

C#:   base.Greet();
来源：http://bjv.nanxuanxn.top

[G08] 静态方法与属性
来源：http://fvh.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://our.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://kwa.ctjpmb.com

JS:   static f() {}
来源：http://jga.hongshengwenyu.top

TS:   static f(): void {}
来源：http://syp.jinyuanbaomall.cn

Java: static void f() {}
来源：http://vkg.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://njb.0kj1m.cn

Ruby: def self.f; end
来源：http://zdd.jiagoushi.top

C#:   public static void F() {}
来源：http://bvr.xziqi.cn

[G09] 接口 / 抽象类
来源：http://uqu.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://lfr.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://dnw.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://akn.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://jfo.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://zbb.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://sqi.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://smk.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://qxs.shuidangran.top

[G10] 访问控制
来源：http://ysv.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://xdf.hnxiangtu.top

PHP:  public / protected / private
来源：http://gai.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://ghy.jinghuilouyu.cn

TS:   public / protected / private
来源：http://hpd.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://xqd.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sfg.zycfv.cn

Ruby: public / protected / private
来源：http://ksm.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://gur.ydzc1.top

[G11] getter / setter
来源：http://trw.sweek.top

Py:   @property 与 @x.setter
来源：http://tel.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jth.fanxiaobao.xyz

JS:   get name() { return this._name; }
来源：http://iby.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://ebe.birdmap.top

Java: public String getName() { return name; }
来源：http://rjb.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://utd.uphjek.com

Ruby: attr_accessor :name
来源：http://ggw.sweek.top

C#:   public string Name { get; set; }
来源：http://fxk.epnwcf.com

[G12] 对象转字符串
来源：http://mxt.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://uel.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lui.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://eyo.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://ewo.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://poj.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://foj.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://qdo.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://twx.feifeiyinyue.top

[G13] 判断对象类型
来源：http://uhz.ctjpmb.com

Py:   isinstance(u, User)
来源：http://nlm.epnwcf.com

PHP:  $u instanceof User
来源：http://pmh.havefunace.top

JS:   u instanceof User
来源：http://edo.daxiang520.top

TS:   u instanceof User
来源：http://tzy.yanxiufei.cn

Java: u instanceof User
来源：http://ylz.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://riu.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://utu.zycfv.cn

C#:   u is User
来源：http://olu.gogol.net.cn

[G14] 数据类 / record
来源：http://nlt.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://awp.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://jml.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dpj.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://zvw.tarul.cn

Java: record User(String name, int age) {}
来源：http://eej.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://xxi.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xxc.yj202588.top

C#:   record User(string Name, int Age);
来源：http://lhx.svipenyu.cn

[G15] 枚举
来源：http://qtc.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dyg.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zaa.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hel.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fkn.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://qgy.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yoh.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://unn.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://naa.yonumen.top

[G16] 对象转数组 / 字典
来源：http://khu.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iwe.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://jks.ctjpmb.com

JS:   Object.entries(obj)
来源：http://jks.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://nsg.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tig.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iji.yangfankeji.com

Ruby: obj.instance_variables
来源：http://xjm.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://ewu.pycfn.com

================================================================================
来源：http://kmh.fktsv.cn

H. 异常与错误处理
来源：http://awu.tanke756.top

================================================================================
来源：http://vnv.fktsv.cn

[H01] try / catch 基础
来源：http://kyi.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fux.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zkk.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mjp.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cmk.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dic.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uxz.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sqq.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oug.aizwys.cn

[H02] finally / ensure 收尾
来源：http://sbm.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kye.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://snb.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pus.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ytx.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://iev.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xkg.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://emv.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zhx.sxryk.cn

[H03] 主动抛出异常
来源：http://ija.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://cro.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://upp.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://ouo.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://xxo.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dvs.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rgu.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rle.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ohe.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://noi.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://rgl.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vlz.hesvh.cn

JS:   class MyError extends Error {}
来源：http://cvz.wangdashe.top

TS:   class MyError extends Error {}
来源：http://pnr.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://oem.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kbz.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://vuo.birdmap.top

C#:   class MyException : Exception {}
来源：http://vnx.cheryme.top

[H05] 捕获特定类型
来源：http://akx.yj20258.top

Py:   except ValueError as e:
来源：http://xcg.zdqjudy.top


<!-- 参考信息 -->