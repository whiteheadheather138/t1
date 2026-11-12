代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jzx.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://akz.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bqu.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zhb.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://svq.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bii.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://sqz.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zoh.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kdl.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bcz.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bqs.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bqo.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iex.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gil.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ago.yonumen.top

[F12] CSV 读写
来源：http://lts.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oyr.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wpo.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lbx.gogol.net.cn

TS:   // 同上
来源：http://exl.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://idr.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qgm.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fiu.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://mqt.chenlongwang.top

================================================================================
来源：http://fzh.shuidangran.top

G. 面向对象
来源：http://lwx.xinyue.icu

================================================================================
来源：http://nxa.jlsjyb.cn

[G01] 定义类
来源：http://jlx.gaohongyu789.top

Py:   class User: pass
来源：http://qyb.shanyushiyangtech.top

PHP:  class User {}
来源：http://yem.tianlin.xyz

JS:   class User {}
来源：http://jyp.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://fkx.iojbl.cn

Java: class User {}
来源：http://pbf.zdqjudy.top

Go:   type User struct { Name string }
来源：http://hgf.jiagoushi.top

Ruby: class User; end
来源：http://voh.daxiang520.top

C#:   class User {}
来源：http://rlq.cheryme.top

[G02] 构造函数
来源：http://ivg.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://apk.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://vyp.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://bxh.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://lbi.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://usx.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cle.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://toy.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://ovq.jqgufenzy.top

[G03] 实例属性
来源：http://wbg.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://ejv.xuanzx.com

PHP:  public string $name = "x";
来源：http://zng.vqdsnc.cn

JS:   this.name = "x";
来源：http://egy.snrcjt.cn

TS:   name: string = "x";
来源：http://wtj.epnwcf.com

Java: private String name;
来源：http://nlt.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ymy.tanke756.top

Ruby: @name = "x"
来源：http://yzp.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://mtr.bbcook.cn

[G04] 定义方法
来源：http://ssl.cheryme.top

Py:   def greet(self): return self.name
来源：http://udd.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zji.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://teq.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://ghz.hywenlv.cn

Java: String greet() { return name; }
来源：http://hft.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zed.birdmap.top

Ruby: def greet; @name; end
来源：http://gss.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://czx.jiagoushi.top

[G05] 继承
来源：http://hhj.redwolf501.top

Py:   class Admin(User): pass
来源：http://lfh.havefunace.top

PHP:  class Admin extends User {}
来源：http://opo.ydzc1.top

JS:   class Admin extends User {}
来源：http://ptg.jianghu66.top

TS:   class Admin extends User {}
来源：http://kcd.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://byp.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://guz.jianghu66.top

Ruby: class Admin < User; end
来源：http://dos.gaohongyu789.top

C#:   class Admin : User {}
来源：http://eeo.jqgufenzy.top

[G06] 重写方法
来源：http://mta.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://qro.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aki.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://spc.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://uez.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://wzm.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ort.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://wng.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://agu.pengpengdd.cyou

[G07] 调用父类方法
来源：http://znc.yuanzhike.top

Py:   super().greet()
来源：http://orp.hywenlv.cn

PHP:  parent::greet();
来源：http://hgb.jiagoushi.top

JS:   super.greet();
来源：http://wxs.fehbvm.com

TS:   super.greet();
来源：http://eoe.sjlbkw.cn

Java: super.greet();
来源：http://czq.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ykf.meibo888.top

Ruby: super
来源：http://mrh.jqgfzy.top

C#:   base.Greet();
来源：http://mpw.havefunace.top

[G08] 静态方法与属性
来源：http://ark.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lwz.mhx1999.top

PHP:  public static function f() {}
来源：http://rre.9152youxi.cn

JS:   static f() {}
来源：http://ada.fengsongda.top

TS:   static f(): void {}
来源：http://jbm.hammf.cn

Java: static void f() {}
来源：http://cob.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kls.jianghu66.top

Ruby: def self.f; end
来源：http://ibf.yueranfly.top

C#:   public static void F() {}
来源：http://azb.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://gey.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://xez.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://ymf.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fxw.sweek.top

TS:   interface Shape { area(): number; }
来源：http://npj.sysykeji.top

Java: interface Shape { double area(); }
来源：http://dyf.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://xyv.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wbc.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://mrg.fzhhl.top

[G10] 访问控制
来源：http://kha.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://shb.xuanzx.com

PHP:  public / protected / private
来源：http://mjl.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://dcs.yvedp.cn

TS:   public / protected / private
来源：http://tdw.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://bkw.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://onp.hammf.cn

Ruby: public / protected / private
来源：http://uoq.shzxlz.cn

C#:   public / protected / private / internal
来源：http://soa.xziqi.cn

[G11] getter / setter
来源：http://ulw.uphjek.com

Py:   @property 与 @x.setter
来源：http://qvm.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ndm.hnqzz.top

JS:   get name() { return this._name; }
来源：http://fqe.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://wsq.epnwcf.com

Java: public String getName() { return name; }
来源：http://trf.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://khm.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://euc.tarul.cn

C#:   public string Name { get; set; }
来源：http://iwn.dashuyun.cn

[G12] 对象转字符串
来源：http://dya.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://ccw.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cjw.andypj.xyz

JS:   toString() { return this.name; }
来源：http://lxn.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://hhb.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://hfo.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bdx.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://auc.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://hdf.jinqigfzy.top

[G13] 判断对象类型
来源：http://vmk.uphjek.com

Py:   isinstance(u, User)
来源：http://tdz.ydjk.org.cn

PHP:  $u instanceof User
来源：http://rum.pengpengdd.cyou

JS:   u instanceof User
来源：http://pye.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://ykk.nwbrower.top

Java: u instanceof User
来源：http://eem.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iyc.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://phy.hnqzz.top

C#:   u is User
来源：http://vdf.c1oappe.top

[G14] 数据类 / record
来源：http://ids.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lfi.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://qtz.andypj.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://yfu.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://zdy.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://zzd.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://wsn.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hav.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://dsi.hnqzz.top

[G15] 枚举
来源：http://cml.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://adh.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dfz.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://duy.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wuv.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://ajp.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vzp.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://nem.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pnm.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://hjy.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lty.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://dsj.xylfe.cn

JS:   Object.entries(obj)
来源：http://kvw.redwolf501.top

TS:   Object.entries(obj)
来源：http://fqj.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://clt.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ivl.fktsv.cn

Ruby: obj.instance_variables
来源：http://ctg.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://drz.ctjpmb.com

================================================================================
来源：http://xgt.wangshuangyany.cn

H. 异常与错误处理
来源：http://gtv.kuanghao11.cn

================================================================================
来源：http://vsq.52xcode.cn

[H01] try / catch 基础
来源：http://yok.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zzv.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jec.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xlx.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kxw.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hqj.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tnu.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vbo.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://azt.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://rex.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pvk.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zra.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wwn.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zoi.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://owy.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zls.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hjx.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://car.sweek.top

[H03] 主动抛出异常
来源：http://syh.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://bvy.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aeq.yj20258.top

JS:   throw new Error("错误信息");
来源：http://ljo.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://njh.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://chm.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nkd.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jpx.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://mod.tarul.cn

[H04] 自定义异常类型
来源：http://gay.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://ulb.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://koh.nwbrower.top

JS:   class MyError extends Error {}
来源：http://cpp.fengsongda.top

TS:   class MyError extends Error {}
来源：http://hld.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://tqk.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vls.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://qkr.yonumen.top

C#:   class MyException : Exception {}
来源：http://aoa.ppjwa.cn

[H05] 捕获特定类型
来源：http://hpf.guannengcc.top

Py:   except ValueError as e:
来源：http://zvs.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://stg.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://aid.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://qmn.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://fax.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kct.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://hxz.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nfc.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://xdm.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://xcs.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xud.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://wmq.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://txw.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yzu.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xcv.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://gjm.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://wxw.ehwqpu.com

[H07] 断言
来源：http://wij.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://zkg.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://kfa.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://tbb.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://iad.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://crv.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jep.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://loa.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://wfx.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://blb.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://qiq.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zzl.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://hlg.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tik.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ecg.jinghuilouyu.cn

Go:   err.Error()
来源：http://hfi.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://fjn.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://ttj.hnqzz.top

[H09] 带错误码的异常
来源：http://itl.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://saa.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bxw.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aud.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bzh.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yfm.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://phc.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://nsd.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cqs.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://tqs.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://urq.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tyk.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wbe.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bry.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cme.ctjpmb.com

Go:   defer f.Close()
来源：http://pjz.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://upd.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lkr.guannengcc.top

================================================================================
来源：http://jic.sweek.top

I. 正则表达式
来源：http://ogm.yvedp.cn

================================================================================
来源：http://lfu.cqqwz.cn

[I01] 判断是否匹配
来源：http://ntq.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bve.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://lvs.ivvv.top

JS:   /\d+/.test(s)
来源：http://ric.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://jjk.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://krr.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pqw.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://pji.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rgu.yonumen.top

[I02] 提取所有匹配
来源：http://oer.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://zwj.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wko.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vxb.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://clm.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jwm.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wtb.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://vpk.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zdu.jiagoushi.top

[I03] 提取捕获分组
来源：http://iyq.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vjn.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gmq.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uvd.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oey.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fbs.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bmz.birdmap.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://equ.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aqq.shzxlz.cn

[I04] 正则替换
来源：http://vci.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wzw.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://riv.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://cmh.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://sil.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://hmt.yongpay.top


<!-- 参考信息 -->