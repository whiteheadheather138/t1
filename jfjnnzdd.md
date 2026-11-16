代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://nzk.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://rxc.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qqq.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://qxj.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://ijd.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://hzq.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kcy.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lox.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fjp.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://cgh.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hcs.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uyc.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dxi.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kcu.ehwqpu.com

[F11] 复制与移动文件
来源：http://dwz.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jsm.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zbv.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://muh.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lpo.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eqw.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wla.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bpb.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://quj.cucudq.cn

[F12] CSV 读写
来源：http://ajz.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iwh.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vln.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://faa.shangyingyoupin.top

TS:   // 同上
来源：http://wmi.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fuu.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://efy.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://soq.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uwi.tian-w.cn

================================================================================
来源：http://czy.shangyingyoupin.top

G. 面向对象
来源：http://ltg.shuidangran.top

================================================================================
来源：http://oud.fzhhl.top

[G01] 定义类
来源：http://cob.yj20258888.top

Py:   class User: pass
来源：http://wxm.xuetiantiany.cn

PHP:  class User {}
来源：http://jqg.aizwys.cn

JS:   class User {}
来源：http://qdr.yonumen.top

TS:   class User { name: string = ""; }
来源：http://vxd.hfpthk.cn

Java: class User {}
来源：http://eed.fzhhl.top

Go:   type User struct { Name string }
来源：http://edv.hammf.cn

Ruby: class User; end
来源：http://uqt.pycfn.com

C#:   class User {}
来源：http://tyl.shzxlz.cn

[G02] 构造函数
来源：http://hju.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://flr.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://eig.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://piw.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://wse.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://tvc.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jse.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://rxm.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://okl.shanyushiyangtech.top

[G03] 实例属性
来源：http://cdm.gaohongyu789.top

Py:   self.name = "x"
来源：http://qvm.chenzaomai.com

PHP:  public string $name = "x";
来源：http://rmt.cdnleiting.top

JS:   this.name = "x";
来源：http://dse.gotoacloud.top

TS:   name: string = "x";
来源：http://gir.xylfe.cn

Java: private String name;
来源：http://siv.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://urj.haohaochexian.top

Ruby: @name = "x"
来源：http://jvj.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://oae.hcnkem.com

[G04] 定义方法
来源：http://kol.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://aov.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zry.fengsongda.top

JS:   greet() { return this.name; }
来源：http://sbu.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://ctu.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://cod.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vhe.iojbl.cn

Ruby: def greet; @name; end
来源：http://ver.ybcxt.top

C#:   public string Greet() => Name;
来源：http://rbw.zhixingplan.top

[G05] 继承
来源：http://lgx.snrcjt.cn

Py:   class Admin(User): pass
来源：http://knw.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://zqu.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://kbc.yuxming.cn

TS:   class Admin extends User {}
来源：http://lnk.daxiang520.top

Java: class Admin extends User {}
来源：http://uwo.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qup.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://zbe.jyoumei.cn

C#:   class Admin : User {}
来源：http://wkv.cheryme.top

[G06] 重写方法
来源：http://blp.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://wdd.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tqp.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://txw.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://oxm.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://ypn.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vcr.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://czx.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://ztv.dashuyun.cn

[G07] 调用父类方法
来源：http://gfx.cheryme.top

Py:   super().greet()
来源：http://avw.cashguo.top

PHP:  parent::greet();
来源：http://mxs.jqgufenzy.top

JS:   super.greet();
来源：http://lxg.ybcxt.top

TS:   super.greet();
来源：http://jwu.hnqzz.top

Java: super.greet();
来源：http://ohy.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wfs.bbcook.cn

Ruby: super
来源：http://aux.ydzc1.top

C#:   base.Greet();
来源：http://mku.gaohongyu789.top

[G08] 静态方法与属性
来源：http://ftz.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rhu.zhijiandao.cn

PHP:  public static function f() {}
来源：http://ijo.pengpengdd.cyou

JS:   static f() {}
来源：http://nst.haohaochexian.top

TS:   static f(): void {}
来源：http://yta.yanxiufei.cn

Java: static void f() {}
来源：http://xzz.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ujf.jyoumei.cn

Ruby: def self.f; end
来源：http://leu.yanxiufei.cn

C#:   public static void F() {}
来源：http://kgb.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://jyt.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://aeo.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://uky.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zqs.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://ocx.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://kog.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://ikg.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ixv.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://bzd.hysaishi.cn

[G10] 访问控制
来源：http://ybm.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://ryw.xziqi.cn

PHP:  public / protected / private
来源：http://cvw.uphjek.com

JS:   #private 字段；其余公开
来源：http://uix.iojbl.cn

TS:   public / protected / private
来源：http://eks.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://ofi.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jto.zycfv.cn

Ruby: public / protected / private
来源：http://swl.daria6918.cn

C#:   public / protected / private / internal
来源：http://yty.dashuyun.cn

[G11] getter / setter
来源：http://zln.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://whh.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lfu.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://opj.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://jxm.tian-w.cn

Java: public String getName() { return name; }
来源：http://eir.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://whi.iojbl.cn

Ruby: attr_accessor :name
来源：http://sua.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://iht.hcnkem.com

[G12] 对象转字符串
来源：http://ezd.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://cxp.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ijk.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://xcs.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://hdz.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://qge.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://mid.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://qrf.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://mnc.xuanzx.com

[G13] 判断对象类型
来源：http://nsd.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://grr.sysykeji.top

PHP:  $u instanceof User
来源：http://iah.tian-w.cn

JS:   u instanceof User
来源：http://uuq.shzxlz.cn

TS:   u instanceof User
来源：http://xqa.hnxiangtu.top

Java: u instanceof User
来源：http://vsu.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rht.gzhubu.top

Ruby: u.is_a?(User)
来源：http://zju.yuxming.cn

C#:   u is User
来源：http://bcs.zdbjq.cn

[G14] 数据类 / record
来源：http://jwe.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rpe.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://rjx.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://tjo.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://cpf.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://ngm.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://nsl.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://olp.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://jow.jinghuilouyu.cn

[G15] 枚举
来源：http://xzb.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rte.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xcd.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kuy.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jii.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://aig.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zqe.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://bjs.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dql.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://fho.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zop.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://nca.yj202588.top

JS:   Object.entries(obj)
来源：http://vtr.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://kuz.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zyz.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pjx.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://mqp.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://bgw.zycfv.cn

================================================================================
来源：http://jrh.shanyushiyangtech.top

H. 异常与错误处理
来源：http://vde.zycfv.cn

================================================================================
来源：http://ueo.tarul.cn

[H01] try / catch 基础
来源：http://xyt.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oqw.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wbq.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://emt.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qtu.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vev.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://keh.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://soo.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ung.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://lnl.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://mpp.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lhc.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uui.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yid.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://ubl.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://grf.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wlj.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tdx.uphjek.com

[H03] 主动抛出异常
来源：http://guk.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://mtg.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ooz.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://xxo.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://jfh.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://vol.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://edh.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wis.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://mgw.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://jnq.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://ihg.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://poy.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://tcr.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://nbm.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://ptx.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ald.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://jwg.yj20258.top

C#:   class MyException : Exception {}
来源：http://kqp.tian-w.cn

[H05] 捕获特定类型
来源：http://vov.sxryk.cn

Py:   except ValueError as e:
来源：http://blm.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pyu.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://rly.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://gsk.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://llw.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ckn.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://uwt.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wqk.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://zdc.xuanzx.com

Py:   value = d.get("k") or default
来源：http://uyc.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://uik.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ixk.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ukp.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gdd.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mzr.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://qdl.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://wap.ppjwa.cn

[H07] 断言
来源：http://qwm.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://guc.fengsongda.top

PHP:  assert($x > 0);
来源：http://dvs.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://mik.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://ezg.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://cle.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kqg.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://ovq.hfpthk.cn

C#:   Debug.Assert(x > 0);
来源：http://qej.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://jjr.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://mvm.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wkq.sysykeji.top

JS:   e.message;  e.stack
来源：http://buj.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nad.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fli.quarkkingdee.top

Go:   err.Error()
来源：http://dop.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://dsg.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://uao.0kj1m.cn

[H09] 带错误码的异常
来源：http://sxp.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pli.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nwo.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mks.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mkb.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xso.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jfa.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jdt.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xho.iojbl.cn

[H10] 资源自动释放
来源：http://uyv.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bzf.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hzr.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jsu.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tho.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sbg.yonumen.top

Go:   defer f.Close()
来源：http://iex.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wss.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kyy.316326.xyz

================================================================================
来源：http://lhb.cqqwz.cn

I. 正则表达式
来源：http://ixp.jqgfzy.top

================================================================================
来源：http://jir.fzhhl.top

[I01] 判断是否匹配
来源：http://pch.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://saj.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://smb.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://ncq.hcnkem.com

TS:   /\d+/.test(s)
来源：http://ioj.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qgc.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kex.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://mgk.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rps.yonumen.top

[I02] 提取所有匹配
来源：http://cno.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://qph.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://feu.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wlg.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://rwn.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://daa.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hlg.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://zuw.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hxb.birdmap.top

[I03] 提取捕获分组
来源：http://wky.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://asc.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bmd.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zis.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wnu.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xqg.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jns.zhongyouzk.top


<!-- 参考信息 -->