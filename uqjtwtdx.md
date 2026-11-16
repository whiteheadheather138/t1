代发 wailian999

[F01] 读取整个文件
来源：http://tgx.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://joe.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://gqs.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ogm.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xqe.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uyi.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kxc.xuanzx.com

Ruby: File.read("a.txt")
来源：http://tts.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://yla.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://oyv.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vxh.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rsk.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tty.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zbv.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sax.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mbs.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ufm.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nmf.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://pyg.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fne.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dfi.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fsh.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://znn.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ggw.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lca.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://zaq.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nci.hysaishi.cn

[F04] 追加写入文件
来源：http://jav.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zur.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lra.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ttl.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tca.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://veg.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vam.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dxc.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dhn.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://ysu.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jst.yongpay.top

PHP:  file_exists("a.txt");
来源：http://knh.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://fso.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://lec.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tna.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wkv.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://qgu.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://qji.pengpengdd.cyou

[F06] 删除文件
来源：http://try.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://nci.shuidangran.top

PHP:  unlink("a.txt");
来源：http://awo.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://cbe.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://uvj.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pnv.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://xjt.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://nxx.yongpay.top

C#:   File.Delete("a.txt");
来源：http://cpd.pycfn.com

[F07] 创建目录（含多级）
来源：http://lyo.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fuj.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yna.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aoj.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhg.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vqb.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dnr.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wiv.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oas.sweek.top

[F08] 遍历目录
来源：http://sja.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wsp.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://frt.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://lhz.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://vey.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rgf.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zsf.fktsv.cn

Ruby: Dir.children("dir")
来源：http://pjl.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://gbw.tianlin.xyz

[F09] 获取文件大小
来源：http://yxx.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://pfn.gzhubu.top

PHP:  filesize("a.txt");
来源：http://dvr.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://npj.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://bbj.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://ysq.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nkw.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://klw.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://ksn.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://ben.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ewe.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xvh.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ncy.ybcxt.top

TS:   path.extname("a.txt")
来源：http://hgw.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://trc.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gyg.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wlo.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eal.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://irf.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://asr.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://woc.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yax.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fvh.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gpz.wangdashe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yoc.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pqb.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kyp.gotoacloud.top

[F12] CSV 读写
来源：http://fsi.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://asu.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yzw.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mty.shanyushiyangtech.top

TS:   // 同上
来源：http://xws.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gdt.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://acv.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fia.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pme.svipenyu.cn

================================================================================
来源：http://khi.shanyushiyangtech.top

G. 面向对象
来源：http://cxs.quarkkingdee.top

================================================================================
来源：http://mdi.ydjk.org.cn

[G01] 定义类
来源：http://vyq.iojbl.cn

Py:   class User: pass
来源：http://zre.fzhhl.top

PHP:  class User {}
来源：http://nwy.yfazqb.com

JS:   class User {}
来源：http://vov.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://snz.yj20258888.top

Java: class User {}
来源：http://ret.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://vos.shangyingyoupin.top

Ruby: class User; end
来源：http://rhx.shangyingyoupin.top

C#:   class User {}
来源：http://mrg.fzhhl.top

[G02] 构造函数
来源：http://ooj.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://sqc.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://knm.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://zsr.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://vaz.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://nkd.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mxm.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://oyp.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://kyd.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://cft.snrcjt.cn

Py:   self.name = "x"
来源：http://xua.zdbjq.cn

PHP:  public string $name = "x";
来源：http://wzw.cucudq.cn

JS:   this.name = "x";
来源：http://qqf.bbcook.cn

TS:   name: string = "x";
来源：http://knu.52xcode.cn

Java: private String name;
来源：http://fzx.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qny.ydzc1.top

Ruby: @name = "x"
来源：http://egk.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://ghe.guannengcc.top

[G04] 定义方法
来源：http://puh.sweek.top

Py:   def greet(self): return self.name
来源：http://ees.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eie.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://xtj.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://hsn.quarkkingdee.top

Java: String greet() { return name; }
来源：http://wov.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pzz.9152youxi.cn

Ruby: def greet; @name; end
来源：http://wde.c1oappe.top

C#:   public string Greet() => Name;
来源：http://juo.ppjwa.cn

[G05] 继承
来源：http://uhh.guannengcc.top

Py:   class Admin(User): pass
来源：http://kyl.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://aav.9152youxi.cn

JS:   class Admin extends User {}
来源：http://uhi.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://ckp.cashguo.top

Java: class Admin extends User {}
来源：http://mgy.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://njd.9152youxi.cn

Ruby: class Admin < User; end
来源：http://clb.ppjwa.cn

C#:   class Admin : User {}
来源：http://sdh.birdmap.top

[G06] 重写方法
来源：http://owf.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://dyp.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rle.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://dnt.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://fsx.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://emp.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mfg.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://vzw.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://ffz.cqqwz.cn

[G07] 调用父类方法
来源：http://zco.yj202588.top

Py:   super().greet()
来源：http://pbc.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://yij.cashguo.top

JS:   super.greet();
来源：http://quu.gaohongyu789.top

TS:   super.greet();
来源：http://qxn.hnxiangtu.top

Java: super.greet();
来源：http://jww.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zpu.daxiang520.top

Ruby: super
来源：http://lpm.yfazqb.com

C#:   base.Greet();
来源：http://xpt.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://nnv.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mad.hesvh.cn

PHP:  public static function f() {}
来源：http://jbi.snrcjt.cn

JS:   static f() {}
来源：http://xjl.316326.xyz

TS:   static f(): void {}
来源：http://aeu.xinyue.icu

Java: static void f() {}
来源：http://myk.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xnp.wangshuangyany.cn

Ruby: def self.f; end
来源：http://otg.sxryk.cn

C#:   public static void F() {}
来源：http://fbm.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://cvx.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ttz.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://vbc.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pgr.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://rvh.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://ezi.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://daz.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uqi.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://hzd.tian-w.cn

[G10] 访问控制
来源：http://yhr.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://qgf.nwbrower.top

PHP:  public / protected / private
来源：http://fnp.xuanzx.com

JS:   #private 字段；其余公开
来源：http://cqb.ehwqpu.com

TS:   public / protected / private
来源：http://vvt.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://wka.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://awe.hfpthk.cn

Ruby: public / protected / private
来源：http://cdj.ehwqpu.com

C#:   public / protected / private / internal
来源：http://bfq.daria6918.cn

[G11] getter / setter
来源：http://plx.wangdashe.top

Py:   @property 与 @x.setter
来源：http://oav.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://doq.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://ymg.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://zdk.hammf.cn

Java: public String getName() { return name; }
来源：http://brw.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mfe.ybcxt.top

Ruby: attr_accessor :name
来源：http://jjg.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://ewk.cheryme.top

[G12] 对象转字符串
来源：http://hel.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://kxi.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nms.nwbrower.top

JS:   toString() { return this.name; }
来源：http://skv.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://rxc.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://zxj.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://lfu.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://roe.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://khx.jiagoushi.top

[G13] 判断对象类型
来源：http://qoj.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://zpy.daria6918.cn

PHP:  $u instanceof User
来源：http://qcg.yongpay.top

JS:   u instanceof User
来源：http://jmq.gzhubu.top

TS:   u instanceof User
来源：http://ggg.kuanghao11.cn

Java: u instanceof User
来源：http://cpg.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fti.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://axs.hesvh.cn

C#:   u is User
来源：http://kde.xinyue.icu

[G14] 数据类 / record
来源：http://gyl.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://opf.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://zxm.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://xxq.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://nhr.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://aqi.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://kay.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cew.yongpay.top

C#:   record User(string Name, int Age);
来源：http://pev.aibaodan.cn

[G15] 枚举
来源：http://bnb.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kvn.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fml.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fjn.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uud.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://wdx.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ohv.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://mqt.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blj.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://iri.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yuu.yongpay.top

PHP:  get_object_vars($obj);
来源：http://zbr.316326.xyz

JS:   Object.entries(obj)
来源：http://ljf.nwbrower.top

TS:   Object.entries(obj)
来源：http://xwy.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kez.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://olt.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://gzn.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://kqo.nwbrower.top

================================================================================
来源：http://htr.sweek.top

H. 异常与错误处理
来源：http://ect.shuidangran.top

================================================================================
来源：http://hyo.bjfxy.top

[H01] try / catch 基础
来源：http://djf.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ikb.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mwq.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wbe.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pxb.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ocu.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ycs.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eft.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eta.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://irs.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://ypu.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://laq.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rwv.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://niu.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://udc.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aei.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://gtj.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://twd.hysaishi.cn

[H03] 主动抛出异常
来源：http://wel.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://kut.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dkr.tanke756.top

JS:   throw new Error("错误信息");
来源：http://buk.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://nnz.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://acu.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gmq.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lms.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://wdu.zdqjudy.top

[H04] 自定义异常类型
来源：http://vil.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://zpc.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://kdx.yonumen.top

JS:   class MyError extends Error {}
来源：http://nuw.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://ipk.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://ivy.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rhh.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://buz.hcnkem.com

C#:   class MyException : Exception {}
来源：http://oim.vqdsnc.cn

[H05] 捕获特定类型
来源：http://vhz.uphjek.com

Py:   except ValueError as e:
来源：http://vus.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://stj.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://sfa.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://gzl.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://roq.birdmap.top


<!-- 参考信息 -->