代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bba.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://jin.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ait.sufxvd.cn

[F04] 追加写入文件
来源：http://mob.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xei.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xsi.yuanzhike.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://skq.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mic.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kwb.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://myi.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hon.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sbp.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://iza.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ofi.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://rlh.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://qnp.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://oja.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://gfk.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mtc.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://xpa.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://pid.xuanzx.com

[F06] 删除文件
来源：http://nce.meibo888.top

Py:   os.remove("a.txt")
来源：http://adh.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://arn.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://vmr.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://bwb.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://scn.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://ocu.yonumen.top

Ruby: File.delete("a.txt")
来源：http://gwe.birdmap.top

C#:   File.Delete("a.txt");
来源：http://sim.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://ajh.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://skt.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mtm.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mcu.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jdp.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ujt.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dwe.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lfv.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ixa.bjfxy.top

[F08] 遍历目录
来源：http://aan.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wnc.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ilk.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://wjy.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://hmu.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mly.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://uct.cucudq.cn

Ruby: Dir.children("dir")
来源：http://tkx.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://ajf.gogol.net.cn

[F09] 获取文件大小
来源：http://uqc.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://vci.tanke756.top

PHP:  filesize("a.txt");
来源：http://upw.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://pms.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://zmu.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://txw.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rnh.uphjek.com

Ruby: File.size("a.txt")
来源：http://vfl.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://del.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://lxn.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wkd.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lwm.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uby.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://tmy.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qww.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ljz.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://enu.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iuz.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://isf.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://loh.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nws.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://noa.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iib.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ffk.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qrn.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nws.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cyv.cdnleiting.top

[F12] CSV 读写
来源：http://our.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://syc.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dzw.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pqs.shanyushiyangkeji.top

TS:   // 同上
来源：http://lry.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fcs.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://efx.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yup.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kwq.shuidangran.top

================================================================================
来源：http://lvs.zycfv.cn

G. 面向对象
来源：http://yzt.fehbvm.com

================================================================================
来源：http://bsm.xingfuxueyuan.xyz

[G01] 定义类
来源：http://fci.iojbl.cn

Py:   class User: pass
来源：http://umd.316326.xyz

PHP:  class User {}
来源：http://gyt.quarkkingdee.top

JS:   class User {}
来源：http://gyh.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://pen.hnqzz.top

Java: class User {}
来源：http://vnl.zycfv.cn

Go:   type User struct { Name string }
来源：http://unm.hysaishi.cn

Ruby: class User; end
来源：http://war.hcnkem.com

C#:   class User {}
来源：http://ktt.meibo888.top

[G02] 构造函数
来源：http://zlr.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://zxz.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://whs.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://tzf.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://ous.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://pcg.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zgi.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://abl.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://hnq.zhoulong.xyz

[G03] 实例属性
来源：http://way.cheryme.top

Py:   self.name = "x"
来源：http://acv.hesvh.cn

PHP:  public string $name = "x";
来源：http://aul.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://zcb.yanxiufei.cn

TS:   name: string = "x";
来源：http://jwk.nanxinkj.top

Java: private String name;
来源：http://mlq.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bgk.uphjek.com

Ruby: @name = "x"
来源：http://eup.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://fax.ydzc1.top

[G04] 定义方法
来源：http://abt.cucudq.cn

Py:   def greet(self): return self.name
来源：http://uyd.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://boy.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://bsz.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://irn.dashuyun.cn

Java: String greet() { return name; }
来源：http://fip.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kzs.0kj1m.cn

Ruby: def greet; @name; end
来源：http://rlf.sweek.top

C#:   public string Greet() => Name;
来源：http://nmv.52xcode.cn

[G05] 继承
来源：http://rpg.gzhubu.top

Py:   class Admin(User): pass
来源：http://oxk.yj20258.top

PHP:  class Admin extends User {}
来源：http://bmu.gogol.net.cn

JS:   class Admin extends User {}
来源：http://eda.gogol.net.cn

TS:   class Admin extends User {}
来源：http://rfy.vehdjk.com

Java: class Admin extends User {}
来源：http://bto.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ijr.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://rvo.cqqwz.cn

C#:   class Admin : User {}
来源：http://mip.gogol.net.cn

[G06] 重写方法
来源：http://lxh.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://mqo.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://zhk.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://zch.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://dyk.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://wmv.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aiz.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://pul.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://rae.yfazqb.com

[G07] 调用父类方法
来源：http://cqt.dashuyun.cn

Py:   super().greet()
来源：http://ilf.zhiwuduotai.top

PHP:  parent::greet();
来源：http://qjj.gotoacloud.top

JS:   super.greet();
来源：http://grf.dianchejie.cn

TS:   super.greet();
来源：http://qoj.iojbl.cn

Java: super.greet();
来源：http://dqw.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nqw.sweek.top

Ruby: super
来源：http://iaw.sweek.top

C#:   base.Greet();
来源：http://ink.nanxuanxn.top

[G08] 静态方法与属性
来源：http://luh.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bug.0kj1m.cn

PHP:  public static function f() {}
来源：http://pbw.ywan-chungtsiang.top

JS:   static f() {}
来源：http://vpe.andypj.xyz

TS:   static f(): void {}
来源：http://haq.zhixingplan.top

Java: static void f() {}
来源：http://lrr.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://bxw.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://hmb.sufxvd.cn

C#:   public static void F() {}
来源：http://szl.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://jfv.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://iei.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://ztk.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xwt.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://tnv.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://qos.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://wkv.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xmj.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://hhp.shuidangran.top

[G10] 访问控制
来源：http://lkv.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://hsl.zhoulong.xyz

PHP:  public / protected / private
来源：http://hhk.bjfxy.top

JS:   #private 字段；其余公开
来源：http://sro.kuanghao11.cn

TS:   public / protected / private
来源：http://qzu.316326.xyz

Java: public / protected / private / 默认包级
来源：http://djk.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tbw.sweek.top

Ruby: public / protected / private
来源：http://gxx.hfpthk.cn

C#:   public / protected / private / internal
来源：http://ddb.yueranfly.top

[G11] getter / setter
来源：http://wym.mhx1999.top

Py:   @property 与 @x.setter
来源：http://aqz.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cgb.xziqi.cn

JS:   get name() { return this._name; }
来源：http://tka.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://dla.zhixingplan.top

Java: public String getName() { return name; }
来源：http://ujm.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mtf.ehwqpu.com

Ruby: attr_accessor :name
来源：http://vyi.tianlin.xyz

C#:   public string Name { get; set; }
来源：http://hqk.quarkkingdee.top

[G12] 对象转字符串
来源：http://acr.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://huv.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kvx.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://nhd.vqdsnc.cn

TS:   toString(): string { return this.name; }
来源：http://anm.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://uqr.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://umc.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://fno.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://xug.yfazqb.com

[G13] 判断对象类型
来源：http://ryh.fzhhl.top

Py:   isinstance(u, User)
来源：http://fks.andypj.xyz

PHP:  $u instanceof User
来源：http://pvz.hysaishi.cn

JS:   u instanceof User
来源：http://xqm.sxryk.cn

TS:   u instanceof User
来源：http://fuk.chenlongwang.top

Java: u instanceof User
来源：http://lun.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xbz.bbcook.cn

Ruby: u.is_a?(User)
来源：http://czl.yj202588.top

C#:   u is User
来源：http://yyb.aizwys.cn

[G14] 数据类 / record
来源：http://ybf.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ykx.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://pkd.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://aqt.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://mok.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://rgb.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://izg.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fqy.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://vkw.quarkkingdee.top

[G15] 枚举
来源：http://lta.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mor.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qod.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lgn.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wrl.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://qzx.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gmx.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://nmi.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bya.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://ukl.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nfr.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://lrw.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://jbq.xinyue.icu

TS:   Object.entries(obj)
来源：http://vns.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nyx.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://swa.ppjwa.cn

Ruby: obj.instance_variables
来源：http://idn.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://hps.ivvv.top

================================================================================
来源：http://ajc.ydjk.org.cn

H. 异常与错误处理
来源：http://wdt.aibaodan.cn

================================================================================
来源：http://bbp.hfpthk.cn

[H01] try / catch 基础
来源：http://zwc.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mjx.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dlc.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ijz.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eyb.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwu.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jom.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mpf.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eqd.yvedp.cn

[H02] finally / ensure 收尾
来源：http://jcr.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jxk.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://xar.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kgd.shangyingyoupin.top

TS:   try { f(); } finally { cleanup(); }
来源：http://khe.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://pkg.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sza.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uuy.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hds.havefunace.top

[H03] 主动抛出异常
来源：http://jvq.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://lyz.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tku.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://zpe.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://klg.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ukp.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oia.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://scr.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gzb.hammf.cn

[H04] 自定义异常类型
来源：http://bsa.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://evr.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dsx.bjfxy.top

JS:   class MyError extends Error {}
来源：http://kee.yj20258888.top

TS:   class MyError extends Error {}
来源：http://wlc.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://dnh.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rjy.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://cip.shuidangran.top

C#:   class MyException : Exception {}
来源：http://yxx.iojbl.cn

[H05] 捕获特定类型
来源：http://rmw.shuidangran.top

Py:   except ValueError as e:
来源：http://tqs.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ogs.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://kho.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://npc.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://xhr.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uyd.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://ast.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://znc.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://jkq.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://fou.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://mrn.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://snh.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uka.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://buo.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ymd.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://kap.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://muh.dashuyun.cn

[H07] 断言
来源：http://ets.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://wbc.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://pda.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://gxd.redwolf501.top

TS:   console.assert(x > 0);
来源：http://juy.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://iqo.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wzr.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lqg.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://ayd.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://eih.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://wpg.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vfa.gaohongyu789.top


<!-- 参考信息 -->