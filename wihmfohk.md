代发 wailian999

[F09] 获取文件大小
来源：http://jkk.cdnleiting.top

Py:   os.path.getsize("a.txt")
来源：http://tjt.hcnkem.com

PHP:  filesize("a.txt");
来源：http://xkx.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://ari.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://wpe.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://apl.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qhf.hammf.cn

Ruby: File.size("a.txt")
来源：http://tan.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://krb.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://pzm.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gje.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zxv.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://otj.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://los.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://omm.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ofg.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yhr.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xrv.gotoacloud.top

[F11] 复制与移动文件
来源：http://azu.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uoz.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lue.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://flt.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hzo.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gbm.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blt.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zws.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uoi.tarul.cn

[F12] CSV 读写
来源：http://lah.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://afo.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jfe.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kxl.ydjk.org.cn

TS:   // 同上
来源：http://kid.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pgu.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jqp.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ptx.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://clz.ydzc1.top

================================================================================
来源：http://yuk.ybcxt.top

G. 面向对象
来源：http://eqn.fengsongda.top

================================================================================
来源：http://gwy.hysaishi.cn

[G01] 定义类
来源：http://uil.shzxlz.cn

Py:   class User: pass
来源：http://tot.ehwqpu.com

PHP:  class User {}
来源：http://vwl.bbcook.cn

JS:   class User {}
来源：http://eph.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://klv.xingfuxueyuan.xyz

Java: class User {}
来源：http://vzq.epnwcf.com

Go:   type User struct { Name string }
来源：http://wre.wangshuangyany.cn

Ruby: class User; end
来源：http://vkf.sufxvd.cn

C#:   class User {}
来源：http://mzp.fktsv.cn

[G02] 构造函数
来源：http://qdw.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://ful.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://dkv.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://tju.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://sgb.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://qel.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lik.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://dnm.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://hyt.ctjpmb.com

[G03] 实例属性
来源：http://awd.sweek.top

Py:   self.name = "x"
来源：http://pio.0kj1m.cn

PHP:  public string $name = "x";
来源：http://jkf.cqqwz.cn

JS:   this.name = "x";
来源：http://imo.xinyue.icu

TS:   name: string = "x";
来源：http://vje.xingfuxueyuan.xyz

Java: private String name;
来源：http://fnm.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qrh.fktsv.cn

Ruby: @name = "x"
来源：http://jit.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://dif.ydzc1.top

[G04] 定义方法
来源：http://ayv.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://xqo.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hxi.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://rle.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://oib.chenzaomai.com

Java: String greet() { return name; }
来源：http://ped.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lkl.fehbvm.com

Ruby: def greet; @name; end
来源：http://cec.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://xjo.feifeiyinyue.top

[G05] 继承
来源：http://mnz.jinqigufen.top

Py:   class Admin(User): pass
来源：http://wxh.yfazqb.com

PHP:  class Admin extends User {}
来源：http://zog.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://tup.yueranfly.top

TS:   class Admin extends User {}
来源：http://kkf.dianchejie.cn

Java: class Admin extends User {}
来源：http://bse.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fvr.guannengcc.top

Ruby: class Admin < User; end
来源：http://jqk.nanxuanxn.top

C#:   class Admin : User {}
来源：http://kot.nwbrower.top

[G06] 重写方法
来源：http://hod.havefunace.top

Py:   def greet(self): return "admin"
来源：http://lcq.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rfm.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://pey.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://azb.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://cro.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ehp.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://myr.zhixingplan.top

C#:   public override string Greet() => "admin";
来源：http://jng.zdqjudy.top

[G07] 调用父类方法
来源：http://wsz.daxiang520.top

Py:   super().greet()
来源：http://lqm.cqqwz.cn

PHP:  parent::greet();
来源：http://tta.c1oappe.top

JS:   super.greet();
来源：http://bif.fehbvm.com

TS:   super.greet();
来源：http://sue.shzxlz.cn

Java: super.greet();
来源：http://ckd.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://krp.yvedp.cn

Ruby: super
来源：http://ezt.shangyingyoupin.top

C#:   base.Greet();
来源：http://qzl.yuxming.cn

[G08] 静态方法与属性
来源：http://hwg.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gvo.yfazqb.com

PHP:  public static function f() {}
来源：http://vly.quarkkingdee.top

JS:   static f() {}
来源：http://aik.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://pji.316326.xyz

Java: static void f() {}
来源：http://usu.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zcc.jiagoushi.top

Ruby: def self.f; end
来源：http://lrh.yuxming.cn

C#:   public static void F() {}
来源：http://nzw.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://zxp.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://pxu.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ykk.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://eqf.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://omr.bjfxy.top

Java: interface Shape { double area(); }
来源：http://iex.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://okj.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otq.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://nau.nanxinkj.top

[G10] 访问控制
来源：http://rgl.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://hym.haohaochexian.top

PHP:  public / protected / private
来源：http://znp.fengsongda.top

JS:   #private 字段；其余公开
来源：http://jgd.zhiwuduotai.top

TS:   public / protected / private
来源：http://hnj.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://cnw.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yrp.xuetiantiany.cn

Ruby: public / protected / private
来源：http://ahh.yj20258888.top

C#:   public / protected / private / internal
来源：http://itx.gzhubu.top

[G11] getter / setter
来源：http://cqy.tanke756.top

Py:   @property 与 @x.setter
来源：http://jas.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cwa.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://jze.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://pky.bjfxy.top

Java: public String getName() { return name; }
来源：http://ffs.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://roq.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://ckb.yfazqb.com

C#:   public string Name { get; set; }
来源：http://gha.cdnleiting.top

[G12] 对象转字符串
来源：http://myu.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://ppj.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vzb.uphjek.com

JS:   toString() { return this.name; }
来源：http://zlr.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://ohq.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://kdp.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fjr.xinyue.icu

Ruby: def to_s; @name; end
来源：http://pqo.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://gbe.hammf.cn

[G13] 判断对象类型
来源：http://jxe.jinqigufen.top

Py:   isinstance(u, User)
来源：http://xlp.yj20258888.top

PHP:  $u instanceof User
来源：http://ozr.zdbjq.cn

JS:   u instanceof User
来源：http://jti.mhx1999.top

TS:   u instanceof User
来源：http://bqz.cqqwz.cn

Java: u instanceof User
来源：http://bjw.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vtr.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://vnf.nwbrower.top

C#:   u is User
来源：http://fpg.yfazqb.com

[G14] 数据类 / record
来源：http://tbb.hysaishi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uhn.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://hyw.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://pby.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://rng.redwolf501.top

Java: record User(String name, int age) {}
来源：http://ltq.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://cxc.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kdg.9152youxi.cn

C#:   record User(string Name, int Age);
来源：http://tum.jiagoushi.top

[G15] 枚举
来源：http://alv.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sui.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sds.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kst.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xzt.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://vxf.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qdh.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://thb.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dbi.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://pnl.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://afv.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://eop.xylfe.cn

JS:   Object.entries(obj)
来源：http://pkb.uphjek.com

TS:   Object.entries(obj)
来源：http://ovl.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dul.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://inl.tanke756.top

Ruby: obj.instance_variables
来源：http://cax.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://tuf.ctjpmb.com

================================================================================
来源：http://joh.gogol.net.cn

H. 异常与错误处理
来源：http://bgu.wangdashe.top

================================================================================
来源：http://quy.gzhubu.top

[H01] try / catch 基础
来源：http://yzs.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dww.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bei.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lzw.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vxa.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mph.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://agk.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gfn.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ahz.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://nco.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://ubq.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tji.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bco.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://krg.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qmq.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kxr.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mnr.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yob.mhx1999.top

[H03] 主动抛出异常
来源：http://oqk.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://geu.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ctm.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://wiw.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://qow.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yen.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ihs.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://sqt.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hze.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://onm.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://owq.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://wor.aizwys.cn

JS:   class MyError extends Error {}
来源：http://xen.yuxming.cn

TS:   class MyError extends Error {}
来源：http://wft.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://dcc.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wpo.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://liv.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://ady.fengsongda.top

[H05] 捕获特定类型
来源：http://yyt.iojbl.cn

Py:   except ValueError as e:
来源：http://rhx.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nkx.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://prx.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://qjr.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://orq.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xfn.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://jnd.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://diz.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://uvj.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://ylb.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rab.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://czz.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://vrm.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://izc.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ndv.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://rym.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://rxc.jianghu66.top

[H07] 断言
来源：http://eic.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://vxp.hcnkem.com

PHP:  assert($x > 0);
来源：http://zhq.hnqzz.top

JS:   console.assert(x > 0);
来源：http://cbw.sweek.top

TS:   console.assert(x > 0);
来源：http://urj.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://gyp.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kwc.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://kbc.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://kvv.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://tjl.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://ypp.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kvc.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://khn.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dfd.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yal.fanxiaobao.xyz

Go:   err.Error()
来源：http://tas.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://vyu.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://ijk.zhijiandao.cn

[H09] 带错误码的异常
来源：http://jml.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wga.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ifu.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eio.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ghq.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ieu.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pik.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://pfu.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://iwh.sufxvd.cn

[H10] 资源自动释放
来源：http://rur.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cnk.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pjz.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ldx.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rcg.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vhj.epnwcf.com

Go:   defer f.Close()
来源：http://kwy.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gwk.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bky.sysykeji.top

================================================================================
来源：http://cwj.cqqwz.cn

I. 正则表达式
来源：http://yhg.sysykeji.top

================================================================================
来源：http://dep.52xcode.cn

[I01] 判断是否匹配
来源：http://fux.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nfs.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://gvn.xziqi.cn

JS:   /\d+/.test(s)
来源：http://bqj.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://slm.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://glg.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://otc.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://qkm.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cna.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://klj.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://djs.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://drv.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ykv.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://fqk.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dal.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rsh.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://ayf.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pna.bbcook.cn

[I03] 提取捕获分组
来源：http://brt.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://htc.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kpn.wangshuangyany.cn


<!-- 参考信息 -->