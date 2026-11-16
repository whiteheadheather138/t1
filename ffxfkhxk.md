代发 wailian999

[F09] 获取文件大小
来源：http://rjo.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://lam.ydzc1.top

PHP:  filesize("a.txt");
来源：http://bad.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://zrs.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://oho.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ouq.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://evl.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://qos.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://ryp.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://hay.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mpv.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rtf.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eoj.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://lwa.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nai.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rqv.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://thq.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bcc.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://thd.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kkz.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kmt.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nbf.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zqe.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sxy.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baf.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rqj.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://btj.cqqwz.cn

[F12] CSV 读写
来源：http://nwy.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lnd.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oyr.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://huo.tarul.cn

TS:   // 同上
来源：http://rhm.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zrz.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wec.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://etw.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rvx.shzxlz.cn

================================================================================
来源：http://wao.snrcjt.cn

G. 面向对象
来源：http://irx.aibaodan.cn

================================================================================
来源：http://pse.zycfv.cn

[G01] 定义类
来源：http://wvj.chenzaomai.com

Py:   class User: pass
来源：http://faa.xziqi.cn

PHP:  class User {}
来源：http://cvx.cdnleiting.top

JS:   class User {}
来源：http://pwn.316326.xyz

TS:   class User { name: string = ""; }
来源：http://bfa.aibaodan.cn

Java: class User {}
来源：http://suz.gogol.net.cn

Go:   type User struct { Name string }
来源：http://odf.andypj.xyz

Ruby: class User; end
来源：http://hlo.kuanghao11.cn

C#:   class User {}
来源：http://hba.xziqi.cn

[G02] 构造函数
来源：http://coy.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://zbl.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://lra.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://xxz.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://vsv.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://jzq.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://whf.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://yyv.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://arq.hysaishi.cn

[G03] 实例属性
来源：http://uaf.yonumen.top

Py:   self.name = "x"
来源：http://swi.meibo888.top

PHP:  public string $name = "x";
来源：http://dei.yj202588.top

JS:   this.name = "x";
来源：http://gqw.vqdsnc.cn

TS:   name: string = "x";
来源：http://jci.jinqigufen.top

Java: private String name;
来源：http://obr.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lyj.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://sbi.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://bac.haohaochexian.top

[G04] 定义方法
来源：http://hul.smart0.xyz

Py:   def greet(self): return self.name
来源：http://ird.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vyy.yfazqb.com

JS:   greet() { return this.name; }
来源：http://kxa.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://rgc.nanxuanxn.top

Java: String greet() { return name; }
来源：http://vxx.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bhr.zdbjq.cn

Ruby: def greet; @name; end
来源：http://qan.havefunace.top

C#:   public string Greet() => Name;
来源：http://lkq.shuidangran.top

[G05] 继承
来源：http://osj.svipenyu.cn

Py:   class Admin(User): pass
来源：http://adh.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://qcq.sysykeji.top

JS:   class Admin extends User {}
来源：http://rof.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://wir.jiagoushi.top

Java: class Admin extends User {}
来源：http://gfb.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://doa.yonumen.top

Ruby: class Admin < User; end
来源：http://eqo.xinyue.icu

C#:   class Admin : User {}
来源：http://idw.sxryk.cn

[G06] 重写方法
来源：http://yku.yj20258.top

Py:   def greet(self): return "admin"
来源：http://bws.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://amb.cashguo.top

JS:   greet() { return "admin"; }
来源：http://cqp.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://poj.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://gww.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tyr.ivvv.top

Ruby: def greet; "admin"; end
来源：http://otz.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://dgt.9152youxi.cn

[G07] 调用父类方法
来源：http://ote.haohaochexian.top

Py:   super().greet()
来源：http://qoj.gotoacloud.top

PHP:  parent::greet();
来源：http://uyu.zdbjq.cn

JS:   super.greet();
来源：http://gao.hesvh.cn

TS:   super.greet();
来源：http://kae.snrcjt.cn

Java: super.greet();
来源：http://ehr.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uof.zhongyouzk.top

Ruby: super
来源：http://yws.tianlin.xyz

C#:   base.Greet();
来源：http://szf.jqgfzy.top

[G08] 静态方法与属性
来源：http://fnp.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://npj.hywenlv.cn

PHP:  public static function f() {}
来源：http://flv.mhx1999.top

JS:   static f() {}
来源：http://ogc.zycfv.cn

TS:   static f(): void {}
来源：http://fhi.nanxinkj.top

Java: static void f() {}
来源：http://lmx.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://zbp.zhengqikj.top

Ruby: def self.f; end
来源：http://uas.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://nud.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://yii.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://odi.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://qdc.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://ljg.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://nfz.yj20258.top

Java: interface Shape { double area(); }
来源：http://fcg.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://zlu.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nux.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://mbq.zdbjq.cn

[G10] 访问控制
来源：http://iwl.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://juw.yj202588.top

PHP:  public / protected / private
来源：http://vph.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://iyq.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://jey.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://ftx.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dfp.andypj.xyz

Ruby: public / protected / private
来源：http://ihx.tian-w.cn

C#:   public / protected / private / internal
来源：http://ubw.gotoacloud.top

[G11] getter / setter
来源：http://zms.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://wlr.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nod.sweek.top

JS:   get name() { return this._name; }
来源：http://mkm.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://ndt.uphjek.com

Java: public String getName() { return name; }
来源：http://vlq.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://har.daria6918.cn

Ruby: attr_accessor :name
来源：http://wot.cucudq.cn

C#:   public string Name { get; set; }
来源：http://rse.aibaodan.cn

[G12] 对象转字符串
来源：http://wto.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://gjc.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mqk.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://nek.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://fjl.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://oyw.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://hci.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://lhh.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://hdl.cashguo.top

[G13] 判断对象类型
来源：http://cdi.yj20258888.top

Py:   isinstance(u, User)
来源：http://ehs.316326.xyz

PHP:  $u instanceof User
来源：http://can.tian-w.cn

JS:   u instanceof User
来源：http://pru.nanxuanxn.top

TS:   u instanceof User
来源：http://uzd.gaohongyu789.top

Java: u instanceof User
来源：http://ucy.havefunace.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ozh.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://xqz.ctjpmb.com

C#:   u is User
来源：http://xwt.hcnkem.com

[G14] 数据类 / record
来源：http://dqy.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yle.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://mwt.hongshengwenyu.top

JS:   // 无内置：普通类或对象字面量
来源：http://myf.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://brm.yueranfly.top

Java: record User(String name, int age) {}
来源：http://bza.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://tfh.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jfe.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://eoo.iojbl.cn

[G15] 枚举
来源：http://tzz.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vcs.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ypt.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wrr.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jjo.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://tom.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://goy.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://svc.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yoz.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://qaf.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ikg.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://oef.andypj.xyz

JS:   Object.entries(obj)
来源：http://hku.yuanzhike.top

TS:   Object.entries(obj)
来源：http://obw.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mgc.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://esb.shuidangran.top

Ruby: obj.instance_variables
来源：http://qmq.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://gzk.jinqigufen.top

================================================================================
来源：http://zjw.hysaishi.cn

H. 异常与错误处理
来源：http://gca.hcnkem.com

================================================================================
来源：http://isc.yanxiufei.cn

[H01] try / catch 基础
来源：http://zwy.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ima.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://log.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rjp.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vbq.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ylw.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://drk.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iuf.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lxr.meibo888.top

[H02] finally / ensure 收尾
来源：http://hia.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vky.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://evc.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://isz.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vzv.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://ztz.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://heb.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qkb.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rhd.shuidangran.top

[H03] 主动抛出异常
来源：http://bkh.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://bgp.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fpt.birdmap.top

JS:   throw new Error("错误信息");
来源：http://mbz.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://ddf.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dja.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tlr.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nqw.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gep.zhixingplan.top

[H04] 自定义异常类型
来源：http://evj.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://ocy.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pak.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://puf.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://wms.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://bwi.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://owh.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://tzs.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://mii.hcnkem.com

[H05] 捕获特定类型
来源：http://mte.hfpthk.cn

Py:   except ValueError as e:
来源：http://muh.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://flt.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://ppr.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://aof.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://xjz.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sss.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://xbh.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fno.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://lrj.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://lix.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kfx.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://lvj.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://bsi.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ekz.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rrv.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://vem.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://qtp.guannengcc.top

[H07] 断言
来源：http://mly.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://vgy.ybcxt.top

PHP:  assert($x > 0);
来源：http://uqo.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://kjp.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://evi.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://cfz.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jdz.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qnn.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://rtn.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://jfj.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://bvh.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fmk.fktsv.cn

JS:   e.message;  e.stack
来源：http://fji.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bpe.hcnkem.com

Java: e.getMessage();  e.printStackTrace()
来源：http://zys.hnqzz.top

Go:   err.Error()
来源：http://wze.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://bid.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://ywf.hnxiangtu.top

[H09] 带错误码的异常
来源：http://gdz.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qwv.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ack.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gpr.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wac.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wgi.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rll.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://enr.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ixv.svipenyu.cn

[H10] 资源自动释放
来源：http://mcl.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ixj.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cvo.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kvi.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nkp.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lzx.shzxlz.cn

Go:   defer f.Close()
来源：http://wcz.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://erk.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pau.nanxinkj.top

================================================================================
来源：http://ibh.yongpay.top

I. 正则表达式
来源：http://urf.316326.xyz

================================================================================
来源：http://qoe.yonumen.top

[I01] 判断是否匹配
来源：http://mzg.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kwj.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://ybs.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://hrn.yueranfly.top

TS:   /\d+/.test(s)
来源：http://uze.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://frs.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eum.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://wlu.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nkd.gzhubu.top

[I02] 提取所有匹配
来源：http://ism.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://hxj.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://inu.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hma.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://faw.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jba.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://esi.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://cfk.gotoacloud.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kgp.jinqigufen.top

[I03] 提取捕获分组
来源：http://uif.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vys.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://znh.sysykeji.top


<!-- 参考信息 -->