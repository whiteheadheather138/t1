代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://qmx.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wop.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://fdc.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://qyk.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wuf.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oak.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://vcl.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://pyd.cheryme.top

[F09] 获取文件大小
来源：http://jmc.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://ltx.gzhubu.top

PHP:  filesize("a.txt");
来源：http://fke.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://gdd.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://qsf.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://evy.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vbi.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://ibg.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://kkz.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://cok.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ufr.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://opc.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gbp.guannengcc.top

TS:   path.extname("a.txt")
来源：http://yyw.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nih.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tan.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dbs.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fbj.dianchejie.cn

[F11] 复制与移动文件
来源：http://kte.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hom.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cpe.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sib.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://huy.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ywh.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dwl.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ese.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xod.tanke756.top

[F12] CSV 读写
来源：http://fdb.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://agt.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ipm.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://icv.quarkkingdee.top

TS:   // 同上
来源：http://vbc.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dwz.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lbf.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hoy.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bew.quarkkingdee.top

================================================================================
来源：http://ywt.52xcode.cn

G. 面向对象
来源：http://khm.xinyue.icu

================================================================================
来源：http://ppb.smart0.xyz

[G01] 定义类
来源：http://hvz.shanyushiyangtech.top

Py:   class User: pass
来源：http://wnp.ywan-chungtsiang.top

PHP:  class User {}
来源：http://wjm.chenzaomai.com

JS:   class User {}
来源：http://gvq.feifeiyinyue.top

TS:   class User { name: string = ""; }
来源：http://yie.jqgufenzy.top

Java: class User {}
来源：http://vtz.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://ngc.hywenlv.cn

Ruby: class User; end
来源：http://ksw.hongshengwenyu.top

C#:   class User {}
来源：http://wbg.yj202588.top

[G02] 构造函数
来源：http://szh.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://aft.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://fgf.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://vyv.cashguo.top

TS:   constructor(public name: string) {}
来源：http://nve.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://ktj.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xgn.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://iah.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://iul.pycfn.com

[G03] 实例属性
来源：http://iwa.chenlongwang.top

Py:   self.name = "x"
来源：http://dvv.tanke756.top

PHP:  public string $name = "x";
来源：http://hbb.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://hxk.aizwys.cn

TS:   name: string = "x";
来源：http://qmn.fehbvm.com

Java: private String name;
来源：http://bsy.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yyx.cqqwz.cn

Ruby: @name = "x"
来源：http://ppe.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://wxw.zhengqikj.top

[G04] 定义方法
来源：http://zbm.sysykeji.top

Py:   def greet(self): return self.name
来源：http://kma.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ule.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://dmx.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://olp.jinqigufen.top

Java: String greet() { return name; }
来源：http://moj.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rwn.sysykeji.top

Ruby: def greet; @name; end
来源：http://tlm.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://qib.yuanzhike.top

[G05] 继承
来源：http://rkb.hammf.cn

Py:   class Admin(User): pass
来源：http://btc.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://fma.ctjpmb.com

JS:   class Admin extends User {}
来源：http://ubz.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://qob.hnxiangtu.top

Java: class Admin extends User {}
来源：http://gml.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uvo.yueranfly.top

Ruby: class Admin < User; end
来源：http://zmx.zhongyouzk.top

C#:   class Admin : User {}
来源：http://olv.jyoumei.cn

[G06] 重写方法
来源：http://egg.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://ojf.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://oob.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://ttv.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://wek.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://pja.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://imw.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://csf.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://vjk.gotoacloud.top

[G07] 调用父类方法
来源：http://svs.hnqzz.top

Py:   super().greet()
来源：http://cgn.cheryme.top

PHP:  parent::greet();
来源：http://pxe.ivvv.top

JS:   super.greet();
来源：http://fpz.pengpengdd.cyou

TS:   super.greet();
来源：http://qkv.snrcjt.cn

Java: super.greet();
来源：http://kfe.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://srp.daxiang520.top

Ruby: super
来源：http://kfn.mhx1999.top

C#:   base.Greet();
来源：http://alv.zhoulong.xyz

[G08] 静态方法与属性
来源：http://pwa.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hfw.tarul.cn

PHP:  public static function f() {}
来源：http://jht.jinyuanbaomall.cn

JS:   static f() {}
来源：http://yna.daria6918.cn

TS:   static f(): void {}
来源：http://tpq.aizwys.cn

Java: static void f() {}
来源：http://ats.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xvi.jqgfzy.top

Ruby: def self.f; end
来源：http://qxd.vqdsnc.cn

C#:   public static void F() {}
来源：http://ljt.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://rwe.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://huc.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://qci.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nrf.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://pkw.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://tmh.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://vem.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://may.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://uoj.ehwqpu.com

[G10] 访问控制
来源：http://hqm.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://gyi.sysykeji.top

PHP:  public / protected / private
来源：http://lge.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://bge.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://yjj.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://pvt.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://obw.jinqigfzy.top

Ruby: public / protected / private
来源：http://yln.fengsongda.top

C#:   public / protected / private / internal
来源：http://wov.gogol.net.cn

[G11] getter / setter
来源：http://mjt.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://aar.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://soi.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://llb.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://vvd.yvedp.cn

Java: public String getName() { return name; }
来源：http://gpj.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hvs.hammf.cn

Ruby: attr_accessor :name
来源：http://iel.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://mjj.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://ymn.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://gls.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nty.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://flv.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://bbj.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://lmy.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vyo.zycfv.cn

Ruby: def to_s; @name; end
来源：http://mvt.sweek.top

C#:   public override string ToString() => Name;
来源：http://hca.xuanzx.com

[G13] 判断对象类型
来源：http://wif.haohaochexian.top

Py:   isinstance(u, User)
来源：http://uia.fktsv.cn

PHP:  $u instanceof User
来源：http://csn.yuanzhike.top

JS:   u instanceof User
来源：http://klt.smart0.xyz

TS:   u instanceof User
来源：http://pip.fktsv.cn

Java: u instanceof User
来源：http://ffk.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nvy.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://uvn.zhixingplan.top

C#:   u is User
来源：http://hwg.shangyingyoupin.top

[G14] 数据类 / record
来源：http://fpd.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://spy.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://ohp.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kgd.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://jmz.epnwcf.com

Java: record User(String name, int age) {}
来源：http://bav.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://xad.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://omw.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://spf.jinghuilouyu.cn

[G15] 枚举
来源：http://owm.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ouh.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gpd.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lnr.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ila.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://ztn.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://heg.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://tub.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qiv.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://xmo.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vgy.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://sev.fengsongda.top

JS:   Object.entries(obj)
来源：http://hvt.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://wug.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yzn.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://zcz.ydzc1.top

Ruby: obj.instance_variables
来源：http://avg.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://flp.hysaishi.cn

================================================================================
来源：http://hjp.dashuyun.cn

H. 异常与错误处理
来源：http://dej.gaohongyu789.top

================================================================================
来源：http://exo.daria6918.cn

[H01] try / catch 基础
来源：http://svx.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qxy.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bcy.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ivb.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dor.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eeb.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cpt.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fuy.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wwr.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://xqg.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://rmt.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ggp.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pju.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mqp.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://ade.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://plb.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xey.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hkx.dashuyun.cn

[H03] 主动抛出异常
来源：http://uqm.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://ryh.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://azo.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://xab.chenjidiqi.icu

TS:   throw new Error("错误信息");
来源：http://ybl.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dkf.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ejj.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://byj.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wzq.epnwcf.com

[H04] 自定义异常类型
来源：http://wgk.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://ptk.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://xis.meibo888.top

JS:   class MyError extends Error {}
来源：http://jkb.ydzc1.top

TS:   class MyError extends Error {}
来源：http://qnu.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://hke.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wgd.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://qli.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://blm.ydjk.org.cn

[H05] 捕获特定类型
来源：http://kpz.316326.xyz

Py:   except ValueError as e:
来源：http://ius.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dca.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://yuv.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://mdb.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://kfb.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://apt.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://qdi.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rcl.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://mph.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://sxq.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://okc.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cgz.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xye.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vcn.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hwt.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://ebg.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://wht.zhaomingkeji.xyz

[H07] 断言
来源：http://svn.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://xmf.fktsv.cn

PHP:  assert($x > 0);
来源：http://jjl.redwolf501.top

JS:   console.assert(x > 0);
来源：http://byg.fengsongda.top

TS:   console.assert(x > 0);
来源：http://ztn.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://qzu.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yzm.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://pah.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://erw.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://nfu.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://spi.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wug.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://hmd.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zwr.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://awk.xinyue.icu

Go:   err.Error()
来源：http://cxb.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://vpc.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://dus.bjfxy.top

[H09] 带错误码的异常
来源：http://cwq.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hcl.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://mxt.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ban.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dtq.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lbr.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://byx.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://hiu.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gjs.sxryk.cn

[H10] 资源自动释放
来源：http://qpu.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qek.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vco.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sdw.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ejg.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gkj.dashuyun.cn

Go:   defer f.Close()
来源：http://gls.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lzn.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ami.ydzc1.top

================================================================================
来源：http://lim.sweek.top

I. 正则表达式
来源：http://cdf.daria6918.cn

================================================================================
来源：http://ekn.hfpthk.cn

[I01] 判断是否匹配
来源：http://gca.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qqa.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://dwh.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://dlh.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://bmq.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jbf.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rue.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://nyn.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mjb.yongpay.top

[I02] 提取所有匹配
来源：http://ivo.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://fwx.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gja.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xum.cqqwz.cn


<!-- 参考信息 -->