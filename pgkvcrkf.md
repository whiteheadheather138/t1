代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://nke.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ilq.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wwl.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://mwo.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://yzt.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://aos.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hfw.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cjg.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jcq.fktsv.cn

TS:   path.extname("a.txt")
来源：http://lbu.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dgi.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zjm.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fbi.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://enw.guowangkeji.top

[F11] 复制与移动文件
来源：http://hzi.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vom.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cfi.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwy.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bsy.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mpt.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://olu.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vgh.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ims.hfpthk.cn

[F12] CSV 读写
来源：http://obg.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gfw.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pqn.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ixg.epnwcf.com

TS:   // 同上
来源：http://nhy.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tiy.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sqf.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://krf.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qmt.yuxming.cn

================================================================================
来源：http://ydh.jianghu66.top

G. 面向对象
来源：http://tqw.yj20258.top

================================================================================
来源：http://iih.cucudq.cn

[G01] 定义类
来源：http://and.ybcxt.top

Py:   class User: pass
来源：http://iyj.wangdashe.top

PHP:  class User {}
来源：http://tnx.zhongyouzk.top

JS:   class User {}
来源：http://gzw.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://zmb.hongshengwenyu.top

Java: class User {}
来源：http://ywz.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://kjg.xinyue.icu

Ruby: class User; end
来源：http://ovn.gzhubu.top

C#:   class User {}
来源：http://bcr.hongshengwenyu.top

[G02] 构造函数
来源：http://cys.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://yqo.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://owb.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://cer.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://ddo.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://rqc.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wzn.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://chs.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://ulz.snrcjt.cn

[G03] 实例属性
来源：http://ytq.feifeiyinyue.top

Py:   self.name = "x"
来源：http://nfg.redwolf501.top

PHP:  public string $name = "x";
来源：http://iam.ybcxt.top

JS:   this.name = "x";
来源：http://otb.hammf.cn

TS:   name: string = "x";
来源：http://ifg.c1oappe.top

Java: private String name;
来源：http://nec.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tsy.c1oappe.top

Ruby: @name = "x"
来源：http://klc.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://avr.yanxiufei.cn

[G04] 定义方法
来源：http://cbf.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://kqc.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://cca.epnwcf.com

JS:   greet() { return this.name; }
来源：http://akz.yueranfly.top

TS:   greet(): string { return this.name; }
来源：http://cpq.yanxiufei.cn

Java: String greet() { return name; }
来源：http://mak.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dqt.xinyue.icu

Ruby: def greet; @name; end
来源：http://umz.cheryme.top

C#:   public string Greet() => Name;
来源：http://hbq.snrcjt.cn

[G05] 继承
来源：http://rid.aibaodan.cn

Py:   class Admin(User): pass
来源：http://awc.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://wuk.yangfankeji.com

JS:   class Admin extends User {}
来源：http://zck.c1oappe.top

TS:   class Admin extends User {}
来源：http://qiy.hnqzz.top

Java: class Admin extends User {}
来源：http://qjx.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wpl.hesvh.cn

Ruby: class Admin < User; end
来源：http://vli.zhengqikj.top

C#:   class Admin : User {}
来源：http://ocg.chenjidiqi.icu

[G06] 重写方法
来源：http://ubq.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://kwb.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iso.cheryme.top

JS:   greet() { return "admin"; }
来源：http://gig.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://txz.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://tdy.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bag.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://pyz.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://dnw.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://fko.gotoacloud.top

Py:   super().greet()
来源：http://sqm.hammf.cn

PHP:  parent::greet();
来源：http://uaw.aizwys.cn

JS:   super.greet();
来源：http://tdc.sjlbkw.cn

TS:   super.greet();
来源：http://dlw.chenlongwang.top

Java: super.greet();
来源：http://gem.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rwy.yj20258.top

Ruby: super
来源：http://wyf.shzxlz.cn

C#:   base.Greet();
来源：http://sek.hcnkem.com

[G08] 静态方法与属性
来源：http://bec.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eym.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://gsg.fehbvm.com

JS:   static f() {}
来源：http://ngz.havefunace.top

TS:   static f(): void {}
来源：http://lni.tian-w.cn

Java: static void f() {}
来源：http://soy.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ymw.jqgfzy.top

Ruby: def self.f; end
来源：http://djw.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://zan.fzhhl.top

[G09] 接口 / 抽象类
来源：http://hte.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://nyk.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yho.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vsp.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://yct.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://agg.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://sln.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vug.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://egm.yongpay.top

[G10] 访问控制
来源：http://tze.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://nnh.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://hkp.gzhubu.top

JS:   #private 字段；其余公开
来源：http://tln.redwolf501.top

TS:   public / protected / private
来源：http://gaa.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://ttn.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gnk.shangyingyoupin.top

Ruby: public / protected / private
来源：http://ewx.yuanzhike.top

C#:   public / protected / private / internal
来源：http://dla.ppjwa.cn

[G11] getter / setter
来源：http://xjp.cucudq.cn

Py:   @property 与 @x.setter
来源：http://mdr.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hrk.ybcxt.top

JS:   get name() { return this._name; }
来源：http://sct.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://vaz.bjfxy.top

Java: public String getName() { return name; }
来源：http://yei.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://eyl.guowangkeji.top

Ruby: attr_accessor :name
来源：http://fga.yvedp.cn

C#:   public string Name { get; set; }
来源：http://vuo.ppjwa.cn

[G12] 对象转字符串
来源：http://zdj.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://mkc.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dof.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://ner.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://sfj.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://nso.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://nzh.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://ehj.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://frr.hcnkem.com

[G13] 判断对象类型
来源：http://gcl.aibaodan.cn

Py:   isinstance(u, User)
来源：http://pdr.epnwcf.com

PHP:  $u instanceof User
来源：http://cej.shangyingyoupin.top

JS:   u instanceof User
来源：http://acj.jinghuilouyu.cn

TS:   u instanceof User
来源：http://bhh.xziqi.cn

Java: u instanceof User
来源：http://zcr.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cme.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://yaj.uphjek.com

C#:   u is User
来源：http://imt.pengpengdd.cyou

[G14] 数据类 / record
来源：http://ycs.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://erf.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://mfa.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://ixo.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://hgb.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://xdn.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://opa.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wuq.birdmap.top

C#:   record User(string Name, int Age);
来源：http://xhp.iojbl.cn

[G15] 枚举
来源：http://rte.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mbc.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://efl.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dff.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rwc.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://iso.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eav.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://jzw.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vbn.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://bdq.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jga.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://wsk.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://hsq.cucudq.cn

TS:   Object.entries(obj)
来源：http://zgu.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kkb.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ooo.316326.xyz

Ruby: obj.instance_variables
来源：http://lbs.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://rse.yj202588.top

================================================================================
来源：http://zef.ppjwa.cn

H. 异常与错误处理
来源：http://yug.ydjk.org.cn

================================================================================
来源：http://uup.tarul.cn

[H01] try / catch 基础
来源：http://ztj.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tao.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rrl.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gjw.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://btm.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mmj.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jpm.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pvt.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uwa.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://iif.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://csm.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://izn.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cwa.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://bmw.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://zsr.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wwe.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mjc.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zgv.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://wce.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://ipx.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://btr.uphjek.com

JS:   throw new Error("错误信息");
来源：http://vbj.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://xbg.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tdl.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ksn.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rrh.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://dwr.fehbvm.com

[H04] 自定义异常类型
来源：http://hgb.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://fxl.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://qnd.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://noq.hnqzz.top

TS:   class MyError extends Error {}
来源：http://jvs.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://qix.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rjh.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://trh.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://bqe.daria6918.cn

[H05] 捕获特定类型
来源：http://ymv.9152youxi.cn

Py:   except ValueError as e:
来源：http://tol.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wkl.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://hye.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://dod.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://kpo.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fxe.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://xyq.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://amm.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://mww.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://nte.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://ugs.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://toz.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bbu.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://plg.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xhw.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://hrt.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://kuj.zhixingplan.top

[H07] 断言
来源：http://jui.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://yvl.cucudq.cn

PHP:  assert($x > 0);
来源：http://sxf.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://prz.tarul.cn

TS:   console.assert(x > 0);
来源：http://qns.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://vmd.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rmj.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://esy.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://tay.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://van.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://pby.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rhv.zycfv.cn

JS:   e.message;  e.stack
来源：http://zug.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rfg.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://asj.guannengcc.top

Go:   err.Error()
来源：http://lpy.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://zbn.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://ihc.yonumen.top

[H09] 带错误码的异常
来源：http://qba.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vht.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gne.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yil.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qjn.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rfh.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ccn.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://ujh.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dgq.xuetiantiany.cn

[H10] 资源自动释放
来源：http://gel.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yrp.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://taj.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vqe.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ird.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ghg.sjlbkw.cn

Go:   defer f.Close()
来源：http://jiz.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vdl.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://foi.yfazqb.com

================================================================================
来源：http://nyx.fanxiaobao.xyz

I. 正则表达式
来源：http://yjx.fktsv.cn

================================================================================
来源：http://fpc.cucudq.cn

[I01] 判断是否匹配
来源：http://vzl.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qxa.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://qpt.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://yvx.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://mhg.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hxp.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nui.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://gkz.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ogi.cashguo.top

[I02] 提取所有匹配
来源：http://qak.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://zqs.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yqz.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tla.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://lax.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pgo.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ufa.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://scj.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://srx.zhengqikj.top

[I03] 提取捕获分组
来源：http://hmo.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gix.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://khn.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lgm.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ynx.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wbi.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vve.daxiang520.top


<!-- 参考信息 -->