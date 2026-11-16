代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://tay.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://uek.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zmx.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://dej.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://uhz.guannengcc.top

[F06] 删除文件
来源：http://eyg.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://twq.pycfn.com

PHP:  unlink("a.txt");
来源：http://yni.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xwh.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://uon.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gwr.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://nyw.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://ctl.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://hzx.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://owj.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lxz.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://idh.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gae.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ptf.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yqf.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nad.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yqf.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wwi.zdqjudy.top

[F08] 遍历目录
来源：http://nan.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://umk.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xli.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://twr.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://ebb.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hcx.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kfx.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://lsi.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://xoe.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://oxm.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://esb.redwolf501.top

PHP:  filesize("a.txt");
来源：http://hlt.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://kau.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://hon.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rzz.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sgn.sysykeji.top

Ruby: File.size("a.txt")
来源：http://ytm.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://azf.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://ttt.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ecp.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://trr.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ipp.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://xao.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qyb.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tpp.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://klr.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mnp.svipenyu.cn

[F11] 复制与移动文件
来源：http://ors.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dik.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ngc.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fdk.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rpg.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qrj.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cal.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nrl.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://akq.sxryk.cn

[F12] CSV 读写
来源：http://oin.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vsp.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qii.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bgo.nanxinkj.top

TS:   // 同上
来源：http://cpy.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://odj.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://seb.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://umy.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ysg.snrcjt.cn

================================================================================
来源：http://ars.52xcode.cn

G. 面向对象
来源：http://hbs.9152youxi.cn

================================================================================
来源：http://fjo.hongshengwenyu.top

[G01] 定义类
来源：http://bua.nanxuanxn.top

Py:   class User: pass
来源：http://tqd.shangyingyoupin.top

PHP:  class User {}
来源：http://xth.nanxuanxn.top

JS:   class User {}
来源：http://lcf.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://zwv.bjfxy.top

Java: class User {}
来源：http://igc.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://bir.xuanzx.com

Ruby: class User; end
来源：http://vqf.zdbjq.cn

C#:   class User {}
来源：http://wle.316326.xyz

[G02] 构造函数
来源：http://bah.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://yxu.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://epm.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://jpu.havefunace.top

TS:   constructor(public name: string) {}
来源：http://hrb.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://wix.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cxk.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://qzc.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://kcw.ctjpmb.com

[G03] 实例属性
来源：http://ice.ehwqpu.com

Py:   self.name = "x"
来源：http://rlf.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://czs.fehbvm.com

JS:   this.name = "x";
来源：http://wss.yangfankeji.com

TS:   name: string = "x";
来源：http://xkz.cheryme.top

Java: private String name;
来源：http://tzz.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jwr.gogol.net.cn

Ruby: @name = "x"
来源：http://gor.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://ixs.yvedp.cn

[G04] 定义方法
来源：http://xsz.xinyue.icu

Py:   def greet(self): return self.name
来源：http://xkw.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mdn.fktsv.cn

JS:   greet() { return this.name; }
来源：http://pux.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://gcp.fzhhl.top

Java: String greet() { return name; }
来源：http://kyf.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://axk.zycfv.cn

Ruby: def greet; @name; end
来源：http://bbm.hnqzz.top

C#:   public string Greet() => Name;
来源：http://teu.havefunace.top

[G05] 继承
来源：http://qvz.jinqigufen.top

Py:   class Admin(User): pass
来源：http://gmh.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://jtp.xuanzx.com

JS:   class Admin extends User {}
来源：http://aei.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://mna.yj20258.top

Java: class Admin extends User {}
来源：http://cqr.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wls.fehbvm.com

Ruby: class Admin < User; end
来源：http://lbk.cqqwz.cn

C#:   class Admin : User {}
来源：http://tzz.feifeiyinyue.top

[G06] 重写方法
来源：http://ear.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://qgg.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://rbz.uphjek.com

JS:   greet() { return "admin"; }
来源：http://abh.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://vyc.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://fnj.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tvs.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://iog.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://fbk.xylfe.cn

[G07] 调用父类方法
来源：http://cdn.yfazqb.com

Py:   super().greet()
来源：http://etz.xuetiantiany.cn

PHP:  parent::greet();
来源：http://iuf.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://xcj.tianlin.xyz

TS:   super.greet();
来源：http://wig.sweek.top

Java: super.greet();
来源：http://uyz.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://php.xinyue.icu

Ruby: super
来源：http://bqp.yangfankeji.com

C#:   base.Greet();
来源：http://mep.shzxlz.cn

[G08] 静态方法与属性
来源：http://lnq.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yuo.yanxiufei.cn

PHP:  public static function f() {}
来源：http://atw.epnwcf.com

JS:   static f() {}
来源：http://utn.xylfe.cn

TS:   static f(): void {}
来源：http://iuw.nanxuanxn.top

Java: static void f() {}
来源：http://hwv.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jje.nwbrower.top

Ruby: def self.f; end
来源：http://fok.316326.xyz

C#:   public static void F() {}
来源：http://wpr.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://uhu.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://vfg.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ntm.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fdm.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://hsx.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://pbn.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://zef.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dkb.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://tjf.hnxiangtu.top

[G10] 访问控制
来源：http://ndw.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://mtz.hfpthk.cn

PHP:  public / protected / private
来源：http://lyv.cucudq.cn

JS:   #private 字段；其余公开
来源：http://ocm.haohaochexian.top

TS:   public / protected / private
来源：http://apk.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://ujh.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://onx.tarul.cn

Ruby: public / protected / private
来源：http://zks.chenlongwang.top

C#:   public / protected / private / internal
来源：http://sho.xinyue.icu

[G11] getter / setter
来源：http://kkw.xziqi.cn

Py:   @property 与 @x.setter
来源：http://gnm.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yfj.cheryme.top

JS:   get name() { return this._name; }
来源：http://fpr.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://uzy.shzxlz.cn

Java: public String getName() { return name; }
来源：http://lml.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rhp.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://ezy.zycfv.cn

C#:   public string Name { get; set; }
来源：http://fbv.shuidangran.top

[G12] 对象转字符串
来源：http://dpf.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://bkw.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://luk.hcnkem.com

JS:   toString() { return this.name; }
来源：http://mmz.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://gsm.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://kxe.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://hay.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://hom.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://jzb.uphjek.com

[G13] 判断对象类型
来源：http://eew.fktsv.cn

Py:   isinstance(u, User)
来源：http://hvp.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://edw.jinqigfzy.top

JS:   u instanceof User
来源：http://xmk.c1oappe.top

TS:   u instanceof User
来源：http://awq.cucudq.cn

Java: u instanceof User
来源：http://mps.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qjz.bjfxy.top

Ruby: u.is_a?(User)
来源：http://ksq.zhongyouzk.top

C#:   u is User
来源：http://gpo.sysykeji.top

[G14] 数据类 / record
来源：http://tow.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gmu.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://zqn.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://qhw.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://dyd.cashguo.top

Java: record User(String name, int age) {}
来源：http://akg.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://sic.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bxi.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://cbg.xingfuxueyuan.xyz

[G15] 枚举
来源：http://wvq.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fsx.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yqt.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tep.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ibn.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://vuf.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ssf.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://ouj.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rnt.havefunace.top

[G16] 对象转数组 / 字典
来源：http://bts.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wsu.hammf.cn

PHP:  get_object_vars($obj);
来源：http://fep.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://car.cucudq.cn

TS:   Object.entries(obj)
来源：http://vir.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://trf.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://svf.cucudq.cn

Ruby: obj.instance_variables
来源：http://bwi.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://fcr.xuanzx.com

================================================================================
来源：http://nef.fengsongda.top

H. 异常与错误处理
来源：http://fqp.xinyue.icu

================================================================================
来源：http://czt.cheryme.top

[H01] try / catch 基础
来源：http://yhs.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zaa.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jvr.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gbd.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mwd.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://olj.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xsv.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cxz.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jep.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://bmk.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://hxg.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bvc.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bvc.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nwt.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://igd.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gww.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bmd.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ttv.cheryme.top

[H03] 主动抛出异常
来源：http://ftq.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://trs.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cgb.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://afa.cashguo.top

TS:   throw new Error("错误信息");
来源：http://mge.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://lyd.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hmb.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://mif.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wqt.ydjk.org.cn

[H04] 自定义异常类型
来源：http://ylz.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://fri.ywan-chungtsiang.top

PHP:  class MyError extends RuntimeException {}
来源：http://kti.daxiang520.top

JS:   class MyError extends Error {}
来源：http://ksg.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://ode.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://plw.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rnc.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://qlc.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://iqh.svipenyu.cn

[H05] 捕获特定类型
来源：http://odg.andypj.xyz

Py:   except ValueError as e:
来源：http://tjn.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ryh.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://yha.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://ggk.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://igg.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fex.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://hjz.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cke.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://hkr.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://qvf.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uyn.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://xig.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://omd.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mcx.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://wby.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://vbr.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://ter.quarkkingdee.top

[H07] 断言
来源：http://hxo.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://bgu.ppjwa.cn

PHP:  assert($x > 0);
来源：http://qou.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://hro.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://jcm.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://vyv.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pqi.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mva.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://vps.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://qcw.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://fvx.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bmz.jiagoushi.top

JS:   e.message;  e.stack
来源：http://ydn.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ons.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ydg.yvedp.cn

Go:   err.Error()
来源：http://fhj.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://kub.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://jql.chenzaomai.com

[H09] 带错误码的异常
来源：http://sai.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bfh.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jjq.hnqzz.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qvh.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tos.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qut.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gzd.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gjt.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://zrx.hcnkem.com

[H10] 资源自动释放
来源：http://ixn.yueranfly.top


<!-- 参考信息 -->