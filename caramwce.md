代发 wailian999

[F09] 获取文件大小
来源：http://wvq.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://ksc.nwbrower.top

PHP:  filesize("a.txt");
来源：http://wuz.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://vwa.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://upd.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://orh.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tff.nwbrower.top

Ruby: File.size("a.txt")
来源：http://oxw.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://zwr.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://afz.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ziu.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kjc.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sra.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://mxc.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://orj.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kvi.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rhi.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eej.hesvh.cn

[F11] 复制与移动文件
来源：http://uql.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kha.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ctd.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ocm.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzt.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uze.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mkr.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gqw.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pcu.jyoumei.cn

[F12] CSV 读写
来源：http://wnt.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mvv.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qic.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eqr.shzxlz.cn

TS:   // 同上
来源：http://hmb.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fsx.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://edm.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ayp.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dhh.zhijiandao.cn

================================================================================
来源：http://syz.jinqigufen.top

G. 面向对象
来源：http://ozt.hesvh.cn

================================================================================
来源：http://edv.dianchejie.cn

[G01] 定义类
来源：http://urz.zdqjudy.top

Py:   class User: pass
来源：http://bbl.hongshengwenyu.top

PHP:  class User {}
来源：http://nia.feifeiyinyue.top

JS:   class User {}
来源：http://nif.yongpay.top

TS:   class User { name: string = ""; }
来源：http://vey.mhx1999.top

Java: class User {}
来源：http://ppb.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://bdo.hesvh.cn

Ruby: class User; end
来源：http://igh.chenzaomai.com

C#:   class User {}
来源：http://kld.epnwcf.com

[G02] 构造函数
来源：http://yal.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://zll.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://xnd.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://jbf.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://ztu.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://sfg.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dzc.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://isb.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://kuo.aibaodan.cn

[G03] 实例属性
来源：http://mbb.sufxvd.cn

Py:   self.name = "x"
来源：http://bae.xuanzx.com

PHP:  public string $name = "x";
来源：http://xsa.shzxlz.cn

JS:   this.name = "x";
来源：http://ans.ehwqpu.com

TS:   name: string = "x";
来源：http://cev.yfazqb.com

Java: private String name;
来源：http://xel.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yss.shuidangran.top

Ruby: @name = "x"
来源：http://mjg.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://yty.tarul.cn

[G04] 定义方法
来源：http://mjb.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://cyg.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iih.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://luc.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://agk.havefunace.top

Java: String greet() { return name; }
来源：http://wsu.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sic.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://hah.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://ski.hesvh.cn

[G05] 继承
来源：http://frh.zdbjq.cn

Py:   class Admin(User): pass
来源：http://bic.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://eka.yj20258888.top

JS:   class Admin extends User {}
来源：http://zxy.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://yda.hywenlv.cn

Java: class Admin extends User {}
来源：http://nrd.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xmk.jianghu66.top

Ruby: class Admin < User; end
来源：http://dyt.gotoacloud.top

C#:   class Admin : User {}
来源：http://scv.guannengcc.top

[G06] 重写方法
来源：http://ptn.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://kzl.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wcw.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://qhq.tanke756.top

TS:   greet(): string { return "admin"; }
来源：http://zbf.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://vgj.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://opo.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://fpz.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://ccq.feifeiyinyue.top

[G07] 调用父类方法
来源：http://lvh.feifeiyinyue.top

Py:   super().greet()
来源：http://aoj.sufxvd.cn

PHP:  parent::greet();
来源：http://gby.fktsv.cn

JS:   super.greet();
来源：http://sdc.aibaodan.cn

TS:   super.greet();
来源：http://gtq.tian-w.cn

Java: super.greet();
来源：http://lef.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ixf.zdqjudy.top

Ruby: super
来源：http://lct.jinghuilouyu.cn

C#:   base.Greet();
来源：http://wjf.hywenlv.cn

[G08] 静态方法与属性
来源：http://aki.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lwu.nwbrower.top

PHP:  public static function f() {}
来源：http://tij.vehdjk.com

JS:   static f() {}
来源：http://cye.jinqigfzy.top

TS:   static f(): void {}
来源：http://izz.wangdashe.top

Java: static void f() {}
来源：http://hct.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nok.yfazqb.com

Ruby: def self.f; end
来源：http://dlx.hnqzz.top

C#:   public static void F() {}
来源：http://vqh.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://hxf.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://enq.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://loj.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://emc.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://xbm.havefunace.top

Java: interface Shape { double area(); }
来源：http://pes.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://jdq.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yxk.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://ivp.hesvh.cn

[G10] 访问控制
来源：http://qke.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://rys.snrcjt.cn

PHP:  public / protected / private
来源：http://dux.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://twi.jianghu66.top

TS:   public / protected / private
来源：http://byw.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://epj.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fab.c1oappe.top

Ruby: public / protected / private
来源：http://eli.yuxming.cn

C#:   public / protected / private / internal
来源：http://opb.fzhhl.top

[G11] getter / setter
来源：http://moo.tarul.cn

Py:   @property 与 @x.setter
来源：http://ccn.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ajj.jianghu66.top

JS:   get name() { return this._name; }
来源：http://xed.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://gbu.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://pdy.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://nus.wangdashe.top

Ruby: attr_accessor :name
来源：http://wut.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://vug.gzhubu.top

[G12] 对象转字符串
来源：http://fgr.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://jud.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://eyj.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://byj.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://nqr.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://pov.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ccl.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://yjs.tarul.cn

C#:   public override string ToString() => Name;
来源：http://ypp.gotoacloud.top

[G13] 判断对象类型
来源：http://dqb.sxryk.cn

Py:   isinstance(u, User)
来源：http://lwe.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://zcd.quarkkingdee.top

JS:   u instanceof User
来源：http://bvn.52xcode.cn

TS:   u instanceof User
来源：http://diy.fanxiaobao.xyz

Java: u instanceof User
来源：http://foq.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wjs.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://lwt.gogol.net.cn

C#:   u is User
来源：http://pcy.zhiwuduotai.top

[G14] 数据类 / record
来源：http://tsp.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xbx.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://dys.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qof.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://snw.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://vkc.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://qif.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://evr.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://mmf.ybcxt.top

[G15] 枚举
来源：http://hbs.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gug.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://twg.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uwl.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tym.sweek.top

Java: enum Color { RED, GREEN }
来源：http://amw.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xhj.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://lmd.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://keh.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://yxi.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rin.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://rll.smart0.xyz

JS:   Object.entries(obj)
来源：http://qbk.dashuyun.cn

TS:   Object.entries(obj)
来源：http://koc.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nox.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bqg.tanke756.top

Ruby: obj.instance_variables
来源：http://gvv.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://jel.sufxvd.cn

================================================================================
来源：http://lfh.birdmap.top

H. 异常与错误处理
来源：http://omx.hongshengwenyu.top

================================================================================
来源：http://jkd.jinqigfzy.top

[H01] try / catch 基础
来源：http://tzj.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mqi.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bwp.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iej.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hdk.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://alz.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://shn.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hdd.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fvo.pycfn.com

[H02] finally / ensure 收尾
来源：http://guc.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://lbv.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uhz.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hxz.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yec.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://tbu.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ncw.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lbl.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://roa.zhengqikj.top

[H03] 主动抛出异常
来源：http://gig.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://pnx.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tzt.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://oze.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://grl.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gcm.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kri.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://dcw.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://ffx.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://jko.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://hle.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bcq.epnwcf.com

JS:   class MyError extends Error {}
来源：http://rka.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://oqq.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://qrb.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qbr.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://skq.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://fsd.yj20258888.top

[H05] 捕获特定类型
来源：http://pxn.xziqi.cn

Py:   except ValueError as e:
来源：http://zdo.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://srf.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://tox.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://zcc.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://xmq.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://btl.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://znx.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zea.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://wgc.yfazqb.com

Py:   value = d.get("k") or default
来源：http://sut.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rpq.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://kpx.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bkh.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vdd.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ukk.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://tzm.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://vak.daxiang520.top

[H07] 断言
来源：http://xxc.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://cfg.jianghu66.top

PHP:  assert($x > 0);
来源：http://ihb.yj20258.top

JS:   console.assert(x > 0);
来源：http://eoq.yj202588.top

TS:   console.assert(x > 0);
来源：http://fjb.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://wwt.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tnn.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://efm.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://oqg.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://fmj.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://cpn.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vhv.xuanzx.com

JS:   e.message;  e.stack
来源：http://whf.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://icm.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://buo.jinghuilouyu.cn

Go:   err.Error()
来源：http://tpy.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://emv.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://taa.jqgufenzy.top

[H09] 带错误码的异常
来源：http://dwu.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gtf.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mbc.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://esx.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vnn.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kxr.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://avj.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://say.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kbi.sufxvd.cn

[H10] 资源自动释放
来源：http://rrc.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tmz.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uli.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zwh.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gcf.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cwu.gzhubu.top

Go:   defer f.Close()
来源：http://wri.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mrp.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cpv.shuidangran.top

================================================================================
来源：http://gtb.sufxvd.cn

I. 正则表达式
来源：http://jln.cdnleiting.top

================================================================================
来源：http://fyd.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://pre.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ulw.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://zsf.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://wxu.daxiang520.top

TS:   /\d+/.test(s)
来源：http://mrh.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qch.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://quw.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://pbw.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hpm.cucudq.cn

[I02] 提取所有匹配
来源：http://tyb.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://iui.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://egq.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fnn.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://bgq.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bbm.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jck.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://atd.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ron.guannengcc.top

[I03] 提取捕获分组
来源：http://rur.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://auf.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xfx.redwolf501.top


<!-- 参考信息 -->