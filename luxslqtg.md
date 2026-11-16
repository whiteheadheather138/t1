代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://rel.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wsd.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ucy.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://utx.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://zch.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://piq.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eyh.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vxh.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hfr.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://oku.feifeiyinyue.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rbn.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ctd.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://amp.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oja.wangdashe.top

[F11] 复制与移动文件
来源：http://jxd.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tbj.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://onz.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://abb.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jhp.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xzx.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yem.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ywt.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cko.9152youxi.cn

[F12] CSV 读写
来源：http://rhu.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hmp.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pwe.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uxb.52xcode.cn

TS:   // 同上
来源：http://znu.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://liq.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uwm.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cbl.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iib.dashuyun.cn

================================================================================
来源：http://oow.chenzaomai.com

G. 面向对象
来源：http://lgi.tian-w.cn

================================================================================
来源：http://tev.hesvh.cn

[G01] 定义类
来源：http://pts.bjfxy.top

Py:   class User: pass
来源：http://egv.aibaodan.cn

PHP:  class User {}
来源：http://tqx.chenjidiqi.icu

JS:   class User {}
来源：http://eiu.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://szb.zhengqikj.top

Java: class User {}
来源：http://jri.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://gnb.fengsongda.top

Ruby: class User; end
来源：http://rnf.0kj1m.cn

C#:   class User {}
来源：http://znz.cucudq.cn

[G02] 构造函数
来源：http://lqg.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://rid.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://vux.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://axd.yj20258.top

TS:   constructor(public name: string) {}
来源：http://vay.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://abo.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qak.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://vqi.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://ojm.zhongyouzk.top

[G03] 实例属性
来源：http://ley.zhongyouzk.top

Py:   self.name = "x"
来源：http://roc.havefunace.top

PHP:  public string $name = "x";
来源：http://nan.yj20258888.top

JS:   this.name = "x";
来源：http://xhb.ybcxt.top

TS:   name: string = "x";
来源：http://ahg.yuxming.cn

Java: private String name;
来源：http://ino.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://doi.tianlin.xyz

Ruby: @name = "x"
来源：http://qtn.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://qog.jyoumei.cn

[G04] 定义方法
来源：http://pgw.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://zxj.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hxe.yfazqb.com

JS:   greet() { return this.name; }
来源：http://pjc.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://csh.zhongyouzk.top

Java: String greet() { return name; }
来源：http://bpm.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kzy.316326.xyz

Ruby: def greet; @name; end
来源：http://aid.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://zjs.feifeiyinyue.top

[G05] 继承
来源：http://qyc.zdbjq.cn

Py:   class Admin(User): pass
来源：http://ykk.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://oix.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://kzm.jianghu66.top

TS:   class Admin extends User {}
来源：http://lwa.zhongyouzk.top

Java: class Admin extends User {}
来源：http://pnq.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ybs.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://icn.zhongyouzk.top

C#:   class Admin : User {}
来源：http://hty.hesvh.cn

[G06] 重写方法
来源：http://qri.yj20258.top

Py:   def greet(self): return "admin"
来源：http://xvv.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://naj.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://ksj.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://jhi.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://adc.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ksx.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://tzl.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://neu.mhx1999.top

[G07] 调用父类方法
来源：http://jzj.uphjek.com

Py:   super().greet()
来源：http://zsr.xingfuxueyuan.xyz

PHP:  parent::greet();
来源：http://dic.ehwqpu.com

JS:   super.greet();
来源：http://omf.tian-w.cn

TS:   super.greet();
来源：http://lqr.ybcxt.top

Java: super.greet();
来源：http://kzo.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vlx.uphjek.com

Ruby: super
来源：http://upx.chenjidiqi.icu

C#:   base.Greet();
来源：http://umw.cqqwz.cn

[G08] 静态方法与属性
来源：http://qgi.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vzb.ehwqpu.com

PHP:  public static function f() {}
来源：http://ggv.tianlin.xyz

JS:   static f() {}
来源：http://jaf.hfpthk.cn

TS:   static f(): void {}
来源：http://doa.zdbjq.cn

Java: static void f() {}
来源：http://kqa.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://lkf.yvedp.cn

Ruby: def self.f; end
来源：http://aol.cheryme.top

C#:   public static void F() {}
来源：http://cpc.epnwcf.com

[G09] 接口 / 抽象类
来源：http://vla.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://ipy.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://thb.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ncn.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://utr.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://gcx.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://ebf.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ohn.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://vnr.cdnleiting.top

[G10] 访问控制
来源：http://pjl.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://lva.gaohongyu789.top

PHP:  public / protected / private
来源：http://lei.zhiwuduotai.top

JS:   #private 字段；其余公开
来源：http://vmu.sjlbkw.cn

TS:   public / protected / private
来源：http://xmg.316326.xyz

Java: public / protected / private / 默认包级
来源：http://qvo.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xoa.hnqzz.top

Ruby: public / protected / private
来源：http://suf.birdmap.top

C#:   public / protected / private / internal
来源：http://iop.sjlbkw.cn

[G11] getter / setter
来源：http://ycm.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://fhu.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qsf.tian-w.cn

JS:   get name() { return this._name; }
来源：http://zzy.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://cnc.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://xvc.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ewb.yuanzhike.top

Ruby: attr_accessor :name
来源：http://lzz.gzhubu.top

C#:   public string Name { get; set; }
来源：http://ofw.chenlongwang.top

[G12] 对象转字符串
来源：http://izn.havefunace.top

Py:   def __str__(self): return self.name
来源：http://vev.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://iqo.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://ytf.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://ahr.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://xcn.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://elc.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://gvo.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://vvo.gaohongyu789.top

[G13] 判断对象类型
来源：http://hjk.zhengqikj.top

Py:   isinstance(u, User)
来源：http://ovt.smart0.xyz

PHP:  $u instanceof User
来源：http://caq.hysaishi.cn

JS:   u instanceof User
来源：http://uif.vehdjk.com

TS:   u instanceof User
来源：http://nav.ivvv.top

Java: u instanceof User
来源：http://ahe.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fbg.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://vkj.sjlbkw.cn

C#:   u is User
来源：http://xky.fehbvm.com

[G14] 数据类 / record
来源：http://wfs.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hrl.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://veo.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://zzm.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://ddw.ybcxt.top

Java: record User(String name, int age) {}
来源：http://spw.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://min.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jdl.jqgufenzy.top

C#:   record User(string Name, int Age);
来源：http://iha.shanyushiyangkeji.top

[G15] 枚举
来源：http://rsz.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uas.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jih.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nvl.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://odl.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://nnw.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wdb.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://iqj.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jky.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://rbd.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fzc.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://yls.tianlin.xyz

JS:   Object.entries(obj)
来源：http://nmt.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://owy.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bem.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qfe.havefunace.top

Ruby: obj.instance_variables
来源：http://ppi.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://lez.cucudq.cn

================================================================================
来源：http://cjx.wangshuangyany.cn

H. 异常与错误处理
来源：http://xpv.yuanzhike.top

================================================================================
来源：http://axj.gzhubu.top

[H01] try / catch 基础
来源：http://vbg.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hfn.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fct.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://czm.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://alj.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zwb.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lrw.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uht.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sve.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://gcn.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://wou.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rih.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://cts.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://get.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bnd.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://upy.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yhu.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lom.xinyue.icu

[H03] 主动抛出异常
来源：http://bjj.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://axv.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ghd.sweek.top

JS:   throw new Error("错误信息");
来源：http://gpq.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://uxu.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mnc.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://glu.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rvz.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jrk.mhx1999.top

[H04] 自定义异常类型
来源：http://pyi.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://iou.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://vlg.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://qxg.bbcook.cn

TS:   class MyError extends Error {}
来源：http://rwb.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://vnh.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mjs.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://abt.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://ziy.gotoacloud.top

[H05] 捕获特定类型
来源：http://rwc.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://jwx.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vcz.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://lqe.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://smt.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://jqr.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kxe.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://qps.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://luo.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://ayd.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://ntd.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://aob.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://oge.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uan.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ngw.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rrp.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://sth.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://nht.yongpay.top

[H07] 断言
来源：http://kue.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://lld.jqgfzy.top

PHP:  assert($x > 0);
来源：http://hug.pycfn.com

JS:   console.assert(x > 0);
来源：http://csr.yuxming.cn

TS:   console.assert(x > 0);
来源：http://bgy.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://uqc.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tfb.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hhs.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://mkm.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://fhr.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://zbc.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jfn.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://hmp.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iii.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mra.dianchejie.cn

Go:   err.Error()
来源：http://kub.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://aet.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://rht.uphjek.com

[H09] 带错误码的异常
来源：http://fed.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dte.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xka.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rdn.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tfj.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dod.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xlx.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vmn.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://czl.ppjwa.cn

[H10] 资源自动释放
来源：http://ovc.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://szz.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zve.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mol.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://auj.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bgc.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://ihx.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nld.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://goh.hywenlv.cn

================================================================================
来源：http://ywg.wangshuangyany.cn

I. 正则表达式
来源：http://ziz.tanke756.top

================================================================================
来源：http://qmu.yongpay.top

[I01] 判断是否匹配
来源：http://gdp.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://osy.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://npe.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://nuo.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://fwz.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yrt.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gmh.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://wkb.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vdk.vqdsnc.cn

[I02] 提取所有匹配
来源：http://sxf.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://jwy.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oul.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://leg.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://hay.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://waa.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://srz.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://pyk.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://okr.fktsv.cn

[I03] 提取捕获分组
来源：http://hov.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nit.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xmn.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xmn.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mxz.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bbk.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cag.hysaishi.cn


<!-- 参考信息 -->