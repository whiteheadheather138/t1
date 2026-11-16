代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hhs.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zup.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://oto.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://iap.jqgfzy.top

[F09] 获取文件大小
来源：http://ddf.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://hti.andypj.xyz

PHP:  filesize("a.txt");
来源：http://lyw.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://fcj.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://pwh.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://ywt.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://amn.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://ugs.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://trv.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://zdl.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ufa.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://azo.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://idg.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://afq.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bwt.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://apf.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vum.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://viw.yfazqb.com

[F11] 复制与移动文件
来源：http://ukg.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dye.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://olk.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cqy.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wfj.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xem.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qbg.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mqh.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xgw.bbcook.cn

[F12] CSV 读写
来源：http://gzs.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qnj.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sjm.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jjg.yanxiufei.cn

TS:   // 同上
来源：http://tci.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bqw.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://swo.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uax.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ypq.zycfv.cn

================================================================================
来源：http://unl.yj202588.top

G. 面向对象
来源：http://bqs.smart0.xyz

================================================================================
来源：http://fww.mhx1999.top

[G01] 定义类
来源：http://mcu.bbcook.cn

Py:   class User: pass
来源：http://cxx.ctjpmb.com

PHP:  class User {}
来源：http://jkh.cashguo.top

JS:   class User {}
来源：http://eel.yonumen.top

TS:   class User { name: string = ""; }
来源：http://ero.hfpthk.cn

Java: class User {}
来源：http://qaa.52xcode.cn

Go:   type User struct { Name string }
来源：http://rnc.yuxming.cn

Ruby: class User; end
来源：http://otg.tarul.cn

C#:   class User {}
来源：http://ctm.tarul.cn

[G02] 构造函数
来源：http://sry.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://wop.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://caz.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://bua.birdmap.top

TS:   constructor(public name: string) {}
来源：http://wlj.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://eid.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jvu.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://nju.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://vzj.aizwys.cn

[G03] 实例属性
来源：http://apt.ydzc1.top

Py:   self.name = "x"
来源：http://hiy.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://xku.yj20258888.top

JS:   this.name = "x";
来源：http://szb.tanke756.top

TS:   name: string = "x";
来源：http://ywg.gzhubu.top

Java: private String name;
来源：http://jrx.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://byt.bjfxy.top

Ruby: @name = "x"
来源：http://zbd.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://lwg.daxiang520.top

[G04] 定义方法
来源：http://mqr.hcnkem.com

Py:   def greet(self): return self.name
来源：http://rgb.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uqd.yfazqb.com

JS:   greet() { return this.name; }
来源：http://png.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://slu.hammf.cn

Java: String greet() { return name; }
来源：http://bhw.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mto.fengsongda.top

Ruby: def greet; @name; end
来源：http://csk.aizwys.cn

C#:   public string Greet() => Name;
来源：http://qjf.gotoacloud.top

[G05] 继承
来源：http://hhp.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://orv.yuxming.cn

PHP:  class Admin extends User {}
来源：http://tnl.nwbrower.top

JS:   class Admin extends User {}
来源：http://chh.epnwcf.com

TS:   class Admin extends User {}
来源：http://vjz.ybcxt.top

Java: class Admin extends User {}
来源：http://swa.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uug.zycfv.cn

Ruby: class Admin < User; end
来源：http://oct.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://mzb.kuanghao11.cn

[G06] 重写方法
来源：http://dlq.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://yxh.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yim.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://nkv.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://pgs.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://kox.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wil.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://zff.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://oip.feifeiyinyue.top

[G07] 调用父类方法
来源：http://btx.ppjwa.cn

Py:   super().greet()
来源：http://cne.wangshuangyany.cn

PHP:  parent::greet();
来源：http://pwk.hnqzz.top

JS:   super.greet();
来源：http://beg.ehwqpu.com

TS:   super.greet();
来源：http://szl.pycfn.com

Java: super.greet();
来源：http://wkk.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://umw.sweek.top

Ruby: super
来源：http://jgo.uphjek.com

C#:   base.Greet();
来源：http://nju.chenlongwang.top

[G08] 静态方法与属性
来源：http://wbp.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dkk.nwbrower.top

PHP:  public static function f() {}
来源：http://jis.tian-w.cn

JS:   static f() {}
来源：http://szr.daria6918.cn

TS:   static f(): void {}
来源：http://gbt.yuxming.cn

Java: static void f() {}
来源：http://bfq.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://clc.xylfe.cn

Ruby: def self.f; end
来源：http://rng.fzhhl.top

C#:   public static void F() {}
来源：http://ymg.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://qzy.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://fhi.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://qic.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yyi.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://rdb.iojbl.cn

Java: interface Shape { double area(); }
来源：http://vcd.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://rza.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mhr.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://eth.gotoacloud.top

[G10] 访问控制
来源：http://ebd.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://dtt.yangfankeji.com

PHP:  public / protected / private
来源：http://qzz.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://epk.shanyushiyangtech.top

TS:   public / protected / private
来源：http://rao.hammf.cn

Java: public / protected / private / 默认包级
来源：http://hmy.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://izm.xuanzx.com

Ruby: public / protected / private
来源：http://jrx.zhixingplan.top

C#:   public / protected / private / internal
来源：http://svp.hnqzz.top

[G11] getter / setter
来源：http://nsu.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://jtj.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wyu.yfazqb.com

JS:   get name() { return this._name; }
来源：http://txv.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://xkh.fengsongda.top

Java: public String getName() { return name; }
来源：http://kuq.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://phy.xziqi.cn

Ruby: attr_accessor :name
来源：http://grl.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://pem.kuanghao11.cn

[G12] 对象转字符串
来源：http://jkd.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://qfq.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zyz.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://jfe.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://rxv.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://cqx.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://fww.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://bqv.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://hpl.yanxiufei.cn

[G13] 判断对象类型
来源：http://tjr.hammf.cn

Py:   isinstance(u, User)
来源：http://rvf.vehdjk.com

PHP:  $u instanceof User
来源：http://trd.jinqigufen.top

JS:   u instanceof User
来源：http://wit.yuanzhike.top

TS:   u instanceof User
来源：http://awp.nwbrower.top

Java: u instanceof User
来源：http://iwr.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cnc.havefunace.top

Ruby: u.is_a?(User)
来源：http://ljv.sweek.top

C#:   u is User
来源：http://faz.ybcxt.top

[G14] 数据类 / record
来源：http://flu.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://owh.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://oxr.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://non.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://ezs.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://eau.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://slb.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ntu.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://mvo.jinqigfzy.top

[G15] 枚举
来源：http://uzk.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aiy.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ere.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jyj.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bsz.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://oit.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gph.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://dep.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gix.fehbvm.com

[G16] 对象转数组 / 字典
来源：http://bgg.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oca.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://xpk.fzhhl.top

JS:   Object.entries(obj)
来源：http://yct.smart0.xyz

TS:   Object.entries(obj)
来源：http://lwe.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gck.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ois.tian-w.cn

Ruby: obj.instance_variables
来源：http://pje.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://yss.xuetiantiany.cn

================================================================================
来源：http://idv.tarul.cn

H. 异常与错误处理
来源：http://pzr.jinghuilouyu.cn

================================================================================
来源：http://bhh.yj20258888.top

[H01] try / catch 基础
来源：http://pot.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eyz.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vxv.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kvi.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfe.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bbp.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fth.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eez.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tki.hcnkem.com

[H02] finally / ensure 收尾
来源：http://lhr.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dqk.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zcw.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ovh.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qpp.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bnk.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hit.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://mtz.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mpj.svipenyu.cn

[H03] 主动抛出异常
来源：http://rdu.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://ruf.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hsi.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://xto.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://tan.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oqi.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qzl.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wgb.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://vyr.kuanghao11.cn

[H04] 自定义异常类型
来源：http://oek.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://uke.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sta.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://kwx.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://wny.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://dhh.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eja.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://uqs.fengsongda.top

C#:   class MyException : Exception {}
来源：http://kbn.ydzc1.top

[H05] 捕获特定类型
来源：http://bpt.jlsjyb.cn

Py:   except ValueError as e:
来源：http://wmx.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hab.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://yrf.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://zwl.jianghu66.top

Java: catch (IOException | SQLException e) {}
来源：http://zpw.cdnleiting.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dyd.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://xuk.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jgg.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://ika.yongpay.top

Py:   value = d.get("k") or default
来源：http://gva.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://vvt.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://jin.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://anw.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://byg.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kuq.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://tpl.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://dpq.nanxuanxn.top

[H07] 断言
来源：http://gwp.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://yxj.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://uqp.gzhubu.top

JS:   console.assert(x > 0);
来源：http://msx.yonumen.top

TS:   console.assert(x > 0);
来源：http://yvp.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://jrp.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wzo.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://ild.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://euj.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://jto.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://mdj.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ehw.yueranfly.top

JS:   e.message;  e.stack
来源：http://lpt.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tcr.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ter.hysaishi.cn

Go:   err.Error()
来源：http://tit.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://blv.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://rkc.xinyue.icu

[H09] 带错误码的异常
来源：http://huo.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jal.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://laj.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bsw.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rhu.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://myo.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pvt.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zhw.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wth.zhijiandao.cn

[H10] 资源自动释放
来源：http://iwv.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://orb.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rbr.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ozf.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cdi.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lrv.nanxuanxn.top

Go:   defer f.Close()
来源：http://ryp.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aqj.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jga.shzxlz.cn

================================================================================
来源：http://ube.shangyingyoupin.top

I. 正则表达式
来源：http://ymj.cheryme.top

================================================================================
来源：http://zui.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://iml.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wis.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ffi.yongpay.top

JS:   /\d+/.test(s)
来源：http://uah.yonumen.top

TS:   /\d+/.test(s)
来源：http://fbf.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://neh.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jot.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://fjv.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cji.sxryk.cn

[I02] 提取所有匹配
来源：http://ckw.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://btt.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ykj.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wdw.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://ony.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fss.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ebn.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://fot.zhijiandao.cn


<!-- 参考信息 -->