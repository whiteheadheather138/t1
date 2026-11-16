代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cas.tarul.cn

TS:   path.extname("a.txt")
来源：http://yfv.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dtr.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pme.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://enr.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aaj.sweek.top

[F11] 复制与移动文件
来源：http://mml.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tel.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xvk.yfazqb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbt.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ucw.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dxc.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tms.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tmj.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://guq.haohaochexian.top

[F12] CSV 读写
来源：http://luu.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dbm.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ovu.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tfg.kuanghao11.cn

TS:   // 同上
来源：http://tnd.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sqk.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jnz.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://quw.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hej.aibaodan.cn

================================================================================
来源：http://dhb.kuanghao11.cn

G. 面向对象
来源：http://atw.gogol.net.cn

================================================================================
来源：http://gtm.ivvv.top

[G01] 定义类
来源：http://ddx.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://lac.9152youxi.cn

PHP:  class User {}
来源：http://hzj.yonumen.top

JS:   class User {}
来源：http://cqz.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://lva.chenlongwang.top

Java: class User {}
来源：http://emj.svipenyu.cn

Go:   type User struct { Name string }
来源：http://qaw.cashguo.top

Ruby: class User; end
来源：http://hfe.xylfe.cn

C#:   class User {}
来源：http://tsu.sysykeji.top

[G02] 构造函数
来源：http://eyq.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://fcv.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://dkv.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://uir.yongpay.top

TS:   constructor(public name: string) {}
来源：http://mzu.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://vyg.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tnr.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://hxh.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://tld.zhaomingkeji.xyz

[G03] 实例属性
来源：http://wkq.sysykeji.top

Py:   self.name = "x"
来源：http://wbu.52xcode.cn

PHP:  public string $name = "x";
来源：http://ima.nwbrower.top

JS:   this.name = "x";
来源：http://nbx.bjfxy.top

TS:   name: string = "x";
来源：http://mui.shuidangran.top

Java: private String name;
来源：http://axw.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qez.gaohongyu789.top

Ruby: @name = "x"
来源：http://szc.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://dme.gzhubu.top

[G04] 定义方法
来源：http://que.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://bya.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cxa.hammf.cn

JS:   greet() { return this.name; }
来源：http://cnm.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://zdh.aizwys.cn

Java: String greet() { return name; }
来源：http://wll.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gey.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://gtg.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://ppo.hnqzz.top

[G05] 继承
来源：http://zbn.yuxming.cn

Py:   class Admin(User): pass
来源：http://gps.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://ygl.ydzc1.top

JS:   class Admin extends User {}
来源：http://iqg.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://rtl.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://emt.ppjwa.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jfb.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://sfv.cheryme.top

C#:   class Admin : User {}
来源：http://yfy.xylfe.cn

[G06] 重写方法
来源：http://xti.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://lik.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mpp.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://pps.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://pih.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://hnn.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://whz.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://xof.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://xhb.guannengcc.top

[G07] 调用父类方法
来源：http://ccs.zhixingplan.top

Py:   super().greet()
来源：http://vov.gaohongyu789.top

PHP:  parent::greet();
来源：http://byl.havefunace.top

JS:   super.greet();
来源：http://jtd.birdmap.top

TS:   super.greet();
来源：http://tft.hesvh.cn

Java: super.greet();
来源：http://xie.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://plc.aizwys.cn

Ruby: super
来源：http://sui.zhengqikj.top

C#:   base.Greet();
来源：http://dyr.0kj1m.cn

[G08] 静态方法与属性
来源：http://thx.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sdb.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://tsu.xinyue.icu

JS:   static f() {}
来源：http://afa.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://fun.jyoumei.cn

Java: static void f() {}
来源：http://rph.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sin.xylfe.cn

Ruby: def self.f; end
来源：http://bfa.yueranfly.top

C#:   public static void F() {}
来源：http://vpd.yuxming.cn

[G09] 接口 / 抽象类
来源：http://ybw.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://hjw.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://suh.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cqx.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://yfx.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://uha.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://rgq.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lmi.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://aku.yongpay.top

[G10] 访问控制
来源：http://xkn.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://aqc.hnqzz.top

PHP:  public / protected / private
来源：http://zxs.ybcxt.top

JS:   #private 字段；其余公开
来源：http://zab.fanxiaobao.xyz

TS:   public / protected / private
来源：http://oxh.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://trt.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://acr.fzhhl.top

Ruby: public / protected / private
来源：http://yvw.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://swg.quarkkingdee.top

[G11] getter / setter
来源：http://nqu.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://mqq.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cqb.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://bro.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://vaa.tian-w.cn

Java: public String getName() { return name; }
来源：http://rsp.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://iwh.ehwqpu.com

Ruby: attr_accessor :name
来源：http://ltr.yj20258888.top

C#:   public string Name { get; set; }
来源：http://gpl.dianchejie.cn

[G12] 对象转字符串
来源：http://nrc.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://kcd.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gis.bbcook.cn

JS:   toString() { return this.name; }
来源：http://atc.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://jzp.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://wyz.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://rkj.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://qzd.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://adn.hfpthk.cn

[G13] 判断对象类型
来源：http://mpb.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://grv.iojbl.cn

PHP:  $u instanceof User
来源：http://lba.birdmap.top

JS:   u instanceof User
来源：http://nsc.zdqjudy.top

TS:   u instanceof User
来源：http://apo.jlsjyb.cn

Java: u instanceof User
来源：http://ghk.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zep.gzhubu.top

Ruby: u.is_a?(User)
来源：http://lnj.shanyushiyangtech.top

C#:   u is User
来源：http://mmg.jianghu66.top

[G14] 数据类 / record
来源：http://zmb.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://stg.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://kgh.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://eki.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://dwz.bbcook.cn

Java: record User(String name, int age) {}
来源：http://bou.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://qzp.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zwk.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://dgy.yonumen.top

[G15] 枚举
来源：http://ztn.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dlz.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cvo.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ktt.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iyr.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://pdf.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ldc.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://rnu.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fpk.hammf.cn

[G16] 对象转数组 / 字典
来源：http://tfh.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gqt.pycfn.com

PHP:  get_object_vars($obj);
来源：http://ubu.hfpthk.cn

JS:   Object.entries(obj)
来源：http://tgc.jianghu66.top

TS:   Object.entries(obj)
来源：http://dey.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wok.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pqv.zdbjq.cn

Ruby: obj.instance_variables
来源：http://ver.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://iis.andypj.xyz

================================================================================
来源：http://jzq.cheryme.top

H. 异常与错误处理
来源：http://raf.yangfankeji.com

================================================================================
来源：http://tnl.gaohongyu789.top

[H01] try / catch 基础
来源：http://wxo.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rkp.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rmg.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jaj.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lrq.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dgn.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xpl.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://euq.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ell.hcnkem.com

[H02] finally / ensure 收尾
来源：http://boi.ydjk.org.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bvj.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://dgv.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eup.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lxh.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eei.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pbs.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ghv.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pai.uphjek.com

[H03] 主动抛出异常
来源：http://cke.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://ilz.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ihq.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://obd.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://cix.yfazqb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://rye.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dsa.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qyu.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://kye.yuxming.cn

[H04] 自定义异常类型
来源：http://spe.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://kwf.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ptc.gzhubu.top

JS:   class MyError extends Error {}
来源：http://ubs.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://wgq.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://urh.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hpx.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://dsk.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://ktn.yangfankeji.com

[H05] 捕获特定类型
来源：http://lqn.pycfn.com

Py:   except ValueError as e:
来源：http://ckd.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pvn.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://irp.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://evl.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://tbv.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tof.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://beq.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xlq.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://yia.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://iuz.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://ves.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pof.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rrc.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qru.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://dkj.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://mkt.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://sla.shzxlz.cn

[H07] 断言
来源：http://met.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://txd.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://jzz.havefunace.top

JS:   console.assert(x > 0);
来源：http://pem.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://lbb.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://vcl.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tkm.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://czc.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://nax.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://ehk.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://uxp.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xnn.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://peg.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ott.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fey.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://dib.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://psw.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://fke.yfazqb.com

[H09] 带错误码的异常
来源：http://iwk.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://enq.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fev.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://skx.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tpq.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jfm.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dud.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ngz.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zuy.yuxming.cn

[H10] 资源自动释放
来源：http://oik.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://geb.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rhc.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eyy.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lyv.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tgp.smart0.xyz

Go:   defer f.Close()
来源：http://tai.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qtm.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iob.vehdjk.com

================================================================================
来源：http://zph.havefunace.top

I. 正则表达式
来源：http://hzh.c1oappe.top

================================================================================
来源：http://hmk.gaohongyu789.top

[I01] 判断是否匹配
来源：http://bzr.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rhq.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lxj.pycfn.com

JS:   /\d+/.test(s)
来源：http://mrm.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://yzj.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nwd.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vap.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://xqb.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://feh.c1oappe.top

[I02] 提取所有匹配
来源：http://clp.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://uja.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pyk.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ebu.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://fdx.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gfi.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cpk.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://cal.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://txe.chenlongwang.top

[I03] 提取捕获分组
来源：http://ywi.jinqigufen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://olq.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xve.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tnc.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yxo.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://crt.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iqc.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bee.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oej.wangshuangyany.cn

[I04] 正则替换
来源：http://tfu.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ore.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ivo.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://fbp.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://hwj.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://uhc.guowangkeji.top


<!-- 参考信息 -->