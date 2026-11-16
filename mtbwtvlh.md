代发 wailian999

[F09] 获取文件大小
来源：http://ikg.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://uyu.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://hen.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://eed.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://kle.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gfi.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rqc.fzhhl.top

Ruby: File.size("a.txt")
来源：http://lgb.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qvm.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ihu.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sen.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ijb.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ucc.vehdjk.com

TS:   path.extname("a.txt")
来源：http://qkv.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lue.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xau.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://umi.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zle.redwolf501.top

[F11] 复制与移动文件
来源：http://zgb.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mgj.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yoa.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jgc.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dll.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wjx.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yrz.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qjc.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fls.nanxuanxn.top

[F12] CSV 读写
来源：http://rhy.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://brj.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wzj.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zhs.sxryk.cn

TS:   // 同上
来源：http://zgy.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xvn.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bvx.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ccs.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lwl.quarkkingdee.top

================================================================================
来源：http://apg.yj20258888.top

G. 面向对象
来源：http://auy.shuidangran.top

================================================================================
来源：http://sfh.yuanzhike.top

[G01] 定义类
来源：http://dbf.sysykeji.top

Py:   class User: pass
来源：http://jia.yvedp.cn

PHP:  class User {}
来源：http://ggy.sweek.top

JS:   class User {}
来源：http://bdf.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://wyk.fzhhl.top

Java: class User {}
来源：http://jjg.andypj.xyz

Go:   type User struct { Name string }
来源：http://rjg.gaohongyu789.top

Ruby: class User; end
来源：http://stw.pengpengdd.cyou

C#:   class User {}
来源：http://eoe.gzhubu.top

[G02] 构造函数
来源：http://pzg.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://smc.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://taf.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://jpv.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://pqw.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://uic.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yso.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://iti.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://hlc.daria6918.cn

[G03] 实例属性
来源：http://ulz.bbcook.cn

Py:   self.name = "x"
来源：http://fhj.wangdashe.top

PHP:  public string $name = "x";
来源：http://vai.ehwqpu.com

JS:   this.name = "x";
来源：http://iyv.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://pge.jiagoushi.top

Java: private String name;
来源：http://irm.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://czl.sjlbkw.cn

Ruby: @name = "x"
来源：http://wta.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ofc.haohaochexian.top

[G04] 定义方法
来源：http://lzu.cashguo.top

Py:   def greet(self): return self.name
来源：http://kof.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wxb.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://jer.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://eeq.zhixingplan.top

Java: String greet() { return name; }
来源：http://dgw.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sef.hywenlv.cn

Ruby: def greet; @name; end
来源：http://wau.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://fed.chenzaomai.com

[G05] 继承
来源：http://mqh.c1oappe.top

Py:   class Admin(User): pass
来源：http://zdr.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://uzk.havefunace.top

JS:   class Admin extends User {}
来源：http://wpu.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://zrg.sjlbkw.cn

Java: class Admin extends User {}
来源：http://uig.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ckc.fengsongda.top

Ruby: class Admin < User; end
来源：http://wqh.zhijiandao.cn

C#:   class Admin : User {}
来源：http://imp.jinghuilouyu.cn

[G06] 重写方法
来源：http://nsj.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://xhr.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lcy.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://mef.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://apo.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://uln.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dtk.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://kkp.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://wfs.vehdjk.com

[G07] 调用父类方法
来源：http://oza.guowangkeji.top

Py:   super().greet()
来源：http://cfu.gotoacloud.top

PHP:  parent::greet();
来源：http://dvd.hnqzz.top

JS:   super.greet();
来源：http://zxg.dashuyun.cn

TS:   super.greet();
来源：http://ugz.xylfe.cn

Java: super.greet();
来源：http://zpa.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rlx.meibo888.top

Ruby: super
来源：http://mji.guowangkeji.top

C#:   base.Greet();
来源：http://dhk.zhoulong.xyz

[G08] 静态方法与属性
来源：http://oem.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rrl.zhongyouzk.top

PHP:  public static function f() {}
来源：http://dwd.tianlin.xyz

JS:   static f() {}
来源：http://avf.zdbjq.cn

TS:   static f(): void {}
来源：http://jsl.wangshuangyany.cn

Java: static void f() {}
来源：http://ptg.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gpl.hnqzz.top

Ruby: def self.f; end
来源：http://neg.gaohongyu789.top

C#:   public static void F() {}
来源：http://fdg.hammf.cn

[G09] 接口 / 抽象类
来源：http://rdy.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://ksr.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lat.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bnk.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://baq.cashguo.top

Java: interface Shape { double area(); }
来源：http://eas.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://kce.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sao.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://owo.xinyue.icu

[G10] 访问控制
来源：http://fno.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://gli.meibo888.top

PHP:  public / protected / private
来源：http://bag.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://bvb.cdnleiting.top

TS:   public / protected / private
来源：http://vxw.hammf.cn

Java: public / protected / private / 默认包级
来源：http://jrn.nanxinkj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lsb.nanxinkj.top

Ruby: public / protected / private
来源：http://nbk.sxryk.cn

C#:   public / protected / private / internal
来源：http://cjb.jinqigufen.top

[G11] getter / setter
来源：http://kxz.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://dsv.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://vtv.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://rmc.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://oiy.sufxvd.cn

Java: public String getName() { return name; }
来源：http://zed.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://bbd.sysykeji.top

Ruby: attr_accessor :name
来源：http://fck.tanke756.top

C#:   public string Name { get; set; }
来源：http://tou.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://rbh.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://hzg.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://obt.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://mvo.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://izj.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://kmm.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://tmm.andypj.xyz

Ruby: def to_s; @name; end
来源：http://del.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://mrl.birdmap.top

[G13] 判断对象类型
来源：http://rxd.uphjek.com

Py:   isinstance(u, User)
来源：http://kds.shuidangran.top

PHP:  $u instanceof User
来源：http://gvk.9152youxi.cn

JS:   u instanceof User
来源：http://djr.xinyue.icu

TS:   u instanceof User
来源：http://erx.smart0.xyz

Java: u instanceof User
来源：http://tsn.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qkb.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://lpg.zdbjq.cn

C#:   u is User
来源：http://sfb.hcnkem.com

[G14] 数据类 / record
来源：http://djd.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nzv.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ayf.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://wss.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://szk.tian-w.cn

Java: record User(String name, int age) {}
来源：http://ttw.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://yoa.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://osh.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://yqp.ehwqpu.com

[G15] 枚举
来源：http://qbv.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://llf.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://new.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kdp.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jkj.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://qvm.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ueb.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://dwc.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vox.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://awh.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sim.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://kwh.daria6918.cn

JS:   Object.entries(obj)
来源：http://sxd.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://dzr.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nkv.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mrz.sxryk.cn

Ruby: obj.instance_variables
来源：http://may.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://lle.ydjk.org.cn

================================================================================
来源：http://xlo.zhoulong.xyz

H. 异常与错误处理
来源：http://oty.fzhhl.top

================================================================================
来源：http://wko.havefunace.top

[H01] try / catch 基础
来源：http://vfs.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bgh.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rto.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ipa.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ppq.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kpl.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://asn.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lln.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://feq.cashguo.top

[H02] finally / ensure 收尾
来源：http://vuu.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://ifa.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vwc.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mse.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ayd.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://jpz.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gqm.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://hqf.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zqb.uphjek.com

[H03] 主动抛出异常
来源：http://slv.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://hur.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eul.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://mdz.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://hbr.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ghe.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://myi.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://igl.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://rtm.zhongyouzk.top

[H04] 自定义异常类型
来源：http://kzz.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://ril.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://bka.mhx1999.top

JS:   class MyError extends Error {}
来源：http://tbi.yvedp.cn

TS:   class MyError extends Error {}
来源：http://egy.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://hav.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pso.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://tng.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://wzf.gzhubu.top

[H05] 捕获特定类型
来源：http://hxd.xinyue.icu

Py:   except ValueError as e:
来源：http://kvs.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wqu.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://llm.gzhubu.top

TS:   if (e instanceof TypeError) {}
来源：http://gyz.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://wsk.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rok.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://bqp.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nnn.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://wig.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://aou.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://luk.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://tky.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://jkr.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mfg.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://wyt.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://ekn.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://ojx.fehbvm.com

[H07] 断言
来源：http://mmd.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://xzg.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://viq.c1oappe.top

JS:   console.assert(x > 0);
来源：http://ehc.sxryk.cn

TS:   console.assert(x > 0);
来源：http://jnp.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://biw.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ibn.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://pre.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://cpu.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://btn.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://bmf.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ujj.sufxvd.cn

JS:   e.message;  e.stack
来源：http://xxp.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ifk.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nku.shuidangran.top

Go:   err.Error()
来源：http://wcx.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://ynp.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://bki.zhoulong.xyz

[H09] 带错误码的异常
来源：http://sjx.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dsh.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kfu.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://alv.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qzn.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mkr.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wrw.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zzk.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://kcv.xuetiantiany.cn

[H10] 资源自动释放
来源：http://kyh.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ipr.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oph.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://exw.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://drq.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uac.hnqzz.top

Go:   defer f.Close()
来源：http://jca.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tpy.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://doc.zdbjq.cn

================================================================================
来源：http://baj.fehbvm.com

I. 正则表达式
来源：http://hqq.xylfe.cn

================================================================================
来源：http://grr.sjlbkw.cn

[I01] 判断是否匹配
来源：http://nui.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sra.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yep.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://kaw.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://lss.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sgj.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rfb.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://kim.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uzd.yanxiufei.cn

[I02] 提取所有匹配
来源：http://ogg.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://bgw.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hey.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fhs.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://aob.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fhn.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jii.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://yuz.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ovr.jinqigfzy.top

[I03] 提取捕获分组
来源：http://dgg.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fzc.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dgb.wangshuangyany.cn


<!-- 参考信息 -->