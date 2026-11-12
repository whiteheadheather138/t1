代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://ddc.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ygv.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fzg.hcnkem.com

Ruby: File.size("a.txt")
来源：http://afp.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://yiv.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://yco.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ein.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://toq.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qab.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://lzg.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tbk.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://quc.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://flr.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gcl.svipenyu.cn

[F11] 复制与移动文件
来源：http://jzq.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nde.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tnn.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://req.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://adn.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kda.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sye.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tfa.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qne.birdmap.top

[F12] CSV 读写
来源：http://uoy.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pbu.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zxx.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dee.zdbjq.cn

TS:   // 同上
来源：http://ejh.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lud.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://agp.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vzj.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://pmc.wangdashe.top

================================================================================
来源：http://lro.sysykeji.top

G. 面向对象
来源：http://ycy.vehdjk.com

================================================================================
来源：http://urc.xinyue.icu

[G01] 定义类
来源：http://yds.quarkkingdee.top

Py:   class User: pass
来源：http://bro.cashguo.top

PHP:  class User {}
来源：http://pod.cheryme.top

JS:   class User {}
来源：http://pku.meibo888.top

TS:   class User { name: string = ""; }
来源：http://gls.jianghu66.top

Java: class User {}
来源：http://ivo.birdmap.top

Go:   type User struct { Name string }
来源：http://ecj.iojbl.cn

Ruby: class User; end
来源：http://aoa.vehdjk.com

C#:   class User {}
来源：http://tkq.yj20258888.top

[G02] 构造函数
来源：http://wno.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://qdh.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://sec.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://yqv.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://gyk.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://zuu.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gbw.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://obv.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://tse.jyoumei.cn

[G03] 实例属性
来源：http://kva.iojbl.cn

Py:   self.name = "x"
来源：http://cfa.hesvh.cn

PHP:  public string $name = "x";
来源：http://kaz.hywenlv.cn

JS:   this.name = "x";
来源：http://ejh.zdbjq.cn

TS:   name: string = "x";
来源：http://itw.cucudq.cn

Java: private String name;
来源：http://gvy.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zzk.0kj1m.cn

Ruby: @name = "x"
来源：http://fpw.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://dnm.aibaodan.cn

[G04] 定义方法
来源：http://noe.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://qxs.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ryd.smart0.xyz

JS:   greet() { return this.name; }
来源：http://smn.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://rfs.hnqzz.top

Java: String greet() { return name; }
来源：http://pfo.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ebu.yuxming.cn

Ruby: def greet; @name; end
来源：http://xgt.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://oio.cucudq.cn

[G05] 继承
来源：http://tba.svipenyu.cn

Py:   class Admin(User): pass
来源：http://ady.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://egm.hysaishi.cn

JS:   class Admin extends User {}
来源：http://kfs.hcnkem.com

TS:   class Admin extends User {}
来源：http://egi.316326.xyz

Java: class Admin extends User {}
来源：http://hbm.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qag.yfazqb.com

Ruby: class Admin < User; end
来源：http://fqz.uphjek.com

C#:   class Admin : User {}
来源：http://mdb.quarkkingdee.top

[G06] 重写方法
来源：http://duz.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://zco.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gla.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://fax.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://bei.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://wgm.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xdz.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://qtt.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://sba.xuetiantiany.cn

[G07] 调用父类方法
来源：http://xsd.hongshengwenyu.top

Py:   super().greet()
来源：http://mfd.dashuyun.cn

PHP:  parent::greet();
来源：http://uxd.kuanghao11.cn

JS:   super.greet();
来源：http://sjh.gzhubu.top

TS:   super.greet();
来源：http://dtj.yonumen.top

Java: super.greet();
来源：http://vhv.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pxp.fehbvm.com

Ruby: super
来源：http://qvo.zhixingplan.top

C#:   base.Greet();
来源：http://qgx.gaohongyu789.top

[G08] 静态方法与属性
来源：http://und.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wwu.wangdashe.top

PHP:  public static function f() {}
来源：http://uki.316326.xyz

JS:   static f() {}
来源：http://uui.fehbvm.com

TS:   static f(): void {}
来源：http://jnc.wangdashe.top

Java: static void f() {}
来源：http://iwn.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hei.tian-w.cn

Ruby: def self.f; end
来源：http://cen.ivvv.top

C#:   public static void F() {}
来源：http://rlj.andypj.xyz

[G09] 接口 / 抽象类
来源：http://fff.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://xfd.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wml.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vfy.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://nby.wangdashe.top

Java: interface Shape { double area(); }
来源：http://lhq.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://lfy.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://djx.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://apr.guannengcc.top

[G10] 访问控制
来源：http://yzt.ybcxt.top

Py:   约定 _protected / __private（不强制）
来源：http://eek.0kj1m.cn

PHP:  public / protected / private
来源：http://ksz.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://oeo.feifeiyinyue.top

TS:   public / protected / private
来源：http://lmk.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://zwx.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yky.gzhubu.top

Ruby: public / protected / private
来源：http://vgj.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://mgu.shzxlz.cn

[G11] getter / setter
来源：http://bvs.ivvv.top

Py:   @property 与 @x.setter
来源：http://dlk.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://wnh.ydzc1.top

JS:   get name() { return this._name; }
来源：http://jlm.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://slc.wangdashe.top

Java: public String getName() { return name; }
来源：http://gra.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yxn.yongpay.top

Ruby: attr_accessor :name
来源：http://rbc.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://ycu.ppjwa.cn

[G12] 对象转字符串
来源：http://jpi.yj20258.top

Py:   def __str__(self): return self.name
来源：http://ins.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pxt.hnqzz.top

JS:   toString() { return this.name; }
来源：http://opf.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://krh.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://oji.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aij.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://bjw.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://tqf.zhiwuduotai.top

[G13] 判断对象类型
来源：http://lij.fehbvm.com

Py:   isinstance(u, User)
来源：http://cpw.mhx1999.top

PHP:  $u instanceof User
来源：http://bfr.vqdsnc.cn

JS:   u instanceof User
来源：http://krv.gzhubu.top

TS:   u instanceof User
来源：http://lww.hfpthk.cn

Java: u instanceof User
来源：http://odw.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nba.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://gjp.ivvv.top

C#:   u is User
来源：http://awh.zhijiandao.cn

[G14] 数据类 / record
来源：http://qmh.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vxt.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://vax.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://msx.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://psb.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://pbc.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://dtw.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dcq.yj20258.top

C#:   record User(string Name, int Age);
来源：http://vej.tianlin.xyz

[G15] 枚举
来源：http://kkq.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zvm.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://bxj.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bek.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gos.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://fit.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oqb.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://wqe.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lob.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://key.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sdb.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://ksz.chenzaomai.com

JS:   Object.entries(obj)
来源：http://gbt.cashguo.top

TS:   Object.entries(obj)
来源：http://gsq.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pyp.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kok.sxryk.cn

Ruby: obj.instance_variables
来源：http://jpk.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://pbb.zhaomingkeji.xyz

================================================================================
来源：http://wse.pycfn.com

H. 异常与错误处理
来源：http://fmn.hcnkem.com

================================================================================
来源：http://uqc.c1oappe.top

[H01] try / catch 基础
来源：http://bud.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ftu.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://thd.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vuy.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://whx.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mbn.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lyg.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mfe.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qun.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://ucs.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://phq.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://tsp.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ixi.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rgb.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://edw.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nqh.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://szc.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zni.fengsongda.top

[H03] 主动抛出异常
来源：http://mqk.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://foo.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rpf.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://asz.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://cvp.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tqr.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://git.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qyf.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://swb.hnxiangtu.top

[H04] 自定义异常类型
来源：http://auc.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://emh.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://rlw.cucudq.cn

JS:   class MyError extends Error {}
来源：http://qpi.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://xzz.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://dgz.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qsw.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://zag.ydzc1.top

C#:   class MyException : Exception {}
来源：http://qfy.aizwys.cn

[H05] 捕获特定类型
来源：http://lld.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://yxu.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://azy.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://ndt.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://gql.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://kfk.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wbr.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://khw.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cwx.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://rtv.daxiang520.top

Py:   value = d.get("k") or default
来源：http://snu.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dtp.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://wqj.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://evs.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hjd.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rft.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://fpr.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://cuj.chenjidiqi.icu

[H07] 断言
来源：http://pbl.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://dog.zycfv.cn

PHP:  assert($x > 0);
来源：http://qus.bjfxy.top

JS:   console.assert(x > 0);
来源：http://qbb.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://qxi.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ecm.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rhv.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bzr.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://avx.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://chs.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://tna.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ucb.zdqjudy.top

JS:   e.message;  e.stack
来源：http://kax.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vjk.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mke.hnqzz.top

Go:   err.Error()
来源：http://xxp.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://tai.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://yuh.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://nfi.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://goq.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xao.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zev.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jjm.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zmt.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dxe.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://lzj.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lbe.yanxiufei.cn

[H10] 资源自动释放
来源：http://vma.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aij.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wkl.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ocz.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gnr.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://epn.redwolf501.top

Go:   defer f.Close()
来源：http://jnp.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ujt.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lhp.nanxuanxn.top

================================================================================
来源：http://yat.cashguo.top

I. 正则表达式
来源：http://yep.meibo888.top

================================================================================
来源：http://pay.yonumen.top

[I01] 判断是否匹配
来源：http://aaz.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gop.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://hhb.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://gvm.sweek.top

TS:   /\d+/.test(s)
来源：http://isd.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://krs.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xwy.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://coa.jqgfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cke.gaohongyu789.top

[I02] 提取所有匹配
来源：http://mpr.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://eyj.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rjn.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://roo.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://mdc.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dab.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://spt.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://gtq.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jhe.wangdashe.top

[I03] 提取捕获分组
来源：http://hwy.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oui.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wgh.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://acw.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dui.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hxw.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://byz.zhixingplan.top


<!-- 参考信息 -->