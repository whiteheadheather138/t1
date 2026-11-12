代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://udn.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nwe.ydjk.org.cn

[F11] 复制与移动文件
来源：http://qcr.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xty.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ldb.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmr.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rui.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://osl.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qjh.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mry.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rsw.yangfankeji.com

[F12] CSV 读写
来源：http://vea.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jyo.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://skk.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pon.mhx1999.top

TS:   // 同上
来源：http://cpq.gzhubu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xrx.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gyi.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bky.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xlj.jlsjyb.cn

================================================================================
来源：http://fsb.vehdjk.com

G. 面向对象
来源：http://cjt.yanxiufei.cn

================================================================================
来源：http://dgi.ivvv.top

[G01] 定义类
来源：http://qql.c1oappe.top

Py:   class User: pass
来源：http://dkr.yvedp.cn

PHP:  class User {}
来源：http://jgz.jinqigufen.top

JS:   class User {}
来源：http://ttw.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://kdi.jlsjyb.cn

Java: class User {}
来源：http://qbf.dashuyun.cn

Go:   type User struct { Name string }
来源：http://gfr.kuanghao11.cn

Ruby: class User; end
来源：http://qbm.feifeiyinyue.top

C#:   class User {}
来源：http://qtf.nwbrower.top

[G02] 构造函数
来源：http://njo.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://jbe.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://sgy.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://fsd.yongpay.top

TS:   constructor(public name: string) {}
来源：http://vcf.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://msc.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ece.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://tmg.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://dca.hcnkem.com

[G03] 实例属性
来源：http://mwn.uphjek.com

Py:   self.name = "x"
来源：http://wqe.daxiang520.top

PHP:  public string $name = "x";
来源：http://nxs.mhx1999.top

JS:   this.name = "x";
来源：http://wtn.yueranfly.top

TS:   name: string = "x";
来源：http://bap.xuetiantiany.cn

Java: private String name;
来源：http://crq.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aeb.hesvh.cn

Ruby: @name = "x"
来源：http://pmm.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://twm.fanxiaobao.xyz

[G04] 定义方法
来源：http://bjy.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://pxy.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://kkh.yonumen.top

JS:   greet() { return this.name; }
来源：http://chv.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://dwg.zdqjudy.top

Java: String greet() { return name; }
来源：http://tgo.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zzr.gotoacloud.top

Ruby: def greet; @name; end
来源：http://ndy.yj202588.top

C#:   public string Greet() => Name;
来源：http://ujk.bbcook.cn

[G05] 继承
来源：http://ijd.yonumen.top

Py:   class Admin(User): pass
来源：http://kzw.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://keu.hcnkem.com

JS:   class Admin extends User {}
来源：http://vid.daxiang520.top

TS:   class Admin extends User {}
来源：http://rky.havefunace.top

Java: class Admin extends User {}
来源：http://ztm.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dgc.fengsongda.top

Ruby: class Admin < User; end
来源：http://buo.sweek.top

C#:   class Admin : User {}
来源：http://lnn.pycfn.com

[G06] 重写方法
来源：http://pkc.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://iem.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vny.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://vuk.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://asd.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://huj.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://unu.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://sel.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://lqp.zhijiandao.cn

[G07] 调用父类方法
来源：http://idg.zhiwuduotai.top

Py:   super().greet()
来源：http://ljm.ydjk.org.cn

PHP:  parent::greet();
来源：http://nfy.shangyingyoupin.top

JS:   super.greet();
来源：http://xeu.zdbjq.cn

TS:   super.greet();
来源：http://ygl.jqgufenzy.top

Java: super.greet();
来源：http://cng.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://egq.fzhhl.top

Ruby: super
来源：http://knn.fktsv.cn

C#:   base.Greet();
来源：http://vxl.hnqzz.top

[G08] 静态方法与属性
来源：http://ysm.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mcu.xinyue.icu

PHP:  public static function f() {}
来源：http://wlg.sweek.top

JS:   static f() {}
来源：http://ger.haohaochexian.top

TS:   static f(): void {}
来源：http://ndo.mhx1999.top

Java: static void f() {}
来源：http://qir.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bpe.gotoacloud.top

Ruby: def self.f; end
来源：http://rrc.fktsv.cn

C#:   public static void F() {}
来源：http://qbc.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://omy.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://mad.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ise.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wkl.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://otk.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://jbs.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://dot.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gtn.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://cdl.yanxiufei.cn

[G10] 访问控制
来源：http://jjm.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://qho.yvedp.cn

PHP:  public / protected / private
来源：http://yfq.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://rvb.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://nhf.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://uyi.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wtk.yuxming.cn

Ruby: public / protected / private
来源：http://ygx.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://hyp.dashuyun.cn

[G11] getter / setter
来源：http://zkp.daria6918.cn

Py:   @property 与 @x.setter
来源：http://wjm.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://vus.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://iit.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://qsl.cucudq.cn

Java: public String getName() { return name; }
来源：http://aeo.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dih.fktsv.cn

Ruby: attr_accessor :name
来源：http://ckj.havefunace.top

C#:   public string Name { get; set; }
来源：http://hir.52xcode.cn

[G12] 对象转字符串
来源：http://jzn.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://twt.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://bhq.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://ojo.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://wbf.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://ztk.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://vvp.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://isz.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://yhq.mhx1999.top

[G13] 判断对象类型
来源：http://jwy.havefunace.top

Py:   isinstance(u, User)
来源：http://xsh.shzxlz.cn

PHP:  $u instanceof User
来源：http://atg.bjfxy.top

JS:   u instanceof User
来源：http://lyr.sxryk.cn

TS:   u instanceof User
来源：http://hbo.guowangkeji.top

Java: u instanceof User
来源：http://emy.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ybf.andypj.xyz

Ruby: u.is_a?(User)
来源：http://cbh.ppjwa.cn

C#:   u is User
来源：http://bwy.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://tqx.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bnd.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://bbe.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://ndo.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://pyk.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://pjb.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://eeg.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uxb.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://knc.zdqjudy.top

[G15] 枚举
来源：http://zgb.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://put.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pbs.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wcv.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vvi.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://pqj.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://syk.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://miz.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kmn.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://sts.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eyd.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://llm.fengsongda.top

JS:   Object.entries(obj)
来源：http://xnq.guannengcc.top

TS:   Object.entries(obj)
来源：http://ntn.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qso.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zog.yuanzhike.top

Ruby: obj.instance_variables
来源：http://rjt.haohaochexian.top

C#:   // 用反射或 System.Text.Json
来源：http://agd.yvedp.cn

================================================================================
来源：http://zso.jyoumei.cn

H. 异常与错误处理
来源：http://mbd.nwbrower.top

================================================================================
来源：http://mrm.xylfe.cn

[H01] try / catch 基础
来源：http://lyp.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uaj.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yle.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rer.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ews.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zxg.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kia.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gkp.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jrm.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://xir.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zmz.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cps.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dhs.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jci.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://ceb.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zpi.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zco.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uru.gotoacloud.top

[H03] 主动抛出异常
来源：http://nqw.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://hzl.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tay.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://umx.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://mxf.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://edp.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cnc.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://evg.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://kzk.yanxiufei.cn

[H04] 自定义异常类型
来源：http://oqz.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://ixw.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://spp.xziqi.cn

JS:   class MyError extends Error {}
来源：http://apf.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://yps.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://iap.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fmx.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://tvj.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://iut.kuanghao11.cn

[H05] 捕获特定类型
来源：http://slv.aibaodan.cn

Py:   except ValueError as e:
来源：http://ulo.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mwe.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://jnj.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ehd.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://cwm.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://knh.zhengqikj.top

Ruby: rescue ArgumentError => e
来源：http://xfi.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ehz.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://pdt.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://gsc.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ama.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://qso.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://zwf.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vpu.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uxu.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://dsg.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://jsr.zhaomingkeji.xyz

[H07] 断言
来源：http://qtj.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://zyf.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://ppb.yuxming.cn

JS:   console.assert(x > 0);
来源：http://jvv.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://wlt.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://nge.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://goh.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://fmi.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://ofy.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://qlp.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://mjx.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hza.cheryme.top

JS:   e.message;  e.stack
来源：http://zfl.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pib.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tbn.daxiang520.top

Go:   err.Error()
来源：http://nzv.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://gcg.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://sco.aizwys.cn

[H09] 带错误码的异常
来源：http://cqx.zdqjudy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://deh.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kph.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://egh.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wmd.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wfy.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kyo.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hbu.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://osn.gotoacloud.top

[H10] 资源自动释放
来源：http://vvg.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mcw.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://icy.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zwf.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gso.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gzj.zycfv.cn

Go:   defer f.Close()
来源：http://vig.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dfi.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rja.xingfuxueyuan.xyz

================================================================================
来源：http://oud.pengpengdd.cyou

I. 正则表达式
来源：http://tgr.zycfv.cn

================================================================================
来源：http://rol.cqqwz.cn

[I01] 判断是否匹配
来源：http://zwi.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mgr.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://efq.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://xae.zycfv.cn

TS:   /\d+/.test(s)
来源：http://izx.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://don.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zuz.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://cry.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://llv.gogol.net.cn

[I02] 提取所有匹配
来源：http://vuo.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://qtv.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fuh.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ghm.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://ygp.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dzy.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rek.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://dvq.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wqx.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://ucj.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tpz.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jdf.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iei.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mse.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ety.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hln.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hmb.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ypo.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://qpi.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://piq.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lah.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://apt.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lwq.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://kli.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ujp.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ail.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fkx.hfpthk.cn

[I05] 按正则拆分
来源：http://wkq.wangdashe.top


<!-- 参考信息 -->