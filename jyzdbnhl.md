代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jxf.hnqzz.top

TS:   path.extname("a.txt")
来源：http://abm.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lvu.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nsg.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nnx.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zxi.xinyue.icu

[F11] 复制与移动文件
来源：http://tib.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nqk.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ptc.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pfu.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ncm.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wsy.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wkq.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://clh.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://scf.xuetiantiany.cn

[F12] CSV 读写
来源：http://rzu.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ysm.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hca.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hrz.jqgufenzy.top

TS:   // 同上
来源：http://lcv.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iwe.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uly.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rml.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xwl.ctjpmb.com

================================================================================
来源：http://csk.feifeiyinyue.top

G. 面向对象
来源：http://crr.yfazqb.com

================================================================================
来源：http://mvm.hnxiangtu.top

[G01] 定义类
来源：http://ptg.yj202588.top

Py:   class User: pass
来源：http://apw.yj20258.top

PHP:  class User {}
来源：http://flr.meibo888.top

JS:   class User {}
来源：http://izm.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://veq.c1oappe.top

Java: class User {}
来源：http://vij.vqdsnc.cn

Go:   type User struct { Name string }
来源：http://ycx.gotoacloud.top

Ruby: class User; end
来源：http://jyp.svipenyu.cn

C#:   class User {}
来源：http://xfw.yfazqb.com

[G02] 构造函数
来源：http://uwd.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://elh.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://nad.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://rih.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://lqn.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://tlp.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baw.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://mvm.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://tgh.bjfxy.top

[G03] 实例属性
来源：http://swh.svipenyu.cn

Py:   self.name = "x"
来源：http://slt.hfpthk.cn

PHP:  public string $name = "x";
来源：http://vqw.pycfn.com

JS:   this.name = "x";
来源：http://mbw.xuetiantiany.cn

TS:   name: string = "x";
来源：http://kpy.tanke756.top

Java: private String name;
来源：http://dlq.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://abv.jqgfzy.top

Ruby: @name = "x"
来源：http://hvn.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://aid.zdqjudy.top

[G04] 定义方法
来源：http://fer.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://ybe.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ven.yj20258888.top

JS:   greet() { return this.name; }
来源：http://vbo.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://xei.yj202588.top

Java: String greet() { return name; }
来源：http://cau.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ksm.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://vqs.pycfn.com

C#:   public string Greet() => Name;
来源：http://cog.bbcook.cn

[G05] 继承
来源：http://ajw.uphjek.com

Py:   class Admin(User): pass
来源：http://flp.xinyue.icu

PHP:  class Admin extends User {}
来源：http://mzi.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://kve.yonumen.top

TS:   class Admin extends User {}
来源：http://zur.316326.xyz

Java: class Admin extends User {}
来源：http://zwp.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xcb.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://hii.kuanghao11.cn

C#:   class Admin : User {}
来源：http://jey.shanyushiyangtech.top

[G06] 重写方法
来源：http://fah.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://xfx.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ldf.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://wmb.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://iyc.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://cjn.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ltp.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://usz.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://zjh.ehwqpu.com

[G07] 调用父类方法
来源：http://xuc.zdbjq.cn

Py:   super().greet()
来源：http://owc.yj20258888.top

PHP:  parent::greet();
来源：http://tdq.yonumen.top

JS:   super.greet();
来源：http://jlm.yfazqb.com

TS:   super.greet();
来源：http://qsl.vqdsnc.cn

Java: super.greet();
来源：http://obq.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bbq.hammf.cn

Ruby: super
来源：http://xye.cheryme.top

C#:   base.Greet();
来源：http://ffw.yfazqb.com

[G08] 静态方法与属性
来源：http://oxm.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tlx.jlsjyb.cn

PHP:  public static function f() {}
来源：http://gpr.gotoacloud.top

JS:   static f() {}
来源：http://enz.jianghu66.top

TS:   static f(): void {}
来源：http://jft.jinqigfzy.top

Java: static void f() {}
来源：http://ewa.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oyl.jinqigufen.top

Ruby: def self.f; end
来源：http://grp.tarul.cn

C#:   public static void F() {}
来源：http://ofc.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://mww.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://pjp.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sbh.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fnf.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://gsf.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://irg.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://pzq.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ifv.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://hfl.hongshengwenyu.top

[G10] 访问控制
来源：http://lip.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://zry.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://tgf.bjfxy.top

JS:   #private 字段；其余公开
来源：http://gki.jinqigfzy.top

TS:   public / protected / private
来源：http://zqt.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://okh.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fmh.fehbvm.com

Ruby: public / protected / private
来源：http://dpc.9152youxi.cn

C#:   public / protected / private / internal
来源：http://ehh.ivvv.top

[G11] getter / setter
来源：http://cjv.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://zsa.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qmf.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://jgp.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://oap.daxiang520.top

Java: public String getName() { return name; }
来源：http://kjo.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cci.ydzc1.top

Ruby: attr_accessor :name
来源：http://srb.52xcode.cn

C#:   public string Name { get; set; }
来源：http://rvi.fktsv.cn

[G12] 对象转字符串
来源：http://beb.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://noy.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://tfs.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://jkz.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://nqm.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://jbc.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://tjw.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://jsz.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://viz.fktsv.cn

[G13] 判断对象类型
来源：http://vwp.dianchejie.cn

Py:   isinstance(u, User)
来源：http://ktf.smart0.xyz

PHP:  $u instanceof User
来源：http://rtm.hnqzz.top

JS:   u instanceof User
来源：http://jpg.dianchejie.cn

TS:   u instanceof User
来源：http://ocg.xziqi.cn

Java: u instanceof User
来源：http://tby.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wbp.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://hti.jianghu66.top

C#:   u is User
来源：http://uyx.fehbvm.com

[G14] 数据类 / record
来源：http://nkm.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pfe.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://lsb.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://sxe.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://yus.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://jdr.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://zup.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eny.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://vfs.ehwqpu.com

[G15] 枚举
来源：http://qta.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ljk.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ikk.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fzp.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vki.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://jht.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kvi.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://oav.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xau.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://pfz.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rjt.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://pzp.yfazqb.com

JS:   Object.entries(obj)
来源：http://ilu.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://qfa.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vjm.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uul.ppjwa.cn

Ruby: obj.instance_variables
来源：http://tzh.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://knv.jinqigfzy.top

================================================================================
来源：http://tcl.hnxiangtu.top

H. 异常与错误处理
来源：http://bqy.shuidangran.top

================================================================================
来源：http://cci.haohaochexian.top

[H01] try / catch 基础
来源：http://tae.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eka.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fde.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bho.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nwt.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://agi.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://znu.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dgf.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ogx.52xcode.cn

[H02] finally / ensure 收尾
来源：http://nsv.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eaj.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://boe.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pvi.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xbr.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gil.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wux.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wjd.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://etr.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://byt.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://zpi.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://acd.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://ehk.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://ogl.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pnx.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nnu.quarkkingdee.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cqd.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://flv.nanxuanxn.top

[H04] 自定义异常类型
来源：http://ijk.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://yqk.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dtp.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://wcw.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://uhf.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://omi.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://otg.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://qkv.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://gow.ydjk.org.cn

[H05] 捕获特定类型
来源：http://uyi.zhoulong.xyz

Py:   except ValueError as e:
来源：http://kjv.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dnh.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://keq.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://gfu.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://jga.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wzs.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://juo.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jyj.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://tlr.bjfxy.top

Py:   value = d.get("k") or default
来源：http://yug.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://dfe.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://amq.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://lrg.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xpv.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mhd.yanxiufei.cn

Ruby: d&.dig(:a, :b)
来源：http://ktg.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://osd.xziqi.cn

[H07] 断言
来源：http://aei.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://xby.yj20258888.top

PHP:  assert($x > 0);
来源：http://xsz.fengsongda.top

JS:   console.assert(x > 0);
来源：http://pek.c1oappe.top

TS:   console.assert(x > 0);
来源：http://avp.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://mcd.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pob.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://sjh.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://mmk.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://tlr.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://dvi.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://azz.andypj.xyz

JS:   e.message;  e.stack
来源：http://sqb.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://exv.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wwv.shanyushiyangkeji.top

Go:   err.Error()
来源：http://isx.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://yrp.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://kbt.jinqigfzy.top

[H09] 带错误码的异常
来源：http://hre.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://plf.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sdw.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lpj.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://frs.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rtg.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fgh.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tld.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cnc.cdnleiting.top

[H10] 资源自动释放
来源：http://sgt.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ubb.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wzl.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vqm.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://opg.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zed.zhiwuduotai.top

Go:   defer f.Close()
来源：http://urb.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ost.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ros.xingfuxueyuan.xyz

================================================================================
来源：http://kgx.zhengqikj.top

I. 正则表达式
来源：http://xyi.shangyingyoupin.top

================================================================================
来源：http://yzu.cheryme.top

[I01] 判断是否匹配
来源：http://vlo.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yfw.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://inb.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://zsh.316326.xyz

TS:   /\d+/.test(s)
来源：http://thu.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uff.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qcw.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://jwu.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eqv.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://vzt.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://hkz.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sem.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zra.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://tmu.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cov.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://etk.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://saf.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://npv.jinqigufen.top

[I03] 提取捕获分组
来源：http://ryf.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lzr.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vfb.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pdo.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fhx.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bny.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rtg.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tkd.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gmv.ybcxt.top

[I04] 正则替换
来源：http://dar.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lor.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rue.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gwf.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qex.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://ljy.yueranfly.top


<!-- 参考信息 -->