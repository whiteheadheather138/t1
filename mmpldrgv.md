代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://kpd.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://vlw.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ayp.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ber.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gro.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://dci.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jai.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zze.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zwz.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xpn.gotoacloud.top

[F11] 复制与移动文件
来源：http://aol.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dto.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qev.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://waw.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iem.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://umv.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qmz.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://afk.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rdn.gaohongyu789.top

[F12] CSV 读写
来源：http://juu.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wsn.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://swe.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hfj.chenlongwang.top

TS:   // 同上
来源：http://avb.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://igl.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qxz.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aco.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jbz.birdmap.top

================================================================================
来源：http://sdw.pycfn.com

G. 面向对象
来源：http://vez.yuxming.cn

================================================================================
来源：http://hqs.hfpthk.cn

[G01] 定义类
来源：http://iwh.meibo888.top

Py:   class User: pass
来源：http://nns.jiagoushi.top

PHP:  class User {}
来源：http://hbl.xylfe.cn

JS:   class User {}
来源：http://ngp.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://ecn.bbcook.cn

Java: class User {}
来源：http://txe.yueranfly.top

Go:   type User struct { Name string }
来源：http://tww.guowangkeji.top

Ruby: class User; end
来源：http://dnz.c1oappe.top

C#:   class User {}
来源：http://wzb.sweek.top

[G02] 构造函数
来源：http://yep.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://xir.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://rob.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://jax.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://mxq.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://mne.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://arp.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://gkp.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://sxx.ydzc1.top

[G03] 实例属性
来源：http://ydz.dashuyun.cn

Py:   self.name = "x"
来源：http://tzg.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://fed.havefunace.top

JS:   this.name = "x";
来源：http://pvz.xziqi.cn

TS:   name: string = "x";
来源：http://rbz.sjlbkw.cn

Java: private String name;
来源：http://amn.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qbl.xinyue.icu

Ruby: @name = "x"
来源：http://tpg.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://lfv.vehdjk.com

[G04] 定义方法
来源：http://tlj.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://cul.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cmf.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://adv.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://ljn.zhengqikj.top

Java: String greet() { return name; }
来源：http://uii.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xss.hywenlv.cn

Ruby: def greet; @name; end
来源：http://npr.epnwcf.com

C#:   public string Greet() => Name;
来源：http://rhq.vqdsnc.cn

[G05] 继承
来源：http://ris.guowangkeji.top

Py:   class Admin(User): pass
来源：http://vno.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://yfc.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://unx.cheryme.top

TS:   class Admin extends User {}
来源：http://ocj.zhijiandao.cn

Java: class Admin extends User {}
来源：http://fvc.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wlv.zhixingplan.top

Ruby: class Admin < User; end
来源：http://rsy.iojbl.cn

C#:   class Admin : User {}
来源：http://zwo.hysaishi.cn

[G06] 重写方法
来源：http://sxy.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://zls.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fvc.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://iut.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://gvr.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://qji.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hnr.birdmap.top

Ruby: def greet; "admin"; end
来源：http://ulu.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://eyt.wangshuangyany.cn

[G07] 调用父类方法
来源：http://xov.xuanzx.com

Py:   super().greet()
来源：http://ena.bjfxy.top

PHP:  parent::greet();
来源：http://oqc.shanyushiyangtech.top

JS:   super.greet();
来源：http://bjp.mhx1999.top

TS:   super.greet();
来源：http://qsd.yueranfly.top

Java: super.greet();
来源：http://gmq.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qid.zycfv.cn

Ruby: super
来源：http://utl.guannengcc.top

C#:   base.Greet();
来源：http://wos.nanxuanxn.top

[G08] 静态方法与属性
来源：http://mxg.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ele.316326.xyz

PHP:  public static function f() {}
来源：http://mnx.kuanghao11.cn

JS:   static f() {}
来源：http://uum.shangyingyoupin.top

TS:   static f(): void {}
来源：http://pwv.bbcook.cn

Java: static void f() {}
来源：http://wvk.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nol.xziqi.cn

Ruby: def self.f; end
来源：http://qel.fktsv.cn

C#:   public static void F() {}
来源：http://fwv.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://jyf.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://ehj.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://tng.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gds.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://pac.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://wxb.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://olw.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ail.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://iju.fehbvm.com

[G10] 访问控制
来源：http://rlb.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://dko.zhoulong.xyz

PHP:  public / protected / private
来源：http://hvh.hnxiangtu.top

JS:   #private 字段；其余公开
来源：http://hgc.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://lnc.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://nii.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uka.yfazqb.com

Ruby: public / protected / private
来源：http://kiu.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://zdl.mhx1999.top

[G11] getter / setter
来源：http://qps.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://ghl.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ltf.bbcook.cn

JS:   get name() { return this._name; }
来源：http://rbj.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://ddk.cucudq.cn

Java: public String getName() { return name; }
来源：http://jjq.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sni.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://btg.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://lcb.andypj.xyz

[G12] 对象转字符串
来源：http://cwj.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://piz.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wit.pycfn.com

JS:   toString() { return this.name; }
来源：http://och.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://nvx.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://nby.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://idg.sysykeji.top

Ruby: def to_s; @name; end
来源：http://pht.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://kuc.xziqi.cn

[G13] 判断对象类型
来源：http://fba.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://ynx.nwbrower.top

PHP:  $u instanceof User
来源：http://zyx.cdnleiting.top

JS:   u instanceof User
来源：http://tug.hnxiangtu.top

TS:   u instanceof User
来源：http://tzq.meibo888.top

Java: u instanceof User
来源：http://ewd.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fut.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://lzn.smart0.xyz

C#:   u is User
来源：http://kjy.xylfe.cn

[G14] 数据类 / record
来源：http://tuc.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jum.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://gfy.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://xkg.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://hmq.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://ebl.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://vin.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jcy.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://rpv.ydzc1.top

[G15] 枚举
来源：http://szu.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://etd.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nie.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://brw.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oue.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://mxi.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iww.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://kwt.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yww.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://skp.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wwk.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://txf.yuanzhike.top

JS:   Object.entries(obj)
来源：http://blp.hnqzz.top

TS:   Object.entries(obj)
来源：http://fhc.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rew.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iqx.ivvv.top

Ruby: obj.instance_variables
来源：http://ixd.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://yrg.ehwqpu.com

================================================================================
来源：http://xbd.sweek.top

H. 异常与错误处理
来源：http://zlo.nanxuanxn.top

================================================================================
来源：http://uei.redwolf501.top

[H01] try / catch 基础
来源：http://ilq.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xgp.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vzt.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zuc.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rwj.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rph.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hxn.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vkz.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gxe.316326.xyz

[H02] finally / ensure 收尾
来源：http://dmx.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://mti.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yhx.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fef.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nbl.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://uwq.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://elj.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zbt.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eop.jyoumei.cn

[H03] 主动抛出异常
来源：http://fnb.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://sod.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gct.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://pxd.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://gqc.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jii.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://duh.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qdt.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fbd.52xcode.cn

[H04] 自定义异常类型
来源：http://toz.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://uip.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vbg.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://dwv.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://ozk.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://mda.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xhh.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://emm.sysykeji.top

C#:   class MyException : Exception {}
来源：http://zwt.dianchejie.cn

[H05] 捕获特定类型
来源：http://pav.birdmap.top

Py:   except ValueError as e:
来源：http://tkt.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://esi.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://uln.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://ndr.xinyue.icu

Java: catch (IOException | SQLException e) {}
来源：http://hzp.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mxz.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://oxs.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jdi.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://uni.cashguo.top

Py:   value = d.get("k") or default
来源：http://hbn.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://yyn.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://ljc.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://xza.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ffy.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dwl.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://uky.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://pts.fanxiaobao.xyz

[H07] 断言
来源：http://wzk.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://mdd.cqqwz.cn

PHP:  assert($x > 0);
来源：http://gqf.meibo888.top

JS:   console.assert(x > 0);
来源：http://zeo.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://prw.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://pva.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sgp.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vqh.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://gze.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://utu.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://lgw.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dxn.zhixingplan.top

JS:   e.message;  e.stack
来源：http://sdg.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jiv.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tem.ywan-chungtsiang.top

Go:   err.Error()
来源：http://pkw.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://tgl.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://rbj.ydjk.org.cn

[H09] 带错误码的异常
来源：http://zbg.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nza.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eln.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nrn.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dcj.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uak.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bnq.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kiy.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vrd.yvedp.cn

[H10] 资源自动释放
来源：http://wmp.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://czo.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://olf.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://led.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ahz.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xsj.gotoacloud.top

Go:   defer f.Close()
来源：http://nhx.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ght.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ufq.cheryme.top

================================================================================
来源：http://blm.cheryme.top

I. 正则表达式
来源：http://mmf.yanxiufei.cn

================================================================================
来源：http://ixb.epnwcf.com

[I01] 判断是否匹配
来源：http://ctm.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cid.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://lwi.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://uew.iojbl.cn

TS:   /\d+/.test(s)
来源：http://txq.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rpw.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://suj.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://eia.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vzp.chenlongwang.top

[I02] 提取所有匹配
来源：http://yfx.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://vlw.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xen.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dfj.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://bnl.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mkx.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uzm.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://cjp.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rxi.mhx1999.top

[I03] 提取捕获分组
来源：http://ryx.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://epd.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ibd.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lli.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pao.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hcy.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jrz.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pff.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rel.wangdashe.top

[I04] 正则替换
来源：http://dli.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://ern.chenlongwang.top


<!-- 参考信息 -->