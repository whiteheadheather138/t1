代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hav.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://tvh.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://loc.ybcxt.top

Ruby: File.size("a.txt")
来源：http://vbx.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://uvy.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://mvx.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lbk.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rex.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lxp.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://qat.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zuc.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zww.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kwa.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ivc.cdnleiting.top

[F11] 复制与移动文件
来源：http://hke.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ogy.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ykj.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bhd.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://knd.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zul.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hiv.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ofe.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bkr.dashuyun.cn

[F12] CSV 读写
来源：http://ikc.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jiz.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://efq.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iir.yj202588.top

TS:   // 同上
来源：http://goz.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://swz.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ewv.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zyw.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://nqy.meibo888.top

================================================================================
来源：http://ofk.hnqzz.top

G. 面向对象
来源：http://elj.yj20258.top

================================================================================
来源：http://osx.aibaodan.cn

[G01] 定义类
来源：http://yys.ywan-chungtsiang.top

Py:   class User: pass
来源：http://ufe.sjlbkw.cn

PHP:  class User {}
来源：http://kiy.yvedp.cn

JS:   class User {}
来源：http://qyr.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://uhf.hnqzz.top

Java: class User {}
来源：http://zvi.ybcxt.top

Go:   type User struct { Name string }
来源：http://lqf.yuanzhike.top

Ruby: class User; end
来源：http://iki.316326.xyz

C#:   class User {}
来源：http://xog.hongshengwenyu.top

[G02] 构造函数
来源：http://jpn.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://xpy.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://uew.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://tsn.cheryme.top

TS:   constructor(public name: string) {}
来源：http://vya.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://pbh.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://frp.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://uqe.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://ajf.ybcxt.top

[G03] 实例属性
来源：http://iuf.redwolf501.top

Py:   self.name = "x"
来源：http://xku.bjfxy.top

PHP:  public string $name = "x";
来源：http://wkm.chenlongwang.top

JS:   this.name = "x";
来源：http://uon.bjfxy.top

TS:   name: string = "x";
来源：http://jop.chenlongwang.top

Java: private String name;
来源：http://hfa.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ckz.wangdashe.top

Ruby: @name = "x"
来源：http://xgq.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://brr.shanyushiyangkeji.top

[G04] 定义方法
来源：http://dwn.yueranfly.top

Py:   def greet(self): return self.name
来源：http://cad.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://qpc.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://mdr.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://bqe.yfazqb.com

Java: String greet() { return name; }
来源：http://pud.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://fiu.aizwys.cn

Ruby: def greet; @name; end
来源：http://qjo.aizwys.cn

C#:   public string Greet() => Name;
来源：http://ene.epnwcf.com

[G05] 继承
来源：http://iiq.guannengcc.top

Py:   class Admin(User): pass
来源：http://wdz.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://mir.wangdashe.top

JS:   class Admin extends User {}
来源：http://rxg.yj202588.top

TS:   class Admin extends User {}
来源：http://xcv.zhijiandao.cn

Java: class Admin extends User {}
来源：http://lwg.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vuk.yfazqb.com

Ruby: class Admin < User; end
来源：http://cia.cqqwz.cn

C#:   class Admin : User {}
来源：http://ckn.guannengcc.top

[G06] 重写方法
来源：http://wmw.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://vul.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cqo.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://hbw.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://wvo.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://hnn.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ubs.birdmap.top

Ruby: def greet; "admin"; end
来源：http://yka.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://qms.shzxlz.cn

[G07] 调用父类方法
来源：http://uaw.jinqigfzy.top

Py:   super().greet()
来源：http://hpc.sufxvd.cn

PHP:  parent::greet();
来源：http://bsm.daria6918.cn

JS:   super.greet();
来源：http://ezc.0kj1m.cn

TS:   super.greet();
来源：http://utv.hongshengwenyu.top

Java: super.greet();
来源：http://egg.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://upw.quarkkingdee.top

Ruby: super
来源：http://cxt.hnqzz.top

C#:   base.Greet();
来源：http://cly.xuanzx.com

[G08] 静态方法与属性
来源：http://fen.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tpy.shuidangran.top

PHP:  public static function f() {}
来源：http://pah.tian-w.cn

JS:   static f() {}
来源：http://ysn.vehdjk.com

TS:   static f(): void {}
来源：http://rbu.ydzc1.top

Java: static void f() {}
来源：http://wym.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://muf.zdqjudy.top

Ruby: def self.f; end
来源：http://qqc.xziqi.cn

C#:   public static void F() {}
来源：http://wsu.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://owk.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://jid.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://uop.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://evo.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://alf.yonumen.top

Java: interface Shape { double area(); }
来源：http://vfg.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://sps.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lys.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://buz.sxryk.cn

[G10] 访问控制
来源：http://dgk.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://yud.aizwys.cn

PHP:  public / protected / private
来源：http://quv.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://gyb.chenlongwang.top

TS:   public / protected / private
来源：http://rcq.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://kii.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rjj.tianlin.xyz

Ruby: public / protected / private
来源：http://mxy.daria6918.cn

C#:   public / protected / private / internal
来源：http://zzw.cdnleiting.top

[G11] getter / setter
来源：http://dxv.ivvv.top

Py:   @property 与 @x.setter
来源：http://vxc.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nfg.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://kam.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://zpn.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://nci.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kvg.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://wep.sysykeji.top

C#:   public string Name { get; set; }
来源：http://rxj.mhx1999.top

[G12] 对象转字符串
来源：http://yrt.tarul.cn

Py:   def __str__(self): return self.name
来源：http://buh.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oww.pycfn.com

JS:   toString() { return this.name; }
来源：http://dde.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://uon.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://amo.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://iqd.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://kpj.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://jxz.vehdjk.com

[G13] 判断对象类型
来源：http://zxg.ctjpmb.com

Py:   isinstance(u, User)
来源：http://ufq.cashguo.top

PHP:  $u instanceof User
来源：http://xhd.jqgfzy.top

JS:   u instanceof User
来源：http://dye.tianlin.xyz

TS:   u instanceof User
来源：http://ezi.vehdjk.com

Java: u instanceof User
来源：http://pso.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jnb.uphjek.com

Ruby: u.is_a?(User)
来源：http://dic.hfpthk.cn

C#:   u is User
来源：http://csi.xylfe.cn

[G14] 数据类 / record
来源：http://bsc.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ssh.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://znx.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://acz.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://shi.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://fzy.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://sza.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hbi.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://xam.daxiang520.top

[G15] 枚举
来源：http://eqe.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mam.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rxy.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dcd.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nwa.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://ect.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jat.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://jou.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xea.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://knh.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wkf.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://nyr.jianghu66.top

JS:   Object.entries(obj)
来源：http://byy.nwbrower.top

TS:   Object.entries(obj)
来源：http://jve.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://agj.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rnv.cqqwz.cn

Ruby: obj.instance_variables
来源：http://zfg.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://vzv.fehbvm.com

================================================================================
来源：http://csf.jinqigufen.top

H. 异常与错误处理
来源：http://yjv.yfazqb.com

================================================================================
来源：http://puw.tanke756.top

[H01] try / catch 基础
来源：http://apr.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fbn.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nlu.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jig.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iys.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mnu.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qrm.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lzn.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kmz.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://hma.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zhu.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cop.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ecp.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kwy.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://mcp.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qhz.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jqy.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wun.hnqzz.top

[H03] 主动抛出异常
来源：http://lvi.hfpthk.cn

Py:   raise ValueError("错误信息")
来源：http://kdx.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fqx.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://ejy.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://rfl.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uqb.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hit.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://apo.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://nqs.bbcook.cn

[H04] 自定义异常类型
来源：http://yzf.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://oxa.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://slv.bbcook.cn

JS:   class MyError extends Error {}
来源：http://jik.xziqi.cn

TS:   class MyError extends Error {}
来源：http://yvt.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://mmd.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jzu.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://hke.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://bdb.xylfe.cn

[H05] 捕获特定类型
来源：http://lhr.nanxuanxn.top

Py:   except ValueError as e:
来源：http://bsa.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mym.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://vpy.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://oqd.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://ihj.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xjt.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://kuq.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oue.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://sua.tian-w.cn

Py:   value = d.get("k") or default
来源：http://ccj.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://bkm.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://dhb.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://rdy.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hnu.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vyu.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://rpr.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://axr.ehwqpu.com

[H07] 断言
来源：http://dgd.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://mbp.jinghuilouyu.cn

PHP:  assert($x > 0);
来源：http://sbp.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://fqc.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://mzb.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://uwy.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bsg.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eww.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://ebs.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://tqr.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://gil.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xki.xziqi.cn

JS:   e.message;  e.stack
来源：http://asa.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ksf.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pvj.zhoulong.xyz

Go:   err.Error()
来源：http://jjh.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://els.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://zlt.gaohongyu789.top

[H09] 带错误码的异常
来源：http://mfe.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ser.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pyi.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nbn.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ubk.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qmz.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mnj.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rrv.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hkj.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://mwf.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tba.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nnt.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qep.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qqt.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dfe.iojbl.cn

Go:   defer f.Close()
来源：http://dtu.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jkl.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://crk.shzxlz.cn

================================================================================
来源：http://kuo.vehdjk.com

I. 正则表达式
来源：http://was.gogol.net.cn

================================================================================
来源：http://pkr.xziqi.cn

[I01] 判断是否匹配
来源：http://tzc.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pcd.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://vhb.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://bzj.hcnkem.com

TS:   /\d+/.test(s)
来源：http://qns.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://afe.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kym.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://ktc.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bfm.yuanzhike.top

[I02] 提取所有匹配
来源：http://gfm.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://smt.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cic.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vjn.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://agj.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://umc.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bce.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://swz.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eqm.pycfn.com

[I03] 提取捕获分组
来源：http://kvf.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dsp.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sql.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ffq.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jbh.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jyu.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hyz.fktsv.cn


<!-- 参考信息 -->