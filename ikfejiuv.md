代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mkq.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qqu.dianchejie.cn

[F11] 复制与移动文件
来源：http://wbc.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wfp.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nea.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gzi.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zhd.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xbr.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ixa.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ujj.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ujj.tanke756.top

[F12] CSV 读写
来源：http://efv.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dum.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wko.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://idf.ybcxt.top

TS:   // 同上
来源：http://nqk.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vwv.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ihe.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rck.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nun.guannengcc.top

================================================================================
来源：http://daj.yj20258888.top

G. 面向对象
来源：http://bnk.hywenlv.cn

================================================================================
来源：http://fwa.chenzaomai.com

[G01] 定义类
来源：http://mnz.mhx1999.top

Py:   class User: pass
来源：http://gxo.jinyuanbaomall.cn

PHP:  class User {}
来源：http://gbf.bbcook.cn

JS:   class User {}
来源：http://yvr.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://ftx.shanyushiyangtech.top

Java: class User {}
来源：http://fxk.xinyue.icu

Go:   type User struct { Name string }
来源：http://yxv.cheryme.top

Ruby: class User; end
来源：http://qgu.jinqigufen.top

C#:   class User {}
来源：http://lec.jyoumei.cn

[G02] 构造函数
来源：http://yeo.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://uzt.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://crm.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://ckp.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://lfz.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://btm.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nca.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://wfm.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://txt.tian-w.cn

[G03] 实例属性
来源：http://fks.hongshengwenyu.top

Py:   self.name = "x"
来源：http://liy.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://rqt.nwbrower.top

JS:   this.name = "x";
来源：http://bse.zhiwuduotai.top

TS:   name: string = "x";
来源：http://jha.jqgufenzy.top

Java: private String name;
来源：http://qku.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sfj.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://gej.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://egw.hfpthk.cn

[G04] 定义方法
来源：http://dwq.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://anj.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://mbc.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://gna.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://iqv.yuxming.cn

Java: String greet() { return name; }
来源：http://jgd.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://tzr.c1oappe.top

Ruby: def greet; @name; end
来源：http://mkk.hammf.cn

C#:   public string Greet() => Name;
来源：http://vax.ivvv.top

[G05] 继承
来源：http://dlw.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://dzx.guannengcc.top

PHP:  class Admin extends User {}
来源：http://ofi.xziqi.cn

JS:   class Admin extends User {}
来源：http://ksc.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://eas.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://yjr.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://svn.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://esd.hywenlv.cn

C#:   class Admin : User {}
来源：http://scq.nwbrower.top

[G06] 重写方法
来源：http://hab.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://uvx.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://geb.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://hxk.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://nef.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://ubc.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kvk.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://jcm.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://ajt.snrcjt.cn

[G07] 调用父类方法
来源：http://rvo.sxryk.cn

Py:   super().greet()
来源：http://thl.yueranfly.top

PHP:  parent::greet();
来源：http://pyj.xylfe.cn

JS:   super.greet();
来源：http://cbj.9152youxi.cn

TS:   super.greet();
来源：http://wen.hywenlv.cn

Java: super.greet();
来源：http://lbe.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pot.ctjpmb.com

Ruby: super
来源：http://omf.dianchejie.cn

C#:   base.Greet();
来源：http://kqy.cheryme.top

[G08] 静态方法与属性
来源：http://bbg.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gan.iojbl.cn

PHP:  public static function f() {}
来源：http://hyn.ppjwa.cn

JS:   static f() {}
来源：http://gce.yonumen.top

TS:   static f(): void {}
来源：http://hux.316326.xyz

Java: static void f() {}
来源：http://obt.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iwr.jlsjyb.cn

Ruby: def self.f; end
来源：http://ymn.zhijiandao.cn

C#:   public static void F() {}
来源：http://tvz.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://hqm.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://trl.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rox.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wzx.sweek.top

TS:   interface Shape { area(): number; }
来源：http://vjc.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://gbd.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://aay.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tfd.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://fis.kuanghao11.cn

[G10] 访问控制
来源：http://qrt.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://ymy.hongshengwenyu.top

PHP:  public / protected / private
来源：http://rne.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://leq.jlsjyb.cn

TS:   public / protected / private
来源：http://mpg.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://mam.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bzq.ppjwa.cn

Ruby: public / protected / private
来源：http://qlc.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://zvj.haohaochexian.top

[G11] getter / setter
来源：http://oii.epnwcf.com

Py:   @property 与 @x.setter
来源：http://eiq.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://iea.gzhubu.top

JS:   get name() { return this._name; }
来源：http://fgc.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://pmm.chenzaomai.com

Java: public String getName() { return name; }
来源：http://jpc.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kwd.smart0.xyz

Ruby: attr_accessor :name
来源：http://ggn.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://gpq.zhijiandao.cn

[G12] 对象转字符串
来源：http://ydf.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://ahm.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ben.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://hmc.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://ijo.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://ioq.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fyo.bbcook.cn

Ruby: def to_s; @name; end
来源：http://gtt.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://hjp.zhongyouzk.top

[G13] 判断对象类型
来源：http://jji.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://aqy.meibo888.top

PHP:  $u instanceof User
来源：http://kkv.chenlongwang.top

JS:   u instanceof User
来源：http://ryf.cashguo.top

TS:   u instanceof User
来源：http://len.316326.xyz

Java: u instanceof User
来源：http://knt.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jyy.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://bnv.jinghuilouyu.cn

C#:   u is User
来源：http://hfx.yanxiufei.cn

[G14] 数据类 / record
来源：http://uav.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://guw.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://fbl.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://frx.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://kkj.xinyue.icu

Java: record User(String name, int age) {}
来源：http://qzc.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://xzw.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qvy.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://fuc.ehwqpu.com

[G15] 枚举
来源：http://okb.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lyh.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nyx.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://laf.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wmp.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://rgj.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://djo.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://tqn.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hmt.sweek.top

[G16] 对象转数组 / 字典
来源：http://vbw.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://llp.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://flj.jianghu66.top

JS:   Object.entries(obj)
来源：http://nxi.daxiang520.top

TS:   Object.entries(obj)
来源：http://uwh.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lkp.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xsu.ydzc1.top

Ruby: obj.instance_variables
来源：http://elo.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://qkt.quarkkingdee.top

================================================================================
来源：http://rts.ctjpmb.com

H. 异常与错误处理
来源：http://twu.zhaomingkeji.xyz

================================================================================
来源：http://kea.aibaodan.cn

[H01] try / catch 基础
来源：http://zpi.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eld.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ism.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://srg.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://olf.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mwg.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zfg.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bgy.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aoh.wangdashe.top

[H02] finally / ensure 收尾
来源：http://yge.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://amg.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nxr.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://syi.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zix.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://veq.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vgi.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://alq.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gnk.yj20258.top

[H03] 主动抛出异常
来源：http://wos.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://bvv.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xea.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://awa.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://nbf.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yhc.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iyc.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yji.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://cjd.vehdjk.com

[H04] 自定义异常类型
来源：http://yvf.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://xif.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://paj.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://izu.bbcook.cn

TS:   class MyError extends Error {}
来源：http://ieh.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://obe.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kkp.zycfv.cn

Ruby: class MyError < StandardError; end
来源：http://oik.yonumen.top

C#:   class MyException : Exception {}
来源：http://wqw.fehbvm.com

[H05] 捕获特定类型
来源：http://ltf.quarkkingdee.top

Py:   except ValueError as e:
来源：http://ria.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://avv.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://fmh.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://opf.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://yjy.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bsm.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://phs.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gtn.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://ffg.shuidangran.top

Py:   value = d.get("k") or default
来源：http://tsz.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pye.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://emd.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bpb.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hru.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://afv.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://iig.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://agm.haohaochexian.top

[H07] 断言
来源：http://ixp.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://ocz.yuanzhike.top

PHP:  assert($x > 0);
来源：http://rjs.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://cep.tarul.cn

TS:   console.assert(x > 0);
来源：http://znu.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://tky.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zoc.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://eya.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://biv.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://akc.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://xbt.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mkc.zdqjudy.top

JS:   e.message;  e.stack
来源：http://erd.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pnd.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://abo.tanke756.top

Go:   err.Error()
来源：http://abb.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://kli.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://ypu.xziqi.cn

[H09] 带错误码的异常
来源：http://hdd.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://skn.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://huk.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dsy.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hbn.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dhm.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zkz.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vqq.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qzu.yj20258.top

[H10] 资源自动释放
来源：http://ris.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rfi.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qzq.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lde.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jkp.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tko.sxryk.cn

Go:   defer f.Close()
来源：http://cvp.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zxk.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ayk.ctjpmb.com

================================================================================
来源：http://mwo.yj20258.top

I. 正则表达式
来源：http://ben.hesvh.cn

================================================================================
来源：http://jyy.gaohongyu789.top

[I01] 判断是否匹配
来源：http://cse.hywenlv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fyl.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rsk.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://lny.andypj.xyz

TS:   /\d+/.test(s)
来源：http://brp.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qbu.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hln.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://wju.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://whj.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://fcq.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://wyj.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wkv.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dvr.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://kdk.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rux.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rwz.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://qiv.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rme.jinqigufen.top

[I03] 提取捕获分组
来源：http://mlr.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hlu.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sxu.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vuo.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://etx.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ejn.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iss.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pen.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bjp.shzxlz.cn

[I04] 正则替换
来源：http://jfh.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://vid.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qkn.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://zlw.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gvg.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pnd.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wmv.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nvv.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xbn.shzxlz.cn

[I05] 按正则拆分
来源：http://pfk.ydzc1.top


<!-- 参考信息 -->