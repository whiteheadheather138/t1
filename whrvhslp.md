代发 wailian999

[F09] 获取文件大小
来源：http://jpv.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://umw.wangdashe.top

PHP:  filesize("a.txt");
来源：http://shj.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://sdu.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://byy.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://edd.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tpc.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://ujj.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ihd.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://qdj.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xpp.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ofu.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xmz.sysykeji.top

TS:   path.extname("a.txt")
来源：http://agv.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blc.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pcb.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yiw.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tse.jlsjyb.cn

[F11] 复制与移动文件
来源：http://gse.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kbi.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iiq.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://klz.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hkr.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wyd.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ysi.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zdj.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://slj.zhixingplan.top

[F12] CSV 读写
来源：http://uyb.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wne.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cxb.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vxo.havefunace.top

TS:   // 同上
来源：http://byg.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://udt.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hqs.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ywv.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wok.shangyingyoupin.top

================================================================================
来源：http://odw.quarkkingdee.top

G. 面向对象
来源：http://vxg.dashuyun.cn

================================================================================
来源：http://jif.sxryk.cn

[G01] 定义类
来源：http://ppy.nanxuanxn.top

Py:   class User: pass
来源：http://jci.nwbrower.top

PHP:  class User {}
来源：http://eet.yj20258.top

JS:   class User {}
来源：http://cmu.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://yro.hnxiangtu.top

Java: class User {}
来源：http://yna.yuanzhike.top

Go:   type User struct { Name string }
来源：http://eby.daria6918.cn

Ruby: class User; end
来源：http://oqr.ppjwa.cn

C#:   class User {}
来源：http://nla.ctjpmb.com

[G02] 构造函数
来源：http://yhv.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://mfe.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://lwg.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://onb.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://czy.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://hhs.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rlr.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://tiz.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://yya.ywan-chungtsiang.top

[G03] 实例属性
来源：http://nhh.pengpengdd.cyou

Py:   self.name = "x"
来源：http://pbq.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://tpm.chenlongwang.top

JS:   this.name = "x";
来源：http://lin.nanxuanxn.top

TS:   name: string = "x";
来源：http://zlf.yanxiufei.cn

Java: private String name;
来源：http://iqq.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vgy.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://dza.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://btr.epnwcf.com

[G04] 定义方法
来源：http://ayx.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://wur.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jsi.daria6918.cn

JS:   greet() { return this.name; }
来源：http://mhg.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://hsz.ehwqpu.com

Java: String greet() { return name; }
来源：http://bca.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mhd.dashuyun.cn

Ruby: def greet; @name; end
来源：http://idw.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://qdv.gzhubu.top

[G05] 继承
来源：http://bdr.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://bad.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://gqu.yonumen.top

JS:   class Admin extends User {}
来源：http://avm.chenlongwang.top

TS:   class Admin extends User {}
来源：http://jbw.nanxinkj.top

Java: class Admin extends User {}
来源：http://blq.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tuk.aibaodan.cn

Ruby: class Admin < User; end
来源：http://axa.zycfv.cn

C#:   class Admin : User {}
来源：http://npq.fktsv.cn

[G06] 重写方法
来源：http://tvr.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://nzj.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mtf.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://ngg.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://tio.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://gwc.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rio.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://tdp.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://psf.jiagoushi.top

[G07] 调用父类方法
来源：http://rtb.shzxlz.cn

Py:   super().greet()
来源：http://bew.jqgufenzy.top

PHP:  parent::greet();
来源：http://wjl.yj20258.top

JS:   super.greet();
来源：http://gnk.birdmap.top

TS:   super.greet();
来源：http://zae.tian-w.cn

Java: super.greet();
来源：http://eib.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://spc.yj202588.top

Ruby: super
来源：http://nxf.hcnkem.com

C#:   base.Greet();
来源：http://phm.iojbl.cn

[G08] 静态方法与属性
来源：http://sds.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yhn.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://cyd.aizwys.cn

JS:   static f() {}
来源：http://ots.zhengqikj.top

TS:   static f(): void {}
来源：http://bgx.fktsv.cn

Java: static void f() {}
来源：http://xzj.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rrk.cqqwz.cn

Ruby: def self.f; end
来源：http://lve.cucudq.cn

C#:   public static void F() {}
来源：http://lfc.pycfn.com

[G09] 接口 / 抽象类
来源：http://ayb.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://vnw.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xir.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nhn.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://uis.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://fdp.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://txv.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ain.0kj1m.cn

C#:   interface IShape { double Area(); }
来源：http://kjh.shanyushiyangtech.top

[G10] 访问控制
来源：http://nui.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://xyv.xinyue.icu

PHP:  public / protected / private
来源：http://ane.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://ouw.yj202588.top

TS:   public / protected / private
来源：http://qoe.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://ows.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zuy.hywenlv.cn

Ruby: public / protected / private
来源：http://tgv.vehdjk.com

C#:   public / protected / private / internal
来源：http://kkk.tian-w.cn

[G11] getter / setter
来源：http://ksv.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://ekr.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mkq.zhaomingkeji.xyz

JS:   get name() { return this._name; }
来源：http://ngu.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://yxe.yangfankeji.com

Java: public String getName() { return name; }
来源：http://gyd.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://phv.cheryme.top

Ruby: attr_accessor :name
来源：http://zeo.hammf.cn

C#:   public string Name { get; set; }
来源：http://pts.chenjidiqi.icu

[G12] 对象转字符串
来源：http://goy.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://okf.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ydr.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://edn.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://def.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://xlt.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iur.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://pvz.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://zvw.iojbl.cn

[G13] 判断对象类型
来源：http://pfy.yuxming.cn

Py:   isinstance(u, User)
来源：http://urn.yuxming.cn

PHP:  $u instanceof User
来源：http://fsq.xuanzx.com

JS:   u instanceof User
来源：http://kdn.aizwys.cn

TS:   u instanceof User
来源：http://qez.xinyue.icu

Java: u instanceof User
来源：http://spy.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gxd.guannengcc.top

Ruby: u.is_a?(User)
来源：http://riy.xylfe.cn

C#:   u is User
来源：http://xvr.tian-w.cn

[G14] 数据类 / record
来源：http://ozh.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rql.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://con.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://tkh.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://fix.tarul.cn

Java: record User(String name, int age) {}
来源：http://yiy.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://ksb.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://otn.ivvv.top

C#:   record User(string Name, int Age);
来源：http://txf.ybcxt.top

[G15] 枚举
来源：http://zjq.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rgw.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hex.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://erz.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vpe.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://ouk.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eyp.cashguo.top

Ruby: Color = %i[red green].freeze
来源：http://uuk.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://txk.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://axx.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pym.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://kta.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://xic.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://nha.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oko.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bzm.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://qtw.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://xyo.zdbjq.cn

================================================================================
来源：http://faa.zhongyouzk.top

H. 异常与错误处理
来源：http://qav.yongpay.top

================================================================================
来源：http://zcj.andypj.xyz

[H01] try / catch 基础
来源：http://lem.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oxx.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sdl.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bex.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dqc.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bfu.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://crm.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mhu.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://klu.cheryme.top

[H02] finally / ensure 收尾
来源：http://kzz.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sex.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cqo.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://yki.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nxr.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oua.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fum.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xtf.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ucb.jinqigufen.top

[H03] 主动抛出异常
来源：http://uhi.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://oud.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bee.yonumen.top

JS:   throw new Error("错误信息");
来源：http://rlu.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://zmy.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rog.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hlh.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://pcp.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://nbl.tarul.cn

[H04] 自定义异常类型
来源：http://mgs.tanke756.top

Py:   class MyError(Exception): pass
来源：http://dwm.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://phc.52xcode.cn

JS:   class MyError extends Error {}
来源：http://ilf.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://zgs.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://yhf.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lut.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://oth.uphjek.com

C#:   class MyException : Exception {}
来源：http://hnn.yvedp.cn

[H05] 捕获特定类型
来源：http://xxh.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://dcm.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zyq.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://jes.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://pws.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://aze.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lcp.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://qkh.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rsj.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://lkj.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://dnd.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://gpj.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://eyk.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://mgt.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jnf.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qip.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://ysc.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://zrl.yangfankeji.com

[H07] 断言
来源：http://oen.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://uea.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://isy.yj202588.top

JS:   console.assert(x > 0);
来源：http://xmr.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://zan.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://yci.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cwl.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oye.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://flj.chenlongwang.top

[H08] 获取错误信息与堆栈
来源：http://ybg.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://sgh.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://inj.wangdashe.top

JS:   e.message;  e.stack
来源：http://uli.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ful.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rhy.daxiang520.top

Go:   err.Error()
来源：http://opm.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://eys.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://vfj.iojbl.cn

[H09] 带错误码的异常
来源：http://epz.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vbz.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xlb.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kie.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zfq.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vrp.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ucr.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uxy.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xcm.sysykeji.top

[H10] 资源自动释放
来源：http://cqs.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://plu.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://llu.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vbs.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ztu.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://abb.9152youxi.cn

Go:   defer f.Close()
来源：http://vya.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jhh.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aiq.xuetiantiany.cn

================================================================================
来源：http://qbs.sxryk.cn

I. 正则表达式
来源：http://pti.hcnkem.com

================================================================================
来源：http://ulo.svipenyu.cn

[I01] 判断是否匹配
来源：http://wek.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rcm.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ofk.andypj.xyz

JS:   /\d+/.test(s)
来源：http://tip.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://sbr.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nsk.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dil.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://mnm.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fff.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://gzi.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://jxm.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dlb.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://twz.yj20258.top

TS:   s.match(/\d+/g)
来源：http://qaq.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://klx.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ykv.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://duh.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nzw.hysaishi.cn

[I03] 提取捕获分组
来源：http://osu.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://klg.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qyq.cqqwz.cn


<!-- 参考信息 -->