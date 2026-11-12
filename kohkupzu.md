代发 wailian999

[F09] 获取文件大小
来源：http://lnr.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://wum.daria6918.cn

PHP:  filesize("a.txt");
来源：http://ygc.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://ejm.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://cjn.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lwg.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://msi.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://iqv.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://yah.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://azz.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ykl.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mll.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pna.yj20258.top

TS:   path.extname("a.txt")
来源：http://eay.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uzs.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jtn.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tdb.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pct.hammf.cn

[F11] 复制与移动文件
来源：http://fid.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://boi.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://duu.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ids.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mgj.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vzx.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gpq.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xpl.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cvd.tanke756.top

[F12] CSV 读写
来源：http://gyv.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mnl.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rtx.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lrp.sufxvd.cn

TS:   // 同上
来源：http://xep.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://roz.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zwh.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fze.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://pob.yvedp.cn

================================================================================
来源：http://agi.kuanghao11.cn

G. 面向对象
来源：http://ewq.bjfxy.top

================================================================================
来源：http://ttw.52xcode.cn

[G01] 定义类
来源：http://lxi.jyoumei.cn

Py:   class User: pass
来源：http://ict.wangshuangyany.cn

PHP:  class User {}
来源：http://vts.jianghu66.top

JS:   class User {}
来源：http://urm.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://sgn.yanxiufei.cn

Java: class User {}
来源：http://mma.hammf.cn

Go:   type User struct { Name string }
来源：http://gjy.jqgfzy.top

Ruby: class User; end
来源：http://xoo.cdnleiting.top

C#:   class User {}
来源：http://nhz.yuanzhike.top

[G02] 构造函数
来源：http://hxg.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://vzu.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://jva.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://fag.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://ypn.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://pxc.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zic.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://fzn.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://qjy.dashuyun.cn

[G03] 实例属性
来源：http://ort.fzhhl.top

Py:   self.name = "x"
来源：http://qux.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://mmn.tanke756.top

JS:   this.name = "x";
来源：http://zgn.feifeiyinyue.top

TS:   name: string = "x";
来源：http://xzd.yuxming.cn

Java: private String name;
来源：http://sip.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uhw.svipenyu.cn

Ruby: @name = "x"
来源：http://rgp.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://dxu.shzxlz.cn

[G04] 定义方法
来源：http://nti.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://nqh.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ivs.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://kmq.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://lvh.zhengqikj.top

Java: String greet() { return name; }
来源：http://lxx.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://abs.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://zoc.jianghu66.top

C#:   public string Greet() => Name;
来源：http://wnr.hnxiangtu.top

[G05] 继承
来源：http://mjv.sweek.top

Py:   class Admin(User): pass
来源：http://qru.tarul.cn

PHP:  class Admin extends User {}
来源：http://rbe.0kj1m.cn

JS:   class Admin extends User {}
来源：http://cdf.jinqigufen.top

TS:   class Admin extends User {}
来源：http://yax.hysaishi.cn

Java: class Admin extends User {}
来源：http://ohv.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dyi.jqgfzy.top

Ruby: class Admin < User; end
来源：http://sxk.epnwcf.com

C#:   class Admin : User {}
来源：http://smm.zhiwuduotai.top

[G06] 重写方法
来源：http://ehv.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://vfp.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cej.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://cof.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://nub.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://knj.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nqr.tarul.cn

Ruby: def greet; "admin"; end
来源：http://nmu.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://jlk.jinqigfzy.top

[G07] 调用父类方法
来源：http://xho.feifeiyinyue.top

Py:   super().greet()
来源：http://jqs.jianghu66.top

PHP:  parent::greet();
来源：http://ksk.gaohongyu789.top

JS:   super.greet();
来源：http://utt.hnqzz.top

TS:   super.greet();
来源：http://yip.xziqi.cn

Java: super.greet();
来源：http://fak.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ydg.mhx1999.top

Ruby: super
来源：http://zkg.meibo888.top

C#:   base.Greet();
来源：http://szm.tianlin.xyz

[G08] 静态方法与属性
来源：http://ouy.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yxu.jqgfzy.top

PHP:  public static function f() {}
来源：http://cpy.shzxlz.cn

JS:   static f() {}
来源：http://igc.yj20258888.top

TS:   static f(): void {}
来源：http://eps.birdmap.top

Java: static void f() {}
来源：http://svj.yonumen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kms.feifeiyinyue.top

Ruby: def self.f; end
来源：http://zvx.aizwys.cn

C#:   public static void F() {}
来源：http://bbb.sxryk.cn

[G09] 接口 / 抽象类
来源：http://xjx.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://vjw.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://ywl.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kml.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://ptf.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://hsp.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://vwx.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vfo.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://uow.jqgfzy.top

[G10] 访问控制
来源：http://drj.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://arj.gogol.net.cn

PHP:  public / protected / private
来源：http://zbj.fehbvm.com

JS:   #private 字段；其余公开
来源：http://tyz.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://aob.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://rop.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://shk.sjlbkw.cn

Ruby: public / protected / private
来源：http://teg.bbcook.cn

C#:   public / protected / private / internal
来源：http://req.pycfn.com

[G11] getter / setter
来源：http://xel.smart0.xyz

Py:   @property 与 @x.setter
来源：http://mjf.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dje.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://nas.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://bry.tian-w.cn

Java: public String getName() { return name; }
来源：http://lhl.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://guu.yuxming.cn

Ruby: attr_accessor :name
来源：http://qhf.fengsongda.top

C#:   public string Name { get; set; }
来源：http://tnm.shzxlz.cn

[G12] 对象转字符串
来源：http://rvm.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://frb.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://jod.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://njp.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://wip.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://lxt.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gnw.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://pba.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://ewp.mhx1999.top

[G13] 判断对象类型
来源：http://rbu.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://ryh.pycfn.com

PHP:  $u instanceof User
来源：http://pbt.hesvh.cn

JS:   u instanceof User
来源：http://rap.havefunace.top

TS:   u instanceof User
来源：http://awx.guowangkeji.top

Java: u instanceof User
来源：http://zdf.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uec.yvedp.cn

Ruby: u.is_a?(User)
来源：http://iam.iojbl.cn

C#:   u is User
来源：http://osb.zhongyouzk.top

[G14] 数据类 / record
来源：http://fql.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ftp.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://mpp.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://cbw.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://prr.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://wje.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://vzl.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wyo.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://ynk.hysaishi.cn

[G15] 枚举
来源：http://nlt.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dop.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nrd.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jie.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cks.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://cnf.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mul.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://tkd.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ezq.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://jmw.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://foz.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://ykb.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://pxw.fehbvm.com

TS:   Object.entries(obj)
来源：http://kxc.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jjj.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wla.cqqwz.cn

Ruby: obj.instance_variables
来源：http://zoa.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://nqs.jlsjyb.cn

================================================================================
来源：http://kfu.zhixingplan.top

H. 异常与错误处理
来源：http://vxi.xylfe.cn

================================================================================
来源：http://ilj.hnqzz.top

[H01] try / catch 基础
来源：http://lrc.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uoy.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://epn.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qdn.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sby.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eej.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iyu.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yts.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hsm.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://gue.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://wgw.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ooe.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mrb.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gvn.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jqn.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jyt.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://slv.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://amc.sysykeji.top

[H03] 主动抛出异常
来源：http://har.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://dpb.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tww.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://qhn.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://nck.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ohq.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sak.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gxd.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://fge.9152youxi.cn

[H04] 自定义异常类型
来源：http://vwl.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://iug.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://ybm.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://zud.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://wfb.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://mgb.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eln.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://ful.hywenlv.cn

C#:   class MyException : Exception {}
来源：http://ael.hywenlv.cn

[H05] 捕获特定类型
来源：http://mlq.jqgufenzy.top

Py:   except ValueError as e:
来源：http://hrb.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rwk.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://gqw.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://mxf.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://uoi.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hhi.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://nvo.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wfz.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://xdw.bbcook.cn

Py:   value = d.get("k") or default
来源：http://mqv.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cso.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://izt.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uic.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dis.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wcl.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://ctl.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://uut.bjfxy.top

[H07] 断言
来源：http://imp.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://rqw.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://uws.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://vys.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://vqr.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://rdu.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mls.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://qub.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://nrc.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://pum.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://zag.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sos.zdqjudy.top

JS:   e.message;  e.stack
来源：http://kzy.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oys.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ged.nanxuanxn.top

Go:   err.Error()
来源：http://weh.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://sqa.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://ghc.cashguo.top

[H09] 带错误码的异常
来源：http://sfd.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pou.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kpz.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ngr.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://srd.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lik.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://asc.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ojq.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ebu.cheryme.top

[H10] 资源自动释放
来源：http://bjh.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xfr.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bdi.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://axk.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xdv.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ble.nanxinkj.top

Go:   defer f.Close()
来源：http://qqh.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fxt.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jdd.aibaodan.cn

================================================================================
来源：http://fwq.andypj.xyz

I. 正则表达式
来源：http://gjo.pycfn.com

================================================================================
来源：http://oat.yj202588.top

[I01] 判断是否匹配
来源：http://qwz.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lis.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://kwh.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://tla.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://twv.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ymh.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://etk.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://shf.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yds.smart0.xyz

[I02] 提取所有匹配
来源：http://aeu.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://rxi.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fej.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://coo.yj202588.top

TS:   s.match(/\d+/g)
来源：http://pbt.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cmc.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rxi.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://mnm.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kbw.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://zap.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zmp.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oaf.yangfankeji.com


<!-- 参考信息 -->