代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://igx.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aik.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nyu.cqqwz.cn

[F08] 遍历目录
来源：http://pha.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mxn.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pck.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://bsv.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://clm.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://piu.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fdp.iojbl.cn

Ruby: Dir.children("dir")
来源：http://ixh.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://nrp.hongshengwenyu.top

[F09] 获取文件大小
来源：http://pbn.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://qbf.xinyue.icu

PHP:  filesize("a.txt");
来源：http://lvu.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://yoq.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://gsz.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://swe.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://npg.jianghu66.top

Ruby: File.size("a.txt")
来源：http://rkl.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://hvq.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://nus.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://agu.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://stt.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gxi.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://vad.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dsd.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fpw.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://snm.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zuj.ydzc1.top

[F11] 复制与移动文件
来源：http://naf.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ejr.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eue.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://erm.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pgz.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ewy.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zlj.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tdi.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pwt.vehdjk.com

[F12] CSV 读写
来源：http://uez.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vxj.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ief.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mzc.jinqigufen.top

TS:   // 同上
来源：http://ljl.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wyv.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mbu.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tpm.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tog.zhaomingkeji.xyz

================================================================================
来源：http://hxd.aizwys.cn

G. 面向对象
来源：http://ksn.yuxming.cn

================================================================================
来源：http://rjr.cqqwz.cn

[G01] 定义类
来源：http://tbl.quarkkingdee.top

Py:   class User: pass
来源：http://dwh.9152youxi.cn

PHP:  class User {}
来源：http://ine.hnxiangtu.top

JS:   class User {}
来源：http://yvc.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://zeh.pengpengdd.cyou

Java: class User {}
来源：http://tuo.nwbrower.top

Go:   type User struct { Name string }
来源：http://iav.ivvv.top

Ruby: class User; end
来源：http://qvi.hfpthk.cn

C#:   class User {}
来源：http://ibz.cdnleiting.top

[G02] 构造函数
来源：http://crs.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://ppj.nwbrower.top

PHP:  public function __construct(public string $name) {}
来源：http://fpc.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://cmi.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://lfr.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://kxz.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://snw.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://fpz.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://ycg.xuetiantiany.cn

[G03] 实例属性
来源：http://oyj.yueranfly.top

Py:   self.name = "x"
来源：http://nay.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://gae.gotoacloud.top

JS:   this.name = "x";
来源：http://crt.cdnleiting.top

TS:   name: string = "x";
来源：http://ofy.fktsv.cn

Java: private String name;
来源：http://btc.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vdn.zhixingplan.top

Ruby: @name = "x"
来源：http://rwi.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://mrm.yj202588.top

[G04] 定义方法
来源：http://gmp.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://iic.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ynv.yongpay.top

JS:   greet() { return this.name; }
来源：http://efu.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://bbb.havefunace.top

Java: String greet() { return name; }
来源：http://fdh.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xmk.mhx1999.top

Ruby: def greet; @name; end
来源：http://lil.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://uht.jinqigufen.top

[G05] 继承
来源：http://cna.shzxlz.cn

Py:   class Admin(User): pass
来源：http://fze.xuanzx.com

PHP:  class Admin extends User {}
来源：http://wwk.yueranfly.top

JS:   class Admin extends User {}
来源：http://mlc.andypj.xyz

TS:   class Admin extends User {}
来源：http://tlj.yvedp.cn

Java: class Admin extends User {}
来源：http://vxp.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wdm.sufxvd.cn

Ruby: class Admin < User; end
来源：http://ljj.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://jcd.xinyue.icu

[G06] 重写方法
来源：http://cdg.nanxuanxn.top

Py:   def greet(self): return "admin"
来源：http://daf.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://mkp.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://guq.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://mfi.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://fni.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mrv.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://sav.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://xkt.chenlongwang.top

[G07] 调用父类方法
来源：http://eur.316326.xyz

Py:   super().greet()
来源：http://ehx.zhengqikj.top

PHP:  parent::greet();
来源：http://kag.vehdjk.com

JS:   super.greet();
来源：http://cfk.hammf.cn

TS:   super.greet();
来源：http://lcx.fktsv.cn

Java: super.greet();
来源：http://iin.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eko.xingfuxueyuan.xyz

Ruby: super
来源：http://pjw.c1oappe.top

C#:   base.Greet();
来源：http://psb.c1oappe.top

[G08] 静态方法与属性
来源：http://ftl.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ysf.nanxuanxn.top

PHP:  public static function f() {}
来源：http://dnj.xinyue.icu

JS:   static f() {}
来源：http://lwa.zdbjq.cn

TS:   static f(): void {}
来源：http://fyo.52xcode.cn

Java: static void f() {}
来源：http://ncq.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tgj.havefunace.top

Ruby: def self.f; end
来源：http://vny.fzhhl.top

C#:   public static void F() {}
来源：http://lhz.hcnkem.com

[G09] 接口 / 抽象类
来源：http://kwc.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://uld.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://phg.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://adl.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://gpv.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://dlw.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://tzd.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xuh.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://gal.zhijiandao.cn

[G10] 访问控制
来源：http://gnk.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://wxf.aizwys.cn

PHP:  public / protected / private
来源：http://hlb.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://fsx.jyoumei.cn

TS:   public / protected / private
来源：http://dns.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://mjo.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://zcf.redwolf501.top

Ruby: public / protected / private
来源：http://beo.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://iai.xziqi.cn

[G11] getter / setter
来源：http://qjc.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://rsz.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gsv.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://bdw.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://lae.redwolf501.top

Java: public String getName() { return name; }
来源：http://ynw.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cjr.wangdashe.top

Ruby: attr_accessor :name
来源：http://dre.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://fxe.mhx1999.top

[G12] 对象转字符串
来源：http://tvb.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://eyc.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://juh.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://fna.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://izt.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://dsh.epnwcf.com

Go:   func (u User) String() string { return u.Name }
来源：http://ivg.ybcxt.top

Ruby: def to_s; @name; end
来源：http://fxf.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://hmi.fktsv.cn

[G13] 判断对象类型
来源：http://gmn.cqqwz.cn

Py:   isinstance(u, User)
来源：http://qqz.fengsongda.top

PHP:  $u instanceof User
来源：http://abv.daria6918.cn

JS:   u instanceof User
来源：http://ioz.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://daj.cashguo.top

Java: u instanceof User
来源：http://sun.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://hwg.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://bqk.zhoulong.xyz

C#:   u is User
来源：http://wzh.ehwqpu.com

[G14] 数据类 / record
来源：http://sxc.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rmf.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://uqa.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://klw.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://iag.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://cop.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://mii.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ctb.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://hcc.jianghu66.top

[G15] 枚举
来源：http://tfg.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xlm.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dys.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zml.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://leq.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://cwm.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://syb.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://jym.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rnw.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://ukl.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fin.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://kfr.tarul.cn

JS:   Object.entries(obj)
来源：http://xng.xziqi.cn

TS:   Object.entries(obj)
来源：http://olj.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://enb.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rmr.mhx1999.top

Ruby: obj.instance_variables
来源：http://skz.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://krv.fzhhl.top

================================================================================
来源：http://ccc.nanxuanxn.top

H. 异常与错误处理
来源：http://vbp.cashguo.top

================================================================================
来源：http://eln.9152youxi.cn

[H01] try / catch 基础
来源：http://wkc.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fmk.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ugs.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gjg.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iuc.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tgb.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wur.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pbu.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uvk.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://wye.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://gir.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ukb.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://plj.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uzi.nanxuanxn.top

Java: try { f(); } finally { cleanup(); }
来源：http://hfv.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cfx.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lcw.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fdt.xinyue.icu

[H03] 主动抛出异常
来源：http://cpa.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://vnu.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aot.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://gtf.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://mpt.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dyt.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hvd.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hiq.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wnx.sysykeji.top

[H04] 自定义异常类型
来源：http://ywy.fzhhl.top

Py:   class MyError(Exception): pass
来源：http://sja.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://kpo.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://pfl.fehbvm.com

TS:   class MyError extends Error {}
来源：http://wgv.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://ybr.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bni.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://zhp.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://opl.zhixingplan.top

[H05] 捕获特定类型
来源：http://grs.epnwcf.com

Py:   except ValueError as e:
来源：http://bil.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mbz.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://ybl.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://jhe.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://hye.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iin.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://mik.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ksq.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://wkf.fengsongda.top

Py:   value = d.get("k") or default
来源：http://jje.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://wfw.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rva.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://yos.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bgk.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qve.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://fcw.sxryk.cn

C#:   obj?.A?.B ?? default
来源：http://res.yfazqb.com

[H07] 断言
来源：http://zyk.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://vhy.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://aau.andypj.xyz

JS:   console.assert(x > 0);
来源：http://sox.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://mvj.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://ict.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nxi.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://rjb.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://ien.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://hgk.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://eap.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rcl.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://kpt.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fhm.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sgg.9152youxi.cn

Go:   err.Error()
来源：http://eju.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://ozv.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://oho.svipenyu.cn

[H09] 带错误码的异常
来源：http://dxg.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qvp.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://qwb.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uct.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bqi.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://myh.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tnd.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zga.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://txa.chenjidiqi.icu

[H10] 资源自动释放
来源：http://xwk.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uff.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wrg.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yii.xuetiantiany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kvt.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mmo.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://wbu.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vch.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nyv.52xcode.cn

================================================================================
来源：http://qqv.cashguo.top

I. 正则表达式
来源：http://dnj.cdnleiting.top

================================================================================
来源：http://uqe.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://hya.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mab.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://olg.nwbrower.top

JS:   /\d+/.test(s)
来源：http://ctj.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://eks.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ohl.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wxp.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://cel.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lfz.jinyuanbaomall.cn


<!-- 参考信息 -->