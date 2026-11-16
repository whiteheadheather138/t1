代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://syf.xuanzx.com

================================================================================
来源：http://cyp.zycfv.cn

F. 文件与目录
来源：http://uqy.tanke756.top

================================================================================
来源：http://sdn.zhengqikj.top

[F01] 读取整个文件
来源：http://flx.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iiy.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://dgv.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wuw.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://irs.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xzb.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ayh.andypj.xyz

Ruby: File.read("a.txt")
来源：http://hrh.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://nzy.yuanzhike.top

[F02] 逐行读取文件
来源：http://wif.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pcs.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ixv.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://puc.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xfs.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://toh.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://urg.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://imy.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://riv.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://zog.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ubj.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zvr.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rih.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cev.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kxm.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jha.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://llt.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bsw.ppjwa.cn

[F04] 追加写入文件
来源：http://fqy.tanke756.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mkn.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wtn.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpj.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vhj.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yjw.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ffv.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://amx.sjlbkw.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jmo.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://zvi.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vqh.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://wln.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://otk.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://cvn.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hav.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://muo.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://qhp.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://wwp.0kj1m.cn

[F06] 删除文件
来源：http://vwr.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://qlh.birdmap.top

PHP:  unlink("a.txt");
来源：http://kog.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://llp.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gyj.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kpm.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://cxc.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://zfw.ivvv.top

C#:   File.Delete("a.txt");
来源：http://aci.c1oappe.top

[F07] 创建目录（含多级）
来源：http://uba.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cxo.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pno.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbo.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ftv.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://opn.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gkh.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jee.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mzh.fehbvm.com

[F08] 遍历目录
来源：http://nkc.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bfh.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://joi.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://dsc.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://vxv.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kjy.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tkb.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://kjw.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://vml.meibo888.top

[F09] 获取文件大小
来源：http://czm.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://zna.ydzc1.top

PHP:  filesize("a.txt");
来源：http://xwj.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://hrh.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://ktb.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://fgx.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hay.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://ihg.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://cli.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://jki.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ryf.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://prw.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gbb.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://wat.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://apr.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oew.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qta.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xka.mhx1999.top

[F11] 复制与移动文件
来源：http://wdr.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yrq.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uzc.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmw.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mql.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mau.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dzq.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gui.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oxo.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://uss.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://olb.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cou.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qcf.pengpengdd.cyou

TS:   // 同上
来源：http://kaw.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mva.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qhm.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kpi.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://evo.yonumen.top

================================================================================
来源：http://svs.havefunace.top

G. 面向对象
来源：http://hgp.tanke756.top

================================================================================
来源：http://tgl.cqqwz.cn

[G01] 定义类
来源：http://mue.zhengqikj.top

Py:   class User: pass
来源：http://ghv.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://hel.fktsv.cn

JS:   class User {}
来源：http://hsq.uphjek.com

TS:   class User { name: string = ""; }
来源：http://mzk.jlsjyb.cn

Java: class User {}
来源：http://uzm.fktsv.cn

Go:   type User struct { Name string }
来源：http://hxs.jinyuanbaomall.cn

Ruby: class User; end
来源：http://lhk.jlsjyb.cn

C#:   class User {}
来源：http://muv.yonumen.top

[G02] 构造函数
来源：http://ddc.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://blj.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://ynm.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://oar.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://xof.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://vbh.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://giu.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://znv.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://iyy.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://tur.fzhhl.top

Py:   self.name = "x"
来源：http://nge.cdnleiting.top

PHP:  public string $name = "x";
来源：http://uxi.sufxvd.cn

JS:   this.name = "x";
来源：http://gbx.0kj1m.cn

TS:   name: string = "x";
来源：http://lrg.wangshuangyany.cn

Java: private String name;
来源：http://azi.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gag.quarkkingdee.top

Ruby: @name = "x"
来源：http://lsb.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://ect.chenlongwang.top

[G04] 定义方法
来源：http://acy.sweek.top

Py:   def greet(self): return self.name
来源：http://obo.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://idh.yj20258888.top

JS:   greet() { return this.name; }
来源：http://qkz.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://lsm.smart0.xyz

Java: String greet() { return name; }
来源：http://xhi.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dsg.chenzaomai.com

Ruby: def greet; @name; end
来源：http://qqm.iojbl.cn

C#:   public string Greet() => Name;
来源：http://nhj.mhx1999.top

[G05] 继承
来源：http://kwj.iojbl.cn

Py:   class Admin(User): pass
来源：http://zjn.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://hzw.jianghu66.top

JS:   class Admin extends User {}
来源：http://atl.cucudq.cn

TS:   class Admin extends User {}
来源：http://vqo.andypj.xyz

Java: class Admin extends User {}
来源：http://iog.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ltv.shzxlz.cn

Ruby: class Admin < User; end
来源：http://ond.nanxuanxn.top

C#:   class Admin : User {}
来源：http://dke.xinyue.icu

[G06] 重写方法
来源：http://pxs.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://dou.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hbp.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://srg.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://sct.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://uxm.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zyj.meibo888.top

Ruby: def greet; "admin"; end
来源：http://ppk.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://kyv.gotoacloud.top

[G07] 调用父类方法
来源：http://hot.aizwys.cn

Py:   super().greet()
来源：http://bys.epnwcf.com

PHP:  parent::greet();
来源：http://zdi.cashguo.top

JS:   super.greet();
来源：http://ale.guannengcc.top

TS:   super.greet();
来源：http://pej.gotoacloud.top

Java: super.greet();
来源：http://tjn.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cyr.feifeiyinyue.top

Ruby: super
来源：http://orb.shuidangran.top

C#:   base.Greet();
来源：http://yns.zhengqikj.top

[G08] 静态方法与属性
来源：http://hfh.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ynb.hesvh.cn

PHP:  public static function f() {}
来源：http://llv.yuanzhike.top

JS:   static f() {}
来源：http://con.ehwqpu.com

TS:   static f(): void {}
来源：http://zwb.svipenyu.cn

Java: static void f() {}
来源：http://jtl.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fzu.shzxlz.cn

Ruby: def self.f; end
来源：http://vpl.jiagoushi.top

C#:   public static void F() {}
来源：http://ftp.hammf.cn

[G09] 接口 / 抽象类
来源：http://sfn.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://hep.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dfl.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://mso.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://rym.sweek.top

Java: interface Shape { double area(); }
来源：http://emc.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://noz.hammf.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lwx.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://aaw.chenlongwang.top

[G10] 访问控制
来源：http://zlv.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://rvt.pycfn.com

PHP:  public / protected / private
来源：http://cza.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://gml.ydzc1.top

TS:   public / protected / private
来源：http://bpa.tanke756.top

Java: public / protected / private / 默认包级
来源：http://ove.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://btc.vqdsnc.cn

Ruby: public / protected / private
来源：http://lpu.cheryme.top

C#:   public / protected / private / internal
来源：http://kfd.c1oappe.top

[G11] getter / setter
来源：http://rax.smart0.xyz

Py:   @property 与 @x.setter
来源：http://ijt.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qcc.bbcook.cn

JS:   get name() { return this._name; }
来源：http://zdn.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://ric.gotoacloud.top

Java: public String getName() { return name; }
来源：http://ovg.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://tek.redwolf501.top

Ruby: attr_accessor :name
来源：http://gky.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://zvm.nanxuanxn.top

[G12] 对象转字符串
来源：http://tvm.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://yra.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qwn.aizwys.cn

JS:   toString() { return this.name; }
来源：http://bak.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://yei.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://xtj.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tgq.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://oda.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://vus.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://vdj.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://ldh.jyoumei.cn

PHP:  $u instanceof User
来源：http://wmd.zhengqikj.top

JS:   u instanceof User
来源：http://ghg.pengpengdd.cyou

TS:   u instanceof User
来源：http://fjg.fanxiaobao.xyz

Java: u instanceof User
来源：http://lep.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://byw.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://ild.guowangkeji.top

C#:   u is User
来源：http://cop.vehdjk.com

[G14] 数据类 / record
来源：http://hwq.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nwd.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://rsa.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://xrd.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://uml.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://eai.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://eew.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hro.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://jgc.shzxlz.cn

[G15] 枚举
来源：http://txe.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pmx.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qkh.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nqn.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bcb.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://xyv.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hjp.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://hgv.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qbb.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://lme.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kli.andypj.xyz

PHP:  get_object_vars($obj);
来源：http://bgw.fktsv.cn

JS:   Object.entries(obj)
来源：http://jbb.sweek.top

TS:   Object.entries(obj)
来源：http://hnv.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zwe.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xmk.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://yau.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://jfk.jlsjyb.cn

================================================================================
来源：http://iqc.xuanzx.com

H. 异常与错误处理
来源：http://yjz.sufxvd.cn

================================================================================
来源：http://lbi.svipenyu.cn

[H01] try / catch 基础
来源：http://ffc.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gni.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rbl.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cih.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pmg.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mwa.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dmx.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lft.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ozx.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://qhb.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://byt.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://oaq.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://meg.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://koc.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://jiw.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ysa.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vul.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dqt.svipenyu.cn

[H03] 主动抛出异常
来源：http://qbg.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://pzt.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qpw.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://hel.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://uob.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uqd.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xco.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://snb.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://bav.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://qph.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://qus.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://twy.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://udb.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://lux.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://non.guowangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vqh.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://snm.redwolf501.top

C#:   class MyException : Exception {}
来源：http://ykj.guannengcc.top

[H05] 捕获特定类型
来源：http://vds.mhx1999.top

Py:   except ValueError as e:
来源：http://bkz.hongshengwenyu.top


<!-- 参考信息 -->