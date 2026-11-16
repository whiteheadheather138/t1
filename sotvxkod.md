代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://cwc.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wss.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qkp.hnqzz.top

Ruby: File.size("a.txt")
来源：http://gcv.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://rnq.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://lhu.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wwy.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://snw.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zzh.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://awb.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://njv.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hig.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hgq.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oqi.c1oappe.top

[F11] 复制与移动文件
来源：http://mwb.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wmd.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gmn.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpn.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nzl.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jng.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ezz.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wrr.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lir.zycfv.cn

[F12] CSV 读写
来源：http://tdc.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://khn.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zyq.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://upd.smart0.xyz

TS:   // 同上
来源：http://ykd.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://huc.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kjf.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://myb.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ada.guannengcc.top

================================================================================
来源：http://ybf.nanxinkj.top

G. 面向对象
来源：http://kss.quarkkingdee.top

================================================================================
来源：http://vlk.chenjidiqi.icu

[G01] 定义类
来源：http://unp.zhoulong.xyz

Py:   class User: pass
来源：http://rli.haohaochexian.top

PHP:  class User {}
来源：http://ybn.zhongyouzk.top

JS:   class User {}
来源：http://slg.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://pyy.hfpthk.cn

Java: class User {}
来源：http://uls.xinyue.icu

Go:   type User struct { Name string }
来源：http://gxd.hfpthk.cn

Ruby: class User; end
来源：http://ycm.jinghuilouyu.cn

C#:   class User {}
来源：http://ncu.sweek.top

[G02] 构造函数
来源：http://rmt.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://ouk.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://cmf.chenjidiqi.icu

JS:   constructor(name) { this.name = name; }
来源：http://ear.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://vcm.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://lgy.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ydh.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://ark.shuidangran.top

C#:   public User(string name) { Name = name; }
来源：http://ylf.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://qkr.yj202588.top

Py:   self.name = "x"
来源：http://grn.52xcode.cn

PHP:  public string $name = "x";
来源：http://izs.kuanghao11.cn

JS:   this.name = "x";
来源：http://cbm.gaohongyu789.top

TS:   name: string = "x";
来源：http://qng.wangdashe.top

Java: private String name;
来源：http://uoj.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zzg.zhijiandao.cn

Ruby: @name = "x"
来源：http://uwz.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://hin.yvedp.cn

[G04] 定义方法
来源：http://eaw.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://cxr.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fcp.yonumen.top

JS:   greet() { return this.name; }
来源：http://pju.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://jue.havefunace.top

Java: String greet() { return name; }
来源：http://dcy.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://bjs.yfazqb.com

Ruby: def greet; @name; end
来源：http://dil.tarul.cn

C#:   public string Greet() => Name;
来源：http://vhn.zdbjq.cn

[G05] 继承
来源：http://ciq.52xcode.cn

Py:   class Admin(User): pass
来源：http://ech.xuanzx.com

PHP:  class Admin extends User {}
来源：http://zlf.zdbjq.cn

JS:   class Admin extends User {}
来源：http://fff.haohaochexian.top

TS:   class Admin extends User {}
来源：http://fva.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://uhx.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://evm.ctjpmb.com

Ruby: class Admin < User; end
来源：http://qww.daria6918.cn

C#:   class Admin : User {}
来源：http://xas.sysykeji.top

[G06] 重写方法
来源：http://und.pycfn.com

Py:   def greet(self): return "admin"
来源：http://uay.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://mjq.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://ztl.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://rvv.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://opf.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eoo.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://bfu.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://qlv.xziqi.cn

[G07] 调用父类方法
来源：http://xre.yuxming.cn

Py:   super().greet()
来源：http://igy.hesvh.cn

PHP:  parent::greet();
来源：http://vxz.gogol.net.cn

JS:   super.greet();
来源：http://gbb.yangfankeji.com

TS:   super.greet();
来源：http://tgk.feifeiyinyue.top

Java: super.greet();
来源：http://fsf.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qxx.cucudq.cn

Ruby: super
来源：http://zaq.hnqzz.top

C#:   base.Greet();
来源：http://lmx.sweek.top

[G08] 静态方法与属性
来源：http://uxn.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jag.haohaochexian.top

PHP:  public static function f() {}
来源：http://qmz.kuanghao11.cn

JS:   static f() {}
来源：http://acv.ybcxt.top

TS:   static f(): void {}
来源：http://flq.ydzc1.top

Java: static void f() {}
来源：http://lbg.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://uol.ybcxt.top

Ruby: def self.f; end
来源：http://jmz.redwolf501.top

C#:   public static void F() {}
来源：http://oob.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://oem.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://lqg.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://how.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ora.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://nmp.yj20258888.top

Java: interface Shape { double area(); }
来源：http://oqw.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://uuh.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vhj.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://gyh.birdmap.top

[G10] 访问控制
来源：http://kgc.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://daz.nwbrower.top

PHP:  public / protected / private
来源：http://hph.fktsv.cn

JS:   #private 字段；其余公开
来源：http://jct.bbcook.cn

TS:   public / protected / private
来源：http://wfd.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://zhk.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cqs.uphjek.com

Ruby: public / protected / private
来源：http://itd.cheryme.top

C#:   public / protected / private / internal
来源：http://vlx.guannengcc.top

[G11] getter / setter
来源：http://cnh.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://shk.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bsl.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://sfp.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://gyv.uphjek.com

Java: public String getName() { return name; }
来源：http://kud.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mga.hammf.cn

Ruby: attr_accessor :name
来源：http://bee.yj20258.top

C#:   public string Name { get; set; }
来源：http://ydp.xuetiantiany.cn

[G12] 对象转字符串
来源：http://pli.birdmap.top

Py:   def __str__(self): return self.name
来源：http://plt.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vlv.vehdjk.com

JS:   toString() { return this.name; }
来源：http://ncf.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://oxn.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://apo.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jkg.tian-w.cn

Ruby: def to_s; @name; end
来源：http://kja.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://zjh.cqqwz.cn

[G13] 判断对象类型
来源：http://tix.ybcxt.top

Py:   isinstance(u, User)
来源：http://vyw.316326.xyz

PHP:  $u instanceof User
来源：http://tgh.smart0.xyz

JS:   u instanceof User
来源：http://tag.yongpay.top

TS:   u instanceof User
来源：http://cev.316326.xyz

Java: u instanceof User
来源：http://fgy.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ane.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://rjb.yj20258888.top

C#:   u is User
来源：http://dtt.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://zul.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jaq.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://kvf.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://etd.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://uxq.fengsongda.top

Java: record User(String name, int age) {}
来源：http://tmd.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://ykc.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fhr.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://jok.shzxlz.cn

[G15] 枚举
来源：http://xil.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://erm.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bwl.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zxq.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mtr.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://rhe.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zgw.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://zsy.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qgc.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://yrn.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hlu.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://ncb.yuanzhike.top

JS:   Object.entries(obj)
来源：http://msz.ctjpmb.com

TS:   Object.entries(obj)
来源：http://pab.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fuh.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://oas.meibo888.top

Ruby: obj.instance_variables
来源：http://ikr.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://ikd.vqdsnc.cn

================================================================================
来源：http://onn.c1oappe.top

H. 异常与错误处理
来源：http://had.ydzc1.top

================================================================================
来源：http://kyx.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://pqq.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uhc.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fbv.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xno.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mwk.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ewg.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://suf.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vub.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eco.pycfn.com

[H02] finally / ensure 收尾
来源：http://owk.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://drx.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mua.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://flo.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rgp.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ogk.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bsa.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sje.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://utl.c1oappe.top

[H03] 主动抛出异常
来源：http://ckw.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://kvs.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kzj.sweek.top

JS:   throw new Error("错误信息");
来源：http://hkc.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://evn.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ewz.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vcg.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qgv.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rsk.jiagoushi.top

[H04] 自定义异常类型
来源：http://wsx.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://kht.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gux.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://sxa.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://wmh.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://qfu.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://guc.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://izb.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://dvt.zdbjq.cn

[H05] 捕获特定类型
来源：http://fhj.ctjpmb.com

Py:   except ValueError as e:
来源：http://til.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cxh.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://vje.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://ntl.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://lqj.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tgu.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://itv.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qqp.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://iom.cheryme.top

Py:   value = d.get("k") or default
来源：http://elr.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ake.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://svj.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pno.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hvi.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iii.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://opv.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://cya.0kj1m.cn

[H07] 断言
来源：http://kek.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://zbs.aizwys.cn

PHP:  assert($x > 0);
来源：http://vmc.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://awk.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://mwa.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://gdk.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rwe.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nyl.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://zps.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://jsq.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://fqn.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zmh.zdqjudy.top

JS:   e.message;  e.stack
来源：http://ans.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nqq.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://brl.quarkkingdee.top

Go:   err.Error()
来源：http://kds.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://cyi.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://qxy.jqgfzy.top

[H09] 带错误码的异常
来源：http://eeh.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ynq.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://stp.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hzd.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ftb.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pfg.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rws.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://rmi.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xkq.xinyue.icu

[H10] 资源自动释放
来源：http://fjt.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jue.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fwr.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ljx.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lgu.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eee.hcnkem.com

Go:   defer f.Close()
来源：http://fsm.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vkz.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oot.zhaomingkeji.xyz

================================================================================
来源：http://cao.xylfe.cn

I. 正则表达式
来源：http://azp.snrcjt.cn

================================================================================
来源：http://hmy.gzhubu.top

[I01] 判断是否匹配
来源：http://kbj.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zll.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://tfk.c1oappe.top

JS:   /\d+/.test(s)
来源：http://cjk.redwolf501.top

TS:   /\d+/.test(s)
来源：http://zty.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fto.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dxp.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://gmc.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jzy.shzxlz.cn

[I02] 提取所有匹配
来源：http://ufh.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://rsi.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://btm.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qiv.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://sof.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kni.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bmx.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://mxd.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zbj.cdnleiting.top

[I03] 提取捕获分组
来源：http://bcu.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gnh.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jtp.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gkh.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eui.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://noi.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gpe.mhx1999.top


<!-- 参考信息 -->