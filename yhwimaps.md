代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://awr.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://qzw.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hgf.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://paj.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ked.xylfe.cn

TS:   path.extname("a.txt")
来源：http://dxx.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pbb.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lew.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kez.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mfj.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://mdp.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tfa.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ltf.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zim.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vyw.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mik.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tru.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aqg.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oba.gaohongyu789.top

[F12] CSV 读写
来源：http://bql.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://irg.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mlo.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yqd.sxryk.cn

TS:   // 同上
来源：http://rjd.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ckq.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nna.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zpz.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mpl.cucudq.cn

================================================================================
来源：http://aoa.zhijiandao.cn

G. 面向对象
来源：http://ozl.yangfankeji.com

================================================================================
来源：http://ehs.bjfxy.top

[G01] 定义类
来源：http://ylw.zhaomingkeji.xyz

Py:   class User: pass
来源：http://ezw.daria6918.cn

PHP:  class User {}
来源：http://dlc.jianghu66.top

JS:   class User {}
来源：http://sgs.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://fvq.feifeiyinyue.top

Java: class User {}
来源：http://vpd.zhengqikj.top

Go:   type User struct { Name string }
来源：http://nrz.tianlin.xyz

Ruby: class User; end
来源：http://uxd.zhongyouzk.top

C#:   class User {}
来源：http://waj.fktsv.cn

[G02] 构造函数
来源：http://unx.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://uko.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://exs.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://npy.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://ptr.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://wen.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cst.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://jbb.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://the.gzhubu.top

[G03] 实例属性
来源：http://tav.jqgfzy.top

Py:   self.name = "x"
来源：http://uri.daxiang520.top

PHP:  public string $name = "x";
来源：http://uoa.c1oappe.top

JS:   this.name = "x";
来源：http://ekc.ybcxt.top

TS:   name: string = "x";
来源：http://ked.hysaishi.cn

Java: private String name;
来源：http://uph.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ogq.daxiang520.top

Ruby: @name = "x"
来源：http://xqu.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://ums.cqqwz.cn

[G04] 定义方法
来源：http://okm.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://cng.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uzz.zycfv.cn

JS:   greet() { return this.name; }
来源：http://mzu.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://sue.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://yfq.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uqe.ppjwa.cn

Ruby: def greet; @name; end
来源：http://uhy.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://imu.nanxuanxn.top

[G05] 继承
来源：http://dux.meibo888.top

Py:   class Admin(User): pass
来源：http://emf.fengsongda.top

PHP:  class Admin extends User {}
来源：http://swk.zdbjq.cn

JS:   class Admin extends User {}
来源：http://dzz.xinyue.icu

TS:   class Admin extends User {}
来源：http://vct.cheryme.top

Java: class Admin extends User {}
来源：http://vku.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yms.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://hnd.tarul.cn

C#:   class Admin : User {}
来源：http://jan.pengpengdd.cyou

[G06] 重写方法
来源：http://sox.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://spl.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://num.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://kme.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://jgd.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://ocr.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://txg.yongpay.top

Ruby: def greet; "admin"; end
来源：http://zvm.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://ckq.uphjek.com

[G07] 调用父类方法
来源：http://kye.sjlbkw.cn

Py:   super().greet()
来源：http://fnn.yonumen.top

PHP:  parent::greet();
来源：http://ipc.yfazqb.com

JS:   super.greet();
来源：http://lxv.vqdsnc.cn

TS:   super.greet();
来源：http://kam.fengsongda.top

Java: super.greet();
来源：http://uhk.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://odo.havefunace.top

Ruby: super
来源：http://gyp.haohaochexian.top

C#:   base.Greet();
来源：http://grr.aibaodan.cn

[G08] 静态方法与属性
来源：http://ftx.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wvx.xuanzx.com

PHP:  public static function f() {}
来源：http://xrb.dashuyun.cn

JS:   static f() {}
来源：http://tme.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://pha.chenjidiqi.icu

Java: static void f() {}
来源：http://kby.yonumen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jff.hesvh.cn

Ruby: def self.f; end
来源：http://agp.andypj.xyz

C#:   public static void F() {}
来源：http://lok.xylfe.cn

[G09] 接口 / 抽象类
来源：http://lub.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://jny.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kfn.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kil.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://jyn.iojbl.cn

Java: interface Shape { double area(); }
来源：http://csl.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://zae.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nfn.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://soi.jianghu66.top

[G10] 访问控制
来源：http://fhd.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://nkf.snrcjt.cn

PHP:  public / protected / private
来源：http://jcf.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://pdb.nanxinkj.top

TS:   public / protected / private
来源：http://rgu.yj202588.top

Java: public / protected / private / 默认包级
来源：http://gxn.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qsn.aizwys.cn

Ruby: public / protected / private
来源：http://fdu.xuanzx.com

C#:   public / protected / private / internal
来源：http://uxp.dianchejie.cn

[G11] getter / setter
来源：http://lvk.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://gcl.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://npr.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://ido.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://olw.yangfankeji.com

Java: public String getName() { return name; }
来源：http://uem.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://aow.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://tib.sysykeji.top

C#:   public string Name { get; set; }
来源：http://tuv.hnxiangtu.top

[G12] 对象转字符串
来源：http://nrn.tanke756.top

Py:   def __str__(self): return self.name
来源：http://opx.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tcu.uphjek.com

JS:   toString() { return this.name; }
来源：http://gqv.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://ywh.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://udy.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://zez.316326.xyz

Ruby: def to_s; @name; end
来源：http://ios.meibo888.top

C#:   public override string ToString() => Name;
来源：http://ijd.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://kqm.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://hve.gzhubu.top

PHP:  $u instanceof User
来源：http://jql.hammf.cn

JS:   u instanceof User
来源：http://pvt.yueranfly.top

TS:   u instanceof User
来源：http://gzg.jianghu66.top

Java: u instanceof User
来源：http://wpg.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jje.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://jvy.zhoulong.xyz

C#:   u is User
来源：http://avn.fktsv.cn

[G14] 数据类 / record
来源：http://ydi.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nvl.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://zsa.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://rmb.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://mcq.shuidangran.top

Java: record User(String name, int age) {}
来源：http://tqs.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://jxz.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://okb.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://tuy.sxryk.cn

[G15] 枚举
来源：http://egj.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xto.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qcs.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oow.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xss.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://tqw.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://itt.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://lhc.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://evm.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://hsg.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zzd.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://eia.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://mrh.yangfankeji.com

TS:   Object.entries(obj)
来源：http://dal.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rbr.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://moi.hesvh.cn

Ruby: obj.instance_variables
来源：http://che.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://ari.yueranfly.top

================================================================================
来源：http://dmb.bjfxy.top

H. 异常与错误处理
来源：http://neg.yvedp.cn

================================================================================
来源：http://kei.svipenyu.cn

[H01] try / catch 基础
来源：http://gtn.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rig.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pyx.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dhh.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sui.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://exk.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dmj.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dvl.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pdv.hnqzz.top

[H02] finally / ensure 收尾
来源：http://cen.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dwe.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ode.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bug.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://aon.ywan-chungtsiang.top

Java: try { f(); } finally { cleanup(); }
来源：http://aiy.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kho.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://qzt.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yof.ydjk.org.cn

[H03] 主动抛出异常
来源：http://ucw.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://njp.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ucx.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://dun.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://osx.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qoy.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iiu.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hsi.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://znp.aibaodan.cn

[H04] 自定义异常类型
来源：http://zxx.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://iry.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://ajf.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://vek.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://wbs.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://ipd.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rua.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://rxk.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://irf.ehwqpu.com

[H05] 捕获特定类型
来源：http://ylo.bbcook.cn

Py:   except ValueError as e:
来源：http://yfu.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xkb.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://ubj.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://oou.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://jum.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ezo.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://tat.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://prs.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://hna.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://xdu.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://dqr.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://efv.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://amu.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fpe.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yxi.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://jha.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://ysz.yj20258888.top

[H07] 断言
来源：http://dxf.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://ejj.chenzaomai.com

PHP:  assert($x > 0);
来源：http://hyf.iojbl.cn

JS:   console.assert(x > 0);
来源：http://hkg.uphjek.com

TS:   console.assert(x > 0);
来源：http://rnx.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://mts.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://efv.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://xrg.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://ima.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://tcr.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://xmk.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yam.jiagoushi.top

JS:   e.message;  e.stack
来源：http://qiu.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ldw.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xkc.epnwcf.com

Go:   err.Error()
来源：http://egg.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://dfv.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://zpf.zhongyouzk.top

[H09] 带错误码的异常
来源：http://unq.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cgm.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pxb.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cgv.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lpa.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uav.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jfe.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://fmb.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://qir.wangshuangyany.cn

[H10] 资源自动释放
来源：http://jdw.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://iwi.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://veh.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://agq.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mok.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rvx.zycfv.cn

Go:   defer f.Close()
来源：http://drr.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dfh.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tte.yangfankeji.com

================================================================================
来源：http://ife.wangdashe.top

I. 正则表达式
来源：http://bon.0kj1m.cn

================================================================================
来源：http://rix.havefunace.top

[I01] 判断是否匹配
来源：http://obb.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xtf.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://vub.pycfn.com

JS:   /\d+/.test(s)
来源：http://wpe.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://uqf.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oxp.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://okw.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://nyl.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lkx.0kj1m.cn

[I02] 提取所有匹配
来源：http://nry.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://ery.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fsk.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kvh.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://yxs.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://akz.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ips.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://lze.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xst.hysaishi.cn

[I03] 提取捕获分组
来源：http://bry.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mmz.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tvw.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mxf.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qgh.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gdl.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jfm.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fby.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://efh.ybcxt.top

[I04] 正则替换
来源：http://vbd.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jjd.chenlongwang.top


<!-- 参考信息 -->