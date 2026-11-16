代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://erd.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://vfb.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://shq.jinqigufen.top

[F04] 追加写入文件
来源：http://cka.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://att.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://utr.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blk.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpi.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zxo.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ozg.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mhr.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kzt.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://nis.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kpa.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://uim.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://vzn.yvedp.cn

TS:   fs.existsSync("a.txt")
来源：http://ush.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://byd.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lzm.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://ldr.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://run.sxryk.cn

[F06] 删除文件
来源：http://fke.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://yil.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://ukv.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dvs.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ill.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xkw.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://kpf.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://fbs.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://opn.ybcxt.top

[F07] 创建目录（含多级）
来源：http://wxq.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eqw.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vtg.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rrz.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xcb.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zvy.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iab.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ukw.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ihe.vehdjk.com

[F08] 遍历目录
来源：http://ppw.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eoi.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zir.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://awr.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://pxa.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ypr.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://lkt.xinyue.icu

Ruby: Dir.children("dir")
来源：http://vxn.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://hqn.pycfn.com

[F09] 获取文件大小
来源：http://zkw.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://lqg.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://vpq.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://elg.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://uvt.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://emg.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mbj.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://fcy.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://bsn.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://cud.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rfc.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vzh.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xvt.yonumen.top

TS:   path.extname("a.txt")
来源：http://tlr.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gga.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nqb.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bgi.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://quq.shuidangran.top

[F11] 复制与移动文件
来源：http://bqo.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://scu.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eiq.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fsb.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://row.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yld.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aet.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qqc.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fhl.sysykeji.top

[F12] CSV 读写
来源：http://eal.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kfr.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://awq.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://clz.tanke756.top

TS:   // 同上
来源：http://mtk.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qil.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cii.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://weh.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cyg.vqdsnc.cn

================================================================================
来源：http://rgk.jinqigufen.top

G. 面向对象
来源：http://zje.hammf.cn

================================================================================
来源：http://uhi.yfazqb.com

[G01] 定义类
来源：http://etq.jiagoushi.top

Py:   class User: pass
来源：http://ovm.zhiwuduotai.top

PHP:  class User {}
来源：http://zvp.jinghuilouyu.cn

JS:   class User {}
来源：http://qea.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://lfd.yfazqb.com

Java: class User {}
来源：http://jmz.cucudq.cn

Go:   type User struct { Name string }
来源：http://gae.kuanghao11.cn

Ruby: class User; end
来源：http://vlq.dashuyun.cn

C#:   class User {}
来源：http://qft.pengpengdd.cyou

[G02] 构造函数
来源：http://ezl.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://mxf.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://dgh.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://cqb.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://hhy.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://roz.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://anj.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://bct.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://jxz.shangyingyoupin.top

[G03] 实例属性
来源：http://qiw.gaohongyu789.top

Py:   self.name = "x"
来源：http://qwv.hammf.cn

PHP:  public string $name = "x";
来源：http://xzr.ctjpmb.com

JS:   this.name = "x";
来源：http://rfu.cashguo.top

TS:   name: string = "x";
来源：http://qje.ybcxt.top

Java: private String name;
来源：http://kcs.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ehs.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://qgj.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://mre.zhaomingkeji.xyz

[G04] 定义方法
来源：http://jhp.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://nry.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dpo.shuidangran.top

JS:   greet() { return this.name; }
来源：http://zpd.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://owy.ybcxt.top

Java: String greet() { return name; }
来源：http://xbr.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uzp.nanxinkj.top

Ruby: def greet; @name; end
来源：http://kma.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://hos.ctjpmb.com

[G05] 继承
来源：http://mau.xylfe.cn

Py:   class Admin(User): pass
来源：http://luz.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://mfa.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://txj.smart0.xyz

TS:   class Admin extends User {}
来源：http://omq.hnqzz.top

Java: class Admin extends User {}
来源：http://sgs.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bbs.chenlongwang.top

Ruby: class Admin < User; end
来源：http://hzf.wangdashe.top

C#:   class Admin : User {}
来源：http://hlt.wangshuangyany.cn

[G06] 重写方法
来源：http://mmm.havefunace.top

Py:   def greet(self): return "admin"
来源：http://cvo.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oib.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://haf.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://mpj.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://ssn.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://czs.yonumen.top

Ruby: def greet; "admin"; end
来源：http://uct.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://cux.bjfxy.top

[G07] 调用父类方法
来源：http://chq.52xcode.cn

Py:   super().greet()
来源：http://ixk.jqgfzy.top

PHP:  parent::greet();
来源：http://zeh.vehdjk.com

JS:   super.greet();
来源：http://ahp.yangfankeji.com

TS:   super.greet();
来源：http://qle.ydzc1.top

Java: super.greet();
来源：http://gip.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aso.316326.xyz

Ruby: super
来源：http://bnd.gotoacloud.top

C#:   base.Greet();
来源：http://sji.xylfe.cn

[G08] 静态方法与属性
来源：http://saf.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vik.0kj1m.cn

PHP:  public static function f() {}
来源：http://lhv.jianghu66.top

JS:   static f() {}
来源：http://fhb.hysaishi.cn

TS:   static f(): void {}
来源：http://rel.zhixingplan.top

Java: static void f() {}
来源：http://lcw.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vam.yj20258.top

Ruby: def self.f; end
来源：http://peo.yj20258888.top

C#:   public static void F() {}
来源：http://qsc.epnwcf.com

[G09] 接口 / 抽象类
来源：http://kph.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://lii.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://idp.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gow.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://hal.yvedp.cn

Java: interface Shape { double area(); }
来源：http://rvf.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://cnn.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ezu.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://bem.zhijiandao.cn

[G10] 访问控制
来源：http://wue.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://etu.jqgufenzy.top

PHP:  public / protected / private
来源：http://gtj.yongpay.top

JS:   #private 字段；其余公开
来源：http://whq.hammf.cn

TS:   public / protected / private
来源：http://zsl.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://kez.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bqr.guannengcc.top

Ruby: public / protected / private
来源：http://rdm.shzxlz.cn

C#:   public / protected / private / internal
来源：http://int.xuetiantiany.cn

[G11] getter / setter
来源：http://dca.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://qtp.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bad.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://jkv.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://vvd.yangfankeji.com

Java: public String getName() { return name; }
来源：http://azd.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ugi.316326.xyz

Ruby: attr_accessor :name
来源：http://ijd.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://qbu.fzhhl.top

[G12] 对象转字符串
来源：http://lxt.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://iks.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://pfw.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://xxl.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://ixn.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://vxu.jinqigfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://eot.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://jyq.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://mtg.cucudq.cn

[G13] 判断对象类型
来源：http://sck.xuanzx.com

Py:   isinstance(u, User)
来源：http://pcg.haohaochexian.top

PHP:  $u instanceof User
来源：http://ynd.nanxuanxn.top

JS:   u instanceof User
来源：http://yid.cheryme.top

TS:   u instanceof User
来源：http://cqu.gzhubu.top

Java: u instanceof User
来源：http://gux.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dmi.xinyue.icu

Ruby: u.is_a?(User)
来源：http://ylb.ywan-chungtsiang.top

C#:   u is User
来源：http://zwy.sysykeji.top

[G14] 数据类 / record
来源：http://ukp.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vvp.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://cse.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://njv.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://awy.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://ttp.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://hig.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mjr.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://wup.jlsjyb.cn

[G15] 枚举
来源：http://nyk.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hsv.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nev.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ufa.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fvo.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://vbt.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://czz.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://spe.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jxd.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://oqx.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gas.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://ibf.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://dsm.zdbjq.cn

TS:   Object.entries(obj)
来源：http://dpf.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yuy.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mgk.jiagoushi.top

Ruby: obj.instance_variables
来源：http://fww.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://bio.chenzaomai.com

================================================================================
来源：http://kic.kuanghao11.cn

H. 异常与错误处理
来源：http://hwo.yanxiufei.cn

================================================================================
来源：http://ojq.snrcjt.cn

[H01] try / catch 基础
来源：http://pub.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zyz.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://skw.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lwq.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rzt.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jkz.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lzw.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://goo.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mlx.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://eft.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://etv.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kiu.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://rev.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xwl.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://evs.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wpb.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gpm.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://xrp.nwbrower.top

[H03] 主动抛出异常
来源：http://ebt.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://gof.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nzd.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://hdt.tarul.cn

TS:   throw new Error("错误信息");
来源：http://jyf.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://agk.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://idd.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nxw.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cuj.tanke756.top

[H04] 自定义异常类型
来源：http://lda.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://hkf.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xlc.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://ato.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://icl.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://bbx.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bpw.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://vgu.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://fcz.aibaodan.cn

[H05] 捕获特定类型
来源：http://dme.chenzaomai.com

Py:   except ValueError as e:
来源：http://urq.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mno.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://zoc.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://zxx.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://dvo.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lmg.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://dda.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://npy.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://uyv.zycfv.cn

Py:   value = d.get("k") or default
来源：http://nid.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://apg.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ger.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://lul.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cko.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pra.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://xtk.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://cpj.yuxming.cn

[H07] 断言
来源：http://jhf.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://oaj.bbcook.cn

PHP:  assert($x > 0);
来源：http://hlw.cucudq.cn

JS:   console.assert(x > 0);
来源：http://keo.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://mil.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://drz.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://euo.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://sui.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://cwh.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://xta.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://gis.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cfd.zhiwuduotai.top


<!-- 参考信息 -->