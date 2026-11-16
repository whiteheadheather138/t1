代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://nbn.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pvy.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://qvy.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://vuz.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xlj.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zxp.sysykeji.top

Ruby: Dir.children("dir")
来源：http://kjq.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://qfz.aibaodan.cn

[F09] 获取文件大小
来源：http://jqt.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://ezw.fehbvm.com

PHP:  filesize("a.txt");
来源：http://lbg.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://mim.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://kru.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://rcp.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bqa.fzhhl.top

Ruby: File.size("a.txt")
来源：http://obe.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://kht.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://iuh.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://adg.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uaa.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gvv.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://mdy.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nix.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fns.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jud.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iiu.yongpay.top

[F11] 复制与移动文件
来源：http://fxv.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sxc.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jhw.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ejd.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jur.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qey.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ily.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hvp.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vnf.ehwqpu.com

[F12] CSV 读写
来源：http://ttg.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ybs.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xgc.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yze.316326.xyz

TS:   // 同上
来源：http://mym.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aap.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://evn.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dlk.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tjp.sufxvd.cn

================================================================================
来源：http://yee.epnwcf.com

G. 面向对象
来源：http://xsy.zdqjudy.top

================================================================================
来源：http://tzl.haohaochexian.top

[G01] 定义类
来源：http://kwp.fanxiaobao.xyz

Py:   class User: pass
来源：http://sxf.jyoumei.cn

PHP:  class User {}
来源：http://hxm.gotoacloud.top

JS:   class User {}
来源：http://loa.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://hhg.hesvh.cn

Java: class User {}
来源：http://gvr.snrcjt.cn

Go:   type User struct { Name string }
来源：http://ezd.xuanzx.com

Ruby: class User; end
来源：http://gym.zhaomingkeji.xyz

C#:   class User {}
来源：http://hxs.fzhhl.top

[G02] 构造函数
来源：http://iba.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://xww.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://qjx.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://zjv.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://hbt.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://eic.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nty.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://cus.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://nst.wangshuangyany.cn

[G03] 实例属性
来源：http://zcr.jinqigfzy.top

Py:   self.name = "x"
来源：http://pbk.ehwqpu.com

PHP:  public string $name = "x";
来源：http://zpb.gaohongyu789.top

JS:   this.name = "x";
来源：http://jsg.sweek.top

TS:   name: string = "x";
来源：http://xqk.yj20258888.top

Java: private String name;
来源：http://wxb.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kue.yuanzhike.top

Ruby: @name = "x"
来源：http://bmq.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://oof.xylfe.cn

[G04] 定义方法
来源：http://byt.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://jxt.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fqm.vehdjk.com

JS:   greet() { return this.name; }
来源：http://dtb.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://kpx.zdbjq.cn

Java: String greet() { return name; }
来源：http://oij.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rci.aizwys.cn

Ruby: def greet; @name; end
来源：http://ugq.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://wsp.tanke756.top

[G05] 继承
来源：http://nzl.0kj1m.cn

Py:   class Admin(User): pass
来源：http://ooj.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://urz.hysaishi.cn

JS:   class Admin extends User {}
来源：http://tef.ppjwa.cn

TS:   class Admin extends User {}
来源：http://ydt.jlsjyb.cn

Java: class Admin extends User {}
来源：http://cil.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nky.zdbjq.cn

Ruby: class Admin < User; end
来源：http://ajj.daxiang520.top

C#:   class Admin : User {}
来源：http://ihf.hywenlv.cn

[G06] 重写方法
来源：http://yaf.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://znu.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jqz.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://xrt.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://vsk.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://bnm.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qva.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://mwn.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://qcz.hammf.cn

[G07] 调用父类方法
来源：http://gna.hnxiangtu.top

Py:   super().greet()
来源：http://zoo.ppjwa.cn

PHP:  parent::greet();
来源：http://fqw.birdmap.top

JS:   super.greet();
来源：http://ual.shanyushiyangtech.top

TS:   super.greet();
来源：http://quw.hywenlv.cn

Java: super.greet();
来源：http://cwu.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ckw.tianlin.xyz

Ruby: super
来源：http://vhd.daria6918.cn

C#:   base.Greet();
来源：http://itm.jqgufenzy.top

[G08] 静态方法与属性
来源：http://fot.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://whx.daxiang520.top

PHP:  public static function f() {}
来源：http://aoc.sxryk.cn

JS:   static f() {}
来源：http://skv.nwbrower.top

TS:   static f(): void {}
来源：http://oxm.tarul.cn

Java: static void f() {}
来源：http://alq.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nvz.hnqzz.top

Ruby: def self.f; end
来源：http://gsk.meibo888.top

C#:   public static void F() {}
来源：http://era.shuidangran.top

[G09] 接口 / 抽象类
来源：http://nsd.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://dod.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://fgu.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nag.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://kkf.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://bpi.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://tex.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://icq.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://bqb.zhixingplan.top

[G10] 访问控制
来源：http://veq.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://bom.sysykeji.top

PHP:  public / protected / private
来源：http://mup.52xcode.cn

JS:   #private 字段；其余公开
来源：http://yzl.daria6918.cn

TS:   public / protected / private
来源：http://dzd.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://drf.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nze.hcnkem.com

Ruby: public / protected / private
来源：http://psr.zdbjq.cn

C#:   public / protected / private / internal
来源：http://kcc.ivvv.top

[G11] getter / setter
来源：http://mlq.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://uiy.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://est.fktsv.cn

JS:   get name() { return this._name; }
来源：http://ytm.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://wnz.ehwqpu.com

Java: public String getName() { return name; }
来源：http://dzu.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://yfl.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://mal.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://gtg.hammf.cn

[G12] 对象转字符串
来源：http://srh.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://xol.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mcw.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://hor.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://ali.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://ccd.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://iyh.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://iuw.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://vwp.tarul.cn

[G13] 判断对象类型
来源：http://sxd.jinqigufen.top

Py:   isinstance(u, User)
来源：http://jcx.gotoacloud.top

PHP:  $u instanceof User
来源：http://zuv.hongshengwenyu.top

JS:   u instanceof User
来源：http://csi.yuanzhike.top

TS:   u instanceof User
来源：http://sru.shanyushiyangkeji.top

Java: u instanceof User
来源：http://czs.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eju.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://ytb.tianlin.xyz

C#:   u is User
来源：http://uzy.sweek.top

[G14] 数据类 / record
来源：http://zow.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rcy.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://gno.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xeu.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://ffh.birdmap.top

Java: record User(String name, int age) {}
来源：http://nrb.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://dwq.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ihn.yongpay.top

C#:   record User(string Name, int Age);
来源：http://hkp.andypj.xyz

[G15] 枚举
来源：http://wcx.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gye.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wyf.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ext.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ujz.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://yur.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://azr.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://pkj.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://crs.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://idr.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cir.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://ied.chenlongwang.top

JS:   Object.entries(obj)
来源：http://gin.svipenyu.cn

TS:   Object.entries(obj)
来源：http://kco.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hox.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jlh.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://yao.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://bci.hongshengwenyu.top

================================================================================
来源：http://gbo.xziqi.cn

H. 异常与错误处理
来源：http://kyo.snrcjt.cn

================================================================================
来源：http://zva.yanxiufei.cn

[H01] try / catch 基础
来源：http://kkc.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ugk.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xht.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ibq.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dtt.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cxp.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fqo.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://clk.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xnp.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://ewy.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rap.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aei.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mfy.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bpq.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yhk.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://nin.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ohj.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bif.fzhhl.top

[H03] 主动抛出异常
来源：http://zca.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://oxq.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://but.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://npi.meibo888.top

TS:   throw new Error("错误信息");
来源：http://ryd.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gdq.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mru.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ldo.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://svm.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://gla.meibo888.top

Py:   class MyError(Exception): pass
来源：http://shu.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ioa.c1oappe.top

JS:   class MyError extends Error {}
来源：http://psa.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://hhf.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://tnt.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ljp.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://azj.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://gdo.pycfn.com

[H05] 捕获特定类型
来源：http://aac.dianchejie.cn

Py:   except ValueError as e:
来源：http://ava.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://djc.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://evi.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://xbf.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://ext.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jam.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://jez.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rev.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://muv.yj202588.top

Py:   value = d.get("k") or default
来源：http://iwm.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://dmg.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://esp.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://plz.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vwb.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cxl.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://tud.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://fka.ydzc1.top

[H07] 断言
来源：http://xuo.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://ett.snrcjt.cn

PHP:  assert($x > 0);
来源：http://wzb.xinyue.icu

JS:   console.assert(x > 0);
来源：http://rpv.c1oappe.top

TS:   console.assert(x > 0);
来源：http://lzx.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://fft.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mbg.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://kuv.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://gsx.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://bni.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://rix.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mco.ctjpmb.com

JS:   e.message;  e.stack
来源：http://jms.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xuu.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://woe.xuetiantiany.cn

Go:   err.Error()
来源：http://rbi.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://mqo.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://sar.fehbvm.com

[H09] 带错误码的异常
来源：http://iti.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iwy.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fmx.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://udr.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://say.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kzg.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jvv.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://mko.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pzo.yuanzhike.top

[H10] 资源自动释放
来源：http://isl.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tet.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jqi.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://chh.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yka.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fdb.svipenyu.cn

Go:   defer f.Close()
来源：http://nkk.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rve.shanyushiyangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ocp.jinyuanbaomall.cn

================================================================================
来源：http://ngv.c1oappe.top

I. 正则表达式
来源：http://iny.yanxiufei.cn

================================================================================
来源：http://mlz.daxiang520.top

[I01] 判断是否匹配
来源：http://qsw.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gvp.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lla.ybcxt.top

JS:   /\d+/.test(s)
来源：http://dnq.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://fsn.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xur.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gmt.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://zkf.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mwj.ydjk.org.cn

[I02] 提取所有匹配
来源：http://ppd.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://pmr.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ulz.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dmr.gzhubu.top


<!-- 参考信息 -->