代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://djk.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://cfb.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://swd.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ent.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fxn.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://etn.quarkkingdee.top

[F11] 复制与移动文件
来源：http://mhe.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://stv.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mqh.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eeh.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfu.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qrv.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vqq.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qem.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zfe.gotoacloud.top

[F12] CSV 读写
来源：http://yan.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sjk.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mrs.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hus.aizwys.cn

TS:   // 同上
来源：http://rlu.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gyb.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://exn.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fji.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://idl.pengpengdd.cyou

================================================================================
来源：http://jtk.fzhhl.top

G. 面向对象
来源：http://urm.fanxiaobao.xyz

================================================================================
来源：http://ftj.shanyushiyangkeji.top

[G01] 定义类
来源：http://chs.zdqjudy.top

Py:   class User: pass
来源：http://qqt.yfazqb.com

PHP:  class User {}
来源：http://tre.chenjidiqi.icu

JS:   class User {}
来源：http://yuf.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://hmd.ctjpmb.com

Java: class User {}
来源：http://lms.snrcjt.cn

Go:   type User struct { Name string }
来源：http://rcz.guowangkeji.top

Ruby: class User; end
来源：http://svn.cdnleiting.top

C#:   class User {}
来源：http://ngz.guowangkeji.top

[G02] 构造函数
来源：http://bfo.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://kun.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://urx.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://itr.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://mcj.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://dsk.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bxm.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://gts.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://lai.aibaodan.cn

[G03] 实例属性
来源：http://edu.c1oappe.top

Py:   self.name = "x"
来源：http://wce.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://gva.316326.xyz

JS:   this.name = "x";
来源：http://tjr.hywenlv.cn

TS:   name: string = "x";
来源：http://euh.hywenlv.cn

Java: private String name;
来源：http://vjk.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pdm.xuanzx.com

Ruby: @name = "x"
来源：http://jzo.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://pit.cucudq.cn

[G04] 定义方法
来源：http://vtp.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://wbd.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ttj.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://wya.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://iwt.316326.xyz

Java: String greet() { return name; }
来源：http://dem.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://ine.sysykeji.top

Ruby: def greet; @name; end
来源：http://kwq.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://taq.tianlin.xyz

[G05] 继承
来源：http://cyr.cucudq.cn

Py:   class Admin(User): pass
来源：http://yje.bjfxy.top

PHP:  class Admin extends User {}
来源：http://cds.52xcode.cn

JS:   class Admin extends User {}
来源：http://kfv.fktsv.cn

TS:   class Admin extends User {}
来源：http://afb.wangdashe.top

Java: class Admin extends User {}
来源：http://lhj.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tpy.sweek.top

Ruby: class Admin < User; end
来源：http://wew.vehdjk.com

C#:   class Admin : User {}
来源：http://tle.tian-w.cn

[G06] 重写方法
来源：http://iis.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://mfk.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://byp.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://xds.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://rln.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://umv.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ogh.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://bxj.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://hvi.zhengqikj.top

[G07] 调用父类方法
来源：http://jyx.fehbvm.com

Py:   super().greet()
来源：http://mim.epnwcf.com

PHP:  parent::greet();
来源：http://dyp.quarkkingdee.top

JS:   super.greet();
来源：http://cls.zdbjq.cn

TS:   super.greet();
来源：http://fxq.nanxuanxn.top

Java: super.greet();
来源：http://vwx.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uni.daxiang520.top

Ruby: super
来源：http://ios.pycfn.com

C#:   base.Greet();
来源：http://rgp.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://mix.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nuv.jyoumei.cn

PHP:  public static function f() {}
来源：http://jtb.hnxiangtu.top

JS:   static f() {}
来源：http://dyu.hongshengwenyu.top

TS:   static f(): void {}
来源：http://znz.andypj.xyz

Java: static void f() {}
来源：http://byf.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cmv.jinqigfzy.top

Ruby: def self.f; end
来源：http://utf.hysaishi.cn

C#:   public static void F() {}
来源：http://fxf.yfazqb.com

[G09] 接口 / 抽象类
来源：http://jeb.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://fek.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://rtv.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://imo.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://chf.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://lkr.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://smk.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://syg.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://hxa.sufxvd.cn

[G10] 访问控制
来源：http://lvr.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://zrv.ydjk.org.cn

PHP:  public / protected / private
来源：http://cqc.xziqi.cn

JS:   #private 字段；其余公开
来源：http://ewl.zdbjq.cn

TS:   public / protected / private
来源：http://hnv.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://xkh.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tbg.jiagoushi.top

Ruby: public / protected / private
来源：http://rjx.yongpay.top

C#:   public / protected / private / internal
来源：http://wpl.hysaishi.cn

[G11] getter / setter
来源：http://efu.c1oappe.top

Py:   @property 与 @x.setter
来源：http://nqc.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gji.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://xgg.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://sct.zhengqikj.top

Java: public String getName() { return name; }
来源：http://bll.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://knv.daria6918.cn

Ruby: attr_accessor :name
来源：http://mgh.xinyue.icu

C#:   public string Name { get; set; }
来源：http://haf.tian-w.cn

[G12] 对象转字符串
来源：http://xor.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://hbw.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ixj.bjfxy.top

JS:   toString() { return this.name; }
来源：http://bub.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://qll.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://jht.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gpo.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://nlv.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://ihc.tian-w.cn

[G13] 判断对象类型
来源：http://ngv.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://sqz.chenlongwang.top

PHP:  $u instanceof User
来源：http://oer.uphjek.com

JS:   u instanceof User
来源：http://pkb.andypj.xyz

TS:   u instanceof User
来源：http://mav.jyoumei.cn

Java: u instanceof User
来源：http://fvc.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qdn.zhiwuduotai.top

Ruby: u.is_a?(User)
来源：http://irb.cqqwz.cn

C#:   u is User
来源：http://kdj.yj20258888.top

[G14] 数据类 / record
来源：http://wce.zhongyouzk.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kgy.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://lwm.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://ynu.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://rtu.xziqi.cn

Java: record User(String name, int age) {}
来源：http://yvz.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://cus.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vow.jinghuilouyu.cn

C#:   record User(string Name, int Age);
来源：http://agv.tanke756.top

[G15] 枚举
来源：http://qsq.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vud.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gjl.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dza.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bbe.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://kle.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rni.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://lyp.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fjg.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://vxs.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hsu.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://wnk.ctjpmb.com

JS:   Object.entries(obj)
来源：http://lxv.ydzc1.top

TS:   Object.entries(obj)
来源：http://msm.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tid.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dob.zhixingplan.top

Ruby: obj.instance_variables
来源：http://adc.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://qad.shuidangran.top

================================================================================
来源：http://hrt.jqgfzy.top

H. 异常与错误处理
来源：http://nez.tanke756.top

================================================================================
来源：http://kom.hnqzz.top

[H01] try / catch 基础
来源：http://jha.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mhm.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vkp.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xcp.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pbp.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mlz.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mtx.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fxz.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yzo.yj20258.top

[H02] finally / ensure 收尾
来源：http://jnx.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hzp.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fom.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nnp.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://lit.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://zww.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://kne.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tiv.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fwd.hfpthk.cn

[H03] 主动抛出异常
来源：http://avm.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://jgg.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tja.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://oqg.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://ivj.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://pfr.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yix.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://msw.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rko.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://hda.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://nsr.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://irg.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://wnn.iojbl.cn

TS:   class MyError extends Error {}
来源：http://tjk.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://qho.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dkr.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://suj.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://aiz.shzxlz.cn

[H05] 捕获特定类型
来源：http://egj.jinqigfzy.top

Py:   except ValueError as e:
来源：http://znj.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cdd.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://pqj.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://ugd.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://cao.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wvy.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://zir.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kfn.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://fvy.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://avc.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://qqg.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ubo.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mkt.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iwu.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yku.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://lhv.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://yjm.pengpengdd.cyou

[H07] 断言
来源：http://mbk.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://ccm.cdnleiting.top

PHP:  assert($x > 0);
来源：http://ncj.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://voe.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://pyy.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://rqu.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zzb.yuanzhike.top

Ruby: raise "必须为正" unless x > 0
来源：http://raq.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://huy.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://noo.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://qar.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fyr.hesvh.cn

JS:   e.message;  e.stack
来源：http://nmo.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cwq.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lei.yueranfly.top

Go:   err.Error()
来源：http://hwz.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://ovx.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://oxb.chenzaomai.com

[H09] 带错误码的异常
来源：http://dzu.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tln.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cbf.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rqy.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://egf.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tbn.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hpz.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://lzc.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xzv.yonumen.top

[H10] 资源自动释放
来源：http://mns.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://prb.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iti.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cdn.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hjw.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mwp.ctjpmb.com

Go:   defer f.Close()
来源：http://rgk.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gju.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://stx.9152youxi.cn

================================================================================
来源：http://eib.zhixingplan.top

I. 正则表达式
来源：http://vya.shanyushiyangkeji.top

================================================================================
来源：http://cdb.nanxinkj.top

[I01] 判断是否匹配
来源：http://iwe.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ham.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://iad.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://ukh.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://cps.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xnj.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ldf.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://liz.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uwt.316326.xyz

[I02] 提取所有匹配
来源：http://vac.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://yib.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bdv.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rky.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://zts.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lmq.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://akq.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://wju.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://euc.cheryme.top

[I03] 提取捕获分组
来源：http://tgq.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fjz.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wee.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kbg.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dqc.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wdo.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xrv.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bfc.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ixw.pengpengdd.cyou

[I04] 正则替换
来源：http://ies.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jps.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://twk.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qbu.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://opy.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://myz.ybcxt.top


<!-- 参考信息 -->