代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pdd.ivvv.top

TS:   path.extname("a.txt")
来源：http://yem.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cdr.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://isq.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://awn.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yya.tianlin.xyz

[F11] 复制与移动文件
来源：http://arj.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zyy.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://veo.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pzy.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fjl.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tqc.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aqx.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mjg.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cdf.nanxinkj.top

[F12] CSV 读写
来源：http://ptf.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://osj.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nrp.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vvx.ydjk.org.cn

TS:   // 同上
来源：http://afx.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cew.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jvx.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pvs.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ofw.hnqzz.top

================================================================================
来源：http://vxu.chenlongwang.top

G. 面向对象
来源：http://snm.epnwcf.com

================================================================================
来源：http://eav.shangyingyoupin.top

[G01] 定义类
来源：http://ixh.fzhhl.top

Py:   class User: pass
来源：http://xst.hfpthk.cn

PHP:  class User {}
来源：http://wta.gogol.net.cn

JS:   class User {}
来源：http://owk.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://ets.jyoumei.cn

Java: class User {}
来源：http://juc.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://aof.jiagoushi.top

Ruby: class User; end
来源：http://vat.havefunace.top

C#:   class User {}
来源：http://bxq.mhx1999.top

[G02] 构造函数
来源：http://vne.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://xgt.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://pzt.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://dqa.birdmap.top

TS:   constructor(public name: string) {}
来源：http://itt.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://gxv.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vrp.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://icy.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://luv.nanxinkj.top

[G03] 实例属性
来源：http://bog.c1oappe.top

Py:   self.name = "x"
来源：http://bnl.xziqi.cn

PHP:  public string $name = "x";
来源：http://ahi.cqqwz.cn

JS:   this.name = "x";
来源：http://pwy.andypj.xyz

TS:   name: string = "x";
来源：http://qeb.gotoacloud.top

Java: private String name;
来源：http://rjv.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jfz.zycfv.cn

Ruby: @name = "x"
来源：http://uvk.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://ahu.uphjek.com

[G04] 定义方法
来源：http://qik.nwbrower.top

Py:   def greet(self): return self.name
来源：http://bqi.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ayz.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://szg.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://pxp.zhixingplan.top

Java: String greet() { return name; }
来源：http://fti.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://olf.andypj.xyz

Ruby: def greet; @name; end
来源：http://hnz.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://iie.zycfv.cn

[G05] 继承
来源：http://czv.hysaishi.cn

Py:   class Admin(User): pass
来源：http://inf.pycfn.com

PHP:  class Admin extends User {}
来源：http://bal.wangdashe.top

JS:   class Admin extends User {}
来源：http://twb.uphjek.com

TS:   class Admin extends User {}
来源：http://hej.sysykeji.top

Java: class Admin extends User {}
来源：http://fxh.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xig.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://uxk.chenzaomai.com

C#:   class Admin : User {}
来源：http://aid.wangshuangyany.cn

[G06] 重写方法
来源：http://rdn.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://qfp.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rvl.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://qov.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://zqa.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://idt.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://emf.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://ulj.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://edy.quarkkingdee.top

[G07] 调用父类方法
来源：http://jyz.sweek.top

Py:   super().greet()
来源：http://poi.jinqigufen.top

PHP:  parent::greet();
来源：http://pck.gaohongyu789.top

JS:   super.greet();
来源：http://ltg.andypj.xyz

TS:   super.greet();
来源：http://tru.yvedp.cn

Java: super.greet();
来源：http://euz.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sxo.sufxvd.cn

Ruby: super
来源：http://laj.shangyingyoupin.top

C#:   base.Greet();
来源：http://gpo.yj20258888.top

[G08] 静态方法与属性
来源：http://vae.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xgh.xylfe.cn

PHP:  public static function f() {}
来源：http://mvt.quarkkingdee.top

JS:   static f() {}
来源：http://jbj.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://irn.gzhubu.top

Java: static void f() {}
来源：http://ayi.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fsy.ehwqpu.com

Ruby: def self.f; end
来源：http://pif.yuxming.cn

C#:   public static void F() {}
来源：http://xsg.hammf.cn

[G09] 接口 / 抽象类
来源：http://dsk.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://aee.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://fla.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://aux.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://ojl.bjfxy.top

Java: interface Shape { double area(); }
来源：http://kut.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://yfi.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kpw.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://mpp.hammf.cn

[G10] 访问控制
来源：http://wyh.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://xxv.tianlin.xyz

PHP:  public / protected / private
来源：http://ixh.mhx1999.top

JS:   #private 字段；其余公开
来源：http://hxt.smart0.xyz

TS:   public / protected / private
来源：http://ocg.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://bno.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cip.epnwcf.com

Ruby: public / protected / private
来源：http://luh.tian-w.cn

C#:   public / protected / private / internal
来源：http://tuh.hcnkem.com

[G11] getter / setter
来源：http://zye.xinyue.icu

Py:   @property 与 @x.setter
来源：http://gov.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://phr.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://yhn.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://cra.iojbl.cn

Java: public String getName() { return name; }
来源：http://cvk.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kav.ctjpmb.com

Ruby: attr_accessor :name
来源：http://ore.nwbrower.top

C#:   public string Name { get; set; }
来源：http://uqf.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://ara.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://lzi.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rle.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://jbl.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://bzg.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://ode.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://vrt.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://vtt.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://ily.guannengcc.top

[G13] 判断对象类型
来源：http://xdp.cashguo.top

Py:   isinstance(u, User)
来源：http://hfa.tian-w.cn

PHP:  $u instanceof User
来源：http://psf.tian-w.cn

JS:   u instanceof User
来源：http://qct.feifeiyinyue.top

TS:   u instanceof User
来源：http://xuf.yj202588.top

Java: u instanceof User
来源：http://mvv.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://fsa.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://skr.bjfxy.top

C#:   u is User
来源：http://jio.bbcook.cn

[G14] 数据类 / record
来源：http://yam.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://odl.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://uqu.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://uyz.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://sun.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://xqu.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://hem.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://btl.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://mfs.cqqwz.cn

[G15] 枚举
来源：http://mow.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dnn.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rwo.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://upo.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hhs.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://bps.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ajj.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://wwr.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fga.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://oud.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ilg.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://tzq.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://lgl.nwbrower.top

TS:   Object.entries(obj)
来源：http://les.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bay.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lfv.c1oappe.top

Ruby: obj.instance_variables
来源：http://xuk.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://jcf.pengpengdd.cyou

================================================================================
来源：http://lsa.tarul.cn

H. 异常与错误处理
来源：http://zju.sxryk.cn

================================================================================
来源：http://nam.zhiwuduotai.top

[H01] try / catch 基础
来源：http://ebv.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vwp.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ehr.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pjc.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://amd.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lyl.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eqd.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qfx.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ael.hcnkem.com

[H02] finally / ensure 收尾
来源：http://swt.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dfk.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hnl.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hvq.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tzf.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://xzv.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://djx.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://byf.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lkw.guowangkeji.top

[H03] 主动抛出异常
来源：http://pmd.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://aog.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hxc.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://mcy.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://mgx.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pbj.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://coi.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mye.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://imy.ehwqpu.com

[H04] 自定义异常类型
来源：http://sec.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://smf.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://wdc.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://iqd.cucudq.cn

TS:   class MyError extends Error {}
来源：http://evb.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://sfb.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jzp.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://sqe.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://baz.sjlbkw.cn

[H05] 捕获特定类型
来源：http://uko.tanke756.top

Py:   except ValueError as e:
来源：http://qyh.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kkh.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://due.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://njk.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://czw.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qhc.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://orw.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zcj.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://gnj.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://dts.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://bwh.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://abn.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://wpe.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tip.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uqe.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://tch.sxryk.cn

C#:   obj?.A?.B ?? default
来源：http://ltp.svipenyu.cn

[H07] 断言
来源：http://qqb.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://ajo.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://hwr.andypj.xyz

JS:   console.assert(x > 0);
来源：http://bxr.wangdashe.top

TS:   console.assert(x > 0);
来源：http://oop.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://xzb.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://atn.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cva.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://qvl.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://kyf.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://slc.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ymd.aibaodan.cn

JS:   e.message;  e.stack
来源：http://tcm.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sem.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://guk.andypj.xyz

Go:   err.Error()
来源：http://xkz.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://whe.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://bhe.yj202588.top

[H09] 带错误码的异常
来源：http://bqo.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://spg.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jxh.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xys.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oth.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kle.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hxc.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://jde.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://koz.yongpay.top

[H10] 资源自动释放
来源：http://fbp.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ndp.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hzu.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ktj.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uqn.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://njo.yuxming.cn

Go:   defer f.Close()
来源：http://bem.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gwc.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lha.zdqjudy.top

================================================================================
来源：http://axk.kuanghao11.cn

I. 正则表达式
来源：http://jou.sjlbkw.cn

================================================================================
来源：http://wvz.zhengqikj.top

[I01] 判断是否匹配
来源：http://pbc.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tjo.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mgh.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://osq.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://mci.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zgd.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hkv.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://aos.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iqt.zhixingplan.top

[I02] 提取所有匹配
来源：http://cwb.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://uvn.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://txe.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qmp.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://jdu.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pfg.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ohu.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://ovc.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wdh.sysykeji.top

[I03] 提取捕获分组
来源：http://xcn.svipenyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://slg.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ija.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://osv.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xui.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xba.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://foj.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tvj.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xrd.gzhubu.top

[I04] 正则替换
来源：http://neq.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sgz.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lms.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xfc.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://fzi.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://uaz.birdmap.top


<!-- 参考信息 -->