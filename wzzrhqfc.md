代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hoo.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://jkv.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cuz.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qxm.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://omy.fktsv.cn

TS:   path.extname("a.txt")
来源：http://rlv.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tyz.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wlr.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mss.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://awj.fzhhl.top

[F11] 复制与移动文件
来源：http://fgh.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ppl.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bny.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rka.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hlb.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uwp.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jpi.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sts.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ndc.epnwcf.com

[F12] CSV 读写
来源：http://bxd.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://flb.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lih.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vwe.ctjpmb.com

TS:   // 同上
来源：http://iuh.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sle.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xse.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zyt.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://abg.wangdashe.top

================================================================================
来源：http://hvl.nwbrower.top

G. 面向对象
来源：http://npo.hongshengwenyu.top

================================================================================
来源：http://eth.zhiwuduotai.top

[G01] 定义类
来源：http://aiw.cashguo.top

Py:   class User: pass
来源：http://ubw.sysykeji.top

PHP:  class User {}
来源：http://apd.wangdashe.top

JS:   class User {}
来源：http://ycn.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://jxb.gogol.net.cn

Java: class User {}
来源：http://oeb.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://eah.svipenyu.cn

Ruby: class User; end
来源：http://ecn.zhiwuduotai.top

C#:   class User {}
来源：http://cii.xylfe.cn

[G02] 构造函数
来源：http://lqw.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://xzm.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://cob.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://esr.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://cqf.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://rdx.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sxt.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://qey.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://oux.redwolf501.top

[G03] 实例属性
来源：http://rto.chenjidiqi.icu

Py:   self.name = "x"
来源：http://swx.smart0.xyz

PHP:  public string $name = "x";
来源：http://bci.yj20258888.top

JS:   this.name = "x";
来源：http://gcr.smart0.xyz

TS:   name: string = "x";
来源：http://eey.mhx1999.top

Java: private String name;
来源：http://spl.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ipd.hammf.cn

Ruby: @name = "x"
来源：http://zpf.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://byy.cdnleiting.top

[G04] 定义方法
来源：http://mie.yj202588.top

Py:   def greet(self): return self.name
来源：http://dwb.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xap.fzhhl.top

JS:   greet() { return this.name; }
来源：http://ddu.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://bcp.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://vsq.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://evv.cheryme.top

Ruby: def greet; @name; end
来源：http://ubw.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://pkt.sysykeji.top

[G05] 继承
来源：http://bvz.bbcook.cn

Py:   class Admin(User): pass
来源：http://rnr.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://eue.haohaochexian.top

JS:   class Admin extends User {}
来源：http://jrl.nwbrower.top

TS:   class Admin extends User {}
来源：http://slw.0kj1m.cn

Java: class Admin extends User {}
来源：http://pir.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ywk.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://gdx.cashguo.top

C#:   class Admin : User {}
来源：http://okt.aizwys.cn

[G06] 重写方法
来源：http://xuu.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://dgr.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sfq.yonumen.top

JS:   greet() { return "admin"; }
来源：http://urk.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://vpc.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://ybq.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tte.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://eww.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://ucg.guannengcc.top

[G07] 调用父类方法
来源：http://eyf.iojbl.cn

Py:   super().greet()
来源：http://wyz.pycfn.com

PHP:  parent::greet();
来源：http://pbw.svipenyu.cn

JS:   super.greet();
来源：http://zup.cdnleiting.top

TS:   super.greet();
来源：http://qwt.dashuyun.cn

Java: super.greet();
来源：http://jsp.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lqo.tianlin.xyz

Ruby: super
来源：http://jox.9152youxi.cn

C#:   base.Greet();
来源：http://crr.yuxming.cn

[G08] 静态方法与属性
来源：http://svd.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rrj.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://ics.jlsjyb.cn

JS:   static f() {}
来源：http://lbg.zdbjq.cn

TS:   static f(): void {}
来源：http://cxq.yueranfly.top

Java: static void f() {}
来源：http://uew.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oou.uphjek.com

Ruby: def self.f; end
来源：http://sfm.xziqi.cn

C#:   public static void F() {}
来源：http://xvm.uphjek.com

[G09] 接口 / 抽象类
来源：http://cim.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://xuz.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ffg.hesvh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kbd.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://njc.mhx1999.top

Java: interface Shape { double area(); }
来源：http://nac.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://sgh.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qyh.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://qsz.havefunace.top

[G10] 访问控制
来源：http://xzs.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://amo.yj20258888.top

PHP:  public / protected / private
来源：http://fgo.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://vpq.andypj.xyz

TS:   public / protected / private
来源：http://zfy.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://qxe.nanxinkj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mbh.xuetiantiany.cn

Ruby: public / protected / private
来源：http://hkl.aizwys.cn

C#:   public / protected / private / internal
来源：http://cxo.9152youxi.cn

[G11] getter / setter
来源：http://lzv.guannengcc.top

Py:   @property 与 @x.setter
来源：http://ggf.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xku.jianghu66.top

JS:   get name() { return this._name; }
来源：http://tox.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://bjr.iojbl.cn

Java: public String getName() { return name; }
来源：http://sdj.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dmq.ehwqpu.com

Ruby: attr_accessor :name
来源：http://nxi.sweek.top

C#:   public string Name { get; set; }
来源：http://skc.zhoulong.xyz

[G12] 对象转字符串
来源：http://eos.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://nsu.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hto.yvedp.cn

JS:   toString() { return this.name; }
来源：http://fdu.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://oip.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://bdw.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://evh.cheryme.top

Ruby: def to_s; @name; end
来源：http://ttq.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://zrn.dashuyun.cn

[G13] 判断对象类型
来源：http://fnw.daxiang520.top

Py:   isinstance(u, User)
来源：http://osi.zdbjq.cn

PHP:  $u instanceof User
来源：http://jkl.316326.xyz

JS:   u instanceof User
来源：http://wqu.dashuyun.cn

TS:   u instanceof User
来源：http://ygz.aibaodan.cn

Java: u instanceof User
来源：http://emi.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kns.xziqi.cn

Ruby: u.is_a?(User)
来源：http://guk.ehwqpu.com

C#:   u is User
来源：http://ubd.quarkkingdee.top

[G14] 数据类 / record
来源：http://oak.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sip.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://mkd.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://thv.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://ejc.zycfv.cn

Java: record User(String name, int age) {}
来源：http://wfs.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://fpp.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kqo.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://axi.fehbvm.com

[G15] 枚举
来源：http://hgo.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tyn.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://cbu.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mhu.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ieh.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://bmh.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kyv.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://wgr.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iek.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://ahk.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zaf.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://rzv.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://jvf.hfpthk.cn

TS:   Object.entries(obj)
来源：http://aoz.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ksz.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tlh.xylfe.cn

Ruby: obj.instance_variables
来源：http://cpk.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://oaf.yonumen.top

================================================================================
来源：http://jaz.0kj1m.cn

H. 异常与错误处理
来源：http://tip.yongpay.top

================================================================================
来源：http://low.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://kwl.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lll.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bhh.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jyr.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vpk.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xnx.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xxu.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://txa.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sjl.daria6918.cn

[H02] finally / ensure 收尾
来源：http://pwj.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://dvq.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vfg.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fje.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dio.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://xpw.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://bwa.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mfo.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://baq.mhx1999.top

[H03] 主动抛出异常
来源：http://ecw.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://luz.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dgs.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://ftd.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://gks.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nnb.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wzb.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wly.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://edw.sweek.top

[H04] 自定义异常类型
来源：http://uqp.yj202588.top

Py:   class MyError(Exception): pass
来源：http://jmi.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ltv.cashguo.top

JS:   class MyError extends Error {}
来源：http://yww.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://pmn.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://yqg.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kan.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://eow.fktsv.cn

C#:   class MyException : Exception {}
来源：http://wyy.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://zej.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://jvn.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tgs.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://yyt.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://ook.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://qpw.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jza.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://xyx.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mcz.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://ohs.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://rrp.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://mfi.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wkx.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cgh.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jki.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pek.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://xjw.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://qpq.hywenlv.cn

[H07] 断言
来源：http://sus.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://npp.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://eid.sysykeji.top

JS:   console.assert(x > 0);
来源：http://tqz.mhx1999.top

TS:   console.assert(x > 0);
来源：http://xoh.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://nex.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vnk.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bsf.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://wiq.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://acj.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://mct.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zwf.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://fvv.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tlu.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://nlx.haohaochexian.top

Go:   err.Error()
来源：http://zno.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://szn.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://dyi.aibaodan.cn

[H09] 带错误码的异常
来源：http://jff.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rzu.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://etv.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dnq.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jxg.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kef.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ajc.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://izz.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wya.gzhubu.top

[H10] 资源自动释放
来源：http://vqs.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bbi.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tyd.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bsm.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dxq.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://itq.chenjidiqi.icu

Go:   defer f.Close()
来源：http://zbf.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://otn.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vlr.yuanzhike.top

================================================================================
来源：http://hik.0kj1m.cn

I. 正则表达式
来源：http://zqt.jinqigfzy.top

================================================================================
来源：http://myp.jyoumei.cn

[I01] 判断是否匹配
来源：http://zly.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jnc.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://ufo.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://fpf.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://ijv.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xxb.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://slc.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://tdm.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ekh.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://hbq.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://crh.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://acp.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rut.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://mjd.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pgc.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ore.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://vvd.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uoa.aibaodan.cn

[I03] 提取捕获分组
来源：http://ywl.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xmf.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ltp.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cyg.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fgi.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eiy.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rpp.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fvw.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sqm.guannengcc.top

[I04] 正则替换
来源：http://mmr.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://akv.fzhhl.top


<!-- 参考信息 -->