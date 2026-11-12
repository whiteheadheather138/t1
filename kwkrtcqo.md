代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://xtw.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://drg.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://ecp.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://ebm.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rdp.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://msy.pycfn.com

Ruby: Dir.children("dir")
来源：http://bzr.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://dst.yanxiufei.cn

[F09] 获取文件大小
来源：http://hay.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://kab.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://gvc.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://mro.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://iyr.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://dou.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bca.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://aoc.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://kok.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://wdk.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://twp.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://udr.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://syg.mhx1999.top

TS:   path.extname("a.txt")
来源：http://zms.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xjz.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ztx.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mzw.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://smh.jianghu66.top

[F11] 复制与移动文件
来源：http://ggt.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjb.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bqe.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qhb.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jji.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ntr.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://odl.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oxn.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uob.yonumen.top

[F12] CSV 读写
来源：http://jju.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://itk.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dgp.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://daa.aizwys.cn

TS:   // 同上
来源：http://ppe.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yyp.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sdj.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zfc.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://btx.zhiwuduotai.top

================================================================================
来源：http://twp.hywenlv.cn

G. 面向对象
来源：http://boh.jqgfzy.top

================================================================================
来源：http://dep.zhaomingkeji.xyz

[G01] 定义类
来源：http://xke.9152youxi.cn

Py:   class User: pass
来源：http://gnr.nwbrower.top

PHP:  class User {}
来源：http://hij.sweek.top

JS:   class User {}
来源：http://kxr.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://hjc.smart0.xyz

Java: class User {}
来源：http://tog.0kj1m.cn

Go:   type User struct { Name string }
来源：http://kie.smart0.xyz

Ruby: class User; end
来源：http://cvm.kuanghao11.cn

C#:   class User {}
来源：http://hah.jinqigfzy.top

[G02] 构造函数
来源：http://txd.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://ssf.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://tsh.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://flb.yj20258.top

TS:   constructor(public name: string) {}
来源：http://xdz.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://eft.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kku.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://kli.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://anl.jyoumei.cn

[G03] 实例属性
来源：http://nbq.nwbrower.top

Py:   self.name = "x"
来源：http://fbp.ybcxt.top

PHP:  public string $name = "x";
来源：http://vfs.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://kiv.epnwcf.com

TS:   name: string = "x";
来源：http://kne.guannengcc.top

Java: private String name;
来源：http://qgs.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yez.smart0.xyz

Ruby: @name = "x"
来源：http://bve.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://fdx.bbcook.cn

[G04] 定义方法
来源：http://gqw.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://pkf.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://okc.hnqzz.top

JS:   greet() { return this.name; }
来源：http://jjo.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://fyo.cucudq.cn

Java: String greet() { return name; }
来源：http://cpt.kuanghao11.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://swo.hammf.cn

Ruby: def greet; @name; end
来源：http://ttv.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://gqe.hammf.cn

[G05] 继承
来源：http://vot.meibo888.top

Py:   class Admin(User): pass
来源：http://yrl.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://grt.ydzc1.top

JS:   class Admin extends User {}
来源：http://emy.sysykeji.top

TS:   class Admin extends User {}
来源：http://knp.yueranfly.top

Java: class Admin extends User {}
来源：http://aaw.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ivc.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://orr.yuxming.cn

C#:   class Admin : User {}
来源：http://hqg.bjfxy.top

[G06] 重写方法
来源：http://nec.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://rab.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qdq.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://tyc.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://zny.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://jua.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xpv.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://tpy.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://tjn.ehwqpu.com

[G07] 调用父类方法
来源：http://rre.hysaishi.cn

Py:   super().greet()
来源：http://cky.uphjek.com

PHP:  parent::greet();
来源：http://kaz.52xcode.cn

JS:   super.greet();
来源：http://zdm.52xcode.cn

TS:   super.greet();
来源：http://ifx.cashguo.top

Java: super.greet();
来源：http://fso.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nap.nwbrower.top

Ruby: super
来源：http://ook.epnwcf.com

C#:   base.Greet();
来源：http://lpf.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://fop.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://use.birdmap.top

PHP:  public static function f() {}
来源：http://kbj.dashuyun.cn

JS:   static f() {}
来源：http://uaj.chenlongwang.top

TS:   static f(): void {}
来源：http://tiv.zhixingplan.top

Java: static void f() {}
来源：http://fcm.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cfa.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://qnr.zdbjq.cn

C#:   public static void F() {}
来源：http://mtz.bjfxy.top

[G09] 接口 / 抽象类
来源：http://taa.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://xkq.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://yxk.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gzf.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://ssy.daria6918.cn

Java: interface Shape { double area(); }
来源：http://qqu.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://mtz.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://foy.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://ytb.quarkkingdee.top

[G10] 访问控制
来源：http://buj.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://nld.birdmap.top

PHP:  public / protected / private
来源：http://oep.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://rwt.sxryk.cn

TS:   public / protected / private
来源：http://ajp.yonumen.top

Java: public / protected / private / 默认包级
来源：http://hkg.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uzs.ydjk.org.cn

Ruby: public / protected / private
来源：http://lvu.yj20258888.top

C#:   public / protected / private / internal
来源：http://nhf.cqqwz.cn

[G11] getter / setter
来源：http://tgd.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://dqg.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yaf.mhx1999.top

JS:   get name() { return this._name; }
来源：http://smy.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://cms.9152youxi.cn

Java: public String getName() { return name; }
来源：http://haw.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dlj.hywenlv.cn

Ruby: attr_accessor :name
来源：http://kij.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://env.ctjpmb.com

[G12] 对象转字符串
来源：http://swa.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://tco.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://yhy.sweek.top

JS:   toString() { return this.name; }
来源：http://utm.sweek.top

TS:   toString(): string { return this.name; }
来源：http://esk.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://ypy.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://tce.hcnkem.com

Ruby: def to_s; @name; end
来源：http://bef.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://mro.fengsongda.top

[G13] 判断对象类型
来源：http://tic.mhx1999.top

Py:   isinstance(u, User)
来源：http://fti.sjlbkw.cn

PHP:  $u instanceof User
来源：http://fow.zhiwuduotai.top

JS:   u instanceof User
来源：http://rsl.yj20258.top

TS:   u instanceof User
来源：http://zxx.aizwys.cn

Java: u instanceof User
来源：http://bbl.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dsu.yueranfly.top

Ruby: u.is_a?(User)
来源：http://gma.9152youxi.cn

C#:   u is User
来源：http://xgb.wangdashe.top

[G14] 数据类 / record
来源：http://krc.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dus.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://hyv.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://zrx.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://ayu.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://muo.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://kux.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dxw.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://scg.jqgufenzy.top

[G15] 枚举
来源：http://kcd.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cix.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sob.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://une.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://msk.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://mos.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jpd.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://lid.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aue.meibo888.top

[G16] 对象转数组 / 字典
来源：http://yut.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rzl.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://jws.gogol.net.cn

JS:   Object.entries(obj)
来源：http://fjd.tarul.cn

TS:   Object.entries(obj)
来源：http://qro.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nbk.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zpe.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://dsj.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://vbq.tarul.cn

================================================================================
来源：http://mcb.ybcxt.top

H. 异常与错误处理
来源：http://rqd.yueranfly.top

================================================================================
来源：http://edy.dashuyun.cn

[H01] try / catch 基础
来源：http://qbc.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hhp.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dbi.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yrd.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fcp.sweek.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mfn.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aeh.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tqg.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ebt.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://ehi.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://vkh.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yee.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cmy.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fud.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://afo.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://njk.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zsk.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ali.hammf.cn

[H03] 主动抛出异常
来源：http://jwn.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://oiz.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qet.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://pml.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://qhl.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kna.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eeq.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gin.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://tcx.bbcook.cn

[H04] 自定义异常类型
来源：http://rjq.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://qxd.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://svk.fehbvm.com

JS:   class MyError extends Error {}
来源：http://pai.epnwcf.com

TS:   class MyError extends Error {}
来源：http://uqz.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://auu.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://krj.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://uzs.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://vpm.vehdjk.com

[H05] 捕获特定类型
来源：http://mpt.havefunace.top

Py:   except ValueError as e:
来源：http://xlg.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sur.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://azm.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://kak.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://pyf.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bny.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://nxw.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cys.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://hov.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://qpv.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vvc.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://jtx.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://rfx.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ksm.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fed.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://uhh.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://srd.jinghuilouyu.cn

[H07] 断言
来源：http://qvm.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://yyj.hesvh.cn

PHP:  assert($x > 0);
来源：http://adw.meibo888.top

JS:   console.assert(x > 0);
来源：http://xnn.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://bfn.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://ryi.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zco.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://tuc.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://udy.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://gsq.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://hcm.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://svp.birdmap.top

JS:   e.message;  e.stack
来源：http://nnr.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nju.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://phi.pycfn.com

Go:   err.Error()
来源：http://ahj.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://ocd.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://jff.bbcook.cn

[H09] 带错误码的异常
来源：http://yzk.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://alg.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://hgi.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yuz.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vnt.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hzx.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ana.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ezk.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ssa.pycfn.com

[H10] 资源自动释放
来源：http://eqz.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwn.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://heg.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bui.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eyd.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://umv.ctjpmb.com

Go:   defer f.Close()
来源：http://dfq.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://njb.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vhq.tarul.cn

================================================================================
来源：http://gtw.wangdashe.top

I. 正则表达式
来源：http://ukb.ybcxt.top

================================================================================
来源：http://ezn.yongpay.top

[I01] 判断是否匹配
来源：http://djv.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ajy.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://sue.zycfv.cn

JS:   /\d+/.test(s)
来源：http://noc.yvedp.cn

TS:   /\d+/.test(s)
来源：http://ckz.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cyi.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cvi.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://xdz.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zae.kuanghao11.cn

[I02] 提取所有匹配
来源：http://yyg.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://nzt.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gmj.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jra.uphjek.com


<!-- 参考信息 -->