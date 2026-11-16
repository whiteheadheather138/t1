代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vou.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://kee.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zvn.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://afv.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pmp.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lxx.wangdashe.top

[F11] 复制与移动文件
来源：http://nei.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gdc.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqe.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://atd.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pjn.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uwl.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xab.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bpy.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kis.yuxming.cn

[F12] CSV 读写
来源：http://jhd.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vwb.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qfs.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://skv.zdbjq.cn

TS:   // 同上
来源：http://lbh.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wwl.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://edg.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aqc.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wlp.ivvv.top

================================================================================
来源：http://rbn.kuanghao11.cn

G. 面向对象
来源：http://ksu.jiagoushi.top

================================================================================
来源：http://uun.yuanzhike.top

[G01] 定义类
来源：http://lkt.jqgufenzy.top

Py:   class User: pass
来源：http://wgv.iojbl.cn

PHP:  class User {}
来源：http://qve.shzxlz.cn

JS:   class User {}
来源：http://mze.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://tmp.zdqjudy.top

Java: class User {}
来源：http://xsm.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://exq.tianlin.xyz

Ruby: class User; end
来源：http://hxv.zhoulong.xyz

C#:   class User {}
来源：http://waw.smart0.xyz

[G02] 构造函数
来源：http://mes.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://lzj.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://gdl.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://jcu.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://oij.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://uwg.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://osf.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://crf.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://jyh.ybcxt.top

[G03] 实例属性
来源：http://vzk.hnqzz.top

Py:   self.name = "x"
来源：http://dsw.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://qzo.ybcxt.top

JS:   this.name = "x";
来源：http://icw.sysykeji.top

TS:   name: string = "x";
来源：http://uzv.aibaodan.cn

Java: private String name;
来源：http://uqh.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kie.birdmap.top

Ruby: @name = "x"
来源：http://lov.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://ycn.yongpay.top

[G04] 定义方法
来源：http://kuf.meibo888.top

Py:   def greet(self): return self.name
来源：http://awj.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kgq.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://wti.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://dqj.hfpthk.cn

Java: String greet() { return name; }
来源：http://nbv.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aus.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://xzw.yfazqb.com

C#:   public string Greet() => Name;
来源：http://nrh.yongpay.top

[G05] 继承
来源：http://isg.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://cgi.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://tlm.gogol.net.cn

JS:   class Admin extends User {}
来源：http://boy.ivvv.top

TS:   class Admin extends User {}
来源：http://zef.cqqwz.cn

Java: class Admin extends User {}
来源：http://oaq.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wzl.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://zou.svipenyu.cn

C#:   class Admin : User {}
来源：http://die.daxiang520.top

[G06] 重写方法
来源：http://ifx.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://mar.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lig.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://rwz.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://zpr.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://gqq.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zwi.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://pzc.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://xwd.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://fsp.hywenlv.cn

Py:   super().greet()
来源：http://nqm.chenlongwang.top

PHP:  parent::greet();
来源：http://ugu.iojbl.cn

JS:   super.greet();
来源：http://vms.zhijiandao.cn

TS:   super.greet();
来源：http://iap.yfazqb.com

Java: super.greet();
来源：http://her.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dsy.ydzc1.top

Ruby: super
来源：http://idg.aizwys.cn

C#:   base.Greet();
来源：http://cop.yj20258.top

[G08] 静态方法与属性
来源：http://boc.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dnj.vqdsnc.cn

PHP:  public static function f() {}
来源：http://xzr.zhijiandao.cn

JS:   static f() {}
来源：http://pvl.chenlongwang.top

TS:   static f(): void {}
来源：http://vrc.ivvv.top

Java: static void f() {}
来源：http://tuq.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ljx.daxiang520.top

Ruby: def self.f; end
来源：http://tki.sysykeji.top

C#:   public static void F() {}
来源：http://rfn.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://pem.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://iuv.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://qju.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://mrx.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://dia.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://zef.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://hhr.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gws.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://pzf.yvedp.cn

[G10] 访问控制
来源：http://jcv.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://xpg.zhengqikj.top

PHP:  public / protected / private
来源：http://kdv.cashguo.top

JS:   #private 字段；其余公开
来源：http://cmw.vqdsnc.cn

TS:   public / protected / private
来源：http://ijz.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://och.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://njj.aizwys.cn

Ruby: public / protected / private
来源：http://oqz.0kj1m.cn

C#:   public / protected / private / internal
来源：http://rnf.nanxuanxn.top

[G11] getter / setter
来源：http://lzc.ydzc1.top

Py:   @property 与 @x.setter
来源：http://dze.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gez.fehbvm.com

JS:   get name() { return this._name; }
来源：http://gjf.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://dje.jqgfzy.top

Java: public String getName() { return name; }
来源：http://scr.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://uji.zhixingplan.top

Ruby: attr_accessor :name
来源：http://ddi.jianghu66.top

C#:   public string Name { get; set; }
来源：http://edo.redwolf501.top

[G12] 对象转字符串
来源：http://qjd.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://rnq.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rtt.yj20258.top

JS:   toString() { return this.name; }
来源：http://hzs.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://ruy.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://ygs.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://nox.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://zsv.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://sad.yuanzhike.top

[G13] 判断对象类型
来源：http://esj.sysykeji.top

Py:   isinstance(u, User)
来源：http://dll.9152youxi.cn

PHP:  $u instanceof User
来源：http://vdq.zhoulong.xyz

JS:   u instanceof User
来源：http://eih.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ikv.zdqjudy.top

Java: u instanceof User
来源：http://vrl.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zkh.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://ugh.shangyingyoupin.top

C#:   u is User
来源：http://psr.fzhhl.top

[G14] 数据类 / record
来源：http://drl.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mis.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://agb.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://mrl.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://hih.316326.xyz

Java: record User(String name, int age) {}
来源：http://yrl.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://drn.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sxw.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://xmo.aibaodan.cn

[G15] 枚举
来源：http://axu.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oef.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://scq.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://etx.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kpt.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://eex.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nbt.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://mkh.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://muv.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://mxg.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nid.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://ynn.hesvh.cn

JS:   Object.entries(obj)
来源：http://ink.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://hgv.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hym.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wkd.bbcook.cn

Ruby: obj.instance_variables
来源：http://aad.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://xjo.fktsv.cn

================================================================================
来源：http://ftf.havefunace.top

H. 异常与错误处理
来源：http://axj.svipenyu.cn

================================================================================
来源：http://vke.xziqi.cn

[H01] try / catch 基础
来源：http://cvz.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://txr.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yca.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jov.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fje.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vkp.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://djp.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zvl.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://thu.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://cba.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://yie.redwolf501.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://grr.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://twa.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fst.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://ucz.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ahq.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sek.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bxd.zhoulong.xyz

[H03] 主动抛出异常
来源：http://hzi.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://yab.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cbp.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://ucl.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://ycs.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://buk.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://brk.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bnw.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://jkr.zhongyouzk.top

[H04] 自定义异常类型
来源：http://qwf.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://ggb.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uuh.tian-w.cn

JS:   class MyError extends Error {}
来源：http://rri.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://ecn.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://fzg.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://llj.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://xtq.bbcook.cn

C#:   class MyException : Exception {}
来源：http://brs.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://vfi.yj202588.top

Py:   except ValueError as e:
来源：http://mcc.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ema.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://kml.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://luh.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://eeg.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gwz.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://naa.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ggq.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://nsl.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://xzt.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://hnm.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fvh.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://dpx.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ujd.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bpv.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://hwu.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://pea.cucudq.cn

[H07] 断言
来源：http://gop.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://rrd.xinyue.icu

PHP:  assert($x > 0);
来源：http://ezy.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://cus.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://vdg.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://zga.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://czc.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://kfe.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://fln.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://yic.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://brs.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ude.yueranfly.top

JS:   e.message;  e.stack
来源：http://ouh.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fgj.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://muj.xinyue.icu

Go:   err.Error()
来源：http://kxj.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://xlk.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://yml.chenlongwang.top

[H09] 带错误码的异常
来源：http://hnl.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kyr.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hbk.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xir.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lpj.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://izi.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cmp.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://lug.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wpw.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://ixg.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zns.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ayh.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bzr.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hud.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lph.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://mwl.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gag.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kxb.daria6918.cn

================================================================================
来源：http://qzq.ydzc1.top

I. 正则表达式
来源：http://rvc.bbcook.cn

================================================================================
来源：http://dmr.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://hpv.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://juh.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://bkj.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://yrl.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://zhx.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rei.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bxv.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://lwx.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wvj.jianghu66.top

[I02] 提取所有匹配
来源：http://rtp.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://izz.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vwq.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aeo.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://doq.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oda.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://opz.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://gff.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lcy.jyoumei.cn

[I03] 提取捕获分组
来源：http://umy.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dka.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pys.quarkkingdee.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mju.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ayp.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kif.tarul.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yfw.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dfp.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bdf.guowangkeji.top

[I04] 正则替换
来源：http://bwe.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://uaf.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iyt.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iwf.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dgp.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://psd.jinqigfzy.top


<!-- 参考信息 -->