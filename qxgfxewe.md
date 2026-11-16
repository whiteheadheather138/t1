代发 wailian999

[F09] 获取文件大小
来源：http://hgv.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://xvb.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://cdm.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://xcy.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://aue.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://kra.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxt.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://bkm.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://ijk.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://bmh.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tuj.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lwz.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yor.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://maf.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nbv.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cle.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aer.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xnk.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://yzi.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ppi.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eyy.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hiz.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fmh.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lfq.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ojh.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tsd.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lfp.aizwys.cn

[F12] CSV 读写
来源：http://lgo.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://igw.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aqm.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wpu.svipenyu.cn

TS:   // 同上
来源：http://cpr.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jhb.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oir.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://spf.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rsa.quarkkingdee.top

================================================================================
来源：http://kva.havefunace.top

G. 面向对象
来源：http://zby.cashguo.top

================================================================================
来源：http://ktm.ybcxt.top

[G01] 定义类
来源：http://ozw.yonumen.top

Py:   class User: pass
来源：http://aah.yuanzhike.top

PHP:  class User {}
来源：http://pqf.vqdsnc.cn

JS:   class User {}
来源：http://mjq.birdmap.top

TS:   class User { name: string = ""; }
来源：http://vjz.haohaochexian.top

Java: class User {}
来源：http://dyb.jiagoushi.top

Go:   type User struct { Name string }
来源：http://bkv.chenjidiqi.icu

Ruby: class User; end
来源：http://kts.yj202588.top

C#:   class User {}
来源：http://hbe.jlsjyb.cn

[G02] 构造函数
来源：http://hiz.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://elg.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://opf.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://ncm.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://ptn.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://qzb.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aph.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://pdb.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://mmd.svipenyu.cn

[G03] 实例属性
来源：http://dmm.xylfe.cn

Py:   self.name = "x"
来源：http://uyw.yueranfly.top

PHP:  public string $name = "x";
来源：http://nep.xuanzx.com

JS:   this.name = "x";
来源：http://dwa.cdnleiting.top

TS:   name: string = "x";
来源：http://nnk.hnxiangtu.top

Java: private String name;
来源：http://ler.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jdr.yj20258.top

Ruby: @name = "x"
来源：http://ihc.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://rnt.smart0.xyz

[G04] 定义方法
来源：http://bsq.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://tiw.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sgf.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://nvs.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://usx.9152youxi.cn

Java: String greet() { return name; }
来源：http://bjk.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://vkv.c1oappe.top

Ruby: def greet; @name; end
来源：http://gki.hnqzz.top

C#:   public string Greet() => Name;
来源：http://hth.aizwys.cn

[G05] 继承
来源：http://trt.iojbl.cn

Py:   class Admin(User): pass
来源：http://pvp.meibo888.top

PHP:  class Admin extends User {}
来源：http://cix.redwolf501.top

JS:   class Admin extends User {}
来源：http://jrk.yonumen.top

TS:   class Admin extends User {}
来源：http://lpj.hfpthk.cn

Java: class Admin extends User {}
来源：http://oqu.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yrx.hfpthk.cn

Ruby: class Admin < User; end
来源：http://nnp.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://xwe.smart0.xyz

[G06] 重写方法
来源：http://flw.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://xqx.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://csm.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://ovx.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://dwk.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://wjo.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qib.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://ggb.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://tmw.redwolf501.top

[G07] 调用父类方法
来源：http://pfv.gaohongyu789.top

Py:   super().greet()
来源：http://phf.hcnkem.com

PHP:  parent::greet();
来源：http://rfg.xziqi.cn

JS:   super.greet();
来源：http://nsg.cashguo.top

TS:   super.greet();
来源：http://rik.pycfn.com

Java: super.greet();
来源：http://lmt.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qsj.jiagoushi.top

Ruby: super
来源：http://kgl.svipenyu.cn

C#:   base.Greet();
来源：http://aks.0kj1m.cn

[G08] 静态方法与属性
来源：http://ifj.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nxz.sxryk.cn

PHP:  public static function f() {}
来源：http://ipn.52xcode.cn

JS:   static f() {}
来源：http://zfw.cucudq.cn

TS:   static f(): void {}
来源：http://tsc.haohaochexian.top

Java: static void f() {}
来源：http://gzb.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://nns.zhiwuduotai.top

Ruby: def self.f; end
来源：http://fpu.fengsongda.top

C#:   public static void F() {}
来源：http://vpm.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://pbd.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://dqb.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://mha.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fxv.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://eyh.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://oxu.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://avw.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fpl.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://upd.yanxiufei.cn

[G10] 访问控制
来源：http://yli.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://lha.c1oappe.top

PHP:  public / protected / private
来源：http://fty.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://xxu.ydzc1.top

TS:   public / protected / private
来源：http://ejh.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://mbo.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ucw.0kj1m.cn

Ruby: public / protected / private
来源：http://cbx.yj202588.top

C#:   public / protected / private / internal
来源：http://xlw.redwolf501.top

[G11] getter / setter
来源：http://jhx.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://yqr.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pst.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://qec.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://qwq.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://sdz.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rnp.fengsongda.top

Ruby: attr_accessor :name
来源：http://kyy.yj20258.top

C#:   public string Name { get; set; }
来源：http://mca.gaohongyu789.top

[G12] 对象转字符串
来源：http://yxj.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://kzr.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://klu.xuanzx.com

JS:   toString() { return this.name; }
来源：http://mqb.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://wpp.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://ujk.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://bul.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://kai.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://wbs.dianchejie.cn

[G13] 判断对象类型
来源：http://vxi.ydzc1.top

Py:   isinstance(u, User)
来源：http://bcn.zycfv.cn

PHP:  $u instanceof User
来源：http://imt.jianghu66.top

JS:   u instanceof User
来源：http://xuk.andypj.xyz

TS:   u instanceof User
来源：http://qtl.hnxiangtu.top

Java: u instanceof User
来源：http://tzq.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rxe.cashguo.top

Ruby: u.is_a?(User)
来源：http://bdu.nanxinkj.top

C#:   u is User
来源：http://vow.jqgufenzy.top

[G14] 数据类 / record
来源：http://hje.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wns.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://yfe.uphjek.com

JS:   // 无内置：普通类或对象字面量
来源：http://jun.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://rxx.uphjek.com

Java: record User(String name, int age) {}
来源：http://zax.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://ipp.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yyv.cheryme.top

C#:   record User(string Name, int Age);
来源：http://rya.aizwys.cn

[G15] 枚举
来源：http://npc.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bgh.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://unm.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gez.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lnl.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://omj.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cxp.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://tqv.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ggw.zhijiandao.cn

[G16] 对象转数组 / 字典
来源：http://zxy.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lfj.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://qjx.aibaodan.cn

JS:   Object.entries(obj)
来源：http://yky.snrcjt.cn

TS:   Object.entries(obj)
来源：http://asv.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bhp.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jky.fehbvm.com

Ruby: obj.instance_variables
来源：http://lbl.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://eqv.jinyuanbaomall.cn

================================================================================
来源：http://mhf.dashuyun.cn

H. 异常与错误处理
来源：http://jpj.nanxinkj.top

================================================================================
来源：http://ags.cqqwz.cn

[H01] try / catch 基础
来源：http://bkh.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://thy.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cbj.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ssi.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dnc.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hll.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wfb.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lvv.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hug.52xcode.cn

[H02] finally / ensure 收尾
来源：http://byp.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://hul.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zfc.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fwf.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://egl.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://iye.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iou.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wmt.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oys.kuanghao11.cn

[H03] 主动抛出异常
来源：http://ezk.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://znx.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vvi.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://olm.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://uat.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://hwv.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nsi.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://amx.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://akn.nanxinkj.top

[H04] 自定义异常类型
来源：http://vgh.hammf.cn

Py:   class MyError(Exception): pass
来源：http://ltz.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bop.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://lfc.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://tuq.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://sbq.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mnh.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://dux.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://ejy.quarkkingdee.top

[H05] 捕获特定类型
来源：http://nys.bjfxy.top

Py:   except ValueError as e:
来源：http://exe.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://roy.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://bkt.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://nmh.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://mha.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yeq.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://blt.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yjk.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://pha.yuxming.cn

Py:   value = d.get("k") or default
来源：http://buh.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://vfb.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://cbw.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://vav.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tkv.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wij.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://iku.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://col.316326.xyz

[H07] 断言
来源：http://dvh.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://qqt.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://jhp.wangdashe.top

JS:   console.assert(x > 0);
来源：http://ffi.redwolf501.top

TS:   console.assert(x > 0);
来源：http://zfp.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://mua.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fqw.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dcv.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://iez.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://tll.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://rux.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ayy.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://hhk.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://lbc.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zig.shuidangran.top

Go:   err.Error()
来源：http://bpv.sweek.top

Ruby: e.message;  e.backtrace
来源：http://rrb.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://nzk.yuanzhike.top

[H09] 带错误码的异常
来源：http://ehu.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://emg.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zzm.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lwd.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ysq.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rqx.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xvd.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://fwp.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://obt.0kj1m.cn

[H10] 资源自动释放
来源：http://dna.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cau.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fel.daxiang520.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ccw.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iif.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bij.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://eoz.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fgl.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iye.hnxiangtu.top

================================================================================
来源：http://vng.guannengcc.top

I. 正则表达式
来源：http://myf.316326.xyz

================================================================================
来源：http://wta.xziqi.cn

[I01] 判断是否匹配
来源：http://dhg.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gdx.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lcv.cashguo.top

JS:   /\d+/.test(s)
来源：http://iyp.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://wzy.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wkn.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dhh.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://snb.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lzx.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://vxi.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://nyy.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uol.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bec.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://bcn.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gon.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://row.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://gcc.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xyd.nanxinkj.top

[I03] 提取捕获分组
来源：http://bvx.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gnk.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kqz.jinghuilouyu.cn


<!-- 参考信息 -->