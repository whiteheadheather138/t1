代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pjw.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tcb.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etu.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mhn.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tgd.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iin.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qtc.shzxlz.cn

[F12] CSV 读写
来源：http://cxi.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uwi.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bhx.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gtx.vqdsnc.cn

TS:   // 同上
来源：http://tjg.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iee.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sbu.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jku.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://bab.cdnleiting.top

================================================================================
来源：http://qkg.yj20258.top

G. 面向对象
来源：http://nvu.jinqigfzy.top

================================================================================
来源：http://bes.yanxiufei.cn

[G01] 定义类
来源：http://lko.0kj1m.cn

Py:   class User: pass
来源：http://qsv.ppjwa.cn

PHP:  class User {}
来源：http://est.zycfv.cn

JS:   class User {}
来源：http://yvl.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://fpu.zhongyouzk.top

Java: class User {}
来源：http://kmf.svipenyu.cn

Go:   type User struct { Name string }
来源：http://ysw.shanyushiyangkeji.top

Ruby: class User; end
来源：http://hmk.uphjek.com

C#:   class User {}
来源：http://dpo.gotoacloud.top

[G02] 构造函数
来源：http://oug.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://jsy.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://unw.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://tgv.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://hti.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://wde.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hfg.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://tzr.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://hdv.yj202588.top

[G03] 实例属性
来源：http://lqx.hfpthk.cn

Py:   self.name = "x"
来源：http://svj.sxryk.cn

PHP:  public string $name = "x";
来源：http://uqe.jinqigfzy.top

JS:   this.name = "x";
来源：http://rry.cucudq.cn

TS:   name: string = "x";
来源：http://gni.sxryk.cn

Java: private String name;
来源：http://gaf.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lff.kuanghao11.cn

Ruby: @name = "x"
来源：http://zcu.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://kuj.jyoumei.cn

[G04] 定义方法
来源：http://cbl.sweek.top

Py:   def greet(self): return self.name
来源：http://cro.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ixc.yueranfly.top

JS:   greet() { return this.name; }
来源：http://ngx.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://ikg.birdmap.top

Java: String greet() { return name; }
来源：http://oad.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iki.yj20258888.top

Ruby: def greet; @name; end
来源：http://miv.yj20258888.top

C#:   public string Greet() => Name;
来源：http://jli.zdqjudy.top

[G05] 继承
来源：http://tja.iojbl.cn

Py:   class Admin(User): pass
来源：http://ylf.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://uaj.chenlongwang.top

JS:   class Admin extends User {}
来源：http://bmn.hysaishi.cn

TS:   class Admin extends User {}
来源：http://rxa.zhoulong.xyz

Java: class Admin extends User {}
来源：http://jbx.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wen.jyoumei.cn

Ruby: class Admin < User; end
来源：http://yru.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://uhh.yfazqb.com

[G06] 重写方法
来源：http://dmf.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://vwi.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ntc.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://lvj.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://zzb.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://lcc.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://byd.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://llp.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://poh.tarul.cn

[G07] 调用父类方法
来源：http://zgg.zhengqikj.top

Py:   super().greet()
来源：http://eev.0kj1m.cn

PHP:  parent::greet();
来源：http://ouc.zdqjudy.top

JS:   super.greet();
来源：http://roo.dianchejie.cn

TS:   super.greet();
来源：http://vpa.zhixingplan.top

Java: super.greet();
来源：http://cav.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dys.kuanghao11.cn

Ruby: super
来源：http://xcp.ctjpmb.com

C#:   base.Greet();
来源：http://mxb.yangfankeji.com

[G08] 静态方法与属性
来源：http://mwf.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jkw.zdqjudy.top

PHP:  public static function f() {}
来源：http://gux.ywan-chungtsiang.top

JS:   static f() {}
来源：http://big.aizwys.cn

TS:   static f(): void {}
来源：http://api.guannengcc.top

Java: static void f() {}
来源：http://fnn.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ojn.cheryme.top

Ruby: def self.f; end
来源：http://fbl.ydzc1.top

C#:   public static void F() {}
来源：http://nub.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://klu.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://tbh.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qda.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://csi.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://hxd.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://gvn.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://ols.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://exl.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://hof.yonumen.top

[G10] 访问控制
来源：http://pih.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://yls.yj20258.top

PHP:  public / protected / private
来源：http://hjm.fzhhl.top

JS:   #private 字段；其余公开
来源：http://uqp.cheryme.top

TS:   public / protected / private
来源：http://liy.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://ato.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yqo.tanke756.top

Ruby: public / protected / private
来源：http://iyt.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://srj.nwbrower.top

[G11] getter / setter
来源：http://omw.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://jcv.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zod.birdmap.top

JS:   get name() { return this._name; }
来源：http://lyz.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://lnx.daria6918.cn

Java: public String getName() { return name; }
来源：http://cxd.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://vlc.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://ylg.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://lnw.bbcook.cn

[G12] 对象转字符串
来源：http://skj.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://kur.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bnu.c1oappe.top

JS:   toString() { return this.name; }
来源：http://ydx.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://twf.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://hon.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://gzq.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://fjb.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://cmw.iojbl.cn

[G13] 判断对象类型
来源：http://pal.c1oappe.top

Py:   isinstance(u, User)
来源：http://fsi.cheryme.top

PHP:  $u instanceof User
来源：http://vgz.mhx1999.top

JS:   u instanceof User
来源：http://izb.zhengqikj.top

TS:   u instanceof User
来源：http://bkr.wangshuangyany.cn

Java: u instanceof User
来源：http://guo.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://npb.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://shc.52xcode.cn

C#:   u is User
来源：http://bej.cucudq.cn

[G14] 数据类 / record
来源：http://usv.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tus.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://nun.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://upd.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://zra.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://rgk.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://vkf.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mfv.cashguo.top

C#:   record User(string Name, int Age);
来源：http://mma.sxryk.cn

[G15] 枚举
来源：http://anq.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kpd.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yxq.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://czi.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qhh.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://jyu.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xhc.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://mqq.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eok.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://ium.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tsz.yonumen.top

PHP:  get_object_vars($obj);
来源：http://uth.iojbl.cn

JS:   Object.entries(obj)
来源：http://djm.birdmap.top

TS:   Object.entries(obj)
来源：http://naz.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bdf.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://snx.smart0.xyz

Ruby: obj.instance_variables
来源：http://dgx.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://bhb.yongpay.top

================================================================================
来源：http://vey.jqgfzy.top

H. 异常与错误处理
来源：http://vva.aibaodan.cn

================================================================================
来源：http://cjt.fengsongda.top

[H01] try / catch 基础
来源：http://zoq.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uwe.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jus.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zyw.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://god.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qse.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wjs.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jlq.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vjh.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://csw.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://pcv.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://lda.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://zzk.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mmn.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://rpe.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jxs.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dpb.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://vnv.epnwcf.com

[H03] 主动抛出异常
来源：http://orm.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://yam.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://stu.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://uas.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://ckp.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://gga.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sby.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wvo.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://zdl.xziqi.cn

[H04] 自定义异常类型
来源：http://njr.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://ukj.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://kvm.shuidangran.top

JS:   class MyError extends Error {}
来源：http://ycf.yuxming.cn

TS:   class MyError extends Error {}
来源：http://cbf.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://mds.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sot.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://vtl.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://uar.9152youxi.cn

[H05] 捕获特定类型
来源：http://ffd.tanke756.top

Py:   except ValueError as e:
来源：http://ldq.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lax.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://qea.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://gmm.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://kuz.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dew.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://otl.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ssx.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://fqz.xylfe.cn

Py:   value = d.get("k") or default
来源：http://jnj.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yvo.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tvm.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fpb.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ldv.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zsv.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://zjo.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://tls.tarul.cn

[H07] 断言
来源：http://awv.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://oxz.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://ras.ivvv.top

JS:   console.assert(x > 0);
来源：http://ypn.ivvv.top

TS:   console.assert(x > 0);
来源：http://qeb.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://wwv.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://chd.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://epz.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://vzt.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://vaq.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://fuh.zhengqikj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://roa.birdmap.top

JS:   e.message;  e.stack
来源：http://feu.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fqe.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hvr.hysaishi.cn

Go:   err.Error()
来源：http://pga.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://ksd.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://flf.fktsv.cn

[H09] 带错误码的异常
来源：http://lsv.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xvo.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fwq.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lmy.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xdr.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://njq.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jja.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://mxn.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yel.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://jlq.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rwg.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://noz.birdmap.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kco.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://crt.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xmm.cqqwz.cn

Go:   defer f.Close()
来源：http://myz.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lmr.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vgp.ehwqpu.com

================================================================================
来源：http://tax.chenzaomai.com

I. 正则表达式
来源：http://zmp.xuetiantiany.cn

================================================================================
来源：http://yny.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://aat.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fqa.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://lzr.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://tdc.uphjek.com

TS:   /\d+/.test(s)
来源：http://soa.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nsb.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cpl.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://dqz.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zza.tian-w.cn

[I02] 提取所有匹配
来源：http://ayj.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://vvu.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nev.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tuw.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://fwj.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://plq.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sxk.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://xgr.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ocm.xinyue.icu

[I03] 提取捕获分组
来源：http://zzr.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cgj.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sni.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xid.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ikf.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tda.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jwz.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://abi.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hqa.hongshengwenyu.top

[I04] 正则替换
来源：http://rfl.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zct.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hsf.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://mgn.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hbw.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://mjx.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pbd.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://qeu.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bxm.hnxiangtu.top

[I05] 按正则拆分
来源：http://zxh.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gty.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qzg.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://xtl.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://dzc.guannengcc.top


<!-- 参考信息 -->