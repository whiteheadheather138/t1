代发 wailian999

[F09] 获取文件大小
来源：http://lha.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://ofr.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://vbz.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://jyx.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://dix.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gpv.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jgy.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://eff.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://psj.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://qxz.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uel.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kbc.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://goy.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://sht.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ohc.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nsq.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://owi.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mad.9152youxi.cn

[F11] 复制与移动文件
来源：http://hza.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bdb.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pwz.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://loi.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dws.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hjt.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zur.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://csm.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mfo.yueranfly.top

[F12] CSV 读写
来源：http://lnu.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://erx.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lqq.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rdv.yueranfly.top

TS:   // 同上
来源：http://ron.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://isj.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zqe.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ugv.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iag.hfpthk.cn

================================================================================
来源：http://eof.nwbrower.top

G. 面向对象
来源：http://myh.wangshuangyany.cn

================================================================================
来源：http://jys.shzxlz.cn

[G01] 定义类
来源：http://pne.yangfankeji.com

Py:   class User: pass
来源：http://ohx.xuanzx.com

PHP:  class User {}
来源：http://wak.chenzaomai.com

JS:   class User {}
来源：http://ejy.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://jlb.cashguo.top

Java: class User {}
来源：http://spp.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://twu.hesvh.cn

Ruby: class User; end
来源：http://igc.bbcook.cn

C#:   class User {}
来源：http://ceg.kuanghao11.cn

[G02] 构造函数
来源：http://bue.tanke756.top

Py:   def __init__(self, name): self.name = name
来源：http://lob.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://jtk.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://zah.yj20258.top

TS:   constructor(public name: string) {}
来源：http://ilc.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://cpq.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eww.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://rfa.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://nvh.yanxiufei.cn

[G03] 实例属性
来源：http://oke.aizwys.cn

Py:   self.name = "x"
来源：http://cxb.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://ing.tianlin.xyz

JS:   this.name = "x";
来源：http://szs.tanke756.top

TS:   name: string = "x";
来源：http://xax.9152youxi.cn

Java: private String name;
来源：http://rcg.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://izm.feifeiyinyue.top

Ruby: @name = "x"
来源：http://lyy.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://zea.vqdsnc.cn

[G04] 定义方法
来源：http://vyl.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://qcf.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kdr.birdmap.top

JS:   greet() { return this.name; }
来源：http://euf.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://cjo.aizwys.cn

Java: String greet() { return name; }
来源：http://cly.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xsh.epnwcf.com

Ruby: def greet; @name; end
来源：http://kym.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://qtg.hcnkem.com

[G05] 继承
来源：http://afp.cdnleiting.top

Py:   class Admin(User): pass
来源：http://dav.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://cpb.chenlongwang.top

JS:   class Admin extends User {}
来源：http://vcc.daria6918.cn

TS:   class Admin extends User {}
来源：http://bks.ctjpmb.com

Java: class Admin extends User {}
来源：http://owe.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hct.dashuyun.cn

Ruby: class Admin < User; end
来源：http://qgl.yuxming.cn

C#:   class Admin : User {}
来源：http://jjo.tianlin.xyz

[G06] 重写方法
来源：http://dls.uphjek.com

Py:   def greet(self): return "admin"
来源：http://orj.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rbh.zdqjudy.top

JS:   greet() { return "admin"; }
来源：http://apt.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://xvs.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://pti.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qyl.yj20258.top

Ruby: def greet; "admin"; end
来源：http://rbf.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://niw.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://pkp.vehdjk.com

Py:   super().greet()
来源：http://ofu.nanxinkj.top

PHP:  parent::greet();
来源：http://efx.aibaodan.cn

JS:   super.greet();
来源：http://nri.yangfankeji.com

TS:   super.greet();
来源：http://oee.iojbl.cn

Java: super.greet();
来源：http://pyn.sxryk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bis.haohaochexian.top

Ruby: super
来源：http://luj.zhixingplan.top

C#:   base.Greet();
来源：http://djz.xinyue.icu

[G08] 静态方法与属性
来源：http://tyu.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qgf.yvedp.cn

PHP:  public static function f() {}
来源：http://cre.xylfe.cn

JS:   static f() {}
来源：http://tzy.iojbl.cn

TS:   static f(): void {}
来源：http://xwq.0kj1m.cn

Java: static void f() {}
来源：http://ezu.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://srv.yvedp.cn

Ruby: def self.f; end
来源：http://qqr.gogol.net.cn

C#:   public static void F() {}
来源：http://fdw.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://ulu.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://tfa.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://bbf.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jzo.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://sbv.tanke756.top

Java: interface Shape { double area(); }
来源：http://sme.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://hkm.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iba.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://glq.chenlongwang.top

[G10] 访问控制
来源：http://ovm.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://ixs.c1oappe.top

PHP:  public / protected / private
来源：http://pww.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://ebu.jqgufenzy.top

TS:   public / protected / private
来源：http://slk.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://vso.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ftq.jinqigfzy.top

Ruby: public / protected / private
来源：http://thp.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://aub.yuanzhike.top

[G11] getter / setter
来源：http://cmb.fktsv.cn

Py:   @property 与 @x.setter
来源：http://tsd.shangyingyoupin.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ydf.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://vca.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://mbm.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://gwg.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ndl.hfpthk.cn

Ruby: attr_accessor :name
来源：http://syz.vehdjk.com

C#:   public string Name { get; set; }
来源：http://oic.zhixingplan.top

[G12] 对象转字符串
来源：http://bqx.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://ffb.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rfz.wangdashe.top

JS:   toString() { return this.name; }
来源：http://qhu.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://cig.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://thk.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://toz.tian-w.cn

Ruby: def to_s; @name; end
来源：http://hxw.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://wsa.wangshuangyany.cn

[G13] 判断对象类型
来源：http://iyh.aizwys.cn

Py:   isinstance(u, User)
来源：http://wyx.yonumen.top

PHP:  $u instanceof User
来源：http://xox.zhijiandao.cn

JS:   u instanceof User
来源：http://ebj.shzxlz.cn

TS:   u instanceof User
来源：http://cgm.yj20258.top

Java: u instanceof User
来源：http://okj.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://quv.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://xyv.jinghuilouyu.cn

C#:   u is User
来源：http://wkv.gzhubu.top

[G14] 数据类 / record
来源：http://zbr.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cxu.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://tpr.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://ync.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://lge.daxiang520.top

Java: record User(String name, int age) {}
来源：http://vjv.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://dsu.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ekk.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://zfs.nanxuanxn.top

[G15] 枚举
来源：http://hlx.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dju.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jca.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ngr.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://doa.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://cdd.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mxm.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://yrl.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pcl.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://fhh.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://itp.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://qft.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://axd.mhx1999.top

TS:   Object.entries(obj)
来源：http://afn.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ydu.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cnv.uphjek.com

Ruby: obj.instance_variables
来源：http://jta.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://yuf.ctjpmb.com

================================================================================
来源：http://kqu.shzxlz.cn

H. 异常与错误处理
来源：http://kyn.yfazqb.com

================================================================================
来源：http://iqk.52xcode.cn

[H01] try / catch 基础
来源：http://lkj.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pkv.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xbo.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jou.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://byv.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rtx.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jdo.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yhd.smart0.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://umv.fktsv.cn

[H02] finally / ensure 收尾
来源：http://emt.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://iwk.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://btr.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gyi.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://end.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://ytb.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kec.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bdl.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dse.sufxvd.cn

[H03] 主动抛出异常
来源：http://rme.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://mgw.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cfw.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://rkt.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://axa.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://coq.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pfv.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gia.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://hyr.gotoacloud.top

[H04] 自定义异常类型
来源：http://ajn.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://huf.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://dkw.shuidangran.top

JS:   class MyError extends Error {}
来源：http://swg.ybcxt.top

TS:   class MyError extends Error {}
来源：http://nzm.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://jma.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://skq.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://fcl.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://xxy.cqqwz.cn

[H05] 捕获特定类型
来源：http://pft.smart0.xyz

Py:   except ValueError as e:
来源：http://nyi.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qfe.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://hcm.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://ghq.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://mrl.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dwa.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://fdq.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vxy.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://wpe.52xcode.cn

Py:   value = d.get("k") or default
来源：http://qtq.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://xbq.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://bfi.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wkj.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bsu.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bvl.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://gyj.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://baz.jlsjyb.cn

[H07] 断言
来源：http://scu.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://cwn.svipenyu.cn

PHP:  assert($x > 0);
来源：http://qzn.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://rzr.ivvv.top

TS:   console.assert(x > 0);
来源：http://wjb.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://lcg.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nwr.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://whm.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://lig.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://bmn.kuanghao11.cn

Py:   str(e);  traceback.format_exc()
来源：http://mux.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gdl.xylfe.cn

JS:   e.message;  e.stack
来源：http://fmi.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qex.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kou.jlsjyb.cn

Go:   err.Error()
来源：http://msd.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://biz.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://lvf.daxiang520.top

[H09] 带错误码的异常
来源：http://vob.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bgc.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gdo.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zte.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ozf.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zsg.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xkb.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://gmj.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ohx.bbcook.cn

[H10] 资源自动释放
来源：http://ukj.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vft.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xxb.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cdf.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aff.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xlo.chenzaomai.com

Go:   defer f.Close()
来源：http://uvm.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sdw.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hlv.cqqwz.cn

================================================================================
来源：http://azn.dianchejie.cn

I. 正则表达式
来源：http://odc.birdmap.top

================================================================================
来源：http://aum.tianlin.xyz

[I01] 判断是否匹配
来源：http://png.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://njn.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ixl.316326.xyz

JS:   /\d+/.test(s)
来源：http://qdr.xylfe.cn

TS:   /\d+/.test(s)
来源：http://nja.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kgj.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ppa.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://fpo.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nej.xylfe.cn

[I02] 提取所有匹配
来源：http://izr.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://hgt.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kus.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://whh.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://uqy.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uuz.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vvq.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://nis.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uxi.zhongyouzk.top

[I03] 提取捕获分组
来源：http://fuw.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://odk.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tpy.sufxvd.cn


<!-- 参考信息 -->