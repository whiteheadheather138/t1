代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wpl.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jdr.dashuyun.cn

[F11] 复制与移动文件
来源：http://tkm.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://plu.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://usi.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wmf.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zfi.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wmi.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tmp.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qlq.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://elq.sjlbkw.cn

[F12] CSV 读写
来源：http://ckr.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://stt.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fph.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bbd.quarkkingdee.top

TS:   // 同上
来源：http://ajr.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ksm.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vzi.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iex.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://lty.gzhubu.top

================================================================================
来源：http://wnn.yangfankeji.com

G. 面向对象
来源：http://rpr.wangdashe.top

================================================================================
来源：http://kig.jqgfzy.top

[G01] 定义类
来源：http://nam.gzhubu.top

Py:   class User: pass
来源：http://ijo.jianghu66.top

PHP:  class User {}
来源：http://ujn.yongpay.top

JS:   class User {}
来源：http://hyk.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://lfg.fktsv.cn

Java: class User {}
来源：http://tzy.jqgfzy.top

Go:   type User struct { Name string }
来源：http://tsf.tarul.cn

Ruby: class User; end
来源：http://gql.birdmap.top

C#:   class User {}
来源：http://ksm.meibo888.top

[G02] 构造函数
来源：http://fom.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://nay.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://nck.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://dku.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://ens.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://cfb.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pnr.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://lbd.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://pfj.ydjk.org.cn

[G03] 实例属性
来源：http://dkv.xinyue.icu

Py:   self.name = "x"
来源：http://fsf.haohaochexian.top

PHP:  public string $name = "x";
来源：http://rmz.sweek.top

JS:   this.name = "x";
来源：http://myw.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://hmh.sufxvd.cn

Java: private String name;
来源：http://uac.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://syg.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://blk.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://jno.hywenlv.cn

[G04] 定义方法
来源：http://bha.yj20258888.top

Py:   def greet(self): return self.name
来源：http://wps.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bee.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://fli.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://vou.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://sbv.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bmh.iojbl.cn

Ruby: def greet; @name; end
来源：http://ktd.birdmap.top

C#:   public string Greet() => Name;
来源：http://aeb.pycfn.com

[G05] 继承
来源：http://dsm.gzhubu.top

Py:   class Admin(User): pass
来源：http://hij.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://lkl.xinyue.icu

JS:   class Admin extends User {}
来源：http://mag.hywenlv.cn

TS:   class Admin extends User {}
来源：http://ekx.ppjwa.cn

Java: class Admin extends User {}
来源：http://jqk.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fkr.meibo888.top

Ruby: class Admin < User; end
来源：http://wpp.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://bdy.ydzc1.top

[G06] 重写方法
来源：http://ppd.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://mfd.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rrp.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://ldx.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://oxm.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://rrc.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://typ.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://aaf.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://tzw.snrcjt.cn

[G07] 调用父类方法
来源：http://fcx.aizwys.cn

Py:   super().greet()
来源：http://byu.wangshuangyany.cn

PHP:  parent::greet();
来源：http://xfa.cdnleiting.top

JS:   super.greet();
来源：http://rnw.pycfn.com

TS:   super.greet();
来源：http://aha.guannengcc.top

Java: super.greet();
来源：http://qmc.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gjb.ehwqpu.com

Ruby: super
来源：http://rmv.wangdashe.top

C#:   base.Greet();
来源：http://pcb.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://ykg.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://amt.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://ljg.ctjpmb.com

JS:   static f() {}
来源：http://sip.hesvh.cn

TS:   static f(): void {}
来源：http://fbv.jinqigufen.top

Java: static void f() {}
来源：http://oio.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yje.smart0.xyz

Ruby: def self.f; end
来源：http://kaf.daxiang520.top

C#:   public static void F() {}
来源：http://aci.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://jud.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://eyz.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://cbm.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://uik.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://cxm.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://ebk.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://fpz.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xcg.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://rft.nanxuanxn.top

[G10] 访问控制
来源：http://jws.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://gab.chenlongwang.top

PHP:  public / protected / private
来源：http://rav.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://xgr.jqgufenzy.top

TS:   public / protected / private
来源：http://veg.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://atm.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://opn.jinqigufen.top

Ruby: public / protected / private
来源：http://uob.hysaishi.cn

C#:   public / protected / private / internal
来源：http://kbm.guannengcc.top

[G11] getter / setter
来源：http://tpn.gzhubu.top

Py:   @property 与 @x.setter
来源：http://oos.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mbq.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://kvt.sweek.top

TS:   get name(): string { return this._name; }
来源：http://alz.iojbl.cn

Java: public String getName() { return name; }
来源：http://img.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://luq.iojbl.cn

Ruby: attr_accessor :name
来源：http://foy.sxryk.cn

C#:   public string Name { get; set; }
来源：http://mmn.zycfv.cn

[G12] 对象转字符串
来源：http://tng.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://dsr.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://swg.daria6918.cn

JS:   toString() { return this.name; }
来源：http://ifz.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://zsw.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://hmm.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nmb.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://ssr.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://qfj.fktsv.cn

[G13] 判断对象类型
来源：http://lbg.yonumen.top

Py:   isinstance(u, User)
来源：http://ymh.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://amd.ivvv.top

JS:   u instanceof User
来源：http://cce.hongshengwenyu.top

TS:   u instanceof User
来源：http://vva.cashguo.top

Java: u instanceof User
来源：http://ndr.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rco.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://bnb.aibaodan.cn

C#:   u is User
来源：http://jph.ppjwa.cn

[G14] 数据类 / record
来源：http://ecx.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qwj.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://keb.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://ixb.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://dbq.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://knq.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://nft.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gwr.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://ekv.kuanghao11.cn

[G15] 枚举
来源：http://gxs.hnxiangtu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yov.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jmz.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qjl.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://por.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://hdm.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pfv.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://dyw.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cqk.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://xrz.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rap.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://yqr.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://jbw.yj20258888.top

TS:   Object.entries(obj)
来源：http://hzh.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://izq.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://myz.zhixingplan.top

Ruby: obj.instance_variables
来源：http://qib.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://yji.ivvv.top

================================================================================
来源：http://cwr.yj20258888.top

H. 异常与错误处理
来源：http://mhf.shzxlz.cn

================================================================================
来源：http://xbr.316326.xyz

[H01] try / catch 基础
来源：http://nvg.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xix.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bqp.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dlt.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bwh.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oht.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zgr.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nzl.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kls.fengsongda.top

[H02] finally / ensure 收尾
来源：http://esf.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://itv.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sti.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://deq.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tdd.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://hlj.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ctb.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qhy.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sku.xinyue.icu

[H03] 主动抛出异常
来源：http://ycr.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://fry.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dez.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://lwn.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://dwm.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tnp.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tuz.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rst.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://fcu.gaohongyu789.top

[H04] 自定义异常类型
来源：http://tml.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://emt.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://lct.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://uuw.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://wdf.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://ptg.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zcy.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://fnr.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://whq.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://pwe.c1oappe.top

Py:   except ValueError as e:
来源：http://wyw.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ufc.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://qvf.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://yck.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://ncp.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://grv.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://wet.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dpt.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://msj.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://fpj.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qcn.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://okf.pycfn.com

TS:   obj?.a?.b;  d ?? default
来源：http://wea.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mso.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jhk.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://ner.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://laj.kuanghao11.cn

[H07] 断言
来源：http://ojs.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://tud.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://ycs.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://aqr.fktsv.cn

TS:   console.assert(x > 0);
来源：http://qgk.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://hei.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tyi.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://rjy.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://tyt.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://ugj.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://ddh.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ldp.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://nyb.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://bld.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oar.yonumen.top

Go:   err.Error()
来源：http://qju.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://oge.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://xbc.yvedp.cn

[H09] 带错误码的异常
来源：http://qbv.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fhj.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://kck.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dea.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://crq.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://syp.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bwd.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nia.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://owi.andypj.xyz

[H10] 资源自动释放
来源：http://ptx.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wwp.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zyz.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://afi.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wjr.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kdk.vehdjk.com

Go:   defer f.Close()
来源：http://fku.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kcd.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rmg.andypj.xyz

================================================================================
来源：http://dys.zycfv.cn

I. 正则表达式
来源：http://iog.yj202588.top

================================================================================
来源：http://hgh.jinqigufen.top

[I01] 判断是否匹配
来源：http://dtw.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uym.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://bwl.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://zem.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://omi.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ota.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hbo.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://rwz.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cgl.chenlongwang.top

[I02] 提取所有匹配
来源：http://uql.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://ufs.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uzi.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qlm.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://xqp.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ayt.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zkj.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://fjo.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uha.yuanzhike.top

[I03] 提取捕获分组
来源：http://yan.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://exr.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hzg.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lja.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rdr.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gti.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dmi.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://giq.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ylt.zycfv.cn

[I04] 正则替换
来源：http://kdm.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://szl.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fpt.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://uvm.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://kct.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ftg.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xog.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bvr.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xra.hnxiangtu.top

[I05] 按正则拆分
来源：http://cmd.ivvv.top


<!-- 参考信息 -->