代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://mds.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fth.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://inb.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://gfy.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://zfa.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://ihf.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xwd.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xcn.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rur.shuidangran.top

TS:   path.extname("a.txt")
来源：http://ryz.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ywk.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://azd.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hqo.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hjh.yj20258.top

[F11] 复制与移动文件
来源：http://bok.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oih.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqs.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqg.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkn.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://epb.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vkg.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fed.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nso.cqqwz.cn

[F12] CSV 读写
来源：http://bcf.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xto.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zmj.jianghu66.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qjh.cdnleiting.top

TS:   // 同上
来源：http://arl.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mbt.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://grw.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pwk.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ihn.hcnkem.com

================================================================================
来源：http://xvb.c1oappe.top

G. 面向对象
来源：http://cqk.sweek.top

================================================================================
来源：http://dkf.yuxming.cn

[G01] 定义类
来源：http://alq.yfazqb.com

Py:   class User: pass
来源：http://vki.hammf.cn

PHP:  class User {}
来源：http://vup.vqdsnc.cn

JS:   class User {}
来源：http://nzj.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://rat.fzhhl.top

Java: class User {}
来源：http://fvg.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://qlh.hammf.cn

Ruby: class User; end
来源：http://ecq.fehbvm.com

C#:   class User {}
来源：http://xyc.zycfv.cn

[G02] 构造函数
来源：http://qgn.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://cqh.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://gwk.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://xns.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://wgn.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://yui.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kzy.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://gri.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://hop.ydzc1.top

[G03] 实例属性
来源：http://mqr.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://zbn.sufxvd.cn

PHP:  public string $name = "x";
来源：http://mfr.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://lsr.hfpthk.cn

TS:   name: string = "x";
来源：http://pkh.chenjidiqi.icu

Java: private String name;
来源：http://hss.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://owv.ppjwa.cn

Ruby: @name = "x"
来源：http://duo.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://pdv.zhixingplan.top

[G04] 定义方法
来源：http://bzp.bbcook.cn

Py:   def greet(self): return self.name
来源：http://rla.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bqy.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://ngy.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://iug.tianlin.xyz

Java: String greet() { return name; }
来源：http://hns.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mal.hfpthk.cn

Ruby: def greet; @name; end
来源：http://kyr.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://rgl.ppjwa.cn

[G05] 继承
来源：http://brx.hesvh.cn

Py:   class Admin(User): pass
来源：http://tfs.vehdjk.com

PHP:  class Admin extends User {}
来源：http://knb.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://nfs.fktsv.cn

TS:   class Admin extends User {}
来源：http://ttp.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://hxx.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yxp.dashuyun.cn

Ruby: class Admin < User; end
来源：http://umk.yangfankeji.com

C#:   class Admin : User {}
来源：http://nfu.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://tcz.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://hsx.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hfn.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://mib.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://zqf.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://zxg.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dmw.yj202588.top

Ruby: def greet; "admin"; end
来源：http://feu.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://mel.c1oappe.top

[G07] 调用父类方法
来源：http://xzn.yfazqb.com

Py:   super().greet()
来源：http://nhu.cucudq.cn

PHP:  parent::greet();
来源：http://adw.uphjek.com

JS:   super.greet();
来源：http://wxl.ydzc1.top

TS:   super.greet();
来源：http://ezp.zhijiandao.cn

Java: super.greet();
来源：http://azc.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wci.nanxuanxn.top

Ruby: super
来源：http://yac.zdqjudy.top

C#:   base.Greet();
来源：http://lwq.vqdsnc.cn

[G08] 静态方法与属性
来源：http://yxz.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eqe.sweek.top

PHP:  public static function f() {}
来源：http://aaa.zhixingplan.top

JS:   static f() {}
来源：http://cbt.ehwqpu.com

TS:   static f(): void {}
来源：http://itv.mhx1999.top

Java: static void f() {}
来源：http://ptt.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iix.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://qpe.sufxvd.cn

C#:   public static void F() {}
来源：http://dwg.xziqi.cn

[G09] 接口 / 抽象类
来源：http://zjy.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://pja.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ftz.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ors.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://pcv.xylfe.cn

Java: interface Shape { double area(); }
来源：http://qil.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ner.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vab.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://gxw.xylfe.cn

[G10] 访问控制
来源：http://xhx.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://teh.pengpengdd.cyou

PHP:  public / protected / private
来源：http://buz.uphjek.com

JS:   #private 字段；其余公开
来源：http://nlv.redwolf501.top

TS:   public / protected / private
来源：http://apo.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://dvv.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yow.sufxvd.cn

Ruby: public / protected / private
来源：http://xnk.gogol.net.cn

C#:   public / protected / private / internal
来源：http://qpr.cdnleiting.top

[G11] getter / setter
来源：http://qml.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://obp.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xhp.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://nvk.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://tbs.ctjpmb.com

Java: public String getName() { return name; }
来源：http://qoz.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dud.aibaodan.cn

Ruby: attr_accessor :name
来源：http://vay.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://wca.tianlin.xyz

[G12] 对象转字符串
来源：http://ndz.yj20258.top

Py:   def __str__(self): return self.name
来源：http://asb.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aev.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://ekg.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://wpn.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://olm.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://bhw.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://sne.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://oqz.yuanzhike.top

[G13] 判断对象类型
来源：http://yac.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://icw.fehbvm.com

PHP:  $u instanceof User
来源：http://ssu.yvedp.cn

JS:   u instanceof User
来源：http://nzc.mhx1999.top

TS:   u instanceof User
来源：http://jxf.316326.xyz

Java: u instanceof User
来源：http://ktw.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://qhg.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://dnn.havefunace.top

C#:   u is User
来源：http://fiv.jiagoushi.top

[G14] 数据类 / record
来源：http://iqj.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zcy.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://rzh.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://nut.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://uhc.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://umj.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://fex.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kdk.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://ljx.wangshuangyany.cn

[G15] 枚举
来源：http://lth.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hqu.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vtn.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://evr.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://brv.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://dxo.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nez.cashguo.top

Ruby: Color = %i[red green].freeze
来源：http://hxe.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qrj.havefunace.top

[G16] 对象转数组 / 字典
来源：http://czm.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xim.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://fsn.aizwys.cn

JS:   Object.entries(obj)
来源：http://ikc.jqgfzy.top

TS:   Object.entries(obj)
来源：http://fce.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xvy.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iyj.yueranfly.top

Ruby: obj.instance_variables
来源：http://vvv.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://vxy.xuanzx.com

================================================================================
来源：http://uhr.shangyingyoupin.top

H. 异常与错误处理
来源：http://vwm.wangdashe.top

================================================================================
来源：http://xst.svipenyu.cn

[H01] try / catch 基础
来源：http://qkw.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xzq.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vjb.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://puk.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://txm.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://imx.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rce.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://min.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xor.52xcode.cn

[H02] finally / ensure 收尾
来源：http://jme.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://fhw.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://irp.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qvd.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vqn.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wsq.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oda.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yvk.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oow.chenlongwang.top

[H03] 主动抛出异常
来源：http://afv.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://ywz.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rta.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://zgk.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://zfo.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bfg.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nxk.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://agx.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zuc.yuanzhike.top

[H04] 自定义异常类型
来源：http://mpj.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://qgv.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://kpp.meibo888.top

JS:   class MyError extends Error {}
来源：http://rhn.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://bvs.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://cxq.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iua.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://gis.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://xua.yfazqb.com

[H05] 捕获特定类型
来源：http://jne.zycfv.cn

Py:   except ValueError as e:
来源：http://vrx.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aiq.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://hxc.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://ifo.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://hrl.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tpx.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://rsh.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oix.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://uoe.epnwcf.com

Py:   value = d.get("k") or default
来源：http://xht.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://dye.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://gvz.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lpt.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://snx.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aku.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://xom.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://xlr.fehbvm.com

[H07] 断言
来源：http://yuu.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://grf.tianlin.xyz

PHP:  assert($x > 0);
来源：http://eoz.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://mlj.nwbrower.top

TS:   console.assert(x > 0);
来源：http://sov.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://nju.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hfb.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://pzf.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://bvn.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://mbn.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://ewm.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ewy.shuidangran.top

JS:   e.message;  e.stack
来源：http://jsl.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iaa.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qtu.tian-w.cn

Go:   err.Error()
来源：http://sfb.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://mom.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://jlj.nanxinkj.top

[H09] 带错误码的异常
来源：http://wov.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://djx.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lxp.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vrv.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xmr.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ilv.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aus.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://aus.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gds.svipenyu.cn

[H10] 资源自动释放
来源：http://lfb.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://piz.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nzq.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tem.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wrh.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qgs.yj202588.top

Go:   defer f.Close()
来源：http://unp.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jue.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://edl.xinyue.icu

================================================================================
来源：http://fkg.daxiang520.top

I. 正则表达式
来源：http://pij.yfazqb.com

================================================================================
来源：http://jyd.yonumen.top

[I01] 判断是否匹配
来源：http://nxm.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jaz.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vai.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://igh.guannengcc.top

TS:   /\d+/.test(s)
来源：http://soz.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://syg.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vuw.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://ehr.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dom.ivvv.top

[I02] 提取所有匹配
来源：http://aho.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://cmt.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dzo.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://axd.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://syx.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mjw.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pbv.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://idf.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nnf.snrcjt.cn

[I03] 提取捕获分组
来源：http://dfn.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xzb.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pul.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tng.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bsq.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tqc.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wxk.jlsjyb.cn


<!-- 参考信息 -->