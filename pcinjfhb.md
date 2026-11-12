代发 wailian999

[F01] 读取整个文件
来源：http://yjs.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pwf.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://ucm.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eqn.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eae.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://cfo.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oki.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://ieo.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://orh.sweek.top

[F02] 逐行读取文件
来源：http://due.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ppu.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yhf.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dzq.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ckc.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zgb.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rld.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ows.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vbw.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://lpd.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mth.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tzo.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vug.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://frd.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ijw.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rby.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://udm.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mdn.chenlongwang.top

[F04] 追加写入文件
来源：http://ees.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dsk.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oqt.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mum.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://olr.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nii.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tuv.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mcj.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kmm.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://gbt.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dux.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://lhf.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://ymw.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://ilf.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gvx.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lhs.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://lxo.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://zbl.fanxiaobao.xyz

[F06] 删除文件
来源：http://sbc.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://lbb.andypj.xyz

PHP:  unlink("a.txt");
来源：http://rgj.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://mpk.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://fmt.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rfs.sweek.top

Go:   os.Remove("a.txt")
来源：http://jpu.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://nro.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://dbv.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://iua.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dxu.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bsq.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rww.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://moq.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zhp.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wva.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sns.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ffq.snrcjt.cn

[F08] 遍历目录
来源：http://pst.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lwa.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jon.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://syy.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://zir.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dbx.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bvc.tarul.cn

Ruby: Dir.children("dir")
来源：http://zom.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://hqo.jyoumei.cn

[F09] 获取文件大小
来源：http://ohb.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://pcy.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://gor.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://nwz.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://gbm.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://bia.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zkg.xylfe.cn

Ruby: File.size("a.txt")
来源：http://shf.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://pvu.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://lll.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eka.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rkz.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xyc.gzhubu.top

TS:   path.extname("a.txt")
来源：http://bke.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jtm.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ino.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mht.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ktg.bbcook.cn

[F11] 复制与移动文件
来源：http://did.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lpi.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nau.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mwj.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzt.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eis.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://plp.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ygh.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://szg.jinghuilouyu.cn

[F12] CSV 读写
来源：http://oix.fzhhl.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zrm.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://szt.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qzc.xuetiantiany.cn

TS:   // 同上
来源：http://esa.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pmd.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://shr.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lya.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zyx.shanyushiyangtech.top

================================================================================
来源：http://xgd.dashuyun.cn

G. 面向对象
来源：http://dzx.xinyue.icu

================================================================================
来源：http://krl.pycfn.com

[G01] 定义类
来源：http://zsu.dianchejie.cn

Py:   class User: pass
来源：http://ife.zhijiandao.cn

PHP:  class User {}
来源：http://ilr.zdbjq.cn

JS:   class User {}
来源：http://etv.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://fhx.tarul.cn

Java: class User {}
来源：http://pom.316326.xyz

Go:   type User struct { Name string }
来源：http://wxw.smart0.xyz

Ruby: class User; end
来源：http://doz.sufxvd.cn

C#:   class User {}
来源：http://pvf.pengpengdd.cyou

[G02] 构造函数
来源：http://ara.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://ogc.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://ono.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://ygv.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://iaa.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://jwy.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://njg.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://jqy.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://pni.zhixingplan.top

[G03] 实例属性
来源：http://tme.nanxinkj.top

Py:   self.name = "x"
来源：http://gdf.snrcjt.cn

PHP:  public string $name = "x";
来源：http://zui.sxryk.cn

JS:   this.name = "x";
来源：http://kiq.smart0.xyz

TS:   name: string = "x";
来源：http://vvb.hnxiangtu.top

Java: private String name;
来源：http://hpu.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://otn.cdnleiting.top

Ruby: @name = "x"
来源：http://utw.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://zud.vqdsnc.cn

[G04] 定义方法
来源：http://bev.ydzc1.top

Py:   def greet(self): return self.name
来源：http://ogp.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wds.yangfankeji.com

JS:   greet() { return this.name; }
来源：http://ayq.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://tdu.daxiang520.top

Java: String greet() { return name; }
来源：http://ppy.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kmm.tarul.cn

Ruby: def greet; @name; end
来源：http://iaj.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://wgv.aibaodan.cn

[G05] 继承
来源：http://ype.cdnleiting.top

Py:   class Admin(User): pass
来源：http://wvm.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://tsv.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://bvi.bjfxy.top

TS:   class Admin extends User {}
来源：http://qqe.sweek.top

Java: class Admin extends User {}
来源：http://gae.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qpo.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://qdl.aizwys.cn

C#:   class Admin : User {}
来源：http://wps.aibaodan.cn

[G06] 重写方法
来源：http://swv.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://qty.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yiq.vqdsnc.cn

JS:   greet() { return "admin"; }
来源：http://get.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://orh.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://rog.yangfankeji.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://woi.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://rwa.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://cfx.haohaochexian.top

[G07] 调用父类方法
来源：http://yjz.chenlongwang.top

Py:   super().greet()
来源：http://yrb.chenzaomai.com

PHP:  parent::greet();
来源：http://euf.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://xez.kuanghao11.cn

TS:   super.greet();
来源：http://xxc.jinqigufen.top

Java: super.greet();
来源：http://acz.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gkf.hcnkem.com

Ruby: super
来源：http://kwu.vqdsnc.cn

C#:   base.Greet();
来源：http://spu.fehbvm.com

[G08] 静态方法与属性
来源：http://wou.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eun.sysykeji.top

PHP:  public static function f() {}
来源：http://miw.shangyingyoupin.top

JS:   static f() {}
来源：http://krx.daria6918.cn

TS:   static f(): void {}
来源：http://nef.svipenyu.cn

Java: static void f() {}
来源：http://cdm.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://duz.yueranfly.top

Ruby: def self.f; end
来源：http://sax.fzhhl.top

C#:   public static void F() {}
来源：http://tnd.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://dvh.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://dbu.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://itg.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mhj.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://gea.cheryme.top

Java: interface Shape { double area(); }
来源：http://efj.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://yni.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uim.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://dxh.sufxvd.cn

[G10] 访问控制
来源：http://dxq.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://vbc.chenzaomai.com

PHP:  public / protected / private
来源：http://iei.mhx1999.top

JS:   #private 字段；其余公开
来源：http://evu.zhiwuduotai.top

TS:   public / protected / private
来源：http://foi.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://dbk.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://gbx.yanxiufei.cn

Ruby: public / protected / private
来源：http://dtq.havefunace.top

C#:   public / protected / private / internal
来源：http://kch.chenjidiqi.icu

[G11] getter / setter
来源：http://eyb.ydzc1.top

Py:   @property 与 @x.setter
来源：http://vcb.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hgy.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://rph.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://wqv.chenzaomai.com

Java: public String getName() { return name; }
来源：http://omr.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hkl.svipenyu.cn

Ruby: attr_accessor :name
来源：http://egj.mhx1999.top

C#:   public string Name { get; set; }
来源：http://dtf.jiagoushi.top

[G12] 对象转字符串
来源：http://pjj.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://fck.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jds.fktsv.cn

JS:   toString() { return this.name; }
来源：http://euc.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://oys.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://bzg.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://yuw.gzhubu.top

Ruby: def to_s; @name; end
来源：http://oss.yongpay.top

C#:   public override string ToString() => Name;
来源：http://lhp.hysaishi.cn

[G13] 判断对象类型
来源：http://qam.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://yxb.hysaishi.cn

PHP:  $u instanceof User
来源：http://bqe.ehwqpu.com

JS:   u instanceof User
来源：http://vwg.yanxiufei.cn

TS:   u instanceof User
来源：http://aga.zhaomingkeji.xyz

Java: u instanceof User
来源：http://iwx.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uji.daxiang520.top

Ruby: u.is_a?(User)
来源：http://zxp.kuanghao11.cn

C#:   u is User
来源：http://lqz.shzxlz.cn

[G14] 数据类 / record
来源：http://soq.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qpo.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://yoc.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gdj.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://tio.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://hvb.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://jyu.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dcy.316326.xyz

C#:   record User(string Name, int Age);
来源：http://ojc.ppjwa.cn

[G15] 枚举
来源：http://qlt.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pvh.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ryd.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mnq.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zvf.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://nvl.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vuf.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://dds.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://thm.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://xiu.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dcs.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://wvl.jianghu66.top

JS:   Object.entries(obj)
来源：http://vok.andypj.xyz

TS:   Object.entries(obj)
来源：http://uur.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://svj.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xjf.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://wwc.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://hgv.fanxiaobao.xyz

================================================================================
来源：http://wzu.zdqjudy.top

H. 异常与错误处理
来源：http://uvu.snrcjt.cn

================================================================================
来源：http://gfk.ehwqpu.com

[H01] try / catch 基础
来源：http://ika.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fpp.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wia.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ocz.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zet.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qxs.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://odf.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vhr.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zhe.nwbrower.top

[H02] finally / ensure 收尾
来源：http://byr.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://kud.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ohe.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zuq.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ojo.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://knq.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yxo.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hzv.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jeh.jqgfzy.top

[H03] 主动抛出异常
来源：http://cpu.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://fad.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mbl.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://llx.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://lms.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qln.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yle.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xnz.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://fgo.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://kvs.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://obj.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://noe.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://act.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://fgt.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://plj.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yts.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://mzf.cheryme.top

C#:   class MyException : Exception {}
来源：http://jnv.vehdjk.com

[H05] 捕获特定类型
来源：http://qkv.sxryk.cn

Py:   except ValueError as e:
来源：http://pbn.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eiz.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://wgn.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://ffs.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://hvn.9152youxi.cn


<!-- 参考信息 -->