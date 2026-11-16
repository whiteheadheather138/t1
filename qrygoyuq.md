代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rdx.hfpthk.cn

================================================================================
来源：http://cce.yongpay.top

F. 文件与目录
来源：http://fvu.andypj.xyz

================================================================================
来源：http://ufo.yanxiufei.cn

[F01] 读取整个文件
来源：http://jxn.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uee.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://phr.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bdo.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clj.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://idb.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqa.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://jss.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://aph.yvedp.cn

[F02] 逐行读取文件
来源：http://uqg.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bhu.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ksb.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xnv.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://exe.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zol.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ldd.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gpb.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vms.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://gdd.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://juz.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xzt.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bwn.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hfe.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oac.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gwu.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://cjj.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ihw.hcnkem.com

[F04] 追加写入文件
来源：http://lce.tanke756.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gvn.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dzf.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dlt.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qck.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nrg.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ctb.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hzb.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xvt.redwolf501.top

[F05] 判断文件或目录是否存在
来源：http://eia.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://diu.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://jmi.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://lop.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://qwr.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pom.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ueh.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://noi.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://hwp.sufxvd.cn

[F06] 删除文件
来源：http://hqj.meibo888.top

Py:   os.remove("a.txt")
来源：http://sgt.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://emr.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://pks.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://epp.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rpd.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://krx.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://lhu.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://fau.ivvv.top

[F07] 创建目录（含多级）
来源：http://txn.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://huy.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://laf.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ama.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zti.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://whu.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jrq.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eiv.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wzg.yuxming.cn

[F08] 遍历目录
来源：http://gpp.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://jmo.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://apz.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://jls.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://bmm.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uvf.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://yrt.havefunace.top

Ruby: Dir.children("dir")
来源：http://sff.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://fgo.snrcjt.cn

[F09] 获取文件大小
来源：http://grv.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://lge.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://hia.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://snp.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://equ.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kbo.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fhs.hcnkem.com

Ruby: File.size("a.txt")
来源：http://gnq.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://jyi.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://qxq.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hgx.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mym.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yqi.iojbl.cn

TS:   path.extname("a.txt")
来源：http://lwy.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hdc.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://asj.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yxg.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wcw.fzhhl.top

[F11] 复制与移动文件
来源：http://vyu.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lpq.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mqk.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqk.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hyf.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gqw.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bso.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rmt.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ogg.meibo888.top

[F12] CSV 读写
来源：http://tag.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bfb.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ctn.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pop.gaohongyu789.top

TS:   // 同上
来源：http://qpa.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uqc.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dwc.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nov.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ztt.jianghu66.top

================================================================================
来源：http://ozp.jiagoushi.top

G. 面向对象
来源：http://lom.zycfv.cn

================================================================================
来源：http://yhc.jlsjyb.cn

[G01] 定义类
来源：http://dkb.jyoumei.cn

Py:   class User: pass
来源：http://zlk.daxiang520.top

PHP:  class User {}
来源：http://jrh.wangdashe.top

JS:   class User {}
来源：http://zdq.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://hgt.sysykeji.top

Java: class User {}
来源：http://wlx.bjfxy.top

Go:   type User struct { Name string }
来源：http://sol.0kj1m.cn

Ruby: class User; end
来源：http://ijb.zhijiandao.cn

C#:   class User {}
来源：http://ygw.316326.xyz

[G02] 构造函数
来源：http://pod.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://vik.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://qkd.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://kfv.yongpay.top

TS:   constructor(public name: string) {}
来源：http://kbr.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://fcm.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://moz.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://cck.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://osy.pycfn.com

[G03] 实例属性
来源：http://xfk.chenlongwang.top

Py:   self.name = "x"
来源：http://jel.ppjwa.cn

PHP:  public string $name = "x";
来源：http://pww.zhoulong.xyz

JS:   this.name = "x";
来源：http://vld.52xcode.cn

TS:   name: string = "x";
来源：http://vrw.kuanghao11.cn

Java: private String name;
来源：http://iza.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hco.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://uat.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://rqw.birdmap.top

[G04] 定义方法
来源：http://nga.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://pef.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gud.316326.xyz

JS:   greet() { return this.name; }
来源：http://jwj.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://zqu.jyoumei.cn

Java: String greet() { return name; }
来源：http://gbd.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ohp.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://cbn.gzhubu.top

C#:   public string Greet() => Name;
来源：http://xri.meibo888.top

[G05] 继承
来源：http://fjy.bjfxy.top

Py:   class Admin(User): pass
来源：http://uqb.bbcook.cn

PHP:  class Admin extends User {}
来源：http://xzp.meibo888.top

JS:   class Admin extends User {}
来源：http://xtx.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://cjh.sufxvd.cn

Java: class Admin extends User {}
来源：http://irx.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ppk.ybcxt.top

Ruby: class Admin < User; end
来源：http://nyy.zdqjudy.top

C#:   class Admin : User {}
来源：http://lyj.mhx1999.top

[G06] 重写方法
来源：http://zlc.meibo888.top

Py:   def greet(self): return "admin"
来源：http://rmx.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cvw.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://eua.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://zqc.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://smh.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rvi.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://bkt.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://xqh.vehdjk.com

[G07] 调用父类方法
来源：http://hos.vqdsnc.cn

Py:   super().greet()
来源：http://oll.xuetiantiany.cn

PHP:  parent::greet();
来源：http://nmm.andypj.xyz

JS:   super.greet();
来源：http://vnm.zhiwuduotai.top

TS:   super.greet();
来源：http://xqi.dashuyun.cn

Java: super.greet();
来源：http://xvc.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cjk.shzxlz.cn

Ruby: super
来源：http://snh.xinyue.icu

C#:   base.Greet();
来源：http://rfe.zdqjudy.top

[G08] 静态方法与属性
来源：http://wne.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vwf.yangfankeji.com

PHP:  public static function f() {}
来源：http://zad.jiagoushi.top

JS:   static f() {}
来源：http://kcr.xylfe.cn

TS:   static f(): void {}
来源：http://xim.mhx1999.top

Java: static void f() {}
来源：http://rtt.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cmh.ppjwa.cn

Ruby: def self.f; end
来源：http://abf.ydzc1.top

C#:   public static void F() {}
来源：http://yro.bjfxy.top

[G09] 接口 / 抽象类
来源：http://dwg.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://beb.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://tbi.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mps.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://tyn.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://bcr.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://lwd.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tff.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://kim.yangfankeji.com

[G10] 访问控制
来源：http://fqe.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://qlt.hcnkem.com

PHP:  public / protected / private
来源：http://oph.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://zfa.kuanghao11.cn

TS:   public / protected / private
来源：http://aoh.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://jei.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dbd.feifeiyinyue.top

Ruby: public / protected / private
来源：http://dsb.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://elj.meibo888.top

[G11] getter / setter
来源：http://lqo.andypj.xyz

Py:   @property 与 @x.setter
来源：http://fkq.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gkj.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://dxv.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://mqj.meibo888.top

Java: public String getName() { return name; }
来源：http://hni.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xjb.haohaochexian.top

Ruby: attr_accessor :name
来源：http://hng.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://bip.jqgfzy.top

[G12] 对象转字符串
来源：http://mwc.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://mqk.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mye.wangdashe.top

JS:   toString() { return this.name; }
来源：http://ldm.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://yzn.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://kda.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://isq.fengsongda.top

Ruby: def to_s; @name; end
来源：http://qbr.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://lkg.jyoumei.cn

[G13] 判断对象类型
来源：http://pdu.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://tht.zycfv.cn

PHP:  $u instanceof User
来源：http://whk.zhijiandao.cn

JS:   u instanceof User
来源：http://hci.hesvh.cn

TS:   u instanceof User
来源：http://fhe.xylfe.cn

Java: u instanceof User
来源：http://rom.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rka.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://nae.yj20258888.top

C#:   u is User
来源：http://yyz.chenjidiqi.icu

[G14] 数据类 / record
来源：http://dvk.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vmu.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://mtn.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cri.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://nty.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://aov.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://khe.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dex.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://mfi.ivvv.top

[G15] 枚举
来源：http://rhv.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rlc.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xfe.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vfj.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qvw.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://oia.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vsg.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://wli.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bto.yj202588.top

[G16] 对象转数组 / 字典
来源：http://yfh.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qbo.ivvv.top

PHP:  get_object_vars($obj);
来源：http://gvd.sweek.top

JS:   Object.entries(obj)
来源：http://ijf.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://kwb.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jno.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xfq.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://phe.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://thh.ybcxt.top

================================================================================
来源：http://fpl.hywenlv.cn

H. 异常与错误处理
来源：http://zxb.hongshengwenyu.top

================================================================================
来源：http://qtf.guannengcc.top

[H01] try / catch 基础
来源：http://wol.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fai.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fdw.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kjn.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ezk.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uto.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ebm.ehwqpu.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yqi.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iff.hnqzz.top

[H02] finally / ensure 收尾
来源：http://hmb.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://dxw.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uim.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://don.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mdn.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://atl.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://shl.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://slo.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nem.gogol.net.cn

[H03] 主动抛出异常
来源：http://aqa.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://qbl.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jdi.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://arw.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://vlm.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://moc.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jhx.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hjm.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bpm.jinqigufen.top

[H04] 自定义异常类型
来源：http://xug.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://qow.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://sqz.cashguo.top

JS:   class MyError extends Error {}
来源：http://ebo.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://kts.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://rqp.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kwg.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://iql.yongpay.top

C#:   class MyException : Exception {}
来源：http://dkm.sxryk.cn

[H05] 捕获特定类型
来源：http://tof.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://dtv.xylfe.cn


<!-- 参考信息 -->