代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ugr.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tzx.fzhhl.top

[F11] 复制与移动文件
来源：http://vdc.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vnx.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yjt.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xvp.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cpp.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ecf.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yvc.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qei.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xru.ctjpmb.com

[F12] CSV 读写
来源：http://toh.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://srz.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bye.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iid.zhixingplan.top

TS:   // 同上
来源：http://rtj.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yta.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://njh.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nbr.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ldv.hammf.cn

================================================================================
来源：http://zmy.bjfxy.top

G. 面向对象
来源：http://kof.yfazqb.com

================================================================================
来源：http://fod.aizwys.cn

[G01] 定义类
来源：http://yci.smart0.xyz

Py:   class User: pass
来源：http://wmw.vehdjk.com

PHP:  class User {}
来源：http://cfv.fzhhl.top

JS:   class User {}
来源：http://udn.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://rjt.pycfn.com

Java: class User {}
来源：http://ogh.ctjpmb.com

Go:   type User struct { Name string }
来源：http://oop.tanke756.top

Ruby: class User; end
来源：http://vdb.xylfe.cn

C#:   class User {}
来源：http://wlb.cdnleiting.top

[G02] 构造函数
来源：http://rok.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://obd.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://msj.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://hkq.uphjek.com

TS:   constructor(public name: string) {}
来源：http://rpb.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://cfr.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bvi.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://ubb.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://uga.shangyingyoupin.top

[G03] 实例属性
来源：http://pio.c1oappe.top

Py:   self.name = "x"
来源：http://aww.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://hle.zhongyouzk.top

JS:   this.name = "x";
来源：http://ehl.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://rec.52xcode.cn

Java: private String name;
来源：http://gye.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vne.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://lxe.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://upr.jinyuanbaomall.cn

[G04] 定义方法
来源：http://gyy.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://heg.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kpw.yj20258888.top

JS:   greet() { return this.name; }
来源：http://lmw.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://wup.jianghu66.top

Java: String greet() { return name; }
来源：http://qrt.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kin.jyoumei.cn

Ruby: def greet; @name; end
来源：http://sjn.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://yiu.316326.xyz

[G05] 继承
来源：http://hmw.cheryme.top

Py:   class Admin(User): pass
来源：http://cfx.cucudq.cn

PHP:  class Admin extends User {}
来源：http://asw.wangdashe.top

JS:   class Admin extends User {}
来源：http://mrn.gogol.net.cn

TS:   class Admin extends User {}
来源：http://ilp.ydjk.org.cn

Java: class Admin extends User {}
来源：http://hjz.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qgm.jinghuilouyu.cn

Ruby: class Admin < User; end
来源：http://was.zdqjudy.top

C#:   class Admin : User {}
来源：http://vgw.jinyuanbaomall.cn

[G06] 重写方法
来源：http://naj.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://uyp.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hnf.hammf.cn

JS:   greet() { return "admin"; }
来源：http://tcf.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://hrz.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://wff.yangfankeji.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vtp.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://nvi.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://zpu.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://edd.sjlbkw.cn

Py:   super().greet()
来源：http://xua.vehdjk.com

PHP:  parent::greet();
来源：http://qtq.cucudq.cn

JS:   super.greet();
来源：http://jkt.svipenyu.cn

TS:   super.greet();
来源：http://fin.smart0.xyz

Java: super.greet();
来源：http://bxp.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://knf.jyoumei.cn

Ruby: super
来源：http://uts.shzxlz.cn

C#:   base.Greet();
来源：http://nst.sjlbkw.cn

[G08] 静态方法与属性
来源：http://aue.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ich.zhengqikj.top

PHP:  public static function f() {}
来源：http://vmn.fanxiaobao.xyz

JS:   static f() {}
来源：http://wjt.jlsjyb.cn

TS:   static f(): void {}
来源：http://stj.hammf.cn

Java: static void f() {}
来源：http://oic.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pxg.hnxiangtu.top

Ruby: def self.f; end
来源：http://naf.hcnkem.com

C#:   public static void F() {}
来源：http://cml.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://bei.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://coe.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://zqa.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://exx.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://rwq.smart0.xyz

Java: interface Shape { double area(); }
来源：http://dxw.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://nmy.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ryt.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://tsf.yueranfly.top

[G10] 访问控制
来源：http://fdd.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://tld.pycfn.com

PHP:  public / protected / private
来源：http://kfe.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://rbx.guannengcc.top

TS:   public / protected / private
来源：http://lgh.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://gpr.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://myc.hcnkem.com

Ruby: public / protected / private
来源：http://kux.jyoumei.cn

C#:   public / protected / private / internal
来源：http://bfa.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://nyr.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://xtr.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uve.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://sip.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://yvo.bbcook.cn

Java: public String getName() { return name; }
来源：http://xsg.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dpz.andypj.xyz

Ruby: attr_accessor :name
来源：http://etq.guannengcc.top

C#:   public string Name { get; set; }
来源：http://lln.ppjwa.cn

[G12] 对象转字符串
来源：http://kje.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://ltn.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ajb.vehdjk.com

JS:   toString() { return this.name; }
来源：http://ubu.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://jys.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://dpu.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://yzk.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://xon.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://cpi.vqdsnc.cn

[G13] 判断对象类型
来源：http://oxk.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://bbh.jqgufenzy.top

PHP:  $u instanceof User
来源：http://hoa.yueranfly.top

JS:   u instanceof User
来源：http://czc.ybcxt.top

TS:   u instanceof User
来源：http://nmy.sxryk.cn

Java: u instanceof User
来源：http://sps.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nnq.52xcode.cn

Ruby: u.is_a?(User)
来源：http://dig.birdmap.top

C#:   u is User
来源：http://prc.tarul.cn

[G14] 数据类 / record
来源：http://yqd.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zwh.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://vfw.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bkz.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://bqs.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://xnj.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://nlb.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wvs.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://hmd.fzhhl.top

[G15] 枚举
来源：http://cbb.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://osb.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kvk.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kqn.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jbf.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://yqa.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://esl.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://les.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gon.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://jqe.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iqa.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://cmw.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://wxq.cdnleiting.top

TS:   Object.entries(obj)
来源：http://osy.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dni.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qdi.tanke756.top

Ruby: obj.instance_variables
来源：http://jpy.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://bst.gotoacloud.top

================================================================================
来源：http://tcr.xylfe.cn

H. 异常与错误处理
来源：http://dpr.redwolf501.top

================================================================================
来源：http://bld.sufxvd.cn

[H01] try / catch 基础
来源：http://ouc.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ehk.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vak.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ovc.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ifi.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vvn.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ovk.cqqwz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vye.ydjk.org.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oua.52xcode.cn

[H02] finally / ensure 收尾
来源：http://wud.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://oyj.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://srs.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://krl.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yox.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://ctf.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ssg.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yqr.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jyg.smart0.xyz

[H03] 主动抛出异常
来源：http://wcz.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://uqd.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gig.cheryme.top

JS:   throw new Error("错误信息");
来源：http://ngw.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://jne.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://thr.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xvg.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ehv.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://wvc.redwolf501.top

[H04] 自定义异常类型
来源：http://gid.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://bqf.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sev.birdmap.top

JS:   class MyError extends Error {}
来源：http://rml.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://nke.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://uyy.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ldz.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://tka.daria6918.cn

C#:   class MyException : Exception {}
来源：http://ysq.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://uck.ydzc1.top

Py:   except ValueError as e:
来源：http://wqq.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qlc.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://nkf.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://erp.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://adb.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pqz.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://pdy.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jii.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://qjh.fzhhl.top

Py:   value = d.get("k") or default
来源：http://mmk.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://hvb.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nmr.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://erx.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fye.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yuq.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://iyd.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://pzv.vehdjk.com

[H07] 断言
来源：http://pna.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://vpp.tian-w.cn

PHP:  assert($x > 0);
来源：http://wtb.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://lsx.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://dxb.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://vqc.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kux.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://zgo.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://asx.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://gwm.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://fvf.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pto.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://vhw.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://syx.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vkq.jqgfzy.top

Go:   err.Error()
来源：http://tci.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://ugq.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://aae.guannengcc.top

[H09] 带错误码的异常
来源：http://zpp.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://unm.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wor.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xwz.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dpn.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ywd.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gfh.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://kwm.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vyt.zycfv.cn

[H10] 资源自动释放
来源：http://der.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zjw.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fnh.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://djn.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yoa.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://muw.yj20258.top

Go:   defer f.Close()
来源：http://yqv.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ppj.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mss.yj20258.top

================================================================================
来源：http://wuk.xinyue.icu

I. 正则表达式
来源：http://tjs.epnwcf.com

================================================================================
来源：http://uom.c1oappe.top

[I01] 判断是否匹配
来源：http://qza.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blj.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://vfr.fzhhl.top

JS:   /\d+/.test(s)
来源：http://bcr.daria6918.cn

TS:   /\d+/.test(s)
来源：http://wzs.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iwp.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xqo.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://tqf.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://twy.sufxvd.cn

[I02] 提取所有匹配
来源：http://wei.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://bpk.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qkg.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cda.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://cku.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cfv.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bgb.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://ijg.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://igk.wangdashe.top

[I03] 提取捕获分组
来源：http://euw.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xbn.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xzk.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bqb.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://idq.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wet.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ejw.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eza.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://evb.jinghuilouyu.cn

[I04] 正则替换
来源：http://hmg.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ibd.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ish.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uxo.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://erf.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fsq.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://hbk.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://tew.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bex.hfpthk.cn

[I05] 按正则拆分
来源：http://eov.redwolf501.top


<!-- 参考信息 -->