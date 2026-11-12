代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://xaw.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://kgv.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zso.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://qjr.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://ydz.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://xgf.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gvh.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sho.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xlp.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://nwy.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwg.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wcy.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pcc.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cvk.xziqi.cn

[F11] 复制与移动文件
来源：http://vfp.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eka.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eei.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tto.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oko.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qde.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vur.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rzg.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aom.dashuyun.cn

[F12] CSV 读写
来源：http://ozw.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tij.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qbp.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hhv.redwolf501.top

TS:   // 同上
来源：http://mrc.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://biz.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dxz.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jhy.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jwr.meibo888.top

================================================================================
来源：http://her.vqdsnc.cn

G. 面向对象
来源：http://skt.0kj1m.cn

================================================================================
来源：http://ihd.zycfv.cn

[G01] 定义类
来源：http://tdm.andypj.xyz

Py:   class User: pass
来源：http://llv.fktsv.cn

PHP:  class User {}
来源：http://gej.jqgfzy.top

JS:   class User {}
来源：http://und.tarul.cn

TS:   class User { name: string = ""; }
来源：http://jab.hammf.cn

Java: class User {}
来源：http://qim.sysykeji.top

Go:   type User struct { Name string }
来源：http://fnz.sjlbkw.cn

Ruby: class User; end
来源：http://swc.smart0.xyz

C#:   class User {}
来源：http://ymf.zhengqikj.top

[G02] 构造函数
来源：http://kis.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://adh.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://kvx.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://qmq.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://otj.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://xxm.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qpn.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://thu.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://gaa.yongpay.top

[G03] 实例属性
来源：http://yga.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://nol.hfpthk.cn

PHP:  public string $name = "x";
来源：http://rvp.hywenlv.cn

JS:   this.name = "x";
来源：http://sab.ehwqpu.com

TS:   name: string = "x";
来源：http://zbb.zhongyouzk.top

Java: private String name;
来源：http://mqu.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jof.birdmap.top

Ruby: @name = "x"
来源：http://vjg.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://jna.c1oappe.top

[G04] 定义方法
来源：http://kbd.xylfe.cn

Py:   def greet(self): return self.name
来源：http://epl.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://nrn.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://ubv.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://smc.xziqi.cn

Java: String greet() { return name; }
来源：http://gdc.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tnr.yonumen.top

Ruby: def greet; @name; end
来源：http://lzt.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://sll.quarkkingdee.top

[G05] 继承
来源：http://mze.dianchejie.cn

Py:   class Admin(User): pass
来源：http://qiy.xuanzx.com

PHP:  class Admin extends User {}
来源：http://pkl.cqqwz.cn

JS:   class Admin extends User {}
来源：http://bnz.jianghu66.top

TS:   class Admin extends User {}
来源：http://guf.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://nud.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gep.hfpthk.cn

Ruby: class Admin < User; end
来源：http://zib.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://uto.jinghuilouyu.cn

[G06] 重写方法
来源：http://url.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://yts.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://czq.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://qog.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://spt.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://mim.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hvs.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://rjo.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://lyt.chenzaomai.com

[G07] 调用父类方法
来源：http://syf.zdbjq.cn

Py:   super().greet()
来源：http://bts.birdmap.top

PHP:  parent::greet();
来源：http://euw.ydjk.org.cn

JS:   super.greet();
来源：http://swk.fehbvm.com

TS:   super.greet();
来源：http://svr.gaohongyu789.top

Java: super.greet();
来源：http://fod.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://del.ywan-chungtsiang.top

Ruby: super
来源：http://xad.zycfv.cn

C#:   base.Greet();
来源：http://dnu.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://few.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xyy.yueranfly.top

PHP:  public static function f() {}
来源：http://btr.chenjidiqi.icu

JS:   static f() {}
来源：http://pgl.yangfankeji.com

TS:   static f(): void {}
来源：http://xgt.zdqjudy.top

Java: static void f() {}
来源：http://fep.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iop.meibo888.top

Ruby: def self.f; end
来源：http://rsg.jinqigufen.top

C#:   public static void F() {}
来源：http://dpd.smart0.xyz

[G09] 接口 / 抽象类
来源：http://qca.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://wor.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mqc.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uts.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://wqf.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://ilq.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://lbw.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://noo.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://paf.yvedp.cn

[G10] 访问控制
来源：http://jwr.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://ahm.meibo888.top

PHP:  public / protected / private
来源：http://lyy.sweek.top

JS:   #private 字段；其余公开
来源：http://wmt.yongpay.top

TS:   public / protected / private
来源：http://dgp.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://oeh.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://ihc.yfazqb.com

Ruby: public / protected / private
来源：http://xbn.jyoumei.cn

C#:   public / protected / private / internal
来源：http://unb.jlsjyb.cn

[G11] getter / setter
来源：http://slf.yueranfly.top

Py:   @property 与 @x.setter
来源：http://oiz.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dwu.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://fpv.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://pwy.pycfn.com

Java: public String getName() { return name; }
来源：http://nyp.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yyn.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://qwz.iojbl.cn

C#:   public string Name { get; set; }
来源：http://cti.yuanzhike.top

[G12] 对象转字符串
来源：http://pws.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://znm.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yro.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://jsq.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://cke.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://nio.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://jjr.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://xpy.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://ljp.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://xjq.meibo888.top

Py:   isinstance(u, User)
来源：http://qyg.gotoacloud.top

PHP:  $u instanceof User
来源：http://giy.quarkkingdee.top

JS:   u instanceof User
来源：http://mqn.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://ijr.zhoulong.xyz

Java: u instanceof User
来源：http://fba.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://esj.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://jku.jlsjyb.cn

C#:   u is User
来源：http://ujx.zhixingplan.top

[G14] 数据类 / record
来源：http://yak.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zpb.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://tir.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://lzo.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://mgb.bjfxy.top

Java: record User(String name, int age) {}
来源：http://ixs.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://jqi.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dvz.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://tvr.uphjek.com

[G15] 枚举
来源：http://rzo.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zlg.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pfz.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vfl.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://srh.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://lka.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mph.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://sib.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zgv.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://vjy.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pmm.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://jqn.bjfxy.top

JS:   Object.entries(obj)
来源：http://vpe.chenlongwang.top

TS:   Object.entries(obj)
来源：http://sfc.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rsm.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qgu.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://pxo.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://qlo.vqdsnc.cn

================================================================================
来源：http://yqg.tanke756.top

H. 异常与错误处理
来源：http://kzj.quarkkingdee.top

================================================================================
来源：http://ylu.zycfv.cn

[H01] try / catch 基础
来源：http://say.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ydp.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kwl.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zyz.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yii.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cyv.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mxq.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://far.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ujw.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://byd.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://mem.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://znw.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://keq.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://daf.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://yjb.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mlr.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://alc.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sfm.aibaodan.cn

[H03] 主动抛出异常
来源：http://udi.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://bkn.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pvc.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://lkk.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://ugu.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ean.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nah.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cgt.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gtu.yuxming.cn

[H04] 自定义异常类型
来源：http://yvi.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://jta.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://qro.tarul.cn

JS:   class MyError extends Error {}
来源：http://ksh.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://dlm.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://igg.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pca.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://ctr.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://inq.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://tvz.cucudq.cn

Py:   except ValueError as e:
来源：http://vgv.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wmv.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://vkl.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://klb.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://omb.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mvz.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://uja.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bqo.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://byl.ybcxt.top

Py:   value = d.get("k") or default
来源：http://ylh.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ucl.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ank.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://fau.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bvu.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cpp.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://fwn.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://uoq.ppjwa.cn

[H07] 断言
来源：http://evl.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://rmk.epnwcf.com

PHP:  assert($x > 0);
来源：http://wjl.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://yda.wangdashe.top

TS:   console.assert(x > 0);
来源：http://svz.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://cws.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://svk.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://daf.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://mxr.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://wqq.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://rre.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rxj.cucudq.cn

JS:   e.message;  e.stack
来源：http://pyf.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rjt.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://eog.yonumen.top

Go:   err.Error()
来源：http://nwo.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://jpv.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://fqu.fehbvm.com

[H09] 带错误码的异常
来源：http://fwn.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vni.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://cxf.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rbm.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tqf.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qfa.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ajx.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://tvl.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zvy.cucudq.cn

[H10] 资源自动释放
来源：http://rzu.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://csl.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ftd.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xuq.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nxe.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wqj.chenjidiqi.icu

Go:   defer f.Close()
来源：http://eof.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tqc.ppjwa.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nrh.iojbl.cn

================================================================================
来源：http://fez.bjfxy.top

I. 正则表达式
来源：http://yrt.zhijiandao.cn

================================================================================
来源：http://jdm.hnqzz.top

[I01] 判断是否匹配
来源：http://wsv.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qgk.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://dfw.xinyue.icu

JS:   /\d+/.test(s)
来源：http://pwe.fehbvm.com

TS:   /\d+/.test(s)
来源：http://sjq.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://keb.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dji.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://twn.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eoc.hammf.cn

[I02] 提取所有匹配
来源：http://cil.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://mei.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://geu.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zoq.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://qlm.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vbr.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://swv.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://ttf.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lxx.gaohongyu789.top

[I03] 提取捕获分组
来源：http://bif.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://glo.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qfx.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ghc.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://crd.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kbo.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vki.wangshuangyany.cn


<!-- 参考信息 -->