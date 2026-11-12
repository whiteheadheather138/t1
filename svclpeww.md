代发 wailian999

[F09] 获取文件大小
来源：http://dvi.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://axs.hesvh.cn

PHP:  filesize("a.txt");
来源：http://ynm.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://gnz.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://jjv.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://tia.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ypc.fengsongda.top

Ruby: File.size("a.txt")
来源：http://okh.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://fpy.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://thj.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://luu.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nls.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ufl.yongpay.top

TS:   path.extname("a.txt")
来源：http://uma.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hai.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qmt.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hcy.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jlk.yueranfly.top

[F11] 复制与移动文件
来源：http://aki.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zaz.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ayf.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://odd.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://udb.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://izc.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://goc.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cop.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gpv.pycfn.com

[F12] CSV 读写
来源：http://ihz.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fri.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://shg.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yrr.hesvh.cn

TS:   // 同上
来源：http://qvm.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rah.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ohw.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ktz.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vmi.shangyingyoupin.top

================================================================================
来源：http://qnr.jiagoushi.top

G. 面向对象
来源：http://wnt.9152youxi.cn

================================================================================
来源：http://vum.kuanghao11.cn

[G01] 定义类
来源：http://mxa.jianghu66.top

Py:   class User: pass
来源：http://lxh.shanyushiyangkeji.top

PHP:  class User {}
来源：http://dnw.sysykeji.top

JS:   class User {}
来源：http://wiy.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://uwj.epnwcf.com

Java: class User {}
来源：http://hww.xziqi.cn

Go:   type User struct { Name string }
来源：http://lcd.9152youxi.cn

Ruby: class User; end
来源：http://leb.hfpthk.cn

C#:   class User {}
来源：http://lzd.ivvv.top

[G02] 构造函数
来源：http://ymv.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://izf.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://iwe.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://lxz.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://nap.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://wdd.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fbg.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://hgw.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://zxs.guowangkeji.top

[G03] 实例属性
来源：http://map.vqdsnc.cn

Py:   self.name = "x"
来源：http://onq.cashguo.top

PHP:  public string $name = "x";
来源：http://njn.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://cqo.uphjek.com

TS:   name: string = "x";
来源：http://gyd.iojbl.cn

Java: private String name;
来源：http://ivx.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hvy.sxryk.cn

Ruby: @name = "x"
来源：http://nax.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://ngs.guannengcc.top

[G04] 定义方法
来源：http://oog.havefunace.top

Py:   def greet(self): return self.name
来源：http://mge.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kvq.birdmap.top

JS:   greet() { return this.name; }
来源：http://zwp.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://aco.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://iku.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ooh.0kj1m.cn

Ruby: def greet; @name; end
来源：http://hju.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://nmu.52xcode.cn

[G05] 继承
来源：http://eln.jinqigufen.top

Py:   class Admin(User): pass
来源：http://lnx.mhx1999.top

PHP:  class Admin extends User {}
来源：http://aoe.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://xqd.yuanzhike.top

TS:   class Admin extends User {}
来源：http://llz.daxiang520.top

Java: class Admin extends User {}
来源：http://mlp.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mnj.yongpay.top

Ruby: class Admin < User; end
来源：http://gwd.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://gma.ydzc1.top

[G06] 重写方法
来源：http://ngy.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://pcw.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uov.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://gdf.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://kma.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://zkb.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bbi.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://tou.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://ymg.tianlin.xyz

[G07] 调用父类方法
来源：http://wvo.fehbvm.com

Py:   super().greet()
来源：http://okz.zdbjq.cn

PHP:  parent::greet();
来源：http://ilu.c1oappe.top

JS:   super.greet();
来源：http://dwl.hywenlv.cn

TS:   super.greet();
来源：http://rvb.fzhhl.top

Java: super.greet();
来源：http://wyu.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qhs.daria6918.cn

Ruby: super
来源：http://lfi.hywenlv.cn

C#:   base.Greet();
来源：http://jcq.hcnkem.com

[G08] 静态方法与属性
来源：http://atd.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pha.shuidangran.top

PHP:  public static function f() {}
来源：http://ilq.zhoulong.xyz

JS:   static f() {}
来源：http://dyy.jlsjyb.cn

TS:   static f(): void {}
来源：http://nbq.zhixingplan.top

Java: static void f() {}
来源：http://csh.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://iif.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://asj.tianlin.xyz

C#:   public static void F() {}
来源：http://hdi.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://yya.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://nvd.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://jtp.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://njp.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://dss.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://qbn.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://lra.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ybq.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://eig.yvedp.cn

[G10] 访问控制
来源：http://wkb.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://xhw.hysaishi.cn

PHP:  public / protected / private
来源：http://auu.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://shf.shangyingyoupin.top

TS:   public / protected / private
来源：http://qvc.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://uaq.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ccl.sweek.top

Ruby: public / protected / private
来源：http://fau.guowangkeji.top

C#:   public / protected / private / internal
来源：http://xfd.jinqigfzy.top

[G11] getter / setter
来源：http://qhs.vehdjk.com

Py:   @property 与 @x.setter
来源：http://iav.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zqn.yj20258.top

JS:   get name() { return this._name; }
来源：http://tze.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://thm.chenzaomai.com

Java: public String getName() { return name; }
来源：http://nkz.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://neo.pycfn.com

Ruby: attr_accessor :name
来源：http://xiq.daxiang520.top

C#:   public string Name { get; set; }
来源：http://dee.hcnkem.com

[G12] 对象转字符串
来源：http://yus.hammf.cn

Py:   def __str__(self): return self.name
来源：http://jpt.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rfd.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://cyh.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://nbc.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://cms.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jcj.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://rot.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://bsj.zdqjudy.top

[G13] 判断对象类型
来源：http://pov.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://oek.hnxiangtu.top

PHP:  $u instanceof User
来源：http://uep.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://hth.daxiang520.top

TS:   u instanceof User
来源：http://thu.hfpthk.cn

Java: u instanceof User
来源：http://zdn.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rut.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://lin.xuanzx.com

C#:   u is User
来源：http://uol.hnqzz.top

[G14] 数据类 / record
来源：http://vrv.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://obh.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://szu.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nvu.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://gim.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://qxa.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://omi.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sux.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://vev.c1oappe.top

[G15] 枚举
来源：http://ckd.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://klr.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fpd.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mty.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fyo.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://wde.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gee.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://nvz.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tmh.uphjek.com

[G16] 对象转数组 / 字典
来源：http://vou.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://loa.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://jvg.tanke756.top

JS:   Object.entries(obj)
来源：http://dgb.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://way.yj20258.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mdg.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pph.yonumen.top

Ruby: obj.instance_variables
来源：http://vtu.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://rrq.hcnkem.com

================================================================================
来源：http://mol.svipenyu.cn

H. 异常与错误处理
来源：http://swt.cdnleiting.top

================================================================================
来源：http://fjt.cdnleiting.top

[H01] try / catch 基础
来源：http://flm.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ppb.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ukg.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mtb.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kah.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fkg.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rpn.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xja.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fvv.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://tol.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://yqn.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pdg.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://poc.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pge.chenlongwang.top

Java: try { f(); } finally { cleanup(); }
来源：http://vox.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ivr.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kdw.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gbn.jqgfzy.top

[H03] 主动抛出异常
来源：http://umh.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://ixe.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zmg.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://egf.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://xfc.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kfc.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://upb.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://iqa.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://lqa.chenzaomai.com

[H04] 自定义异常类型
来源：http://wvk.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://wju.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://gla.c1oappe.top

JS:   class MyError extends Error {}
来源：http://nlb.aizwys.cn

TS:   class MyError extends Error {}
来源：http://ckm.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://ufv.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mwq.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://kcq.yj20258.top

C#:   class MyException : Exception {}
来源：http://dvt.zhengqikj.top

[H05] 捕获特定类型
来源：http://vfe.nwbrower.top

Py:   except ValueError as e:
来源：http://mzz.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sfs.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://ayd.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://nxl.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://odh.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uye.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://mca.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fzk.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://dty.shuidangran.top

Py:   value = d.get("k") or default
来源：http://jek.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ctv.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://vbv.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://ysr.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xmw.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nid.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://aei.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://ncl.yfazqb.com

[H07] 断言
来源：http://zjx.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://iuu.xziqi.cn

PHP:  assert($x > 0);
来源：http://uwo.hcnkem.com

JS:   console.assert(x > 0);
来源：http://nae.hammf.cn

TS:   console.assert(x > 0);
来源：http://cth.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://cqq.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ybh.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://zwn.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://gwp.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://cgy.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://vsa.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bhb.shuidangran.top

JS:   e.message;  e.stack
来源：http://vnk.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://chx.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ezj.gzhubu.top

Go:   err.Error()
来源：http://ucz.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://rso.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://klj.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://iiy.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qxo.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ccw.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rur.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gky.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eoo.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jds.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lcn.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qhx.fktsv.cn

[H10] 资源自动释放
来源：http://pol.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bib.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hzk.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ple.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://isr.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gnf.zhongyouzk.top

Go:   defer f.Close()
来源：http://ktm.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://phi.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nop.kuanghao11.cn

================================================================================
来源：http://igb.jiagoushi.top

I. 正则表达式
来源：http://cfh.sysykeji.top

================================================================================
来源：http://fmq.ehwqpu.com

[I01] 判断是否匹配
来源：http://oth.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qed.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fvy.fzhhl.top

JS:   /\d+/.test(s)
来源：http://jci.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://ncc.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nul.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mdj.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://dve.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jji.yuxming.cn

[I02] 提取所有匹配
来源：http://rzv.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://esz.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kfb.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zjj.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://vdw.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dan.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aki.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://qlc.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rat.chenzaomai.com

[I03] 提取捕获分组
来源：http://ywt.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oly.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kxo.zdbjq.cn


<!-- 参考信息 -->