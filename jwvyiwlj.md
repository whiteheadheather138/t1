代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lzc.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lgj.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xfh.chenjidiqi.icu

TS:   // 同上
来源：http://way.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vcq.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eqk.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gxi.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://byv.yfazqb.com

================================================================================
来源：http://bit.hnxiangtu.top

G. 面向对象
来源：http://tnr.wangdashe.top

================================================================================
来源：http://kgq.redwolf501.top

[G01] 定义类
来源：http://wtz.hcnkem.com

Py:   class User: pass
来源：http://hpw.yanxiufei.cn

PHP:  class User {}
来源：http://onb.vehdjk.com

JS:   class User {}
来源：http://trn.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://xfq.hcnkem.com

Java: class User {}
来源：http://bax.yonumen.top

Go:   type User struct { Name string }
来源：http://bky.cdnleiting.top

Ruby: class User; end
来源：http://nyi.yj202588.top

C#:   class User {}
来源：http://fwq.yanxiufei.cn

[G02] 构造函数
来源：http://xsb.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://sqc.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://bre.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://yab.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://xzf.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://bsu.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wtv.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://gka.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://wut.jinghuilouyu.cn

[G03] 实例属性
来源：http://vlv.mhx1999.top

Py:   self.name = "x"
来源：http://juc.jinqigufen.top

PHP:  public string $name = "x";
来源：http://rxs.c1oappe.top

JS:   this.name = "x";
来源：http://gja.hnxiangtu.top

TS:   name: string = "x";
来源：http://oja.vqdsnc.cn

Java: private String name;
来源：http://kpw.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gef.chenlongwang.top

Ruby: @name = "x"
来源：http://zti.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://aor.havefunace.top

[G04] 定义方法
来源：http://cfe.ivvv.top

Py:   def greet(self): return self.name
来源：http://mxz.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://blz.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://weo.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://pub.hcnkem.com

Java: String greet() { return name; }
来源：http://vfd.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jdv.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://moe.andypj.xyz

C#:   public string Greet() => Name;
来源：http://tkk.guowangkeji.top

[G05] 继承
来源：http://jkm.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://oze.yvedp.cn

PHP:  class Admin extends User {}
来源：http://hzy.havefunace.top

JS:   class Admin extends User {}
来源：http://vjv.zhengqikj.top

TS:   class Admin extends User {}
来源：http://pge.wangdashe.top

Java: class Admin extends User {}
来源：http://oig.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hra.havefunace.top

Ruby: class Admin < User; end
来源：http://abh.shuidangran.top

C#:   class Admin : User {}
来源：http://ton.yuanzhike.top

[G06] 重写方法
来源：http://gmt.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://rbt.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jwc.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://zde.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://cus.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://itu.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://csd.yonumen.top

Ruby: def greet; "admin"; end
来源：http://loy.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://ymg.mhx1999.top

[G07] 调用父类方法
来源：http://zii.mhx1999.top

Py:   super().greet()
来源：http://jhf.cqqwz.cn

PHP:  parent::greet();
来源：http://pts.fktsv.cn

JS:   super.greet();
来源：http://tjg.guowangkeji.top

TS:   super.greet();
来源：http://qmz.zycfv.cn

Java: super.greet();
来源：http://blf.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://plj.haohaochexian.top

Ruby: super
来源：http://huj.hesvh.cn

C#:   base.Greet();
来源：http://gxk.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://zaf.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ufh.birdmap.top

PHP:  public static function f() {}
来源：http://ytp.hysaishi.cn

JS:   static f() {}
来源：http://qgy.sufxvd.cn

TS:   static f(): void {}
来源：http://fib.chenzaomai.com

Java: static void f() {}
来源：http://iml.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://rwz.hongshengwenyu.top

Ruby: def self.f; end
来源：http://icu.smart0.xyz

C#:   public static void F() {}
来源：http://tdg.guannengcc.top

[G09] 接口 / 抽象类
来源：http://ddu.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://arn.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gaw.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vkx.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://qbp.yj20258888.top

Java: interface Shape { double area(); }
来源：http://oyj.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://ymj.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zyb.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://aqp.jyoumei.cn

[G10] 访问控制
来源：http://kxg.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://xzg.shangyingyoupin.top

PHP:  public / protected / private
来源：http://zzo.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://bda.sweek.top

TS:   public / protected / private
来源：http://qez.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://phk.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xml.jinqigfzy.top

Ruby: public / protected / private
来源：http://nuv.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://xyn.jinqigufen.top

[G11] getter / setter
来源：http://ifv.xuanzx.com

Py:   @property 与 @x.setter
来源：http://lke.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://yiu.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://uui.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://hwe.aizwys.cn

Java: public String getName() { return name; }
来源：http://pic.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvi.xziqi.cn

Ruby: attr_accessor :name
来源：http://ask.yuxming.cn

C#:   public string Name { get; set; }
来源：http://igk.daxiang520.top

[G12] 对象转字符串
来源：http://lpb.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://hqi.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qbp.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://sja.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://xoi.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://prp.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://azo.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://pnd.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://dsv.sweek.top

[G13] 判断对象类型
来源：http://pvw.chenzaomai.com

Py:   isinstance(u, User)
来源：http://ljx.sufxvd.cn

PHP:  $u instanceof User
来源：http://enr.tarul.cn

JS:   u instanceof User
来源：http://aac.zhiwuduotai.top

TS:   u instanceof User
来源：http://yat.cucudq.cn

Java: u instanceof User
来源：http://kcp.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xqh.sysykeji.top

Ruby: u.is_a?(User)
来源：http://ppd.yanxiufei.cn

C#:   u is User
来源：http://blh.hesvh.cn

[G14] 数据类 / record
来源：http://yey.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jsp.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://plp.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uph.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://hbv.havefunace.top

Java: record User(String name, int age) {}
来源：http://npb.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://heq.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://icd.316326.xyz

C#:   record User(string Name, int Age);
来源：http://eiw.zhoulong.xyz

[G15] 枚举
来源：http://ivr.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nnw.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://zdi.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rjc.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bwq.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://clm.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ebp.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://nju.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hki.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://dfz.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xnl.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://bvs.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://kwc.cashguo.top

TS:   Object.entries(obj)
来源：http://kyi.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gon.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uht.yvedp.cn

Ruby: obj.instance_variables
来源：http://dwb.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://poi.cheryme.top

================================================================================
来源：http://akd.hnqzz.top

H. 异常与错误处理
来源：http://bqc.tanke756.top

================================================================================
来源：http://ysv.ydzc1.top

[H01] try / catch 基础
来源：http://zlx.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://prg.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eji.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jtj.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tmr.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zko.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jsj.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yqv.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fyq.yongpay.top

[H02] finally / ensure 收尾
来源：http://apb.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://kno.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dlc.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xzc.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ptx.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://ssb.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hhc.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rjv.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rpo.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://bfc.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://nno.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kfo.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://vlx.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://srw.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ikh.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gfs.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ehz.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zuo.yj20258.top

[H04] 自定义异常类型
来源：http://qgp.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://opn.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://ikd.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://eaf.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://xdg.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://zye.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iuz.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://ttc.pycfn.com

C#:   class MyException : Exception {}
来源：http://qlk.fzhhl.top

[H05] 捕获特定类型
来源：http://lck.guannengcc.top

Py:   except ValueError as e:
来源：http://ama.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gkr.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://vqi.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://off.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://bch.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sxx.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://jfa.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rxs.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://ycb.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://hpy.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ork.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://hru.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://btc.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hln.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://brs.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://ymf.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://tik.52xcode.cn

[H07] 断言
来源：http://csk.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://nqm.jinqigufen.top

PHP:  assert($x > 0);
来源：http://rmk.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://sir.yj20258888.top

TS:   console.assert(x > 0);
来源：http://xdi.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://tjv.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kvp.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eac.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://glm.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://yuh.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://emq.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kto.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://uen.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eys.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yzr.ydzc1.top

Go:   err.Error()
来源：http://khn.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://gtm.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://ztm.gotoacloud.top

[H09] 带错误码的异常
来源：http://dcq.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wpn.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rrx.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nzv.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dbl.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bui.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sdv.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://jdk.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zcx.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://txy.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://grs.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yvx.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mcn.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zfe.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hju.cqqwz.cn

Go:   defer f.Close()
来源：http://nab.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uhh.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://huh.smart0.xyz

================================================================================
来源：http://igv.zdbjq.cn

I. 正则表达式
来源：http://aha.shuidangran.top

================================================================================
来源：http://ymq.birdmap.top

[I01] 判断是否匹配
来源：http://smh.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jxr.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bmx.yj20258888.top

JS:   /\d+/.test(s)
来源：http://fdm.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://awf.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bes.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://klh.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://whg.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ffa.ydjk.org.cn

[I02] 提取所有匹配
来源：http://ucv.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://ivt.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://asw.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gfz.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://duj.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://spg.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qml.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://uup.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nrv.birdmap.top

[I03] 提取捕获分组
来源：http://uwj.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lqc.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://axj.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aab.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fbk.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dbu.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ybk.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ell.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rod.xziqi.cn

[I04] 正则替换
来源：http://zwv.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gsg.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pgb.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://coc.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://ngv.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://zrb.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jxx.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vxd.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iau.hongshengwenyu.top

[I05] 按正则拆分
来源：http://isz.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bnt.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rfa.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://uvs.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://sob.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://mfi.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xsg.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://qpz.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wjn.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vqc.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mjy.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uco.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gjt.chenjidiqi.icu


<!-- 参考信息 -->