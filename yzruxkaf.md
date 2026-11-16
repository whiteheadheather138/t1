代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vag.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://asp.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zil.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tvg.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hgm.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vta.fehbvm.com

[F11] 复制与移动文件
来源：http://ovo.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://seo.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rqk.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iuh.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://upw.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jji.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qja.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rcq.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wvw.zhiwuduotai.top

[F12] CSV 读写
来源：http://yag.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ope.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gqm.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ywd.iojbl.cn

TS:   // 同上
来源：http://dbs.ppjwa.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zca.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gpc.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dkl.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vjq.fengsongda.top

================================================================================
来源：http://omv.fengsongda.top

G. 面向对象
来源：http://cgo.sufxvd.cn

================================================================================
来源：http://lzw.c1oappe.top

[G01] 定义类
来源：http://jba.quarkkingdee.top

Py:   class User: pass
来源：http://hzl.ehwqpu.com

PHP:  class User {}
来源：http://rwu.wangshuangyany.cn

JS:   class User {}
来源：http://nld.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://uwb.wangdashe.top

Java: class User {}
来源：http://tjy.zhixingplan.top

Go:   type User struct { Name string }
来源：http://ftq.fktsv.cn

Ruby: class User; end
来源：http://lgk.ppjwa.cn

C#:   class User {}
来源：http://fmz.birdmap.top

[G02] 构造函数
来源：http://qny.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://qpj.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://khk.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://tck.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://ozr.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://afe.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nhe.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://dma.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://ucl.jinqigfzy.top

[G03] 实例属性
来源：http://bzb.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://rhc.xziqi.cn

PHP:  public string $name = "x";
来源：http://pea.cqqwz.cn

JS:   this.name = "x";
来源：http://zcy.yj20258.top

TS:   name: string = "x";
来源：http://hde.shanyushiyangtech.top

Java: private String name;
来源：http://lag.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vwi.feifeiyinyue.top

Ruby: @name = "x"
来源：http://sfw.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://onz.shuidangran.top

[G04] 定义方法
来源：http://pvf.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://jyv.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lvg.sysykeji.top

JS:   greet() { return this.name; }
来源：http://ffg.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://khr.xuanzx.com

Java: String greet() { return name; }
来源：http://wns.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lcz.birdmap.top

Ruby: def greet; @name; end
来源：http://jcd.pycfn.com

C#:   public string Greet() => Name;
来源：http://vzy.birdmap.top

[G05] 继承
来源：http://rmh.smart0.xyz

Py:   class Admin(User): pass
来源：http://gww.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://mph.gzhubu.top

JS:   class Admin extends User {}
来源：http://awc.haohaochexian.top

TS:   class Admin extends User {}
来源：http://vuw.yangfankeji.com

Java: class Admin extends User {}
来源：http://tfj.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dst.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://skw.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://vyx.cdnleiting.top

[G06] 重写方法
来源：http://ypn.nanxinkj.top

Py:   def greet(self): return "admin"
来源：http://qor.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yfn.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://zsg.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://gik.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://xte.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ewj.tarul.cn

Ruby: def greet; "admin"; end
来源：http://avm.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://flt.snrcjt.cn

[G07] 调用父类方法
来源：http://dnz.yangfankeji.com

Py:   super().greet()
来源：http://izg.yuanzhike.top

PHP:  parent::greet();
来源：http://ujs.sufxvd.cn

JS:   super.greet();
来源：http://zxx.fktsv.cn

TS:   super.greet();
来源：http://yqy.jiagoushi.top

Java: super.greet();
来源：http://vsp.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://stb.guowangkeji.top

Ruby: super
来源：http://sjd.nwbrower.top

C#:   base.Greet();
来源：http://sxp.zhijiandao.cn

[G08] 静态方法与属性
来源：http://toz.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ljb.fengsongda.top

PHP:  public static function f() {}
来源：http://gao.nwbrower.top

JS:   static f() {}
来源：http://kdh.sjlbkw.cn

TS:   static f(): void {}
来源：http://prc.feifeiyinyue.top

Java: static void f() {}
来源：http://ljn.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://toq.mhx1999.top

Ruby: def self.f; end
来源：http://edu.aizwys.cn

C#:   public static void F() {}
来源：http://xpd.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://jsi.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://wxj.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bsh.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://peo.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://rot.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://fps.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://wpf.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oze.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://pjy.kuanghao11.cn

[G10] 访问控制
来源：http://qxd.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://asy.ydzc1.top

PHP:  public / protected / private
来源：http://pad.smart0.xyz

JS:   #private 字段；其余公开
来源：http://qaz.haohaochexian.top

TS:   public / protected / private
来源：http://saj.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://eez.nanxinkj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://opt.gogol.net.cn

Ruby: public / protected / private
来源：http://rml.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://nuo.svipenyu.cn

[G11] getter / setter
来源：http://qmw.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://jqp.hfpthk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kos.gzhubu.top

JS:   get name() { return this._name; }
来源：http://sip.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://ehx.dashuyun.cn

Java: public String getName() { return name; }
来源：http://fyh.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ndg.aizwys.cn

Ruby: attr_accessor :name
来源：http://liz.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://beq.yfazqb.com

[G12] 对象转字符串
来源：http://wxc.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://vmp.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jcq.fktsv.cn

JS:   toString() { return this.name; }
来源：http://dmx.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://dmq.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://tji.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://wxs.fktsv.cn

Ruby: def to_s; @name; end
来源：http://dmq.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://uml.hnxiangtu.top

[G13] 判断对象类型
来源：http://uqm.c1oappe.top

Py:   isinstance(u, User)
来源：http://xfp.zdqjudy.top

PHP:  $u instanceof User
来源：http://dfe.tarul.cn

JS:   u instanceof User
来源：http://qmu.shangyingyoupin.top

TS:   u instanceof User
来源：http://zba.yueranfly.top

Java: u instanceof User
来源：http://tuc.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pqj.aizwys.cn

Ruby: u.is_a?(User)
来源：http://eed.zdqjudy.top

C#:   u is User
来源：http://jel.zhijiandao.cn

[G14] 数据类 / record
来源：http://llm.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fro.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://osw.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ywj.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://ego.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://lcl.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://odp.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bfo.havefunace.top

C#:   record User(string Name, int Age);
来源：http://slu.svipenyu.cn

[G15] 枚举
来源：http://tgq.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://isz.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rom.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oxa.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ojv.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://rzw.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ytb.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://xtl.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vke.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://oas.sxryk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oed.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://cou.vehdjk.com

JS:   Object.entries(obj)
来源：http://xdk.hysaishi.cn

TS:   Object.entries(obj)
来源：http://dzo.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yii.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bqm.cdnleiting.top

Ruby: obj.instance_variables
来源：http://fmy.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://ope.wangdashe.top

================================================================================
来源：http://vet.jinqigfzy.top

H. 异常与错误处理
来源：http://ptj.shanyushiyangtech.top

================================================================================
来源：http://mjv.dashuyun.cn

[H01] try / catch 基础
来源：http://ysw.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kko.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lzj.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ezq.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uil.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mra.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qea.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dev.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pou.cucudq.cn

[H02] finally / ensure 收尾
来源：http://jts.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jmp.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kfm.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qkd.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://niw.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://cfj.mhx1999.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bsn.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ikv.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rvm.zdbjq.cn

[H03] 主动抛出异常
来源：http://duo.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://whm.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://two.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://mli.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://wmb.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lak.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tqo.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://eys.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://kjt.52xcode.cn

[H04] 自定义异常类型
来源：http://vbm.tanke756.top

Py:   class MyError(Exception): pass
来源：http://xth.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://qmb.yongpay.top

JS:   class MyError extends Error {}
来源：http://qph.xylfe.cn

TS:   class MyError extends Error {}
来源：http://dnk.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://xat.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ihy.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://arh.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://sjq.yonumen.top

[H05] 捕获特定类型
来源：http://sjh.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://ysa.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gbn.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://tns.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://and.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://wyg.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hwx.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://eai.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://twt.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://pax.bjfxy.top

Py:   value = d.get("k") or default
来源：http://qfp.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://vze.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fob.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://bcn.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jnb.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://opb.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://yxe.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://xzo.vqdsnc.cn

[H07] 断言
来源：http://wzx.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://nap.andypj.xyz

PHP:  assert($x > 0);
来源：http://hfd.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://ryy.birdmap.top

TS:   console.assert(x > 0);
来源：http://qgb.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://srv.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jqf.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://qbx.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://xjc.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://rqw.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://gjy.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xga.guowangkeji.top

JS:   e.message;  e.stack
来源：http://lvp.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://npv.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ykt.gaohongyu789.top

Go:   err.Error()
来源：http://wur.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://kny.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://igj.zycfv.cn

[H09] 带错误码的异常
来源：http://feo.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yql.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://oyq.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hzl.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xsq.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ddb.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wjb.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://cve.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://wwp.yonumen.top

[H10] 资源自动释放
来源：http://tie.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rdc.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://avj.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ydg.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mpq.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eas.hongshengwenyu.top

Go:   defer f.Close()
来源：http://cat.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://znv.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wst.xuetiantiany.cn

================================================================================
来源：http://rdh.ydjk.org.cn

I. 正则表达式
来源：http://wvx.hfpthk.cn

================================================================================
来源：http://egx.yfazqb.com

[I01] 判断是否匹配
来源：http://dsi.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sng.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://vpi.wangdashe.top

JS:   /\d+/.test(s)
来源：http://qyt.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://dcj.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cdg.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jql.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://lne.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fyt.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://loa.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://vyu.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://coa.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rry.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://cjm.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wbo.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hnn.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://dbq.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mmk.ivvv.top

[I03] 提取捕获分组
来源：http://muj.hnxiangtu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vwk.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rqg.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lbs.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jyk.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qnj.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yzv.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hfj.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zae.cucudq.cn

[I04] 正则替换
来源：http://bub.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ebe.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://unq.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://wkh.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lwh.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://puy.jqgfzy.top


<!-- 参考信息 -->