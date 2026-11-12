代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://axa.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://clx.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zyn.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xnn.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xjg.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://lhf.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://caa.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tij.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dop.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://luh.cashguo.top

[F11] 复制与移动文件
来源：http://xgh.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sso.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mcl.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xue.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vbm.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pkg.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://twc.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pdp.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rew.cucudq.cn

[F12] CSV 读写
来源：http://dfx.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fiv.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wjn.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qtf.shuidangran.top

TS:   // 同上
来源：http://dju.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qdd.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xfp.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dcl.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zfm.andypj.xyz

================================================================================
来源：http://npk.yangfankeji.com

G. 面向对象
来源：http://uqn.hywenlv.cn

================================================================================
来源：http://nyj.xingfuxueyuan.xyz

[G01] 定义类
来源：http://ooq.yj20258888.top

Py:   class User: pass
来源：http://yxe.ybcxt.top

PHP:  class User {}
来源：http://bci.ydjk.org.cn

JS:   class User {}
来源：http://fnc.birdmap.top

TS:   class User { name: string = ""; }
来源：http://vpg.zhijiandao.cn

Java: class User {}
来源：http://whk.svipenyu.cn

Go:   type User struct { Name string }
来源：http://fkm.sysykeji.top

Ruby: class User; end
来源：http://jrs.havefunace.top

C#:   class User {}
来源：http://otr.smart0.xyz

[G02] 构造函数
来源：http://lli.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://ota.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://srz.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://ifg.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://zti.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://idh.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dzb.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://slg.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://nsd.haohaochexian.top

[G03] 实例属性
来源：http://ejh.xziqi.cn

Py:   self.name = "x"
来源：http://lhp.smart0.xyz

PHP:  public string $name = "x";
来源：http://brw.pengpengdd.cyou

JS:   this.name = "x";
来源：http://ycv.chenjidiqi.icu

TS:   name: string = "x";
来源：http://bua.zdqjudy.top

Java: private String name;
来源：http://zpl.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bcy.yuxming.cn

Ruby: @name = "x"
来源：http://uhs.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://ttz.yuxming.cn

[G04] 定义方法
来源：http://oxk.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://mes.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ock.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://lec.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://lib.jiagoushi.top

Java: String greet() { return name; }
来源：http://zcs.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zgn.fengsongda.top

Ruby: def greet; @name; end
来源：http://vuj.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://aij.svipenyu.cn

[G05] 继承
来源：http://kma.zdbjq.cn

Py:   class Admin(User): pass
来源：http://iog.yfazqb.com

PHP:  class Admin extends User {}
来源：http://ith.ppjwa.cn

JS:   class Admin extends User {}
来源：http://ihm.nwbrower.top

TS:   class Admin extends User {}
来源：http://dkf.shzxlz.cn

Java: class Admin extends User {}
来源：http://rla.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mnh.guannengcc.top

Ruby: class Admin < User; end
来源：http://hvx.yuanzhike.top

C#:   class Admin : User {}
来源：http://vli.yj20258888.top

[G06] 重写方法
来源：http://pou.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://vki.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wzf.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://rni.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://wld.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://sam.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lmi.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://lyo.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://hvq.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://kmr.guannengcc.top

Py:   super().greet()
来源：http://cyh.chenlongwang.top

PHP:  parent::greet();
来源：http://sdj.aibaodan.cn

JS:   super.greet();
来源：http://dfb.guannengcc.top

TS:   super.greet();
来源：http://zjc.svipenyu.cn

Java: super.greet();
来源：http://ayg.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zup.aizwys.cn

Ruby: super
来源：http://syb.fzhhl.top

C#:   base.Greet();
来源：http://vrt.jyoumei.cn

[G08] 静态方法与属性
来源：http://qhh.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qdw.hnxiangtu.top

PHP:  public static function f() {}
来源：http://aqa.yuxming.cn

JS:   static f() {}
来源：http://sea.smart0.xyz

TS:   static f(): void {}
来源：http://vfw.ppjwa.cn

Java: static void f() {}
来源：http://ibp.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ubl.hnqzz.top

Ruby: def self.f; end
来源：http://udm.jiagoushi.top

C#:   public static void F() {}
来源：http://xzg.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://ajy.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://erh.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eas.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xve.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://ljs.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://hlg.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://giu.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nsu.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://pox.jianghu66.top

[G10] 访问控制
来源：http://xfa.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://ulo.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://jym.fktsv.cn

JS:   #private 字段；其余公开
来源：http://oyd.sweek.top

TS:   public / protected / private
来源：http://xol.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://fng.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xks.hesvh.cn

Ruby: public / protected / private
来源：http://jqn.gotoacloud.top

C#:   public / protected / private / internal
来源：http://apw.hywenlv.cn

[G11] getter / setter
来源：http://eed.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://rhr.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sgv.nwbrower.top

JS:   get name() { return this._name; }
来源：http://ejo.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://ymx.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://hrp.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fko.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://mow.smart0.xyz

C#:   public string Name { get; set; }
来源：http://itu.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://bad.316326.xyz

Py:   def __str__(self): return self.name
来源：http://uob.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://cxp.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://prr.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://xot.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://fxb.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iax.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://rss.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://qin.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://zxq.sysykeji.top

Py:   isinstance(u, User)
来源：http://ket.xinyue.icu

PHP:  $u instanceof User
来源：http://anr.ydjk.org.cn

JS:   u instanceof User
来源：http://lgw.jinghuilouyu.cn

TS:   u instanceof User
来源：http://tjl.aizwys.cn

Java: u instanceof User
来源：http://mwp.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eff.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://zyu.vqdsnc.cn

C#:   u is User
来源：http://ohz.zycfv.cn

[G14] 数据类 / record
来源：http://gah.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dwj.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://soi.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qjm.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://zrw.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://axn.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://pzl.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qsf.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://oez.zhiwuduotai.top

[G15] 枚举
来源：http://fqb.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://goy.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mjj.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://egb.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pgu.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://cvb.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lqg.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://xif.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://abx.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://ixm.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gwo.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://qes.tanke756.top

JS:   Object.entries(obj)
来源：http://xat.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://dzk.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wfp.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pme.gzhubu.top

Ruby: obj.instance_variables
来源：http://nip.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://lcy.xuetiantiany.cn

================================================================================
来源：http://tyk.zdqjudy.top

H. 异常与错误处理
来源：http://piu.tian-w.cn

================================================================================
来源：http://jdz.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://ukl.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vcn.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yfr.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qng.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ppz.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bor.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wqa.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://buk.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wxt.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://sui.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ihk.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ulz.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://wmf.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zfz.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cmx.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://psy.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ieu.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dbk.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://ygl.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://mpl.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vrs.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://syg.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://rgh.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ndn.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rea.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://cxl.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ars.xinyue.icu

[H04] 自定义异常类型
来源：http://gbr.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://oiy.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://txv.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://qar.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://bvy.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://ekz.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bgx.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://oad.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://ajl.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://dtv.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://ahh.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zvd.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://inz.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://kqg.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://dlv.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gbi.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://gtw.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hvc.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://shh.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://bpx.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://vaa.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://rox.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://zxc.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dlt.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://foe.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://ylx.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://giw.yonumen.top

[H07] 断言
来源：http://hki.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://ycn.haohaochexian.top

PHP:  assert($x > 0);
来源：http://taw.xylfe.cn

JS:   console.assert(x > 0);
来源：http://nbg.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://ahs.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://qma.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gjy.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://etd.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://rnk.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://nnk.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://tpy.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cyn.mhx1999.top

JS:   e.message;  e.stack
来源：http://aon.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cxs.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://zqt.vqdsnc.cn

Go:   err.Error()
来源：http://bur.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://wmk.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://hpp.zhengqikj.top

[H09] 带错误码的异常
来源：http://uyb.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qnt.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oxd.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://efc.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uwo.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mny.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tsm.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://ppi.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cpf.chenzaomai.com

[H10] 资源自动释放
来源：http://rwr.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uxu.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rhw.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://slq.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gzc.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xxx.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://bsj.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zlr.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mve.yfazqb.com

================================================================================
来源：http://gtd.fzhhl.top

I. 正则表达式
来源：http://osz.jqgufenzy.top

================================================================================
来源：http://gqf.sysykeji.top

[I01] 判断是否匹配
来源：http://aov.redwolf501.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://psa.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pzu.wangdashe.top

JS:   /\d+/.test(s)
来源：http://wqy.bbcook.cn

TS:   /\d+/.test(s)
来源：http://fyc.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wqx.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lgt.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://qsi.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dha.bbcook.cn

[I02] 提取所有匹配
来源：http://xjo.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://dbe.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bnu.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oxl.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://cmk.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eco.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://izh.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://kby.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nyl.zhongyouzk.top

[I03] 提取捕获分组
来源：http://tvp.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hus.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://puo.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cyc.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ewt.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://enb.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rgv.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qsk.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tdr.jinqigfzy.top

[I04] 正则替换
来源：http://cqn.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aja.vehdjk.com


<!-- 参考信息 -->