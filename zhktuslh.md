代发 wailian999

[F09] 获取文件大小
来源：http://ltc.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://vub.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://qac.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://qba.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://ass.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://iuw.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ldn.yj20258.top

Ruby: File.size("a.txt")
来源：http://rpj.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://kgf.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://nph.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uuh.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zsm.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pfg.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://ypa.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbl.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cpr.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://skr.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://otb.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://tyc.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hei.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lan.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nrd.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ofn.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hcv.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aer.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cge.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jij.bbcook.cn

[F12] CSV 读写
来源：http://ncv.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sxl.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bpe.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://otw.tianlin.xyz

TS:   // 同上
来源：http://rly.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hzr.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yoz.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jvd.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wdv.yuxming.cn

================================================================================
来源：http://uky.cheryme.top

G. 面向对象
来源：http://afj.hongshengwenyu.top

================================================================================
来源：http://qea.sweek.top

[G01] 定义类
来源：http://oee.nwbrower.top

Py:   class User: pass
来源：http://mtf.shzxlz.cn

PHP:  class User {}
来源：http://lni.316326.xyz

JS:   class User {}
来源：http://mge.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://owo.redwolf501.top

Java: class User {}
来源：http://gud.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://fuf.tanke756.top

Ruby: class User; end
来源：http://cbb.yuanzhike.top

C#:   class User {}
来源：http://slw.havefunace.top

[G02] 构造函数
来源：http://pod.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://zjj.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://onl.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://xfl.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://sof.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://hrg.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qxs.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://jlm.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://aal.cqqwz.cn

[G03] 实例属性
来源：http://fgu.vehdjk.com

Py:   self.name = "x"
来源：http://hwv.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://dct.fzhhl.top

JS:   this.name = "x";
来源：http://pkq.xuanzx.com

TS:   name: string = "x";
来源：http://pgw.tarul.cn

Java: private String name;
来源：http://gqt.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mnb.zdbjq.cn

Ruby: @name = "x"
来源：http://rgd.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://vsa.haohaochexian.top

[G04] 定义方法
来源：http://txd.pycfn.com

Py:   def greet(self): return self.name
来源：http://mjy.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rxt.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://hon.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://rzm.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://aoj.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://bqe.nwbrower.top

Ruby: def greet; @name; end
来源：http://jxp.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://dzp.bbcook.cn

[G05] 继承
来源：http://gsw.yuxming.cn

Py:   class Admin(User): pass
来源：http://ehl.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://hvi.uphjek.com

JS:   class Admin extends User {}
来源：http://puw.iojbl.cn

TS:   class Admin extends User {}
来源：http://htf.zycfv.cn

Java: class Admin extends User {}
来源：http://ugg.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ude.xinyue.icu

Ruby: class Admin < User; end
来源：http://fnp.zycfv.cn

C#:   class Admin : User {}
来源：http://tac.havefunace.top

[G06] 重写方法
来源：http://cpi.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://mvi.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sji.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://fti.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://elw.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://xwd.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ano.uphjek.com

Ruby: def greet; "admin"; end
来源：http://czd.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://lyd.xuanzx.com

[G07] 调用父类方法
来源：http://ymx.daria6918.cn

Py:   super().greet()
来源：http://nnt.hcnkem.com

PHP:  parent::greet();
来源：http://eco.jyoumei.cn

JS:   super.greet();
来源：http://anr.yvedp.cn

TS:   super.greet();
来源：http://por.ppjwa.cn

Java: super.greet();
来源：http://fqi.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ohi.hammf.cn

Ruby: super
来源：http://flr.quarkkingdee.top

C#:   base.Greet();
来源：http://nny.sxryk.cn

[G08] 静态方法与属性
来源：http://uxv.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tto.ydzc1.top

PHP:  public static function f() {}
来源：http://gle.sufxvd.cn

JS:   static f() {}
来源：http://mvf.zdbjq.cn

TS:   static f(): void {}
来源：http://kof.yuxming.cn

Java: static void f() {}
来源：http://cuc.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zmy.snrcjt.cn

Ruby: def self.f; end
来源：http://kzj.aibaodan.cn

C#:   public static void F() {}
来源：http://hgd.birdmap.top

[G09] 接口 / 抽象类
来源：http://gbn.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://ikz.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://utl.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qio.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://lpx.cheryme.top

Java: interface Shape { double area(); }
来源：http://nxc.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://cnw.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ufe.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://hrf.zycfv.cn

[G10] 访问控制
来源：http://fma.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://dgl.shzxlz.cn

PHP:  public / protected / private
来源：http://wnq.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://zdb.wangshuangyany.cn

TS:   public / protected / private
来源：http://bvd.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://wlj.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://irx.cucudq.cn

Ruby: public / protected / private
来源：http://qmh.tianlin.xyz

C#:   public / protected / private / internal
来源：http://vyu.hysaishi.cn

[G11] getter / setter
来源：http://rte.xziqi.cn

Py:   @property 与 @x.setter
来源：http://msl.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xns.yuxming.cn

JS:   get name() { return this._name; }
来源：http://uts.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://wqz.snrcjt.cn

Java: public String getName() { return name; }
来源：http://ddm.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uqa.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://qcj.gzhubu.top

C#:   public string Name { get; set; }
来源：http://rvz.hfpthk.cn

[G12] 对象转字符串
来源：http://sjn.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://vzp.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lwz.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://nmw.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://dlk.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://qoq.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ofu.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://thr.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://vjb.yangfankeji.com

[G13] 判断对象类型
来源：http://acf.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://dkt.guowangkeji.top

PHP:  $u instanceof User
来源：http://fru.xuetiantiany.cn

JS:   u instanceof User
来源：http://gwv.jinghuilouyu.cn

TS:   u instanceof User
来源：http://wos.hysaishi.cn

Java: u instanceof User
来源：http://cbl.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rtb.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://cgr.9152youxi.cn

C#:   u is User
来源：http://amo.yanxiufei.cn

[G14] 数据类 / record
来源：http://ybf.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lii.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://fic.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yop.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://fku.ivvv.top

Java: record User(String name, int age) {}
来源：http://pue.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://jmc.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dfq.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://fba.fanxiaobao.xyz

[G15] 枚举
来源：http://zfg.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nbt.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dva.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://klc.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ngq.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://knl.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ish.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://xsn.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://feq.yonumen.top

[G16] 对象转数组 / 字典
来源：http://cnc.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://srn.316326.xyz

PHP:  get_object_vars($obj);
来源：http://hii.guannengcc.top

JS:   Object.entries(obj)
来源：http://mha.hesvh.cn

TS:   Object.entries(obj)
来源：http://paf.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eii.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wjd.svipenyu.cn

Ruby: obj.instance_variables
来源：http://gjv.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://ohs.gogol.net.cn

================================================================================
来源：http://woe.shzxlz.cn

H. 异常与错误处理
来源：http://hah.316326.xyz

================================================================================
来源：http://qkx.chenjidiqi.icu

[H01] try / catch 基础
来源：http://wmu.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xrw.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rae.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bxt.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yfg.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qfm.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qia.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lif.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nyy.daria6918.cn

[H02] finally / ensure 收尾
来源：http://pbu.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://vhj.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qtc.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qot.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xhu.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://dda.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xjw.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nyy.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ghx.shzxlz.cn

[H03] 主动抛出异常
来源：http://asx.cdnleiting.top

Py:   raise ValueError("错误信息")
来源：http://hgk.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://huy.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://khm.meibo888.top

TS:   throw new Error("错误信息");
来源：http://prg.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dya.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tah.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pff.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vvy.wangdashe.top

[H04] 自定义异常类型
来源：http://fkj.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://xiq.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://nlq.shuidangran.top

JS:   class MyError extends Error {}
来源：http://vwk.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://uil.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://jiy.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jxf.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://vbg.xziqi.cn

C#:   class MyException : Exception {}
来源：http://pmx.pycfn.com

[H05] 捕获特定类型
来源：http://nvj.cheryme.top

Py:   except ValueError as e:
来源：http://xbo.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vqz.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://qaz.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://hjx.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://khz.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gdj.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://wbq.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zea.vehdjk.com

[H06] 可选值 / 空值安全访问
来源：http://xie.ydzc1.top

Py:   value = d.get("k") or default
来源：http://opa.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://oee.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://bqf.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://cft.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gxi.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ouv.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://lqt.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://ybg.jinqigfzy.top

[H07] 断言
来源：http://iax.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://mlz.bbcook.cn

PHP:  assert($x > 0);
来源：http://tkz.nwbrower.top

JS:   console.assert(x > 0);
来源：http://udj.yonumen.top

TS:   console.assert(x > 0);
来源：http://jie.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://cgw.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kzg.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rkk.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://gaf.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://pqt.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://wvl.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://awj.sysykeji.top

JS:   e.message;  e.stack
来源：http://mcf.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yyr.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hix.zdqjudy.top

Go:   err.Error()
来源：http://btr.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://uxl.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://duu.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://eis.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yob.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jhl.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aak.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fpt.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ysd.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rqk.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://vsw.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ock.hongshengwenyu.top

[H10] 资源自动释放
来源：http://zbv.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ljj.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cnz.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kbd.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://geo.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pis.aibaodan.cn

Go:   defer f.Close()
来源：http://mrk.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pcr.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vay.hysaishi.cn

================================================================================
来源：http://hrk.fehbvm.com

I. 正则表达式
来源：http://ira.fktsv.cn

================================================================================
来源：http://cnp.yonumen.top

[I01] 判断是否匹配
来源：http://ryq.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dmf.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://cqc.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://xrf.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://urj.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kqu.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://djy.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://wle.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wuv.316326.xyz

[I02] 提取所有匹配
来源：http://dem.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://cuw.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gvh.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fqe.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://usn.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://quu.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lfm.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://frh.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zco.9152youxi.cn

[I03] 提取捕获分组
来源：http://wjc.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pxp.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xgd.cucudq.cn


<!-- 参考信息 -->