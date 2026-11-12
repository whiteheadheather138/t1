代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://jdl.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uab.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://kti.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://lgg.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://evv.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qhb.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://wlg.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://mqv.pengpengdd.cyou

[F09] 获取文件大小
来源：http://atj.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://spf.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://kkz.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://pyy.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://luy.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://vtt.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bxy.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://uqr.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://qli.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://hbb.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bub.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pxu.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fdz.meibo888.top

TS:   path.extname("a.txt")
来源：http://jkv.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hhj.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nkq.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jxg.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hba.xylfe.cn

[F11] 复制与移动文件
来源：http://zlf.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mev.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://thd.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mqh.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yrr.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://guk.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ftv.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hqq.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eeg.xinyue.icu

[F12] CSV 读写
来源：http://rqi.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://slv.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xyk.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qjw.chenjidiqi.icu

TS:   // 同上
来源：http://kil.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dbw.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qwe.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zjl.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ijs.zhixingplan.top

================================================================================
来源：http://bls.tianlin.xyz

G. 面向对象
来源：http://xri.fehbvm.com

================================================================================
来源：http://uqc.guannengcc.top

[G01] 定义类
来源：http://evh.yueranfly.top

Py:   class User: pass
来源：http://frp.0kj1m.cn

PHP:  class User {}
来源：http://ian.yj202588.top

JS:   class User {}
来源：http://rtm.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://qrw.bjfxy.top

Java: class User {}
来源：http://chu.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://xyr.yangfankeji.com

Ruby: class User; end
来源：http://ejm.hcnkem.com

C#:   class User {}
来源：http://cvp.fehbvm.com

[G02] 构造函数
来源：http://vnn.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://ycj.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://cvb.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://bza.pycfn.com

TS:   constructor(public name: string) {}
来源：http://giz.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://lkm.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mff.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://ltj.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://yuk.hnxiangtu.top

[G03] 实例属性
来源：http://cry.chenlongwang.top

Py:   self.name = "x"
来源：http://cti.tarul.cn

PHP:  public string $name = "x";
来源：http://pbb.meibo888.top

JS:   this.name = "x";
来源：http://zqv.tanke756.top

TS:   name: string = "x";
来源：http://jtf.jinqigufen.top

Java: private String name;
来源：http://xhi.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ass.cheryme.top

Ruby: @name = "x"
来源：http://wrg.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://uui.ywan-chungtsiang.top

[G04] 定义方法
来源：http://lct.guannengcc.top

Py:   def greet(self): return self.name
来源：http://lkb.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gog.cashguo.top

JS:   greet() { return this.name; }
来源：http://hzj.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://dvp.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://ihr.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xeq.nanxinkj.top

Ruby: def greet; @name; end
来源：http://lug.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://gid.snrcjt.cn

[G05] 继承
来源：http://hxm.hnqzz.top

Py:   class Admin(User): pass
来源：http://tsi.ivvv.top

PHP:  class Admin extends User {}
来源：http://jwr.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://zof.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://hhl.jlsjyb.cn

Java: class Admin extends User {}
来源：http://rfj.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zfc.hfpthk.cn

Ruby: class Admin < User; end
来源：http://qbe.cdnleiting.top

C#:   class Admin : User {}
来源：http://wdm.ehwqpu.com

[G06] 重写方法
来源：http://gny.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://tmf.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rfe.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://int.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://quv.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://wir.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xkc.316326.xyz

Ruby: def greet; "admin"; end
来源：http://pkj.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://gdc.xziqi.cn

[G07] 调用父类方法
来源：http://vkt.pengpengdd.cyou

Py:   super().greet()
来源：http://dcx.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://pih.jqgfzy.top

JS:   super.greet();
来源：http://zrx.haohaochexian.top

TS:   super.greet();
来源：http://bhy.shuidangran.top

Java: super.greet();
来源：http://xrr.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gcm.birdmap.top

Ruby: super
来源：http://kwl.iojbl.cn

C#:   base.Greet();
来源：http://qiu.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://nei.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eyf.haohaochexian.top

PHP:  public static function f() {}
来源：http://wxo.fehbvm.com

JS:   static f() {}
来源：http://eay.hesvh.cn

TS:   static f(): void {}
来源：http://hnm.smart0.xyz

Java: static void f() {}
来源：http://htv.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wdo.fktsv.cn

Ruby: def self.f; end
来源：http://gps.svipenyu.cn

C#:   public static void F() {}
来源：http://fkl.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://rmc.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://uxt.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://dln.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rso.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://jho.shuidangran.top

Java: interface Shape { double area(); }
来源：http://qvt.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://paf.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://csf.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://dvz.snrcjt.cn

[G10] 访问控制
来源：http://cwl.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://tzi.hfpthk.cn

PHP:  public / protected / private
来源：http://vjq.sweek.top

JS:   #private 字段；其余公开
来源：http://xzc.pycfn.com

TS:   public / protected / private
来源：http://wld.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://xyk.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fkb.ppjwa.cn

Ruby: public / protected / private
来源：http://tel.pycfn.com

C#:   public / protected / private / internal
来源：http://oyn.zdbjq.cn

[G11] getter / setter
来源：http://hhz.ydzc1.top

Py:   @property 与 @x.setter
来源：http://qop.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ulq.yfazqb.com

JS:   get name() { return this._name; }
来源：http://tyu.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://fkg.fehbvm.com

Java: public String getName() { return name; }
来源：http://bnr.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rcn.fzhhl.top

Ruby: attr_accessor :name
来源：http://ibo.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://kij.wangdashe.top

[G12] 对象转字符串
来源：http://bte.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://hpe.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fmw.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://llv.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://fne.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://buj.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jgk.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://efr.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://ffy.hcnkem.com

[G13] 判断对象类型
来源：http://qii.gogol.net.cn

Py:   isinstance(u, User)
来源：http://yim.bjfxy.top

PHP:  $u instanceof User
来源：http://mvi.c1oappe.top

JS:   u instanceof User
来源：http://bkl.cashguo.top

TS:   u instanceof User
来源：http://tbx.sweek.top

Java: u instanceof User
来源：http://qgr.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aqb.316326.xyz

Ruby: u.is_a?(User)
来源：http://htr.gogol.net.cn

C#:   u is User
来源：http://zla.hammf.cn

[G14] 数据类 / record
来源：http://yah.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zce.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://nfp.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://oqm.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://owr.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://tqx.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://euu.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jmv.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://hci.zhoulong.xyz

[G15] 枚举
来源：http://iam.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://krs.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://inu.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sus.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://evr.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://fxo.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xtg.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://fem.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mxm.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://jju.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lhp.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://ywo.sufxvd.cn

JS:   Object.entries(obj)
来源：http://wor.hysaishi.cn

TS:   Object.entries(obj)
来源：http://dvr.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ifl.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vdj.birdmap.top

Ruby: obj.instance_variables
来源：http://air.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://lox.shangyingyoupin.top

================================================================================
来源：http://imw.ppjwa.cn

H. 异常与错误处理
来源：http://rng.gotoacloud.top

================================================================================
来源：http://zjt.vqdsnc.cn

[H01] try / catch 基础
来源：http://shr.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cfw.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://acn.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozx.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zax.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kho.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xxw.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ncr.tianlin.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://akg.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://kfn.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bzc.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ptr.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ejw.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xhg.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yjw.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fdj.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kao.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dsc.sysykeji.top

[H03] 主动抛出异常
来源：http://ozt.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://sno.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gok.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://kxp.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://lqb.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://ytc.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wuy.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://fab.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://vwg.hnqzz.top

[H04] 自定义异常类型
来源：http://iyw.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://eoi.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://nkr.epnwcf.com

JS:   class MyError extends Error {}
来源：http://jbv.xylfe.cn

TS:   class MyError extends Error {}
来源：http://zbx.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://bbt.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qls.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://usw.xylfe.cn

C#:   class MyException : Exception {}
来源：http://pun.kuanghao11.cn

[H05] 捕获特定类型
来源：http://gks.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://kdc.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cyb.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://ayd.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://lgy.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://ajm.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gvk.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://otb.dianchejie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gji.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://pqo.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://lmr.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://qrj.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://ila.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://jqs.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://abb.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qbd.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://ath.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://vqd.hesvh.cn

[H07] 断言
来源：http://cpd.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://fti.316326.xyz

PHP:  assert($x > 0);
来源：http://woy.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://hot.uphjek.com

TS:   console.assert(x > 0);
来源：http://eke.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://ant.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ikc.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ugf.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://zre.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://gjr.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://alg.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://the.nwbrower.top

JS:   e.message;  e.stack
来源：http://ejp.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pkt.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://unb.fehbvm.com

Go:   err.Error()
来源：http://txz.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://hif.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://jbr.hywenlv.cn

[H09] 带错误码的异常
来源：http://cws.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mjj.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xau.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lek.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sdm.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rsq.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jjd.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oun.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hrb.hcnkem.com

[H10] 资源自动释放
来源：http://hqv.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aje.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://drh.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wqq.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cub.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://geh.yj202588.top

Go:   defer f.Close()
来源：http://geo.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ipg.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vkr.cheryme.top

================================================================================
来源：http://xys.gzhubu.top

I. 正则表达式
来源：http://ecc.wangshuangyany.cn

================================================================================
来源：http://yew.hfpthk.cn

[I01] 判断是否匹配
来源：http://cro.vehdjk.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mlc.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://vti.gzhubu.top

JS:   /\d+/.test(s)
来源：http://zhx.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://wmb.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://axr.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kyj.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://vpg.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hcx.hnxiangtu.top

[I02] 提取所有匹配
来源：http://jal.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://kzb.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bsj.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qnq.ydzc1.top


<!-- 参考信息 -->