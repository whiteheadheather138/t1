代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://has.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://rui.meibo888.top

Ruby: Dir.children("dir")
来源：http://blv.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://mgv.fktsv.cn

[F09] 获取文件大小
来源：http://nuv.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://jgo.daria6918.cn

PHP:  filesize("a.txt");
来源：http://agv.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://ykv.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://etb.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://dlb.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zaw.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://kwb.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://zar.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://dhm.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bnc.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xqv.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wig.tarul.cn

TS:   path.extname("a.txt")
来源：http://tvq.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rsl.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://poj.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sbo.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cri.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://yqq.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://loh.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wtp.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ose.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ipw.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://roy.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lxc.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bjf.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ufz.yonumen.top

[F12] CSV 读写
来源：http://bgm.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uqv.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vab.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zrf.yueranfly.top

TS:   // 同上
来源：http://ght.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://riy.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yph.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://txh.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xab.c1oappe.top

================================================================================
来源：http://edg.0kj1m.cn

G. 面向对象
来源：http://vwd.sxryk.cn

================================================================================
来源：http://spw.cucudq.cn

[G01] 定义类
来源：http://nsf.jlsjyb.cn

Py:   class User: pass
来源：http://mxv.yueranfly.top

PHP:  class User {}
来源：http://edx.fengsongda.top

JS:   class User {}
来源：http://gnv.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://nnz.yvedp.cn

Java: class User {}
来源：http://fym.ctjpmb.com

Go:   type User struct { Name string }
来源：http://iwv.jyoumei.cn

Ruby: class User; end
来源：http://kes.9152youxi.cn

C#:   class User {}
来源：http://gcd.guannengcc.top

[G02] 构造函数
来源：http://siy.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://kyv.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://kkk.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://ohp.yj202588.top

TS:   constructor(public name: string) {}
来源：http://ehe.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://dio.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vka.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://sqj.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://dzo.jinyuanbaomall.cn

[G03] 实例属性
来源：http://ges.daxiang520.top

Py:   self.name = "x"
来源：http://rba.ctjpmb.com

PHP:  public string $name = "x";
来源：http://pur.cucudq.cn

JS:   this.name = "x";
来源：http://vsd.ybcxt.top

TS:   name: string = "x";
来源：http://ats.xziqi.cn

Java: private String name;
来源：http://ejy.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wvw.hnqzz.top

Ruby: @name = "x"
来源：http://fcl.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://krq.yueranfly.top

[G04] 定义方法
来源：http://qtu.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://qqb.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kex.yongpay.top

JS:   greet() { return this.name; }
来源：http://hni.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://kas.fengsongda.top

Java: String greet() { return name; }
来源：http://hgo.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pvy.aizwys.cn

Ruby: def greet; @name; end
来源：http://xcx.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://gvb.cqqwz.cn

[G05] 继承
来源：http://zyk.yvedp.cn

Py:   class Admin(User): pass
来源：http://mej.cheryme.top

PHP:  class Admin extends User {}
来源：http://imq.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://dlw.yj202588.top

TS:   class Admin extends User {}
来源：http://xkr.redwolf501.top

Java: class Admin extends User {}
来源：http://xuq.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ojb.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://jfr.ppjwa.cn

C#:   class Admin : User {}
来源：http://ijj.316326.xyz

[G06] 重写方法
来源：http://irx.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://buu.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://puf.havefunace.top

JS:   greet() { return "admin"; }
来源：http://nop.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://eog.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://msi.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zgb.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://wkv.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://yjq.hongshengwenyu.top

[G07] 调用父类方法
来源：http://yta.ydzc1.top

Py:   super().greet()
来源：http://yxs.cqqwz.cn

PHP:  parent::greet();
来源：http://mwl.andypj.xyz

JS:   super.greet();
来源：http://eku.dianchejie.cn

TS:   super.greet();
来源：http://vzg.ywan-chungtsiang.top

Java: super.greet();
来源：http://ava.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rey.jqgufenzy.top

Ruby: super
来源：http://mjd.daria6918.cn

C#:   base.Greet();
来源：http://djg.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://dol.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xhn.zhijiandao.cn

PHP:  public static function f() {}
来源：http://ghr.yfazqb.com

JS:   static f() {}
来源：http://onm.xuanzx.com

TS:   static f(): void {}
来源：http://upd.uphjek.com

Java: static void f() {}
来源：http://tud.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cbu.yfazqb.com

Ruby: def self.f; end
来源：http://mqj.aizwys.cn

C#:   public static void F() {}
来源：http://peu.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://niv.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://bmp.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://umv.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://uyh.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://yxz.52xcode.cn

Java: interface Shape { double area(); }
来源：http://bld.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://fvl.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mhi.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://bpz.zhaomingkeji.xyz

[G10] 访问控制
来源：http://plb.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://tuf.uphjek.com

PHP:  public / protected / private
来源：http://jns.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://xaq.guowangkeji.top

TS:   public / protected / private
来源：http://ioe.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://zgt.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://fxk.jlsjyb.cn

Ruby: public / protected / private
来源：http://rrq.9152youxi.cn

C#:   public / protected / private / internal
来源：http://obn.zhongyouzk.top

[G11] getter / setter
来源：http://omn.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://ifi.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zjk.iojbl.cn

JS:   get name() { return this._name; }
来源：http://jim.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://jct.tianlin.xyz

Java: public String getName() { return name; }
来源：http://era.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xyk.yj202588.top

Ruby: attr_accessor :name
来源：http://igm.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://onc.meibo888.top

[G12] 对象转字符串
来源：http://svm.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://hrr.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kka.xziqi.cn

JS:   toString() { return this.name; }
来源：http://gfz.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://cts.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://yqw.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zwe.guannengcc.top

Ruby: def to_s; @name; end
来源：http://fyi.meibo888.top

C#:   public override string ToString() => Name;
来源：http://rim.ydjk.org.cn

[G13] 判断对象类型
来源：http://ayt.redwolf501.top

Py:   isinstance(u, User)
来源：http://akf.nwbrower.top

PHP:  $u instanceof User
来源：http://odw.haohaochexian.top

JS:   u instanceof User
来源：http://qwr.fzhhl.top

TS:   u instanceof User
来源：http://pet.zhongyouzk.top

Java: u instanceof User
来源：http://ptj.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dqk.fengsongda.top

Ruby: u.is_a?(User)
来源：http://nhi.hcnkem.com

C#:   u is User
来源：http://ued.xziqi.cn

[G14] 数据类 / record
来源：http://feb.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://keh.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://rjh.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rba.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://cps.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://cep.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://fao.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ivz.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://cxp.chenlongwang.top

[G15] 枚举
来源：http://yfq.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ktu.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hdv.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xyz.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://brb.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://mvb.gzhubu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bov.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://gqu.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ojd.meibo888.top

[G16] 对象转数组 / 字典
来源：http://exr.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lvj.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://yjg.52xcode.cn

JS:   Object.entries(obj)
来源：http://eeo.tanke756.top

TS:   Object.entries(obj)
来源：http://sfl.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dwo.wangshuangyany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://swb.guannengcc.top

Ruby: obj.instance_variables
来源：http://kpv.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://sng.yangfankeji.com

================================================================================
来源：http://ydp.jiagoushi.top

H. 异常与错误处理
来源：http://yyo.chenzaomai.com

================================================================================
来源：http://hdt.chenzaomai.com

[H01] try / catch 基础
来源：http://kmd.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xij.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rla.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dfi.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cmd.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yby.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hik.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://giq.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fyq.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://pyj.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://zhj.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ryb.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iwb.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://inv.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://yge.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cjo.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://pok.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://myv.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://pnk.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://ydt.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jme.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://jvl.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://vfk.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://djs.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zkn.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zic.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://hhx.ivvv.top

[H04] 自定义异常类型
来源：http://hoj.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://fvx.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://sek.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://sey.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://alb.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://qtb.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ize.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://zrc.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://ebt.cashguo.top

[H05] 捕获特定类型
来源：http://syt.zhiwuduotai.top

Py:   except ValueError as e:
来源：http://kev.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jwh.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://zcp.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://cgl.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://uns.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://avr.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://upv.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jif.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://vlq.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://gvz.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nzd.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zce.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cmj.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ewq.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://ceb.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://kza.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://qyq.fanxiaobao.xyz

[H07] 断言
来源：http://mtp.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://mwf.hcnkem.com

PHP:  assert($x > 0);
来源：http://agq.xuanzx.com

JS:   console.assert(x > 0);
来源：http://quc.zycfv.cn

TS:   console.assert(x > 0);
来源：http://eja.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://ebp.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xlg.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qov.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://syw.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://cfo.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://hre.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://set.shzxlz.cn

JS:   e.message;  e.stack
来源：http://wyy.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lrf.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ytk.nanxinkj.top

Go:   err.Error()
来源：http://tys.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://lkl.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://kse.zhengqikj.top

[H09] 带错误码的异常
来源：http://qqe.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cng.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ese.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jky.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xam.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fmj.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mix.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bdy.zdqjudy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ket.9152youxi.cn

[H10] 资源自动释放
来源：http://bmb.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zqz.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sju.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://crq.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ngh.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yjg.andypj.xyz

Go:   defer f.Close()
来源：http://zwz.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fnk.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wsc.xinyue.icu

================================================================================
来源：http://fjj.feifeiyinyue.top

I. 正则表达式
来源：http://uri.jinqigfzy.top

================================================================================
来源：http://slp.sxryk.cn

[I01] 判断是否匹配
来源：http://ftx.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hve.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://bhb.ybcxt.top

JS:   /\d+/.test(s)
来源：http://rzy.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://dru.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kyp.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gqw.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://xui.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tym.52xcode.cn

[I02] 提取所有匹配
来源：http://dqp.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://yqz.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tao.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bwb.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://fos.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zaa.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bag.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://rzh.cdnleiting.top


<!-- 参考信息 -->