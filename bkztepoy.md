代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://myw.yuxming.cn

TS:   path.extname("a.txt")
来源：http://zcn.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wuv.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fjf.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xkl.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dua.jinqigufen.top

[F11] 复制与移动文件
来源：http://wxy.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fdp.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kmr.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bfz.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ray.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rrk.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rqb.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aiy.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rqv.kuanghao11.cn

[F12] CSV 读写
来源：http://cbp.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lwl.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://msd.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ycx.316326.xyz

TS:   // 同上
来源：http://thy.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fju.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://djp.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ymp.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://loh.sufxvd.cn

================================================================================
来源：http://grt.bbcook.cn

G. 面向对象
来源：http://cib.nanxinkj.top

================================================================================
来源：http://umw.yuxming.cn

[G01] 定义类
来源：http://sga.yj20258888.top

Py:   class User: pass
来源：http://xao.yfazqb.com

PHP:  class User {}
来源：http://tba.zdbjq.cn

JS:   class User {}
来源：http://gsv.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://jpx.sxryk.cn

Java: class User {}
来源：http://ebf.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://mnk.aibaodan.cn

Ruby: class User; end
来源：http://lef.zdqjudy.top

C#:   class User {}
来源：http://ivs.jyoumei.cn

[G02] 构造函数
来源：http://tll.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://uot.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://mvr.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://ukv.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://bqn.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://gxl.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mkd.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://pnq.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://zmf.dashuyun.cn

[G03] 实例属性
来源：http://dlj.uphjek.com

Py:   self.name = "x"
来源：http://ppz.hesvh.cn

PHP:  public string $name = "x";
来源：http://bgc.gaohongyu789.top

JS:   this.name = "x";
来源：http://vqx.epnwcf.com

TS:   name: string = "x";
来源：http://gxh.yangfankeji.com

Java: private String name;
来源：http://tfo.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pjw.zhiwuduotai.top

Ruby: @name = "x"
来源：http://jfp.hfpthk.cn

C#:   public string Name { get; set; } = "x";
来源：http://tvt.aizwys.cn

[G04] 定义方法
来源：http://leq.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://ufd.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://odm.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://yhb.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://acj.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://avg.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://git.ehwqpu.com

Ruby: def greet; @name; end
来源：http://inp.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://ley.daxiang520.top

[G05] 继承
来源：http://blx.nwbrower.top

Py:   class Admin(User): pass
来源：http://gae.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://bhg.daxiang520.top

JS:   class Admin extends User {}
来源：http://ajr.yonumen.top

TS:   class Admin extends User {}
来源：http://xdz.dashuyun.cn

Java: class Admin extends User {}
来源：http://juu.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ori.zhengqikj.top

Ruby: class Admin < User; end
来源：http://xph.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://djr.zhoulong.xyz

[G06] 重写方法
来源：http://ywo.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://sfl.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://omz.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://gnl.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://fpi.yanxiufei.cn

Java: @Override String greet() { return "admin"; }
来源：http://yub.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qpa.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://ftu.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://ssl.quarkkingdee.top

[G07] 调用父类方法
来源：http://xvy.dianchejie.cn

Py:   super().greet()
来源：http://znu.ehwqpu.com

PHP:  parent::greet();
来源：http://lbe.ydjk.org.cn

JS:   super.greet();
来源：http://qfd.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://njb.aibaodan.cn

Java: super.greet();
来源：http://fpf.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fbp.uphjek.com

Ruby: super
来源：http://oco.sjlbkw.cn

C#:   base.Greet();
来源：http://drw.hfpthk.cn

[G08] 静态方法与属性
来源：http://ckm.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vog.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://wwp.gzhubu.top

JS:   static f() {}
来源：http://tow.hysaishi.cn

TS:   static f(): void {}
来源：http://upr.tanke756.top

Java: static void f() {}
来源：http://cas.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yzg.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://hpq.cucudq.cn

C#:   public static void F() {}
来源：http://lsv.daria6918.cn

[G09] 接口 / 抽象类
来源：http://bdy.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://bii.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://gjb.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xgk.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://qkv.ybcxt.top

Java: interface Shape { double area(); }
来源：http://uqr.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://paa.gaohongyu789.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zii.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://lew.tian-w.cn

[G10] 访问控制
来源：http://owi.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://sbq.dianchejie.cn

PHP:  public / protected / private
来源：http://nxs.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://tup.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://uuc.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://vvk.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wyx.vqdsnc.cn

Ruby: public / protected / private
来源：http://lny.aizwys.cn

C#:   public / protected / private / internal
来源：http://svv.cdnleiting.top

[G11] getter / setter
来源：http://knb.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://mms.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gcf.zycfv.cn

JS:   get name() { return this._name; }
来源：http://exk.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://kwb.havefunace.top

Java: public String getName() { return name; }
来源：http://dbh.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bls.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://yvd.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://odf.zhijiandao.cn

[G12] 对象转字符串
来源：http://khl.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://uqw.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://agc.hammf.cn

JS:   toString() { return this.name; }
来源：http://jkj.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://tdf.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://lhi.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://hrk.meibo888.top

Ruby: def to_s; @name; end
来源：http://fjb.cashguo.top

C#:   public override string ToString() => Name;
来源：http://neh.nanxinkj.top

[G13] 判断对象类型
来源：http://svx.snrcjt.cn

Py:   isinstance(u, User)
来源：http://ymw.0kj1m.cn

PHP:  $u instanceof User
来源：http://xaw.meibo888.top

JS:   u instanceof User
来源：http://uwu.tianlin.xyz

TS:   u instanceof User
来源：http://pbp.daria6918.cn

Java: u instanceof User
来源：http://rqt.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qhe.c1oappe.top

Ruby: u.is_a?(User)
来源：http://uvy.chenzaomai.com

C#:   u is User
来源：http://efm.ivvv.top

[G14] 数据类 / record
来源：http://dqg.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jrj.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://nfv.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://egd.svipenyu.cn

TS:   type User = { name: string; age: number };
来源：http://ozy.havefunace.top

Java: record User(String name, int age) {}
来源：http://lcy.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://nsk.redwolf501.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://guu.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://jnh.yuanzhike.top

[G15] 枚举
来源：http://pra.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://swx.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yrg.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xps.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tyc.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://xzt.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://skc.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://lqc.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zdy.cashguo.top

[G16] 对象转数组 / 字典
来源：http://knh.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cch.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://wpv.jinqigufen.top

JS:   Object.entries(obj)
来源：http://ieq.ehwqpu.com

TS:   Object.entries(obj)
来源：http://xqr.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ufe.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gjt.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://xel.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://pkw.jinyuanbaomall.cn

================================================================================
来源：http://skj.bbcook.cn

H. 异常与错误处理
来源：http://tdj.zycfv.cn

================================================================================
来源：http://afz.ctjpmb.com

[H01] try / catch 基础
来源：http://bpt.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vvn.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://riu.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lqm.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rpl.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eax.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yng.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mya.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mhy.hesvh.cn

[H02] finally / ensure 收尾
来源：http://ugf.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jhl.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zsq.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://heg.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://lra.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://xvl.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ako.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eer.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://shk.haohaochexian.top

[H03] 主动抛出异常
来源：http://rdw.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://jbx.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tli.316326.xyz

JS:   throw new Error("错误信息");
来源：http://lfr.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://jac.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rwc.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mbe.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://juo.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://cal.jyoumei.cn

[H04] 自定义异常类型
来源：http://gol.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://bng.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://ogr.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://oqy.tian-w.cn

TS:   class MyError extends Error {}
来源：http://gls.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://csl.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aij.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://aev.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://tec.hywenlv.cn

[H05] 捕获特定类型
来源：http://xpg.yangfankeji.com

Py:   except ValueError as e:
来源：http://xue.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pne.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://kvt.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://oyq.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://feb.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ijr.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://hex.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ufy.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://vmi.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://nci.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://shn.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://yrv.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://oej.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fov.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://fqu.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://zoz.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://nfq.yvedp.cn

[H07] 断言
来源：http://jjx.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://yal.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://bra.cucudq.cn

JS:   console.assert(x > 0);
来源：http://aaf.daxiang520.top

TS:   console.assert(x > 0);
来源：http://dtk.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://kmx.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iek.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://jfp.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://tfz.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://uwy.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://aku.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qqp.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://lri.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cgg.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ukm.jinqigfzy.top

Go:   err.Error()
来源：http://oxm.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://ilc.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://ovm.cdnleiting.top

[H09] 带错误码的异常
来源：http://zlv.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fro.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://xoe.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yxh.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://irq.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pfb.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xvg.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://qfr.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nxa.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://tat.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jna.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xli.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://szo.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zga.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ywd.ppjwa.cn

Go:   defer f.Close()
来源：http://til.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yty.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iry.bbcook.cn

================================================================================
来源：http://dun.nanxuanxn.top

I. 正则表达式
来源：http://qvu.sysykeji.top

================================================================================
来源：http://yub.mhx1999.top

[I01] 判断是否匹配
来源：http://tmq.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bka.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://bkx.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://ojn.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://ggu.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jqa.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gid.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://ssv.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vwr.fktsv.cn

[I02] 提取所有匹配
来源：http://vfn.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://bzv.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jsv.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bst.yonumen.top

TS:   s.match(/\d+/g)
来源：http://ser.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://abu.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xyd.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://gaw.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://glj.hfpthk.cn

[I03] 提取捕获分组
来源：http://kkm.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vgy.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hjq.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pmv.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sih.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xys.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ldm.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://auj.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nol.yuxming.cn

[I04] 正则替换
来源：http://chu.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://suk.cdnleiting.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://udc.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lwy.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://idm.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://uur.bjfxy.top


<!-- 参考信息 -->