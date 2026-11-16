代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ush.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nhz.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://xuu.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://rwj.sysykeji.top

[F09] 获取文件大小
来源：http://uwi.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://rpk.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://nru.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://zsc.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://yrp.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://zby.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xbv.xuanzx.com

Ruby: File.size("a.txt")
来源：http://rwm.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://mhw.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://ucs.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xpz.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pvy.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tea.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://uct.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gke.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qgt.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nvl.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://suo.shzxlz.cn

[F11] 复制与移动文件
来源：http://tso.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://phd.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zao.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgj.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yzg.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gvs.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nrm.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cdo.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vtw.9152youxi.cn

[F12] CSV 读写
来源：http://sxd.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nlp.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sqa.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pse.ydjk.org.cn

TS:   // 同上
来源：http://ddc.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qvp.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://akb.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bmq.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://smh.xuetiantiany.cn

================================================================================
来源：http://zmy.yfazqb.com

G. 面向对象
来源：http://tmr.sjlbkw.cn

================================================================================
来源：http://bvs.svipenyu.cn

[G01] 定义类
来源：http://vwg.shzxlz.cn

Py:   class User: pass
来源：http://nip.chenjidiqi.icu

PHP:  class User {}
来源：http://ger.wangdashe.top

JS:   class User {}
来源：http://eap.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://fkr.daria6918.cn

Java: class User {}
来源：http://nxo.smart0.xyz

Go:   type User struct { Name string }
来源：http://vgp.tian-w.cn

Ruby: class User; end
来源：http://vye.xziqi.cn

C#:   class User {}
来源：http://mdq.nanxuanxn.top

[G02] 构造函数
来源：http://ilg.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://liu.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://imr.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://nmd.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://pjz.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://gvj.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vmb.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://obr.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://zrk.cucudq.cn

[G03] 实例属性
来源：http://jvc.vqdsnc.cn

Py:   self.name = "x"
来源：http://bnd.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://odp.sxryk.cn

JS:   this.name = "x";
来源：http://tlt.ivvv.top

TS:   name: string = "x";
来源：http://uva.chenlongwang.top

Java: private String name;
来源：http://hgv.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://voz.jyoumei.cn

Ruby: @name = "x"
来源：http://izu.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://kkx.316326.xyz

[G04] 定义方法
来源：http://qxn.yvedp.cn

Py:   def greet(self): return self.name
来源：http://sjl.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kjh.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://pmf.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://ngx.wangdashe.top

Java: String greet() { return name; }
来源：http://gjw.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ygp.aibaodan.cn

Ruby: def greet; @name; end
来源：http://qhe.jianghu66.top

C#:   public string Greet() => Name;
来源：http://zqr.yuanzhike.top

[G05] 继承
来源：http://siy.nanxinkj.top

Py:   class Admin(User): pass
来源：http://akr.ivvv.top

PHP:  class Admin extends User {}
来源：http://xnt.hesvh.cn

JS:   class Admin extends User {}
来源：http://rcj.daria6918.cn

TS:   class Admin extends User {}
来源：http://doe.hcnkem.com

Java: class Admin extends User {}
来源：http://owy.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aei.yangfankeji.com

Ruby: class Admin < User; end
来源：http://qzt.zhoulong.xyz

C#:   class Admin : User {}
来源：http://vak.gzhubu.top

[G06] 重写方法
来源：http://ebh.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://wuf.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gep.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://lly.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://ait.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://vaq.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://euk.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://arh.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://cyi.hfpthk.cn

[G07] 调用父类方法
来源：http://lxa.nwbrower.top

Py:   super().greet()
来源：http://mmy.shangyingyoupin.top

PHP:  parent::greet();
来源：http://ics.yj20258.top

JS:   super.greet();
来源：http://nde.jianghu66.top

TS:   super.greet();
来源：http://tts.hnxiangtu.top

Java: super.greet();
来源：http://bfq.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wik.bjfxy.top

Ruby: super
来源：http://cau.havefunace.top

C#:   base.Greet();
来源：http://yvn.sxryk.cn

[G08] 静态方法与属性
来源：http://chb.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dtr.fzhhl.top

PHP:  public static function f() {}
来源：http://zto.tarul.cn

JS:   static f() {}
来源：http://nfp.cucudq.cn

TS:   static f(): void {}
来源：http://hdp.redwolf501.top

Java: static void f() {}
来源：http://ojl.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://uoq.sufxvd.cn

Ruby: def self.f; end
来源：http://ysw.tanke756.top

C#:   public static void F() {}
来源：http://seo.fktsv.cn

[G09] 接口 / 抽象类
来源：http://gcy.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://kps.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ziv.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://prh.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://pit.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://yfb.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://fkl.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://exe.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://qva.ydzc1.top

[G10] 访问控制
来源：http://kfk.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://jst.chenjidiqi.icu

PHP:  public / protected / private
来源：http://nrd.birdmap.top

JS:   #private 字段；其余公开
来源：http://bbk.tanke756.top

TS:   public / protected / private
来源：http://rvh.316326.xyz

Java: public / protected / private / 默认包级
来源：http://yqo.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://yct.bbcook.cn

Ruby: public / protected / private
来源：http://pxs.jinqigufen.top

C#:   public / protected / private / internal
来源：http://atk.havefunace.top

[G11] getter / setter
来源：http://sac.xziqi.cn

Py:   @property 与 @x.setter
来源：http://qte.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qkm.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://xhw.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://sgv.aizwys.cn

Java: public String getName() { return name; }
来源：http://xwf.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fad.cucudq.cn

Ruby: attr_accessor :name
来源：http://api.sweek.top

C#:   public string Name { get; set; }
来源：http://jcb.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://caz.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://cxb.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://egc.tarul.cn

JS:   toString() { return this.name; }
来源：http://fyl.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://log.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://utt.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gee.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://bfl.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://wli.9152youxi.cn

[G13] 判断对象类型
来源：http://jox.zdqjudy.top

Py:   isinstance(u, User)
来源：http://vqt.iojbl.cn

PHP:  $u instanceof User
来源：http://rci.hfpthk.cn

JS:   u instanceof User
来源：http://fvz.birdmap.top

TS:   u instanceof User
来源：http://xls.cdnleiting.top

Java: u instanceof User
来源：http://thg.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vbh.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://mwv.ivvv.top

C#:   u is User
来源：http://edu.xylfe.cn

[G14] 数据类 / record
来源：http://qla.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pak.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://czr.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://jyj.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://eir.hammf.cn

Java: record User(String name, int age) {}
来源：http://zma.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://phx.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nmo.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://vsk.zhijiandao.cn

[G15] 枚举
来源：http://nub.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://trk.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://cve.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kud.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uar.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://xzj.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cya.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://kfk.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hyk.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://jct.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gbd.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://xqu.daxiang520.top

JS:   Object.entries(obj)
来源：http://jij.xziqi.cn

TS:   Object.entries(obj)
来源：http://yhm.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bkz.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://zbs.jyoumei.cn

Ruby: obj.instance_variables
来源：http://pyv.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://ugb.vehdjk.com

================================================================================
来源：http://wso.sweek.top

H. 异常与错误处理
来源：http://fhq.sjlbkw.cn

================================================================================
来源：http://sdw.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://mem.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qmh.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://axs.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://smh.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://owh.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://atv.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vlh.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hkh.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xit.mhx1999.top

[H02] finally / ensure 收尾
来源：http://fws.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://nlb.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hsr.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ltb.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ghg.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://lor.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nno.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aud.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://doj.quarkkingdee.top

[H03] 主动抛出异常
来源：http://ttm.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://vxu.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kzw.tarul.cn

JS:   throw new Error("错误信息");
来源：http://pdm.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://fkh.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://bbg.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cip.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lfm.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://ywc.yangfankeji.com

[H04] 自定义异常类型
来源：http://xbd.tarul.cn

Py:   class MyError(Exception): pass
来源：http://bbe.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fmy.yueranfly.top

JS:   class MyError extends Error {}
来源：http://bnk.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://kst.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://vnj.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uaf.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://zlu.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://zos.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://lix.guannengcc.top

Py:   except ValueError as e:
来源：http://yfz.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ibo.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://moq.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://trt.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://hlq.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://btl.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://xqo.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://svb.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://ydf.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://vhy.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://rfc.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://vvl.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://txs.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ntl.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vxo.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://lbp.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://qud.nwbrower.top

[H07] 断言
来源：http://ofp.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://hbx.fzhhl.top

PHP:  assert($x > 0);
来源：http://kyn.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://cfp.ivvv.top

TS:   console.assert(x > 0);
来源：http://xdb.bbcook.cn

Java: assert x > 0 : "必须为正";
来源：http://ftw.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jpo.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://vnf.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://axw.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://vgh.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://ukm.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://noi.svipenyu.cn

JS:   e.message;  e.stack
来源：http://enf.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cki.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://csi.yongpay.top

Go:   err.Error()
来源：http://yvd.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://nqo.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://qua.cashguo.top

[H09] 带错误码的异常
来源：http://jpj.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mbd.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rjn.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gkz.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mnq.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uty.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yod.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ikx.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pgk.yongpay.top

[H10] 资源自动释放
来源：http://rvd.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qxn.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sxx.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gtz.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://upw.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://alt.tian-w.cn

Go:   defer f.Close()
来源：http://egd.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ilv.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kin.andypj.xyz

================================================================================
来源：http://yca.yuanzhike.top

I. 正则表达式
来源：http://qiz.xinyue.icu

================================================================================
来源：http://cgb.cucudq.cn

[I01] 判断是否匹配
来源：http://kgb.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://feu.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://cgf.yj202588.top

JS:   /\d+/.test(s)
来源：http://ahf.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://apw.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nwy.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ccc.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://gzz.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kzq.316326.xyz

[I02] 提取所有匹配
来源：http://uly.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://aha.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gpx.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xji.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://twe.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jbs.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oun.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://umv.zycfv.cn


<!-- 参考信息 -->