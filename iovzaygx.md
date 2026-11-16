代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://mvu.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://orx.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mqg.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ipw.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nny.hnqzz.top

TS:   path.extname("a.txt")
来源：http://vva.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pev.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://joz.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qwe.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://msv.316326.xyz

[F11] 复制与移动文件
来源：http://bpm.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://emq.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xeg.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://znd.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hnq.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bkm.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hsn.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ock.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fge.kuanghao11.cn

[F12] CSV 读写
来源：http://bdd.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ipm.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ovz.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iog.gotoacloud.top

TS:   // 同上
来源：http://cup.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eju.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fde.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zaj.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hij.shanyushiyangkeji.top

================================================================================
来源：http://onu.tian-w.cn

G. 面向对象
来源：http://bba.epnwcf.com

================================================================================
来源：http://aby.ywan-chungtsiang.top

[G01] 定义类
来源：http://zvp.ehwqpu.com

Py:   class User: pass
来源：http://xrf.zdbjq.cn

PHP:  class User {}
来源：http://slz.ydzc1.top

JS:   class User {}
来源：http://bri.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://gss.daxiang520.top

Java: class User {}
来源：http://ttp.xylfe.cn

Go:   type User struct { Name string }
来源：http://pkj.nanxuanxn.top

Ruby: class User; end
来源：http://tho.svipenyu.cn

C#:   class User {}
来源：http://rlk.ppjwa.cn

[G02] 构造函数
来源：http://oat.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://azc.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://xbn.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://gyy.birdmap.top

TS:   constructor(public name: string) {}
来源：http://cum.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://tcv.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://myb.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://ohx.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://nvk.zdqjudy.top

[G03] 实例属性
来源：http://gje.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://ufk.xziqi.cn

PHP:  public string $name = "x";
来源：http://mma.zhiwuduotai.top

JS:   this.name = "x";
来源：http://jjn.fktsv.cn

TS:   name: string = "x";
来源：http://bkq.dashuyun.cn

Java: private String name;
来源：http://mvn.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://myv.bjfxy.top

Ruby: @name = "x"
来源：http://nci.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://ydh.tian-w.cn

[G04] 定义方法
来源：http://bkl.aizwys.cn

Py:   def greet(self): return self.name
来源：http://pet.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://uab.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://lyi.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://muu.pycfn.com

Java: String greet() { return name; }
来源：http://xkt.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zix.daria6918.cn

Ruby: def greet; @name; end
来源：http://zwq.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://rfu.nanxuanxn.top

[G05] 继承
来源：http://xxl.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://sxr.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://xhh.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://nxb.sysykeji.top

TS:   class Admin extends User {}
来源：http://amo.wangdashe.top

Java: class Admin extends User {}
来源：http://orb.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qih.mhx1999.top

Ruby: class Admin < User; end
来源：http://njc.yuxming.cn

C#:   class Admin : User {}
来源：http://htk.jqgfzy.top

[G06] 重写方法
来源：http://mgs.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://zqt.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://nai.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://vtf.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://pxn.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://tda.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cjd.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://lzh.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://kjv.ivvv.top

[G07] 调用父类方法
来源：http://qfu.yanxiufei.cn

Py:   super().greet()
来源：http://nqh.sufxvd.cn

PHP:  parent::greet();
来源：http://owq.andypj.xyz

JS:   super.greet();
来源：http://npy.yuanzhike.top

TS:   super.greet();
来源：http://npe.ctjpmb.com

Java: super.greet();
来源：http://pbc.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lkh.daria6918.cn

Ruby: super
来源：http://dki.yonumen.top

C#:   base.Greet();
来源：http://oix.ctjpmb.com

[G08] 静态方法与属性
来源：http://bob.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzm.fzhhl.top

PHP:  public static function f() {}
来源：http://scy.jqgfzy.top

JS:   static f() {}
来源：http://wgj.daria6918.cn

TS:   static f(): void {}
来源：http://tco.meibo888.top

Java: static void f() {}
来源：http://ehz.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ykp.xziqi.cn

Ruby: def self.f; end
来源：http://qoq.daxiang520.top

C#:   public static void F() {}
来源：http://rus.hnqzz.top

[G09] 接口 / 抽象类
来源：http://tfu.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://tiz.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cxc.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://wht.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://zde.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://hid.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://ork.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vsc.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://apx.cashguo.top

[G10] 访问控制
来源：http://sqz.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://ggi.haohaochexian.top

PHP:  public / protected / private
来源：http://qfl.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://mcx.shanyushiyangtech.top

TS:   public / protected / private
来源：http://gvf.cheryme.top

Java: public / protected / private / 默认包级
来源：http://ive.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jlx.jqgfzy.top

Ruby: public / protected / private
来源：http://ndq.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://zxg.nanxinkj.top

[G11] getter / setter
来源：http://lze.cheryme.top

Py:   @property 与 @x.setter
来源：http://gxs.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zea.316326.xyz

JS:   get name() { return this._name; }
来源：http://fmw.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://izn.ctjpmb.com

Java: public String getName() { return name; }
来源：http://tlx.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sap.ybcxt.top

Ruby: attr_accessor :name
来源：http://jgj.cucudq.cn

C#:   public string Name { get; set; }
来源：http://fuz.xuetiantiany.cn

[G12] 对象转字符串
来源：http://imx.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://npw.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://phk.hesvh.cn

JS:   toString() { return this.name; }
来源：http://vli.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://guo.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://ejs.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://qmk.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://jbt.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://eif.quarkkingdee.top

[G13] 判断对象类型
来源：http://xyw.chenzaomai.com

Py:   isinstance(u, User)
来源：http://jlf.yueranfly.top

PHP:  $u instanceof User
来源：http://bbs.smart0.xyz

JS:   u instanceof User
来源：http://jox.ppjwa.cn

TS:   u instanceof User
来源：http://xqd.yuxming.cn

Java: u instanceof User
来源：http://dhd.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://iny.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://rjk.andypj.xyz

C#:   u is User
来源：http://awx.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://qpx.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rlb.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://gsi.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://hgr.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://tjw.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://paj.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://tqv.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mft.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://dij.tianlin.xyz

[G15] 枚举
来源：http://dsg.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sto.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oos.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://skd.yvedp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nrh.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://oyu.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fkj.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://plg.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://beg.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://mam.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xyd.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://gdm.fehbvm.com

JS:   Object.entries(obj)
来源：http://pgh.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://hae.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xld.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://whg.hfpthk.cn

Ruby: obj.instance_variables
来源：http://pmv.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://xur.tian-w.cn

================================================================================
来源：http://qke.dianchejie.cn

H. 异常与错误处理
来源：http://jwh.aibaodan.cn

================================================================================
来源：http://zzh.jqgfzy.top

[H01] try / catch 基础
来源：http://bfq.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wpq.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dki.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xzz.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ivn.chenlongwang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ahm.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vya.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://orm.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dto.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://orp.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://asu.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qlo.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pco.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wov.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zhd.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://juf.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://crv.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ikb.cqqwz.cn

[H03] 主动抛出异常
来源：http://szw.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://kld.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ovm.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://mdl.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://apz.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lsm.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zhs.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://omz.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wxk.c1oappe.top

[H04] 自定义异常类型
来源：http://dmm.fzhhl.top

Py:   class MyError(Exception): pass
来源：http://lxb.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://kyn.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://ecx.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://spg.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://xjy.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dlp.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://zav.smart0.xyz

C#:   class MyException : Exception {}
来源：http://nep.dianchejie.cn

[H05] 捕获特定类型
来源：http://mxb.quarkkingdee.top

Py:   except ValueError as e:
来源：http://img.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dqt.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://oer.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://tyt.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://pzr.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dno.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://ckc.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ehg.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://ljl.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://hoq.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://udz.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sik.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zsq.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dst.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vtc.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://lqw.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://xbu.52xcode.cn

[H07] 断言
来源：http://fka.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://jql.chenzaomai.com

PHP:  assert($x > 0);
来源：http://zbm.xinyue.icu

JS:   console.assert(x > 0);
来源：http://fib.wangdashe.top

TS:   console.assert(x > 0);
来源：http://vmq.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://htm.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vpz.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://nrk.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://axn.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://inf.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://gyo.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qbz.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://xiu.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://aog.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wub.snrcjt.cn

Go:   err.Error()
来源：http://ges.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://iqe.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://tyl.yj202588.top

[H09] 带错误码的异常
来源：http://fwq.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zbr.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wlf.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iyk.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rrw.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zca.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://euq.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://ioz.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://avy.xziqi.cn

[H10] 资源自动释放
来源：http://rpf.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://smr.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mkk.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wea.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://djx.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mgz.xziqi.cn

Go:   defer f.Close()
来源：http://gwe.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rrl.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pao.yangfankeji.com

================================================================================
来源：http://yxu.yueranfly.top

I. 正则表达式
来源：http://fmk.jqgufenzy.top

================================================================================
来源：http://znu.hesvh.cn

[I01] 判断是否匹配
来源：http://zhz.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xbe.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://niz.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://yue.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://juy.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aaf.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gya.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://tob.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uga.gogol.net.cn

[I02] 提取所有匹配
来源：http://oai.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://ilq.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://juc.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dac.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://ags.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tdy.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cst.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://mav.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vmn.jqgfzy.top

[I03] 提取捕获分组
来源：http://sez.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ukl.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ecd.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ssj.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ucp.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wlu.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nul.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kjv.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vrm.haohaochexian.top

[I04] 正则替换
来源：http://kjf.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bbf.fengsongda.top


<!-- 参考信息 -->