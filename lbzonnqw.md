代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xhf.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://few.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://fys.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dun.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uba.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gjf.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nfm.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fpm.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://seo.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://gzp.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rxm.iojbl.cn

[F04] 追加写入文件
来源：http://nii.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mjl.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zlm.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xhj.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vwn.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wyb.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ltr.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ijr.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://shy.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://aov.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nmx.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://xxb.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://uyi.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://gjr.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://was.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yop.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://gec.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://qpo.hfpthk.cn

[F06] 删除文件
来源：http://wmb.yueranfly.top

Py:   os.remove("a.txt")
来源：http://vzu.xuanzx.com

PHP:  unlink("a.txt");
来源：http://mmr.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://tqo.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://gfn.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ago.cheryme.top

Go:   os.Remove("a.txt")
来源：http://atq.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://ihl.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://lww.andypj.xyz

[F07] 创建目录（含多级）
来源：http://otc.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ezh.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cst.9152youxi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sem.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jcb.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uji.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lun.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vbp.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lzo.vehdjk.com

[F08] 遍历目录
来源：http://htw.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://efk.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vup.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://lue.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://hjm.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rwa.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pqk.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://ajg.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://tku.zhoulong.xyz

[F09] 获取文件大小
来源：http://yzw.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://nqc.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://ocr.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://mul.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://kww.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://son.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ths.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://vxs.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://zdr.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://xsh.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ser.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jmm.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zya.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://ohe.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yhv.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ffs.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ufr.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kxa.0kj1m.cn

[F11] 复制与移动文件
来源：http://bpt.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ohz.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oat.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oep.fengsongda.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qaj.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wjf.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ttg.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rzk.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wjt.chenjidiqi.icu

[F12] CSV 读写
来源：http://qho.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qfs.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ejl.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bbd.shangyingyoupin.top

TS:   // 同上
来源：http://ctt.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://viz.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cfe.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mxf.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qju.hfpthk.cn

================================================================================
来源：http://wfw.yuxming.cn

G. 面向对象
来源：http://axi.xuetiantiany.cn

================================================================================
来源：http://xet.zdqjudy.top

[G01] 定义类
来源：http://zwq.shzxlz.cn

Py:   class User: pass
来源：http://qqf.meibo888.top

PHP:  class User {}
来源：http://duf.yanxiufei.cn

JS:   class User {}
来源：http://sqb.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://lvc.dianchejie.cn

Java: class User {}
来源：http://kyg.ctjpmb.com

Go:   type User struct { Name string }
来源：http://irs.hnqzz.top

Ruby: class User; end
来源：http://tkj.hfpthk.cn

C#:   class User {}
来源：http://pvk.xylfe.cn

[G02] 构造函数
来源：http://mjd.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://jrv.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://gjs.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://hwp.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://hkg.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://bdu.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cos.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://pfo.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://dyh.dashuyun.cn

[G03] 实例属性
来源：http://mme.xziqi.cn

Py:   self.name = "x"
来源：http://bdx.xylfe.cn

PHP:  public string $name = "x";
来源：http://dbq.hysaishi.cn

JS:   this.name = "x";
来源：http://nzj.ybcxt.top

TS:   name: string = "x";
来源：http://szr.ydjk.org.cn

Java: private String name;
来源：http://wyw.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wbj.feifeiyinyue.top

Ruby: @name = "x"
来源：http://zns.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://vyg.ywan-chungtsiang.top

[G04] 定义方法
来源：http://yqt.iojbl.cn

Py:   def greet(self): return self.name
来源：http://txa.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mfx.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://jkf.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://czy.fengsongda.top

Java: String greet() { return name; }
来源：http://ylg.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mbp.jinqigufen.top

Ruby: def greet; @name; end
来源：http://uog.aizwys.cn

C#:   public string Greet() => Name;
来源：http://ldd.svipenyu.cn

[G05] 继承
来源：http://oua.9152youxi.cn

Py:   class Admin(User): pass
来源：http://iwk.52xcode.cn

PHP:  class Admin extends User {}
来源：http://vyk.yfazqb.com

JS:   class Admin extends User {}
来源：http://ack.cucudq.cn

TS:   class Admin extends User {}
来源：http://drl.kuanghao11.cn

Java: class Admin extends User {}
来源：http://swd.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mta.uphjek.com

Ruby: class Admin < User; end
来源：http://iio.52xcode.cn

C#:   class Admin : User {}
来源：http://xem.shuidangran.top

[G06] 重写方法
来源：http://ojd.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://uys.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://psn.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://neg.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://vgs.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://npj.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wwd.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://bwe.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://pig.mhx1999.top

[G07] 调用父类方法
来源：http://cpw.xuanzx.com

Py:   super().greet()
来源：http://jqd.tarul.cn

PHP:  parent::greet();
来源：http://vpr.yanxiufei.cn

JS:   super.greet();
来源：http://ezy.zhijiandao.cn

TS:   super.greet();
来源：http://sjr.guannengcc.top

Java: super.greet();
来源：http://vit.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hwl.cdnleiting.top

Ruby: super
来源：http://lar.ydzc1.top

C#:   base.Greet();
来源：http://qgg.yuanzhike.top

[G08] 静态方法与属性
来源：http://tbl.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ucr.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://xli.quarkkingdee.top

JS:   static f() {}
来源：http://xxq.birdmap.top

TS:   static f(): void {}
来源：http://wsu.zhaomingkeji.xyz

Java: static void f() {}
来源：http://phq.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wib.jinqigfzy.top

Ruby: def self.f; end
来源：http://tqd.haohaochexian.top

C#:   public static void F() {}
来源：http://nec.wangdashe.top

[G09] 接口 / 抽象类
来源：http://flk.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://wwr.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://yih.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fxw.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://ewm.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://ntk.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://dou.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vfk.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://etk.gaohongyu789.top

[G10] 访问控制
来源：http://ody.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://ity.ydjk.org.cn

PHP:  public / protected / private
来源：http://oyh.bjfxy.top

JS:   #private 字段；其余公开
来源：http://vea.fzhhl.top

TS:   public / protected / private
来源：http://iwz.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://xep.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xyk.nanxinkj.top

Ruby: public / protected / private
来源：http://lvz.smart0.xyz

C#:   public / protected / private / internal
来源：http://gna.kuanghao11.cn

[G11] getter / setter
来源：http://yil.fktsv.cn

Py:   @property 与 @x.setter
来源：http://flf.shangyingyoupin.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pyg.yj202588.top

JS:   get name() { return this._name; }
来源：http://usm.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://bwf.0kj1m.cn

Java: public String getName() { return name; }
来源：http://gxz.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://npp.jianghu66.top

Ruby: attr_accessor :name
来源：http://ppu.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://ekw.pycfn.com

[G12] 对象转字符串
来源：http://aep.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://mqr.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eqr.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://taj.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://ykc.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://yvm.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ywq.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://kyj.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://lhj.316326.xyz

[G13] 判断对象类型
来源：http://drt.sweek.top

Py:   isinstance(u, User)
来源：http://vtq.yfazqb.com

PHP:  $u instanceof User
来源：http://bqi.xziqi.cn

JS:   u instanceof User
来源：http://ykz.guowangkeji.top

TS:   u instanceof User
来源：http://tci.yonumen.top

Java: u instanceof User
来源：http://bzm.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oxb.jianghu66.top

Ruby: u.is_a?(User)
来源：http://wpu.zhongyouzk.top

C#:   u is User
来源：http://pmq.havefunace.top

[G14] 数据类 / record
来源：http://gub.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gnr.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://quw.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://cml.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://csw.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://qhl.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://yki.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hgh.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://aom.yanxiufei.cn

[G15] 枚举
来源：http://zmr.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://drk.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ffs.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dgu.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xqh.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://rex.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vud.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://qpq.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kqc.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://nqp.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zut.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://gte.hfpthk.cn

JS:   Object.entries(obj)
来源：http://lht.jinqigufen.top

TS:   Object.entries(obj)
来源：http://wxj.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rcu.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://msk.9152youxi.cn

Ruby: obj.instance_variables
来源：http://piw.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://iqq.yonumen.top

================================================================================
来源：http://egw.jqgfzy.top

H. 异常与错误处理
来源：http://ywe.xuetiantiany.cn

================================================================================
来源：http://kqu.pycfn.com

[H01] try / catch 基础
来源：http://dpt.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://edf.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://man.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mcs.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iqd.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rpw.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oyk.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://spy.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qqr.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://gpx.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://zoz.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lof.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sfg.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vey.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dof.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://jqo.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hjo.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qqs.sufxvd.cn

[H03] 主动抛出异常
来源：http://ide.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://ilw.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mpo.yonumen.top

JS:   throw new Error("错误信息");
来源：http://ogx.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://wba.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lgb.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wia.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ygw.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://ntw.chenzaomai.com

[H04] 自定义异常类型
来源：http://aio.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://fpb.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://rnv.cashguo.top

JS:   class MyError extends Error {}
来源：http://ask.epnwcf.com

TS:   class MyError extends Error {}
来源：http://eiz.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://vzx.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dij.sweek.top

Ruby: class MyError < StandardError; end
来源：http://got.tian-w.cn

C#:   class MyException : Exception {}
来源：http://viz.yuxming.cn

[H05] 捕获特定类型
来源：http://xll.tanke756.top

Py:   except ValueError as e:
来源：http://poy.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ffi.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://mxc.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://ilb.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://bmc.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ezv.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://cou.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kxe.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://pll.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://jbu.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://fhd.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wcv.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://slx.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zzg.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fag.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://bgz.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://cqv.xuanzx.com

[H07] 断言
来源：http://jyf.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://yka.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://gvn.yongpay.top

JS:   console.assert(x > 0);
来源：http://eoo.chenlongwang.top


<!-- 参考信息 -->