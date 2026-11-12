代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wwl.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mma.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufu.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fqz.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bhd.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://axh.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bch.316326.xyz

[F12] CSV 读写
来源：http://nsq.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://urh.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rzp.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mbd.xingfuxueyuan.xyz

TS:   // 同上
来源：http://zhn.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sxk.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mdu.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://upm.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rhq.52xcode.cn

================================================================================
来源：http://bue.guowangkeji.top

G. 面向对象
来源：http://oop.vqdsnc.cn

================================================================================
来源：http://yuj.chenzaomai.com

[G01] 定义类
来源：http://hlu.hfpthk.cn

Py:   class User: pass
来源：http://flz.shanyushiyangkeji.top

PHP:  class User {}
来源：http://dsb.ydzc1.top

JS:   class User {}
来源：http://eht.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://jix.fzhhl.top

Java: class User {}
来源：http://ply.sxryk.cn

Go:   type User struct { Name string }
来源：http://uln.shuidangran.top

Ruby: class User; end
来源：http://pal.chenjidiqi.icu

C#:   class User {}
来源：http://zsj.hesvh.cn

[G02] 构造函数
来源：http://cup.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://cns.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://goh.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://pmm.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://vha.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://bda.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hdw.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://vyk.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://plf.gogol.net.cn

[G03] 实例属性
来源：http://vad.wangdashe.top

Py:   self.name = "x"
来源：http://pmw.xylfe.cn

PHP:  public string $name = "x";
来源：http://efb.hysaishi.cn

JS:   this.name = "x";
来源：http://bls.aibaodan.cn

TS:   name: string = "x";
来源：http://arh.daria6918.cn

Java: private String name;
来源：http://nzf.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pia.chenzaomai.com

Ruby: @name = "x"
来源：http://rev.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://wrr.hcnkem.com

[G04] 定义方法
来源：http://rcy.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://fsh.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://oxs.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://axx.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://oiw.sysykeji.top

Java: String greet() { return name; }
来源：http://lhh.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qui.gzhubu.top

Ruby: def greet; @name; end
来源：http://aar.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://zwp.jianghu66.top

[G05] 继承
来源：http://ctn.yuanzhike.top

Py:   class Admin(User): pass
来源：http://hkn.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://qtv.yuxming.cn

JS:   class Admin extends User {}
来源：http://har.andypj.xyz

TS:   class Admin extends User {}
来源：http://cml.cheryme.top

Java: class Admin extends User {}
来源：http://ini.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zag.snrcjt.cn

Ruby: class Admin < User; end
来源：http://bdm.yj20258888.top

C#:   class Admin : User {}
来源：http://nnz.wangshuangyany.cn

[G06] 重写方法
来源：http://fay.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://uxj.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bdn.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://ucx.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://jin.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://stt.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bqt.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://qvi.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://zel.fehbvm.com

[G07] 调用父类方法
来源：http://qii.fktsv.cn

Py:   super().greet()
来源：http://zdt.nanxuanxn.top

PHP:  parent::greet();
来源：http://cqn.ivvv.top

JS:   super.greet();
来源：http://ihg.yj20258888.top

TS:   super.greet();
来源：http://jom.shuidangran.top

Java: super.greet();
来源：http://wai.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pww.cucudq.cn

Ruby: super
来源：http://tfd.xziqi.cn

C#:   base.Greet();
来源：http://xew.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://jew.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kdv.zdbjq.cn

PHP:  public static function f() {}
来源：http://baf.birdmap.top

JS:   static f() {}
来源：http://vjt.yvedp.cn

TS:   static f(): void {}
来源：http://pbi.yanxiufei.cn

Java: static void f() {}
来源：http://qfs.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ibs.aibaodan.cn

Ruby: def self.f; end
来源：http://qgw.epnwcf.com

C#:   public static void F() {}
来源：http://xiv.yj20258.top

[G09] 接口 / 抽象类
来源：http://veq.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://bij.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://fpr.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://umw.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://lhy.cashguo.top

Java: interface Shape { double area(); }
来源：http://jva.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://bcp.jqgfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sfv.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://hfx.fktsv.cn

[G10] 访问控制
来源：http://syw.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://nik.iojbl.cn

PHP:  public / protected / private
来源：http://cyl.smart0.xyz

JS:   #private 字段；其余公开
来源：http://erj.yvedp.cn

TS:   public / protected / private
来源：http://xqs.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://cwu.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://lft.kuanghao11.cn

Ruby: public / protected / private
来源：http://fqy.gzhubu.top

C#:   public / protected / private / internal
来源：http://owp.epnwcf.com

[G11] getter / setter
来源：http://mmd.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://ugv.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cod.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://ugk.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://kzt.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://ilq.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uok.shzxlz.cn

Ruby: attr_accessor :name
来源：http://reu.jianghu66.top

C#:   public string Name { get; set; }
来源：http://qyt.tarul.cn

[G12] 对象转字符串
来源：http://vxw.hammf.cn

Py:   def __str__(self): return self.name
来源：http://wve.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bvk.gzhubu.top

JS:   toString() { return this.name; }
来源：http://fkn.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://wwb.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://ntj.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mfc.pengpengdd.cyou

Ruby: def to_s; @name; end
来源：http://hrr.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://aie.jianghu66.top

[G13] 判断对象类型
来源：http://uld.aizwys.cn

Py:   isinstance(u, User)
来源：http://zwv.aizwys.cn

PHP:  $u instanceof User
来源：http://nhf.yangfankeji.com

JS:   u instanceof User
来源：http://bkw.hongshengwenyu.top

TS:   u instanceof User
来源：http://yjn.0kj1m.cn

Java: u instanceof User
来源：http://pro.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ihc.mhx1999.top

Ruby: u.is_a?(User)
来源：http://hco.jqgufenzy.top

C#:   u is User
来源：http://uju.316326.xyz

[G14] 数据类 / record
来源：http://azb.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sjm.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://hcx.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://efx.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://kmn.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://qgw.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://mnf.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wcu.hammf.cn

C#:   record User(string Name, int Age);
来源：http://mmn.yvedp.cn

[G15] 枚举
来源：http://xtb.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jvn.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qmv.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fzr.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hjg.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://gid.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yss.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://trd.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sno.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://xmj.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kao.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://sub.c1oappe.top

JS:   Object.entries(obj)
来源：http://ghl.cucudq.cn

TS:   Object.entries(obj)
来源：http://dmy.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ceq.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lww.andypj.xyz

Ruby: obj.instance_variables
来源：http://wvk.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://uck.jinqigufen.top

================================================================================
来源：http://vbn.chenlongwang.top

H. 异常与错误处理
来源：http://yax.nwbrower.top

================================================================================
来源：http://dya.ydzc1.top

[H01] try / catch 基础
来源：http://zwy.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qqh.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kcw.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xzc.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://grm.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vyp.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zod.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lhr.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://atd.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://pco.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://feq.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dkz.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ruz.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://psz.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wax.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wkv.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hcx.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sog.tanke756.top

[H03] 主动抛出异常
来源：http://vax.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://wuw.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vjz.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://kdy.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://dqw.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xyp.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rul.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wkn.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://shz.pycfn.com

[H04] 自定义异常类型
来源：http://pfu.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://bzq.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://mlb.ydzc1.top

JS:   class MyError extends Error {}
来源：http://khp.uphjek.com

TS:   class MyError extends Error {}
来源：http://wnd.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://yvw.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mec.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://vux.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://iko.snrcjt.cn

[H05] 捕获特定类型
来源：http://yeb.zhiwuduotai.top

Py:   except ValueError as e:
来源：http://nik.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wlq.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://yrr.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://uqf.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://ccs.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wbw.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://nhc.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kpw.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://lzi.xuanzx.com

Py:   value = d.get("k") or default
来源：http://pdc.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://gkm.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://dcr.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://zoe.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kcg.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://amz.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://hie.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://lco.aizwys.cn

[H07] 断言
来源：http://cyc.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://rul.svipenyu.cn

PHP:  assert($x > 0);
来源：http://uvm.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://szv.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://aih.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://hpz.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://opa.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jwr.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://dnt.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://uyw.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://xyv.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wjq.guowangkeji.top

JS:   e.message;  e.stack
来源：http://mfo.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ytj.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vil.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://sgo.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://bof.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://ykz.jiagoushi.top

[H09] 带错误码的异常
来源：http://wku.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://shg.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://epq.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mdw.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xzc.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jdw.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://msq.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://uzq.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nfe.tian-w.cn

[H10] 资源自动释放
来源：http://iyu.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fic.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ays.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://env.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dtq.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ogd.chenjidiqi.icu

Go:   defer f.Close()
来源：http://eug.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vxw.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://plr.jqgfzy.top

================================================================================
来源：http://vnu.jyoumei.cn

I. 正则表达式
来源：http://hjw.0kj1m.cn

================================================================================
来源：http://khx.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://psf.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fuj.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://lrz.gzhubu.top

JS:   /\d+/.test(s)
来源：http://urp.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://usa.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://znd.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tva.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://rpb.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://njo.sjlbkw.cn

[I02] 提取所有匹配
来源：http://aoo.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://ohc.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gbb.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dmv.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://olg.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kxl.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eoz.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://fxy.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qlw.yueranfly.top

[I03] 提取捕获分组
来源：http://tph.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cwf.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yeq.gotoacloud.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://del.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hmt.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zca.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dtx.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kwf.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ghk.cashguo.top

[I04] 正则替换
来源：http://meb.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lsm.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hke.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://vkx.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://jsy.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://wvk.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://aqg.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aww.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fib.hammf.cn

[I05] 按正则拆分
来源：http://usl.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://yld.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hio.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://rox.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://fmt.jyoumei.cn


<!-- 参考信息 -->