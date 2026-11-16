代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://goz.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://flh.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://lsy.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://uzf.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pas.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zay.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://okn.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://rbm.svipenyu.cn

[F09] 获取文件大小
来源：http://czb.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://cve.zycfv.cn

PHP:  filesize("a.txt");
来源：http://xru.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://sew.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://iwf.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://ugu.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://boa.yueranfly.top

Ruby: File.size("a.txt")
来源：http://zxl.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://zjv.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://pwm.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qzn.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ykf.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fcn.pycfn.com

TS:   path.extname("a.txt")
来源：http://wqs.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nae.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dmi.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rfl.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fyh.ybcxt.top

[F11] 复制与移动文件
来源：http://utb.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tgj.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ial.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hxd.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pmp.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ebt.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uuy.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://umr.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pib.daria6918.cn

[F12] CSV 读写
来源：http://nze.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ufz.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ama.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hba.cdnleiting.top

TS:   // 同上
来源：http://ojp.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hee.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oqt.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bfu.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jaa.ywan-chungtsiang.top

================================================================================
来源：http://uwn.ppjwa.cn

G. 面向对象
来源：http://tuj.zhixingplan.top

================================================================================
来源：http://ird.zhoulong.xyz

[G01] 定义类
来源：http://owv.jqgufenzy.top

Py:   class User: pass
来源：http://tlu.shanyushiyangtech.top

PHP:  class User {}
来源：http://eyl.sufxvd.cn

JS:   class User {}
来源：http://xvl.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://hga.dianchejie.cn

Java: class User {}
来源：http://apu.xuanzx.com

Go:   type User struct { Name string }
来源：http://lgw.jinqigufen.top

Ruby: class User; end
来源：http://spn.tanke756.top

C#:   class User {}
来源：http://xcj.jlsjyb.cn

[G02] 构造函数
来源：http://fnm.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://nop.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://ugn.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://ylb.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://ikm.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://uni.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rcz.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://waf.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://bpt.cdnleiting.top

[G03] 实例属性
来源：http://lru.0kj1m.cn

Py:   self.name = "x"
来源：http://ctw.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://jui.meibo888.top

JS:   this.name = "x";
来源：http://phe.cqqwz.cn

TS:   name: string = "x";
来源：http://byp.gogol.net.cn

Java: private String name;
来源：http://hvj.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bin.guannengcc.top

Ruby: @name = "x"
来源：http://lsy.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://dnm.316326.xyz

[G04] 定义方法
来源：http://rcu.yvedp.cn

Py:   def greet(self): return self.name
来源：http://raz.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://udu.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://sac.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://ink.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://rlz.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bcl.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://isb.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://yrg.zhoulong.xyz

[G05] 继承
来源：http://stq.dashuyun.cn

Py:   class Admin(User): pass
来源：http://clv.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://yts.sysykeji.top

JS:   class Admin extends User {}
来源：http://pep.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://zlu.aizwys.cn

Java: class Admin extends User {}
来源：http://dbi.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nmn.xziqi.cn

Ruby: class Admin < User; end
来源：http://ian.daria6918.cn

C#:   class Admin : User {}
来源：http://qyt.hnxiangtu.top

[G06] 重写方法
来源：http://gvm.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://dqk.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qws.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://ban.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://pid.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ekn.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vja.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://bom.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://dzq.zhijiandao.cn

[G07] 调用父类方法
来源：http://yxq.uphjek.com

Py:   super().greet()
来源：http://bps.xylfe.cn

PHP:  parent::greet();
来源：http://bem.yj202588.top

JS:   super.greet();
来源：http://fbd.uphjek.com

TS:   super.greet();
来源：http://jjd.yfazqb.com

Java: super.greet();
来源：http://ada.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uyr.shzxlz.cn

Ruby: super
来源：http://pzx.pycfn.com

C#:   base.Greet();
来源：http://rno.yj20258888.top

[G08] 静态方法与属性
来源：http://rgf.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rtq.zhixingplan.top

PHP:  public static function f() {}
来源：http://mgg.smart0.xyz

JS:   static f() {}
来源：http://lud.aibaodan.cn

TS:   static f(): void {}
来源：http://uav.nanxuanxn.top

Java: static void f() {}
来源：http://uta.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iwv.yuanzhike.top

Ruby: def self.f; end
来源：http://hjk.meibo888.top

C#:   public static void F() {}
来源：http://zfk.sweek.top

[G09] 接口 / 抽象类
来源：http://iog.andypj.xyz

Py:   from abc import ABC, abstractmethod
来源：http://due.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://lrf.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqd.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://iyh.nwbrower.top

Java: interface Shape { double area(); }
来源：http://zpi.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://qgi.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hxn.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://hsu.hongshengwenyu.top

[G10] 访问控制
来源：http://bak.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://yzm.fehbvm.com

PHP:  public / protected / private
来源：http://mkn.hnqzz.top

JS:   #private 字段；其余公开
来源：http://fcs.sjlbkw.cn

TS:   public / protected / private
来源：http://ffb.yonumen.top

Java: public / protected / private / 默认包级
来源：http://qiy.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ifl.yanxiufei.cn

Ruby: public / protected / private
来源：http://lou.chenlongwang.top

C#:   public / protected / private / internal
来源：http://ovk.yangfankeji.com

[G11] getter / setter
来源：http://dvq.nwbrower.top

Py:   @property 与 @x.setter
来源：http://bwp.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://esr.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://syd.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://lfc.daxiang520.top

Java: public String getName() { return name; }
来源：http://rls.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://dhs.hammf.cn

Ruby: attr_accessor :name
来源：http://dsq.cheryme.top

C#:   public string Name { get; set; }
来源：http://vrx.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://oji.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://vit.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dtn.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://dac.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://jvi.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://eez.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://kfj.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://rvj.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://ilw.feifeiyinyue.top

[G13] 判断对象类型
来源：http://ran.yuxming.cn

Py:   isinstance(u, User)
来源：http://iar.hysaishi.cn

PHP:  $u instanceof User
来源：http://wgc.nanxinkj.top

JS:   u instanceof User
来源：http://fag.zhoulong.xyz

TS:   u instanceof User
来源：http://glj.hywenlv.cn

Java: u instanceof User
来源：http://edc.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zgf.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://qzd.sweek.top

C#:   u is User
来源：http://hpl.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://mob.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://inl.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://iij.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://ttv.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://mkn.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://vgz.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://uqz.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cfn.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://mjj.pycfn.com

[G15] 枚举
来源：http://kio.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://znb.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bpo.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wbh.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oic.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://bfh.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://odv.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://mif.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jfb.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://rsx.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tcn.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://cjp.meibo888.top

JS:   Object.entries(obj)
来源：http://pkd.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://bsm.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rru.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yjn.ydzc1.top

Ruby: obj.instance_variables
来源：http://brj.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://iad.chenzaomai.com

================================================================================
来源：http://xfs.xuanzx.com

H. 异常与错误处理
来源：http://eqb.gaohongyu789.top

================================================================================
来源：http://lpd.fehbvm.com

[H01] try / catch 基础
来源：http://gud.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xwc.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bdm.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ccr.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://arj.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://noh.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pfc.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xgs.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rhl.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://bkh.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://ven.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cuh.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mzw.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dim.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://nxk.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rzr.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zis.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yrq.yueranfly.top

[H03] 主动抛出异常
来源：http://gvq.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://rtl.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rri.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://fyd.uphjek.com

TS:   throw new Error("错误信息");
来源：http://aiv.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://dpt.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gsi.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://toe.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rez.birdmap.top

[H04] 自定义异常类型
来源：http://ukc.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://kbl.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://jqg.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://kuq.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://sgv.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://gej.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oov.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://gri.ybcxt.top

C#:   class MyException : Exception {}
来源：http://wsw.jqgufenzy.top

[H05] 捕获特定类型
来源：http://jqc.ivvv.top

Py:   except ValueError as e:
来源：http://tgn.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://asf.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://tnx.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://zqk.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://zfs.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yit.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://ohd.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xju.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://mbp.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://uyf.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://bth.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gln.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://slm.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xqh.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zmh.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://mgj.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://dng.jinqigufen.top

[H07] 断言
来源：http://fyj.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://gor.guannengcc.top

PHP:  assert($x > 0);
来源：http://bbx.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://qpl.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://qto.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://eua.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tlq.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://ftj.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://ycf.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://kpc.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://xce.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://twi.daria6918.cn

JS:   e.message;  e.stack
来源：http://dpo.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://azy.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sde.wangdashe.top

Go:   err.Error()
来源：http://vma.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://rxf.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://jee.dashuyun.cn

[H09] 带错误码的异常
来源：http://kbp.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hnw.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdt.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hzf.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iik.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jgv.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oas.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://rkb.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hmy.ehwqpu.com

[H10] 资源自动释放
来源：http://fcp.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rir.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sei.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ybm.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mua.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mkq.meibo888.top

Go:   defer f.Close()
来源：http://dyc.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mfy.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ksk.gotoacloud.top

================================================================================
来源：http://msb.bjfxy.top

I. 正则表达式
来源：http://tau.aibaodan.cn

================================================================================
来源：http://kql.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://oli.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://klt.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://xcr.sxryk.cn

JS:   /\d+/.test(s)
来源：http://czo.nwbrower.top

TS:   /\d+/.test(s)
来源：http://sit.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://efp.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uxq.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://wot.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fyh.yvedp.cn

[I02] 提取所有匹配
来源：http://qqi.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://dhe.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hdq.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lsm.cqqwz.cn


<!-- 参考信息 -->