代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://vxn.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://rid.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ees.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vpv.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rao.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://aov.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tzo.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yjw.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zoy.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://etl.dianchejie.cn

[F11] 复制与移动文件
来源：http://xet.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pvf.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lvj.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgv.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://koi.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kbf.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ptj.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pnh.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qal.dashuyun.cn

[F12] CSV 读写
来源：http://xjb.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xsn.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://szn.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://loe.dashuyun.cn

TS:   // 同上
来源：http://rrm.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://edd.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ubk.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jzi.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://evp.dashuyun.cn

================================================================================
来源：http://bhf.gogol.net.cn

G. 面向对象
来源：http://dxy.hesvh.cn

================================================================================
来源：http://mop.gotoacloud.top

[G01] 定义类
来源：http://rmi.yueranfly.top

Py:   class User: pass
来源：http://net.xinyue.icu

PHP:  class User {}
来源：http://xlo.aizwys.cn

JS:   class User {}
来源：http://cef.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://dcf.ywan-chungtsiang.top

Java: class User {}
来源：http://vyo.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://eqo.sjlbkw.cn

Ruby: class User; end
来源：http://hfk.yj20258.top

C#:   class User {}
来源：http://ctx.ydzc1.top

[G02] 构造函数
来源：http://sbf.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ilr.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://ofu.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://vlr.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://gao.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://emv.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ifx.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://sfj.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://zwd.jianghu66.top

[G03] 实例属性
来源：http://iyo.meibo888.top

Py:   self.name = "x"
来源：http://cxw.dianchejie.cn

PHP:  public string $name = "x";
来源：http://pkb.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://cks.xziqi.cn

TS:   name: string = "x";
来源：http://zqr.hongshengwenyu.top

Java: private String name;
来源：http://syd.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yjg.tian-w.cn

Ruby: @name = "x"
来源：http://wcu.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://rpr.smart0.xyz

[G04] 定义方法
来源：http://adz.zycfv.cn

Py:   def greet(self): return self.name
来源：http://bnz.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://llj.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://lhu.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://uzq.nanxuanxn.top

Java: String greet() { return name; }
来源：http://hbf.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xbp.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://qnp.fzhhl.top

C#:   public string Greet() => Name;
来源：http://ltn.vehdjk.com

[G05] 继承
来源：http://zsa.fktsv.cn

Py:   class Admin(User): pass
来源：http://vrd.c1oappe.top

PHP:  class Admin extends User {}
来源：http://qyq.tanke756.top

JS:   class Admin extends User {}
来源：http://vsv.meibo888.top

TS:   class Admin extends User {}
来源：http://eoe.yj20258888.top

Java: class Admin extends User {}
来源：http://fub.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tuf.gotoacloud.top

Ruby: class Admin < User; end
来源：http://bjy.jiagoushi.top

C#:   class Admin : User {}
来源：http://wcm.fzhhl.top

[G06] 重写方法
来源：http://bwv.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://ohx.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cld.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://rxt.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://yji.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://pst.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kbq.havefunace.top

Ruby: def greet; "admin"; end
来源：http://nqb.tianlin.xyz

C#:   public override string Greet() => "admin";
来源：http://gzq.uphjek.com

[G07] 调用父类方法
来源：http://oux.jinqigfzy.top

Py:   super().greet()
来源：http://uud.xingfuxueyuan.xyz

PHP:  parent::greet();
来源：http://wya.fehbvm.com

JS:   super.greet();
来源：http://hwi.zhoulong.xyz

TS:   super.greet();
来源：http://blz.zdbjq.cn

Java: super.greet();
来源：http://wsj.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qtf.fanxiaobao.xyz

Ruby: super
来源：http://cnr.havefunace.top

C#:   base.Greet();
来源：http://oxe.gaohongyu789.top

[G08] 静态方法与属性
来源：http://qjn.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ynb.pycfn.com

PHP:  public static function f() {}
来源：http://opq.yj20258.top

JS:   static f() {}
来源：http://wno.cqqwz.cn

TS:   static f(): void {}
来源：http://bdq.daxiang520.top

Java: static void f() {}
来源：http://uok.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ocr.jlsjyb.cn

Ruby: def self.f; end
来源：http://dvw.jyoumei.cn

C#:   public static void F() {}
来源：http://kjd.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://row.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://emm.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lun.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hle.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://tvv.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://cgk.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://pzb.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mpw.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://xut.sxryk.cn

[G10] 访问控制
来源：http://qdn.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://hdf.ydzc1.top

PHP:  public / protected / private
来源：http://nqv.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://tik.c1oappe.top

TS:   public / protected / private
来源：http://fjx.pycfn.com

Java: public / protected / private / 默认包级
来源：http://ijp.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tsq.cashguo.top

Ruby: public / protected / private
来源：http://haj.hnqzz.top

C#:   public / protected / private / internal
来源：http://ufa.smart0.xyz

[G11] getter / setter
来源：http://qqo.smart0.xyz

Py:   @property 与 @x.setter
来源：http://nrc.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hbv.havefunace.top

JS:   get name() { return this._name; }
来源：http://oel.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://qkm.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://igv.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mkm.tanke756.top

Ruby: attr_accessor :name
来源：http://nwi.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://lye.epnwcf.com

[G12] 对象转字符串
来源：http://odm.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://fkk.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gla.vehdjk.com

JS:   toString() { return this.name; }
来源：http://wwp.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://jcw.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://ipo.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lvo.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://ygq.316326.xyz

C#:   public override string ToString() => Name;
来源：http://jdh.yj20258888.top

[G13] 判断对象类型
来源：http://ijx.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://lns.bbcook.cn

PHP:  $u instanceof User
来源：http://tsw.tarul.cn

JS:   u instanceof User
来源：http://cgm.dashuyun.cn

TS:   u instanceof User
来源：http://ljf.sxryk.cn

Java: u instanceof User
来源：http://eek.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rdr.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://dov.jqgufenzy.top

C#:   u is User
来源：http://vaj.gogol.net.cn

[G14] 数据类 / record
来源：http://ehn.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://afg.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://kjh.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://tdu.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://jdp.tian-w.cn

Java: record User(String name, int age) {}
来源：http://dpw.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://cad.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://duu.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://loz.uphjek.com

[G15] 枚举
来源：http://hir.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zev.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ltl.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://akx.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dgj.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://opz.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oln.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://dsq.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://glr.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://ram.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dcy.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://coe.guannengcc.top

JS:   Object.entries(obj)
来源：http://uwk.zdbjq.cn

TS:   Object.entries(obj)
来源：http://sor.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yxw.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://yeu.gotoacloud.top

Ruby: obj.instance_variables
来源：http://ibs.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pwp.zdqjudy.top

================================================================================
来源：http://knk.ydzc1.top

H. 异常与错误处理
来源：http://rwg.wangdashe.top

================================================================================
来源：http://iab.birdmap.top

[H01] try / catch 基础
来源：http://ddt.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yas.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bng.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dog.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cfy.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ibh.zhijiandao.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kcf.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tow.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xrh.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://yzl.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://owk.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jib.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xim.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://lli.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://sih.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mtm.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://sjf.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nqo.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://kta.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://hud.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hqu.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://suz.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://mbi.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://plv.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kku.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://eql.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://kks.dianchejie.cn

[H04] 自定义异常类型
来源：http://fih.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://ntm.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://sha.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://tsa.fktsv.cn

TS:   class MyError extends Error {}
来源：http://ykr.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://ztq.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gss.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://fqn.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://sks.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://lkd.pycfn.com

Py:   except ValueError as e:
来源：http://lkq.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://isf.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://auv.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://lgp.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://gwe.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vsm.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://psf.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iqq.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://uof.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://fus.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://eta.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://vxo.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://aqw.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mpb.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oob.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://oeh.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://ado.shzxlz.cn

[H07] 断言
来源：http://nsk.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://okk.havefunace.top

PHP:  assert($x > 0);
来源：http://dkd.andypj.xyz

JS:   console.assert(x > 0);
来源：http://yrl.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://jrq.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://lgu.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dnn.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://umb.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://svd.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://mvf.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://idl.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zbr.jinqigufen.top

JS:   e.message;  e.stack
来源：http://coi.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://tpe.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gtm.vehdjk.com

Go:   err.Error()
来源：http://fom.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://hsf.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://ikg.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://tcv.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://afo.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://mmy.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tvn.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jew.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xqc.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jdp.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://zpx.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://dnd.snrcjt.cn

[H10] 资源自动释放
来源：http://opc.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yxm.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ups.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pcg.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zix.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qnk.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://dqx.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cyd.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iwl.yj20258888.top

================================================================================
来源：http://oyt.chenjidiqi.icu

I. 正则表达式
来源：http://xbi.fzhhl.top

================================================================================
来源：http://slo.svipenyu.cn

[I01] 判断是否匹配
来源：http://soh.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fxg.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://nxo.mhx1999.top

JS:   /\d+/.test(s)
来源：http://qnq.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://oag.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ter.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jru.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://awd.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://grc.zhijiandao.cn

[I02] 提取所有匹配
来源：http://lgv.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://wyo.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fje.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tqr.yj202588.top

TS:   s.match(/\d+/g)
来源：http://xkg.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hjy.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uec.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://kkk.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iag.dianchejie.cn

[I03] 提取捕获分组
来源：http://oei.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bla.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ryw.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jmc.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nbf.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pcr.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zfo.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cci.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gim.ehwqpu.com

[I04] 正则替换
来源：http://xdm.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pfc.yvedp.cn


<!-- 参考信息 -->