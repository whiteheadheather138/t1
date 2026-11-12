代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xfr.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xlh.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://koo.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://gcd.yuxming.cn

[F09] 获取文件大小
来源：http://isr.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://xlb.c1oappe.top

PHP:  filesize("a.txt");
来源：http://gfp.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://bea.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://fkj.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://yip.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zmq.hcnkem.com

Ruby: File.size("a.txt")
来源：http://zwm.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://itt.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://hio.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://piu.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sek.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vnv.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://wpn.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lly.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://enw.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oxo.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hbe.xuanzx.com

[F11] 复制与移动文件
来源：http://mhn.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aqo.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sxm.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xrt.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vkq.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aub.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ahd.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gut.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://del.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://kze.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oqd.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://maj.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xfo.hysaishi.cn

TS:   // 同上
来源：http://hkt.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qae.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zjg.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xse.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rqb.chenjidiqi.icu

================================================================================
来源：http://kvw.guowangkeji.top

G. 面向对象
来源：http://gqu.yongpay.top

================================================================================
来源：http://ulo.quarkkingdee.top

[G01] 定义类
来源：http://uin.xziqi.cn

Py:   class User: pass
来源：http://gpu.hesvh.cn

PHP:  class User {}
来源：http://zeb.daxiang520.top

JS:   class User {}
来源：http://wwm.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://pft.aibaodan.cn

Java: class User {}
来源：http://nib.zhengqikj.top

Go:   type User struct { Name string }
来源：http://iev.mhx1999.top

Ruby: class User; end
来源：http://muw.redwolf501.top

C#:   class User {}
来源：http://ygr.cdnleiting.top

[G02] 构造函数
来源：http://pni.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://lyw.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://lni.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://qvt.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://mfn.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://sqv.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fta.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://ldc.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://zzu.ivvv.top

[G03] 实例属性
来源：http://zhx.smart0.xyz

Py:   self.name = "x"
来源：http://ypd.redwolf501.top

PHP:  public string $name = "x";
来源：http://zmo.cdnleiting.top

JS:   this.name = "x";
来源：http://ewd.zycfv.cn

TS:   name: string = "x";
来源：http://dcz.sysykeji.top

Java: private String name;
来源：http://ezr.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ngh.hnqzz.top

Ruby: @name = "x"
来源：http://hpr.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://auj.sysykeji.top

[G04] 定义方法
来源：http://wjf.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://wwn.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iqi.vehdjk.com

JS:   greet() { return this.name; }
来源：http://ivg.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://zoz.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://jmk.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://gsn.redwolf501.top

Ruby: def greet; @name; end
来源：http://fvg.hesvh.cn

C#:   public string Greet() => Name;
来源：http://zjr.fanxiaobao.xyz

[G05] 继承
来源：http://iaq.xylfe.cn

Py:   class Admin(User): pass
来源：http://jzv.daxiang520.top

PHP:  class Admin extends User {}
来源：http://vip.jianghu66.top

JS:   class Admin extends User {}
来源：http://gbo.tanke756.top

TS:   class Admin extends User {}
来源：http://smp.daxiang520.top

Java: class Admin extends User {}
来源：http://ayw.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rgb.fengsongda.top

Ruby: class Admin < User; end
来源：http://zng.yuxming.cn

C#:   class Admin : User {}
来源：http://moz.xuanzx.com

[G06] 重写方法
来源：http://qkw.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://czn.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jkh.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://kyd.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://kdo.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://fzb.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yxk.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://fan.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://chd.bjfxy.top

[G07] 调用父类方法
来源：http://uyx.xuanzx.com

Py:   super().greet()
来源：http://ayj.havefunace.top

PHP:  parent::greet();
来源：http://agv.ppjwa.cn

JS:   super.greet();
来源：http://cbu.birdmap.top

TS:   super.greet();
来源：http://qjh.vehdjk.com

Java: super.greet();
来源：http://frl.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ogu.redwolf501.top

Ruby: super
来源：http://blv.chenlongwang.top

C#:   base.Greet();
来源：http://fzq.yongpay.top

[G08] 静态方法与属性
来源：http://odj.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ndt.jinqigufen.top

PHP:  public static function f() {}
来源：http://gkt.chenzaomai.com

JS:   static f() {}
来源：http://llr.fehbvm.com

TS:   static f(): void {}
来源：http://ucn.hcnkem.com

Java: static void f() {}
来源：http://zco.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://onn.chenlongwang.top

Ruby: def self.f; end
来源：http://izt.mhx1999.top

C#:   public static void F() {}
来源：http://xit.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://crf.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://jxs.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oqe.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tyk.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://hvh.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://wdk.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://rzn.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lkx.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://ydw.iojbl.cn

[G10] 访问控制
来源：http://thq.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://cde.havefunace.top

PHP:  public / protected / private
来源：http://mdg.yvedp.cn

JS:   #private 字段；其余公开
来源：http://ewi.tanke756.top

TS:   public / protected / private
来源：http://rwi.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://srw.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rbb.sjlbkw.cn

Ruby: public / protected / private
来源：http://vvu.xziqi.cn

C#:   public / protected / private / internal
来源：http://stu.haohaochexian.top

[G11] getter / setter
来源：http://rtf.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://lfr.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yrg.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://bdu.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://cac.hfpthk.cn

Java: public String getName() { return name; }
来源：http://lej.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kge.hysaishi.cn

Ruby: attr_accessor :name
来源：http://zqg.ivvv.top

C#:   public string Name { get; set; }
来源：http://yws.hesvh.cn

[G12] 对象转字符串
来源：http://fgj.cheryme.top

Py:   def __str__(self): return self.name
来源：http://pkr.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ain.cashguo.top

JS:   toString() { return this.name; }
来源：http://sbx.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://poc.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://nqp.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://stz.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://sip.nwbrower.top

C#:   public override string ToString() => Name;
来源：http://kgu.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://hhp.xinyue.icu

Py:   isinstance(u, User)
来源：http://oov.bjfxy.top

PHP:  $u instanceof User
来源：http://bwy.hnxiangtu.top

JS:   u instanceof User
来源：http://ken.ydjk.org.cn

TS:   u instanceof User
来源：http://tot.yangfankeji.com

Java: u instanceof User
来源：http://qdy.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zhd.cucudq.cn

Ruby: u.is_a?(User)
来源：http://zug.gotoacloud.top

C#:   u is User
来源：http://fcw.sxryk.cn

[G14] 数据类 / record
来源：http://dwq.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lal.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://nvs.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://raw.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://big.cucudq.cn

Java: record User(String name, int age) {}
来源：http://aoi.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://nas.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://szu.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://tbe.jqgufenzy.top

[G15] 枚举
来源：http://jic.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dhj.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mji.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mey.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eei.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://laq.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://myw.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://nai.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://obr.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://buj.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dvv.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://uez.bbcook.cn

JS:   Object.entries(obj)
来源：http://vcx.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://qye.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ucd.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://asu.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://nnm.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://jez.aibaodan.cn

================================================================================
来源：http://csh.tanke756.top

H. 异常与错误处理
来源：http://hoc.guowangkeji.top

================================================================================
来源：http://ytp.ppjwa.cn

[H01] try / catch 基础
来源：http://wto.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uot.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dga.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hkm.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tke.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://prh.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aed.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tne.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ygi.daria6918.cn

[H02] finally / ensure 收尾
来源：http://nga.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://csy.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mza.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://fpb.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vsx.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hli.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gfd.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fnp.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lfy.yanxiufei.cn

[H03] 主动抛出异常
来源：http://hit.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://vqb.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sti.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://gtq.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://ixr.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ryt.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pdd.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://esu.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://uvu.andypj.xyz

[H04] 自定义异常类型
来源：http://ygy.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://nye.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vlw.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://mju.gzhubu.top

TS:   class MyError extends Error {}
来源：http://cjb.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://cgt.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rcf.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://hlf.xinyue.icu

C#:   class MyException : Exception {}
来源：http://ndn.52xcode.cn

[H05] 捕获特定类型
来源：http://dks.cdnleiting.top

Py:   except ValueError as e:
来源：http://qyd.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ibm.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://ylv.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://wic.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://uno.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kva.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://uxx.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tax.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://yif.xinyue.icu

Py:   value = d.get("k") or default
来源：http://wrw.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://wcl.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://jty.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://hmd.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cjb.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ucn.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://ahz.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://loy.52xcode.cn

[H07] 断言
来源：http://qid.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://brs.0kj1m.cn

PHP:  assert($x > 0);
来源：http://wqg.xylfe.cn

JS:   console.assert(x > 0);
来源：http://qdg.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://znd.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://zxh.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://elg.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://sgu.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://fyh.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://bsl.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://hia.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fpg.sweek.top

JS:   e.message;  e.stack
来源：http://cej.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ina.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jls.tian-w.cn

Go:   err.Error()
来源：http://etr.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://vuf.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://tfl.shzxlz.cn

[H09] 带错误码的异常
来源：http://nkz.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fou.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sgq.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rdp.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://utn.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://byy.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zrr.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eqa.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rft.fengsongda.top

[H10] 资源自动释放
来源：http://xjf.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bal.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ons.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gfe.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xtr.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://utm.zdqjudy.top

Go:   defer f.Close()
来源：http://gkr.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qda.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sri.epnwcf.com

================================================================================
来源：http://yyv.iojbl.cn

I. 正则表达式
来源：http://eid.quarkkingdee.top

================================================================================
来源：http://ntz.ehwqpu.com

[I01] 判断是否匹配
来源：http://evo.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nkl.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://aua.fehbvm.com

JS:   /\d+/.test(s)
来源：http://wdc.aizwys.cn

TS:   /\d+/.test(s)
来源：http://yck.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cck.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blz.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://and.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hzy.yonumen.top

[I02] 提取所有匹配
来源：http://rdm.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://kmo.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nfg.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wuo.yj202588.top

TS:   s.match(/\d+/g)
来源：http://wwp.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hso.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qoq.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://spg.hammf.cn


<!-- 参考信息 -->