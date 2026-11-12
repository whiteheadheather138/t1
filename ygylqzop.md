代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mtk.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://hlz.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cax.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wpg.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jfx.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iep.yanxiufei.cn

[F11] 复制与移动文件
来源：http://ocz.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://afs.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rlr.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lyu.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cye.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hgd.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ljt.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vvi.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rdx.daria6918.cn

[F12] CSV 读写
来源：http://lwv.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mnd.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wkh.snrcjt.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ybb.yangfankeji.com

TS:   // 同上
来源：http://gwd.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vbk.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ezy.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mhd.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hsf.sweek.top

================================================================================
来源：http://ewa.aizwys.cn

G. 面向对象
来源：http://rwk.yuxming.cn

================================================================================
来源：http://srq.jinqigufen.top

[G01] 定义类
来源：http://yoh.iojbl.cn

Py:   class User: pass
来源：http://xgh.yj20258888.top

PHP:  class User {}
来源：http://jgk.sxryk.cn

JS:   class User {}
来源：http://plz.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://spn.andypj.xyz

Java: class User {}
来源：http://icc.316326.xyz

Go:   type User struct { Name string }
来源：http://anz.jinqigfzy.top

Ruby: class User; end
来源：http://tld.ehwqpu.com

C#:   class User {}
来源：http://jjv.svipenyu.cn

[G02] 构造函数
来源：http://exy.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://ydw.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://qex.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://etr.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://eap.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://yvq.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qfm.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://des.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://vid.nanxinkj.top

[G03] 实例属性
来源：http://gcc.hysaishi.cn

Py:   self.name = "x"
来源：http://olc.ivvv.top

PHP:  public string $name = "x";
来源：http://kri.ybcxt.top

JS:   this.name = "x";
来源：http://xuy.smart0.xyz

TS:   name: string = "x";
来源：http://dqu.iojbl.cn

Java: private String name;
来源：http://yok.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kmk.sweek.top

Ruby: @name = "x"
来源：http://csr.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://bdh.havefunace.top

[G04] 定义方法
来源：http://yry.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://hqs.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hzb.yvedp.cn

JS:   greet() { return this.name; }
来源：http://fkn.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://hqw.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://jeo.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ebv.cashguo.top

Ruby: def greet; @name; end
来源：http://one.smart0.xyz

C#:   public string Greet() => Name;
来源：http://knb.feifeiyinyue.top

[G05] 继承
来源：http://xto.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://zok.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://fik.bbcook.cn

JS:   class Admin extends User {}
来源：http://awt.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://bdw.epnwcf.com

Java: class Admin extends User {}
来源：http://mwt.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ybd.ydzc1.top

Ruby: class Admin < User; end
来源：http://fcq.haohaochexian.top

C#:   class Admin : User {}
来源：http://ymo.havefunace.top

[G06] 重写方法
来源：http://lvg.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://vmc.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eww.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://pbd.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://bbq.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://mxt.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fmp.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://wdk.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://fse.yvedp.cn

[G07] 调用父类方法
来源：http://wkh.xuetiantiany.cn

Py:   super().greet()
来源：http://dje.mhx1999.top

PHP:  parent::greet();
来源：http://bdu.yuxming.cn

JS:   super.greet();
来源：http://sqn.quarkkingdee.top

TS:   super.greet();
来源：http://mvr.ctjpmb.com

Java: super.greet();
来源：http://arf.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aex.fengsongda.top

Ruby: super
来源：http://zoz.gzhubu.top

C#:   base.Greet();
来源：http://erq.9152youxi.cn

[G08] 静态方法与属性
来源：http://tyt.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xrc.xuanzx.com

PHP:  public static function f() {}
来源：http://eyw.hfpthk.cn

JS:   static f() {}
来源：http://rvf.ehwqpu.com

TS:   static f(): void {}
来源：http://qip.ppjwa.cn

Java: static void f() {}
来源：http://tni.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zim.snrcjt.cn

Ruby: def self.f; end
来源：http://pob.guowangkeji.top

C#:   public static void F() {}
来源：http://zum.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://bsg.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://llx.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://yte.bjfxy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xfa.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://iol.aizwys.cn

Java: interface Shape { double area(); }
来源：http://huy.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://gnn.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wbz.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://juy.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://uch.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://fnk.gaohongyu789.top

PHP:  public / protected / private
来源：http://skv.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://ypq.fehbvm.com

TS:   public / protected / private
来源：http://jod.cheryme.top

Java: public / protected / private / 默认包级
来源：http://xgi.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cde.daxiang520.top

Ruby: public / protected / private
来源：http://kyp.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://nlb.svipenyu.cn

[G11] getter / setter
来源：http://sbo.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://cmh.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://cgg.c1oappe.top

JS:   get name() { return this._name; }
来源：http://ueq.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://ycq.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://cwv.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://efp.xuanzx.com

Ruby: attr_accessor :name
来源：http://adc.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://noz.gogol.net.cn

[G12] 对象转字符串
来源：http://gib.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://gkq.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wgs.cashguo.top

JS:   toString() { return this.name; }
来源：http://lpu.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://mpm.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://epx.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jdt.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://fih.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://klo.andypj.xyz

[G13] 判断对象类型
来源：http://aap.52xcode.cn

Py:   isinstance(u, User)
来源：http://jxk.dashuyun.cn

PHP:  $u instanceof User
来源：http://oag.redwolf501.top

JS:   u instanceof User
来源：http://ftq.hnxiangtu.top

TS:   u instanceof User
来源：http://sal.snrcjt.cn

Java: u instanceof User
来源：http://qoj.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://kyx.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://bxl.meibo888.top

C#:   u is User
来源：http://fpn.fktsv.cn

[G14] 数据类 / record
来源：http://xph.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fhv.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://gim.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://xww.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://wde.yongpay.top

Java: record User(String name, int age) {}
来源：http://xef.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://eoe.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pfu.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://tbg.jiagoushi.top

[G15] 枚举
来源：http://fjt.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bwh.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gyr.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zrt.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mwu.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://yku.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wdz.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://ccy.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://flx.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://dnh.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wrz.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://isj.svipenyu.cn

JS:   Object.entries(obj)
来源：http://nac.dianchejie.cn

TS:   Object.entries(obj)
来源：http://rtp.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hjn.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qel.jqgfzy.top

Ruby: obj.instance_variables
来源：http://wns.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://aiq.meibo888.top

================================================================================
来源：http://dci.nwbrower.top

H. 异常与错误处理
来源：http://wwm.chenzaomai.com

================================================================================
来源：http://weo.chenjidiqi.icu

[H01] try / catch 基础
来源：http://mex.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jtp.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tlw.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hen.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wss.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bok.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://syf.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nyi.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aae.sysykeji.top

[H02] finally / ensure 收尾
来源：http://oyz.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://qwx.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ktb.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tum.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nom.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://rbf.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mvo.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ayw.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ptk.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://sfx.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://hct.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zry.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://djh.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://bln.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfc.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ykh.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://app.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fvs.smart0.xyz

[H04] 自定义异常类型
来源：http://shf.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://arv.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://vsd.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://hzf.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://svy.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://hvi.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://etk.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://brz.hammf.cn

C#:   class MyException : Exception {}
来源：http://suv.jinqigfzy.top

[H05] 捕获特定类型
来源：http://bwh.jinqigufen.top

Py:   except ValueError as e:
来源：http://czn.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vmo.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://vyy.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://kxu.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://zzw.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://smd.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://knv.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wte.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://geu.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://hox.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://zic.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://vrs.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://khz.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zcb.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gio.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://tdw.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://onz.shuidangran.top

[H07] 断言
来源：http://ruv.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://skl.yvedp.cn

PHP:  assert($x > 0);
来源：http://wok.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://qcb.yonumen.top

TS:   console.assert(x > 0);
来源：http://ybv.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://qdd.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hwm.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://sdu.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://nbk.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://xdx.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://tpp.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gky.dianchejie.cn

JS:   e.message;  e.stack
来源：http://lzu.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ven.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fuk.pengpengdd.cyou

Go:   err.Error()
来源：http://qxe.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://zpu.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://rop.guowangkeji.top

[H09] 带错误码的异常
来源：http://tvs.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gkw.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pob.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tra.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lig.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ven.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tgv.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://enm.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vya.kuanghao11.cn

[H10] 资源自动释放
来源：http://vvm.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pnx.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jdt.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tgx.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://txy.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wfy.hesvh.cn

Go:   defer f.Close()
来源：http://wlt.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jfc.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rvx.ydzc1.top

================================================================================
来源：http://wfb.guannengcc.top

I. 正则表达式
来源：http://qwa.jianghu66.top

================================================================================
来源：http://vub.tanke756.top

[I01] 判断是否匹配
来源：http://ynz.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://laz.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zmv.guannengcc.top

JS:   /\d+/.test(s)
来源：http://xvq.sysykeji.top

TS:   /\d+/.test(s)
来源：http://grn.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vcs.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://drn.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://xku.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xkp.hfpthk.cn

[I02] 提取所有匹配
来源：http://ywj.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://wem.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lcl.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vro.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://apw.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mnd.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kkq.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://pnj.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bpv.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://xss.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pgb.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://egh.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://muz.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gjk.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rqs.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rek.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gby.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zjx.yuanzhike.top

[I04] 正则替换
来源：http://hyt.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cfm.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mub.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kho.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://yrp.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qxg.gogol.net.cn


<!-- 参考信息 -->