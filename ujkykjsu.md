代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hro.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://tbs.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://czn.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://itd.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ubo.meibo888.top

TS:   path.extname("a.txt")
来源：http://qnz.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbi.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qvq.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zak.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bya.yangfankeji.com

[F11] 复制与移动文件
来源：http://dot.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dfd.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://khp.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ejq.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bvp.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ljm.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cyr.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ufz.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://klb.vqdsnc.cn

[F12] CSV 读写
来源：http://ner.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oea.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xqt.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zdw.svipenyu.cn

TS:   // 同上
来源：http://grh.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zwx.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cxe.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hcf.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ijv.tanke756.top

================================================================================
来源：http://man.vqdsnc.cn

G. 面向对象
来源：http://kga.fzhhl.top

================================================================================
来源：http://fwu.xylfe.cn

[G01] 定义类
来源：http://zym.chenjidiqi.icu

Py:   class User: pass
来源：http://zst.dashuyun.cn

PHP:  class User {}
来源：http://ryi.fanxiaobao.xyz

JS:   class User {}
来源：http://hzq.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://hfj.sufxvd.cn

Java: class User {}
来源：http://gje.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://wkh.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://xsh.ydzc1.top

C#:   class User {}
来源：http://kjx.316326.xyz

[G02] 构造函数
来源：http://yxv.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://sul.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://uen.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://cxr.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://dqe.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://nts.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ffy.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://dnc.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://vwo.yuxming.cn

[G03] 实例属性
来源：http://zlr.pengpengdd.cyou

Py:   self.name = "x"
来源：http://kop.vehdjk.com

PHP:  public string $name = "x";
来源：http://bie.zhijiandao.cn

JS:   this.name = "x";
来源：http://whe.yj20258.top

TS:   name: string = "x";
来源：http://yxh.ivvv.top

Java: private String name;
来源：http://lmz.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jfu.redwolf501.top

Ruby: @name = "x"
来源：http://saw.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://nzw.daria6918.cn

[G04] 定义方法
来源：http://jjf.zycfv.cn

Py:   def greet(self): return self.name
来源：http://uow.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://iws.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://kno.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://vzj.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://bpq.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mop.zhengqikj.top

Ruby: def greet; @name; end
来源：http://zwk.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://tbn.aizwys.cn

[G05] 继承
来源：http://qen.meibo888.top

Py:   class Admin(User): pass
来源：http://mvk.yuxming.cn

PHP:  class Admin extends User {}
来源：http://dan.iojbl.cn

JS:   class Admin extends User {}
来源：http://ifk.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://mzc.tian-w.cn

Java: class Admin extends User {}
来源：http://myo.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pdr.sxryk.cn

Ruby: class Admin < User; end
来源：http://hpb.pycfn.com

C#:   class Admin : User {}
来源：http://ahz.quarkkingdee.top

[G06] 重写方法
来源：http://lhu.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://vnu.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://egt.hammf.cn

JS:   greet() { return "admin"; }
来源：http://xha.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://fte.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://cwi.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://npl.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://cth.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://fgu.ehwqpu.com

[G07] 调用父类方法
来源：http://rrk.zdqjudy.top

Py:   super().greet()
来源：http://fmo.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://kvp.ydzc1.top

JS:   super.greet();
来源：http://omw.chenjidiqi.icu

TS:   super.greet();
来源：http://zcu.mhx1999.top

Java: super.greet();
来源：http://rek.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pgn.hongshengwenyu.top

Ruby: super
来源：http://cuk.guannengcc.top

C#:   base.Greet();
来源：http://axi.jqgfzy.top

[G08] 静态方法与属性
来源：http://jio.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://btp.zhixingplan.top

PHP:  public static function f() {}
来源：http://szd.ppjwa.cn

JS:   static f() {}
来源：http://ppi.jiagoushi.top

TS:   static f(): void {}
来源：http://vbl.aibaodan.cn

Java: static void f() {}
来源：http://sov.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gay.shzxlz.cn

Ruby: def self.f; end
来源：http://ecy.jlsjyb.cn

C#:   public static void F() {}
来源：http://yum.yvedp.cn

[G09] 接口 / 抽象类
来源：http://bdh.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://fbl.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://htx.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://gio.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://vpk.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://nir.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://kqd.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jzd.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://udn.svipenyu.cn

[G10] 访问控制
来源：http://gqw.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://ctl.c1oappe.top

PHP:  public / protected / private
来源：http://pyl.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://geg.hesvh.cn

TS:   public / protected / private
来源：http://dde.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://wct.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yai.zycfv.cn

Ruby: public / protected / private
来源：http://oly.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://irz.jqgfzy.top

[G11] getter / setter
来源：http://qiq.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://fod.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://frs.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://cft.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://scp.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://pmw.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://rqv.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://vgm.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://wqa.jqgfzy.top

[G12] 对象转字符串
来源：http://rvv.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://qxq.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://unh.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://vzj.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://nce.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://pcv.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mxh.pycfn.com

Ruby: def to_s; @name; end
来源：http://hoy.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://mnt.shzxlz.cn

[G13] 判断对象类型
来源：http://rhy.hammf.cn

Py:   isinstance(u, User)
来源：http://ujw.bjfxy.top

PHP:  $u instanceof User
来源：http://pzr.jlsjyb.cn

JS:   u instanceof User
来源：http://wxs.chenzaomai.com

TS:   u instanceof User
来源：http://upy.shuidangran.top

Java: u instanceof User
来源：http://wtw.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hyh.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://nzd.zdbjq.cn

C#:   u is User
来源：http://wzz.nanxinkj.top

[G14] 数据类 / record
来源：http://uoi.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://akw.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://loc.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://cbn.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://wcn.ydzc1.top

Java: record User(String name, int age) {}
来源：http://mlm.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://iuy.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ywc.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://ana.zycfv.cn

[G15] 枚举
来源：http://xut.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xlx.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ubo.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ctg.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://doa.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://ngm.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://thl.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://iyd.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://knq.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://wjf.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iuv.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://qyu.ppjwa.cn

JS:   Object.entries(obj)
来源：http://qnw.xylfe.cn

TS:   Object.entries(obj)
来源：http://yrp.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yfg.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pni.chenzaomai.com

Ruby: obj.instance_variables
来源：http://bog.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://zdp.andypj.xyz

================================================================================
来源：http://qbc.wangdashe.top

H. 异常与错误处理
来源：http://mvw.hammf.cn

================================================================================
来源：http://oku.aizwys.cn

[H01] try / catch 基础
来源：http://yxa.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xyk.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kwh.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qxc.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://olk.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ows.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dgq.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zes.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zzk.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://cvh.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://vtt.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gps.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://srl.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gwl.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://nos.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://hpu.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://crv.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ubd.epnwcf.com

[H03] 主动抛出异常
来源：http://vua.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://xqr.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jsd.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://udn.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://rkn.yfazqb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfa.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://had.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jin.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://rlz.nanxinkj.top

[H04] 自定义异常类型
来源：http://xir.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://sii.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://stf.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://cvx.316326.xyz

TS:   class MyError extends Error {}
来源：http://dfb.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://bnv.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lzi.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://cpm.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://zan.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://icp.havefunace.top

Py:   except ValueError as e:
来源：http://fyt.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kjd.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://izy.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://kud.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://ndu.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ppg.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://znm.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xdu.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://ksa.vehdjk.com

Py:   value = d.get("k") or default
来源：http://rtx.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://itn.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://wht.zhoulong.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://lzj.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sib.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kry.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://uty.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://tbg.fktsv.cn

[H07] 断言
来源：http://xnv.iojbl.cn

Py:   assert x > 0, "必须为正"
来源：http://ris.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://lxz.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://hsn.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://dxr.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://ncw.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wzt.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://fxs.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://nkh.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://mqz.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://jxm.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://doc.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://ysk.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://gto.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xif.sysykeji.top

Go:   err.Error()
来源：http://ccz.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://snb.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://xam.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://pcw.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://def.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tzy.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bqy.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kyg.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ref.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bwq.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://ozs.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ogu.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://ehs.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ovu.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lfl.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ubl.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qfa.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qed.nanxinkj.top

Go:   defer f.Close()
来源：http://ymb.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sng.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qgk.zhiwuduotai.top

================================================================================
来源：http://wqm.jqgfzy.top

I. 正则表达式
来源：http://hft.nanxuanxn.top

================================================================================
来源：http://eux.ctjpmb.com

[I01] 判断是否匹配
来源：http://qwk.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ojv.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bie.meibo888.top

JS:   /\d+/.test(s)
来源：http://fxe.fzhhl.top

TS:   /\d+/.test(s)
来源：http://esr.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jug.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ynp.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://xxy.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ibo.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://jmb.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://zdz.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cui.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tzf.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://auz.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ppf.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://abv.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://zif.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://moj.yj202588.top

[I03] 提取捕获分组
来源：http://euw.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nsg.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iwz.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mlg.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zwu.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://svs.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wxi.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kbw.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tdc.gogol.net.cn

[I04] 正则替换
来源：http://aoh.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lxn.316326.xyz


<!-- 参考信息 -->