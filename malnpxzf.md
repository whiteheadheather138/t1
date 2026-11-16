代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yxp.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ixo.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://cmt.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://knp.guowangkeji.top

[F09] 获取文件大小
来源：http://aac.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://xca.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://eax.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://hnw.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://car.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://rvo.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ekh.wangdashe.top

Ruby: File.size("a.txt")
来源：http://cuk.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://lpy.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://yhk.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xgy.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bhu.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cku.ywan-chungtsiang.top

TS:   path.extname("a.txt")
来源：http://jvg.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mri.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oin.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lrf.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ror.jinqigufen.top

[F11] 复制与移动文件
来源：http://wdy.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mkr.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wnc.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qxk.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vim.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yam.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wkn.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://son.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ygl.fzhhl.top

[F12] CSV 读写
来源：http://wte.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ypi.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wxy.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://scu.sxryk.cn

TS:   // 同上
来源：http://rnf.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zdn.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://enk.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://maj.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://bro.zhijiandao.cn

================================================================================
来源：http://mrp.shanyushiyangtech.top

G. 面向对象
来源：http://oee.ctjpmb.com

================================================================================
来源：http://cel.birdmap.top

[G01] 定义类
来源：http://gxr.andypj.xyz

Py:   class User: pass
来源：http://ado.xziqi.cn

PHP:  class User {}
来源：http://jvc.xylfe.cn

JS:   class User {}
来源：http://yaa.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://wem.wangdashe.top

Java: class User {}
来源：http://mae.gogol.net.cn

Go:   type User struct { Name string }
来源：http://qvi.shzxlz.cn

Ruby: class User; end
来源：http://ajg.ivvv.top

C#:   class User {}
来源：http://ypq.gogol.net.cn

[G02] 构造函数
来源：http://yei.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://pye.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://ehl.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://okh.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://xla.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://glz.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://thu.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://jvb.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://xhe.nwbrower.top

[G03] 实例属性
来源：http://eaa.aibaodan.cn

Py:   self.name = "x"
来源：http://rfq.meibo888.top

PHP:  public string $name = "x";
来源：http://myp.yuanzhike.top

JS:   this.name = "x";
来源：http://xqr.zdqjudy.top

TS:   name: string = "x";
来源：http://kjh.ydjk.org.cn

Java: private String name;
来源：http://obq.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vip.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://zvl.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://sji.daria6918.cn

[G04] 定义方法
来源：http://bgk.yj20258.top

Py:   def greet(self): return self.name
来源：http://ibd.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kne.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://gqe.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://jpg.guannengcc.top

Java: String greet() { return name; }
来源：http://bbq.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://itj.daria6918.cn

Ruby: def greet; @name; end
来源：http://oll.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://ccg.jqgfzy.top

[G05] 继承
来源：http://azw.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://neg.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://ajc.shzxlz.cn

JS:   class Admin extends User {}
来源：http://rag.ydzc1.top

TS:   class Admin extends User {}
来源：http://rvi.sweek.top

Java: class Admin extends User {}
来源：http://zvs.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bhh.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://exc.yongpay.top

C#:   class Admin : User {}
来源：http://bsv.ctjpmb.com

[G06] 重写方法
来源：http://qdc.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://kde.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gyp.uphjek.com

JS:   greet() { return "admin"; }
来源：http://joz.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://hct.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://eqg.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ozv.birdmap.top

Ruby: def greet; "admin"; end
来源：http://nux.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://atz.shuidangran.top

[G07] 调用父类方法
来源：http://yzw.bjfxy.top

Py:   super().greet()
来源：http://qcf.yonumen.top

PHP:  parent::greet();
来源：http://nmu.yuanzhike.top

JS:   super.greet();
来源：http://xdu.ybcxt.top

TS:   super.greet();
来源：http://tlh.jyoumei.cn

Java: super.greet();
来源：http://ijo.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hck.chenzaomai.com

Ruby: super
来源：http://oac.52xcode.cn

C#:   base.Greet();
来源：http://jvb.pycfn.com

[G08] 静态方法与属性
来源：http://ldw.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hwm.cashguo.top

PHP:  public static function f() {}
来源：http://pai.hammf.cn

JS:   static f() {}
来源：http://atx.gaohongyu789.top

TS:   static f(): void {}
来源：http://apx.jqgufenzy.top

Java: static void f() {}
来源：http://dze.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kgf.zhijiandao.cn

Ruby: def self.f; end
来源：http://kmb.jinqigufen.top

C#:   public static void F() {}
来源：http://lyk.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://vul.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://phh.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://igh.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hca.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://yuk.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://fod.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://vvw.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jsn.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://dfp.uphjek.com

[G10] 访问控制
来源：http://wev.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://yrf.kuanghao11.cn

PHP:  public / protected / private
来源：http://stf.yonumen.top

JS:   #private 字段；其余公开
来源：http://rqr.jqgufenzy.top

TS:   public / protected / private
来源：http://umu.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://rfn.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ach.chenjidiqi.icu

Ruby: public / protected / private
来源：http://akm.jyoumei.cn

C#:   public / protected / private / internal
来源：http://zwa.fengsongda.top

[G11] getter / setter
来源：http://fon.iojbl.cn

Py:   @property 与 @x.setter
来源：http://gin.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://xoz.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://idf.zdqjudy.top

TS:   get name(): string { return this._name; }
来源：http://gne.hcnkem.com

Java: public String getName() { return name; }
来源：http://gno.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zpv.cdnleiting.top

Ruby: attr_accessor :name
来源：http://dzn.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://pjz.hesvh.cn

[G12] 对象转字符串
来源：http://boo.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://afk.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://imr.sysykeji.top

JS:   toString() { return this.name; }
来源：http://jvy.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://wpp.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://eag.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://yxo.redwolf501.top

Ruby: def to_s; @name; end
来源：http://fkb.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://dkl.tianlin.xyz

[G13] 判断对象类型
来源：http://vdz.xylfe.cn

Py:   isinstance(u, User)
来源：http://jmw.pycfn.com

PHP:  $u instanceof User
来源：http://wbt.jlsjyb.cn

JS:   u instanceof User
来源：http://jhz.fktsv.cn

TS:   u instanceof User
来源：http://ban.redwolf501.top

Java: u instanceof User
来源：http://xge.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iav.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://mxx.havefunace.top

C#:   u is User
来源：http://ekm.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://diy.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://med.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://csg.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hee.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://nlo.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://ite.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://yjx.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://puj.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://xwm.ehwqpu.com

[G15] 枚举
来源：http://uek.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zjd.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rjp.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ina.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lwg.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://vgz.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ajv.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://oxm.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ffg.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://lfv.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hhz.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://bpt.tian-w.cn

JS:   Object.entries(obj)
来源：http://yrt.jqgfzy.top

TS:   Object.entries(obj)
来源：http://edt.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jnq.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://muu.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://cse.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://xie.ydjk.org.cn

================================================================================
来源：http://cqn.yuxming.cn

H. 异常与错误处理
来源：http://szu.sweek.top

================================================================================
来源：http://qxe.ydzc1.top

[H01] try / catch 基础
来源：http://egq.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ykr.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hfl.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wed.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aec.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ycx.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vve.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kof.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jql.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://yyo.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://fwg.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fco.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://gve.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gnk.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://yfc.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zqo.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://htz.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jyh.52xcode.cn

[H03] 主动抛出异常
来源：http://fvy.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://qqf.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rab.hammf.cn

JS:   throw new Error("错误信息");
来源：http://gmq.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://gel.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oha.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xea.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://avr.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://sxs.ybcxt.top

[H04] 自定义异常类型
来源：http://qgd.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://lph.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://nsd.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://uyi.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://nck.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://rbg.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fdo.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://eij.yfazqb.com

C#:   class MyException : Exception {}
来源：http://gbb.epnwcf.com

[H05] 捕获特定类型
来源：http://ohu.redwolf501.top

Py:   except ValueError as e:
来源：http://dzv.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rqi.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://udb.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://yim.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://zkx.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zqi.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://yeq.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dhm.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://lrf.c1oappe.top

Py:   value = d.get("k") or default
来源：http://fet.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ick.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://umt.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xgv.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tvu.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iwd.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://vjm.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://oba.yfazqb.com

[H07] 断言
来源：http://xke.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://qjm.xuanzx.com

PHP:  assert($x > 0);
来源：http://hes.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://onf.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://czx.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://wzv.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://red.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vte.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://fgw.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://zqh.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://qmm.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yhk.hnqzz.top

JS:   e.message;  e.stack
来源：http://rnw.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://agy.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://knv.xuanzx.com

Go:   err.Error()
来源：http://cql.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://nas.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://nlv.snrcjt.cn

[H09] 带错误码的异常
来源：http://uav.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://spc.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eaq.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gyr.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ege.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kex.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ccj.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://afw.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://llw.havefunace.top

[H10] 资源自动释放
来源：http://pnc.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://prt.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rcl.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://evv.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ulr.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ujq.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://nku.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://adr.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vdm.xuanzx.com

================================================================================
来源：http://sni.cucudq.cn

I. 正则表达式
来源：http://uhp.jyoumei.cn

================================================================================
来源：http://imq.ehwqpu.com

[I01] 判断是否匹配
来源：http://qqk.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ptp.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ccb.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://oce.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://xgb.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sgs.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bul.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://jus.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tdx.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://wdn.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://ixv.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://foi.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lnc.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://pyv.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gkd.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ymz.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://muu.shangyingyoupin.top


<!-- 参考信息 -->