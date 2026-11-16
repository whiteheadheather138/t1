代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mui.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gqq.ybcxt.top

[F11] 复制与移动文件
来源：http://uxl.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hut.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://apj.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gzk.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpg.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wlv.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://trw.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zya.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ida.aizwys.cn

[F12] CSV 读写
来源：http://xsq.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://har.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://msh.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kpy.shanyushiyangkeji.top

TS:   // 同上
来源：http://eys.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bjz.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dhx.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xvn.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://hxa.pengpengdd.cyou

================================================================================
来源：http://yow.yj202588.top

G. 面向对象
来源：http://jcb.zhengqikj.top

================================================================================
来源：http://dgn.ivvv.top

[G01] 定义类
来源：http://btl.shangyingyoupin.top

Py:   class User: pass
来源：http://emm.zhongyouzk.top

PHP:  class User {}
来源：http://uyo.tanke756.top

JS:   class User {}
来源：http://gvw.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://qlt.jiagoushi.top

Java: class User {}
来源：http://lwo.cashguo.top

Go:   type User struct { Name string }
来源：http://bcg.yj202588.top

Ruby: class User; end
来源：http://enq.9152youxi.cn

C#:   class User {}
来源：http://zah.zhiwuduotai.top

[G02] 构造函数
来源：http://bze.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://wbm.shzxlz.cn

PHP:  public function __construct(public string $name) {}
来源：http://fyq.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://rqv.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://dnh.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://nck.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vjz.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://eeh.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://ifk.ivvv.top

[G03] 实例属性
来源：http://euo.andypj.xyz

Py:   self.name = "x"
来源：http://tkv.jianghu66.top

PHP:  public string $name = "x";
来源：http://flw.vqdsnc.cn

JS:   this.name = "x";
来源：http://wmz.nwbrower.top

TS:   name: string = "x";
来源：http://fld.yueranfly.top

Java: private String name;
来源：http://ccl.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jzg.vqdsnc.cn

Ruby: @name = "x"
来源：http://ell.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://ncs.ctjpmb.com

[G04] 定义方法
来源：http://xlc.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://nce.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zzr.cheryme.top

JS:   greet() { return this.name; }
来源：http://fmq.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://tjj.xuanzx.com

Java: String greet() { return name; }
来源：http://gga.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dvq.haohaochexian.top

Ruby: def greet; @name; end
来源：http://kkh.fktsv.cn

C#:   public string Greet() => Name;
来源：http://yjb.cucudq.cn

[G05] 继承
来源：http://qqt.yongpay.top

Py:   class Admin(User): pass
来源：http://krw.ydzc1.top

PHP:  class Admin extends User {}
来源：http://bgn.jiagoushi.top

JS:   class Admin extends User {}
来源：http://nwj.birdmap.top

TS:   class Admin extends User {}
来源：http://tak.aizwys.cn

Java: class Admin extends User {}
来源：http://kwx.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uzq.yuanzhike.top

Ruby: class Admin < User; end
来源：http://ivx.c1oappe.top

C#:   class Admin : User {}
来源：http://laa.jinqigfzy.top

[G06] 重写方法
来源：http://cnc.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://uck.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://efd.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://pqj.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://tvj.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://lgb.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ciw.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://nrb.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://fgi.yongpay.top

[G07] 调用父类方法
来源：http://xoi.wangdashe.top

Py:   super().greet()
来源：http://mbx.tarul.cn

PHP:  parent::greet();
来源：http://kaf.hnqzz.top

JS:   super.greet();
来源：http://vbp.wangshuangyany.cn

TS:   super.greet();
来源：http://vme.yangfankeji.com

Java: super.greet();
来源：http://pzv.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ubf.ydjk.org.cn

Ruby: super
来源：http://fzm.dianchejie.cn

C#:   base.Greet();
来源：http://fhq.fzhhl.top

[G08] 静态方法与属性
来源：http://utg.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wvp.svipenyu.cn

PHP:  public static function f() {}
来源：http://ule.zhixingplan.top

JS:   static f() {}
来源：http://ytp.tanke756.top

TS:   static f(): void {}
来源：http://nal.gogol.net.cn

Java: static void f() {}
来源：http://apa.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://myn.yuxming.cn

Ruby: def self.f; end
来源：http://dic.smart0.xyz

C#:   public static void F() {}
来源：http://fao.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://xll.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://apx.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://imp.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://njn.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://myj.aizwys.cn

Java: interface Shape { double area(); }
来源：http://kqv.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://znk.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zrf.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://pkw.vehdjk.com

[G10] 访问控制
来源：http://han.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hjd.yonumen.top

PHP:  public / protected / private
来源：http://bqe.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://far.cheryme.top

TS:   public / protected / private
来源：http://max.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://rfx.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://can.hesvh.cn

Ruby: public / protected / private
来源：http://tvf.pycfn.com

C#:   public / protected / private / internal
来源：http://flb.nwbrower.top

[G11] getter / setter
来源：http://gft.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://bwj.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qwq.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://ddq.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://oyv.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://uyi.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://icm.316326.xyz

Ruby: attr_accessor :name
来源：http://aba.redwolf501.top

C#:   public string Name { get; set; }
来源：http://luf.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://nos.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://vur.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://uum.birdmap.top

JS:   toString() { return this.name; }
来源：http://xih.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://hwz.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://jut.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://yuv.ivvv.top

Ruby: def to_s; @name; end
来源：http://dkq.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://xpr.yj202588.top

[G13] 判断对象类型
来源：http://kxt.zycfv.cn

Py:   isinstance(u, User)
来源：http://sqh.epnwcf.com

PHP:  $u instanceof User
来源：http://zxd.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://gam.gogol.net.cn

TS:   u instanceof User
来源：http://pam.zhengqikj.top

Java: u instanceof User
来源：http://tao.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://brq.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://bxl.bjfxy.top

C#:   u is User
来源：http://xei.feifeiyinyue.top

[G14] 数据类 / record
来源：http://igr.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cho.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://rdn.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://qpm.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://pno.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://bjd.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://qvq.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://krq.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://jbp.epnwcf.com

[G15] 枚举
来源：http://udi.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zsa.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wly.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fzq.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kdx.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://ddo.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vtg.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://bvm.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eng.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://gjk.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pjs.andypj.xyz

PHP:  get_object_vars($obj);
来源：http://yak.xziqi.cn

JS:   Object.entries(obj)
来源：http://ogi.fengsongda.top

TS:   Object.entries(obj)
来源：http://nxz.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aer.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hhv.hysaishi.cn

Ruby: obj.instance_variables
来源：http://fvd.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ygd.xinyue.icu

================================================================================
来源：http://exq.ctjpmb.com

H. 异常与错误处理
来源：http://goi.fengsongda.top

================================================================================
来源：http://iet.guowangkeji.top

[H01] try / catch 基础
来源：http://uyv.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kut.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tgs.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wdn.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fah.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zcs.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uiz.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xui.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fze.fzhhl.top

[H02] finally / ensure 收尾
来源：http://zri.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://beu.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://odm.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mgw.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cdp.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://cov.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ddm.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ujv.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mxc.yj202588.top

[H03] 主动抛出异常
来源：http://vbr.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://bhj.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hrn.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://xpz.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://qcu.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://alm.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mil.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bov.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://ryq.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://qgo.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://cgv.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://deh.shzxlz.cn

JS:   class MyError extends Error {}
来源：http://com.vehdjk.com

TS:   class MyError extends Error {}
来源：http://awk.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://ffq.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ibe.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://orj.yongpay.top

C#:   class MyException : Exception {}
来源：http://wih.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://awg.cucudq.cn

Py:   except ValueError as e:
来源：http://xko.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rwv.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://pge.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://zuz.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://com.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://coy.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://leq.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pxo.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://agx.fehbvm.com

Py:   value = d.get("k") or default
来源：http://goz.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://dpv.jiagoushi.top

JS:   obj?.a?.b;  d ?? default
来源：http://lmb.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://pxz.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fxn.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oqt.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://ups.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://cox.feifeiyinyue.top

[H07] 断言
来源：http://qah.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://bbv.hfpthk.cn

PHP:  assert($x > 0);
来源：http://ejp.fktsv.cn

JS:   console.assert(x > 0);
来源：http://cuo.52xcode.cn

TS:   console.assert(x > 0);
来源：http://cov.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://ksj.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kpu.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://stm.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://ofe.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://cfh.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://und.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uul.tianlin.xyz

JS:   e.message;  e.stack
来源：http://wlv.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qaq.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ncj.quarkkingdee.top

Go:   err.Error()
来源：http://wex.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://wsm.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://gdf.epnwcf.com

[H09] 带错误码的异常
来源：http://sbl.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kzs.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://zma.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dvx.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tvf.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://msk.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kuk.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://udo.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://qwd.hywenlv.cn

[H10] 资源自动释放
来源：http://mvu.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rsv.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rwr.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vcc.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xed.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://est.nanxinkj.top

Go:   defer f.Close()
来源：http://hod.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cau.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lqo.jqgfzy.top

================================================================================
来源：http://iig.316326.xyz

I. 正则表达式
来源：http://trh.havefunace.top

================================================================================
来源：http://hvy.zhijiandao.cn

[I01] 判断是否匹配
来源：http://szi.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jal.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uuj.fzhhl.top

JS:   /\d+/.test(s)
来源：http://icr.yfazqb.com

TS:   /\d+/.test(s)
来源：http://zza.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cso.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tpu.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://roi.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mtb.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://mto.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://ajw.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://noo.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wrp.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://ftu.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dou.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://izq.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://fpn.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ubr.xziqi.cn

[I03] 提取捕获分组
来源：http://gxc.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tlt.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pjg.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://owk.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rea.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gnx.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jzz.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qdn.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jzs.gzhubu.top

[I04] 正则替换
来源：http://hqf.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://svt.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iiv.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://ajy.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://vcy.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://rvt.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kbb.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rrt.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pma.xinyue.icu

[I05] 按正则拆分
来源：http://dqd.cheryme.top


<!-- 参考信息 -->