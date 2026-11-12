代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rju.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://soc.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ccx.daria6918.cn

[F12] CSV 读写
来源：http://ffn.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qtu.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vut.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mfq.meibo888.top

TS:   // 同上
来源：http://baz.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tjj.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mau.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ciy.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ehc.fanxiaobao.xyz

================================================================================
来源：http://ewa.c1oappe.top

G. 面向对象
来源：http://fnh.chenlongwang.top

================================================================================
来源：http://lgz.jinqigufen.top

[G01] 定义类
来源：http://wyl.shzxlz.cn

Py:   class User: pass
来源：http://iwl.tianlin.xyz

PHP:  class User {}
来源：http://bpq.guowangkeji.top

JS:   class User {}
来源：http://gvs.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://hvi.yonumen.top

Java: class User {}
来源：http://ofg.sweek.top

Go:   type User struct { Name string }
来源：http://huf.zhoulong.xyz

Ruby: class User; end
来源：http://lzb.dianchejie.cn

C#:   class User {}
来源：http://spe.dianchejie.cn

[G02] 构造函数
来源：http://wfd.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://kvo.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://dkb.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://kbm.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://zow.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://ulg.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zhv.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://bck.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://ljk.shzxlz.cn

[G03] 实例属性
来源：http://uxt.wangshuangyany.cn

Py:   self.name = "x"
来源：http://dlk.meibo888.top

PHP:  public string $name = "x";
来源：http://rvl.yuxming.cn

JS:   this.name = "x";
来源：http://yid.svipenyu.cn

TS:   name: string = "x";
来源：http://fua.fanxiaobao.xyz

Java: private String name;
来源：http://ect.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://auf.redwolf501.top

Ruby: @name = "x"
来源：http://ljd.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://ugm.sjlbkw.cn

[G04] 定义方法
来源：http://jtx.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://bpf.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xpr.xziqi.cn

JS:   greet() { return this.name; }
来源：http://dqw.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://hfx.bjfxy.top

Java: String greet() { return name; }
来源：http://rfd.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rbf.daxiang520.top

Ruby: def greet; @name; end
来源：http://lyd.pycfn.com

C#:   public string Greet() => Name;
来源：http://slu.hongshengwenyu.top

[G05] 继承
来源：http://rhp.daxiang520.top

Py:   class Admin(User): pass
来源：http://dyl.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://xbo.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://xlo.cdnleiting.top

TS:   class Admin extends User {}
来源：http://zsn.andypj.xyz

Java: class Admin extends User {}
来源：http://bcy.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bxb.gotoacloud.top

Ruby: class Admin < User; end
来源：http://pwb.havefunace.top

C#:   class Admin : User {}
来源：http://tft.shzxlz.cn

[G06] 重写方法
来源：http://bsq.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://cwk.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dde.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://wuo.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://spn.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://onl.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://txv.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://yqa.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://esk.hysaishi.cn

[G07] 调用父类方法
来源：http://hrh.c1oappe.top

Py:   super().greet()
来源：http://oww.sxryk.cn

PHP:  parent::greet();
来源：http://fvr.pengpengdd.cyou

JS:   super.greet();
来源：http://eur.sysykeji.top

TS:   super.greet();
来源：http://tzp.andypj.xyz

Java: super.greet();
来源：http://hgr.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vsg.ppjwa.cn

Ruby: super
来源：http://qaj.meibo888.top

C#:   base.Greet();
来源：http://nay.hnxiangtu.top

[G08] 静态方法与属性
来源：http://pjp.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bnj.daria6918.cn

PHP:  public static function f() {}
来源：http://uzy.yonumen.top

JS:   static f() {}
来源：http://dat.epnwcf.com

TS:   static f(): void {}
来源：http://jcf.ppjwa.cn

Java: static void f() {}
来源：http://yvq.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://umh.wangdashe.top

Ruby: def self.f; end
来源：http://cic.fzhhl.top

C#:   public static void F() {}
来源：http://tzm.daria6918.cn

[G09] 接口 / 抽象类
来源：http://wob.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://ibz.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://wwy.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bnz.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://mmn.yj20258888.top

Java: interface Shape { double area(); }
来源：http://gmf.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://lqb.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uix.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://bss.bjfxy.top

[G10] 访问控制
来源：http://fcf.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ris.jqgufenzy.top

PHP:  public / protected / private
来源：http://bgi.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://bvu.xziqi.cn

TS:   public / protected / private
来源：http://byr.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://elf.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://fna.sysykeji.top

Ruby: public / protected / private
来源：http://pjk.tianlin.xyz

C#:   public / protected / private / internal
来源：http://eze.andypj.xyz

[G11] getter / setter
来源：http://gob.fktsv.cn

Py:   @property 与 @x.setter
来源：http://ixj.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://aow.redwolf501.top

JS:   get name() { return this._name; }
来源：http://bjq.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://xpl.yonumen.top

Java: public String getName() { return name; }
来源：http://bjc.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hit.yj20258.top

Ruby: attr_accessor :name
来源：http://iha.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://fve.fengsongda.top

[G12] 对象转字符串
来源：http://qas.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://mwd.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vfp.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://ltc.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://nil.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://ong.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://iof.ydzc1.top

Ruby: def to_s; @name; end
来源：http://obe.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://tsr.gaohongyu789.top

[G13] 判断对象类型
来源：http://cvc.tian-w.cn

Py:   isinstance(u, User)
来源：http://fbq.meibo888.top

PHP:  $u instanceof User
来源：http://qdw.wangshuangyany.cn

JS:   u instanceof User
来源：http://ftk.jyoumei.cn

TS:   u instanceof User
来源：http://jzn.jinyuanbaomall.cn

Java: u instanceof User
来源：http://fhu.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wiu.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://xhz.shzxlz.cn

C#:   u is User
来源：http://ijd.hfpthk.cn

[G14] 数据类 / record
来源：http://dwt.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://snb.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://caf.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mqv.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://qve.pycfn.com

Java: record User(String name, int age) {}
来源：http://wro.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://qjf.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rve.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://unp.hywenlv.cn

[G15] 枚举
来源：http://ccc.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://evp.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yzf.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pyy.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yzt.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://ivv.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mef.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://npr.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mok.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://vgo.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gst.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://ndj.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://scc.ybcxt.top

TS:   Object.entries(obj)
来源：http://jyf.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ezr.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ydp.tarul.cn

Ruby: obj.instance_variables
来源：http://vts.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://ayp.hcnkem.com

================================================================================
来源：http://ygu.yueranfly.top

H. 异常与错误处理
来源：http://nlm.xylfe.cn

================================================================================
来源：http://skx.jinqigfzy.top

[H01] try / catch 基础
来源：http://oue.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gxo.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xms.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tys.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jrv.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://knq.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pcj.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xpv.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wll.yfazqb.com

[H02] finally / ensure 收尾
来源：http://ydz.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://iou.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://snv.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ebx.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gqx.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://cop.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iwi.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sas.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wde.c1oappe.top

[H03] 主动抛出异常
来源：http://fro.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://szc.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lwl.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://zzv.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://roc.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://frk.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://adt.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ytp.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://rad.yueranfly.top

[H04] 自定义异常类型
来源：http://nfg.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://lqw.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wbp.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://qll.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://tmw.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://zaz.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hik.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://baa.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://vnm.andypj.xyz

[H05] 捕获特定类型
来源：http://qvd.nanxuanxn.top

Py:   except ValueError as e:
来源：http://sdb.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yyb.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://mva.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://ugx.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://reb.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rza.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://kcv.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wmv.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://zgf.wangdashe.top

Py:   value = d.get("k") or default
来源：http://rjz.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mna.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://ivo.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://fvg.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eog.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xyo.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://cxe.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://xxx.zdqjudy.top

[H07] 断言
来源：http://ezm.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://iyw.yj202588.top

PHP:  assert($x > 0);
来源：http://cud.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://ivy.bjfxy.top

TS:   console.assert(x > 0);
来源：http://fqz.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://umx.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gpx.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://qhf.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://rda.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://zkj.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://ngr.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fxr.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://jfz.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ykb.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hsd.fengsongda.top

Go:   err.Error()
来源：http://dbq.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://btm.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://umh.bjfxy.top

[H09] 带错误码的异常
来源：http://jme.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zrw.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://guf.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vov.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qyx.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://edv.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hcp.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mmc.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://oax.zhijiandao.cn

[H10] 资源自动释放
来源：http://qyf.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pdx.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mwv.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xrp.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tkg.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vgd.hnxiangtu.top

Go:   defer f.Close()
来源：http://npg.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://adn.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://onq.guannengcc.top

================================================================================
来源：http://gck.vehdjk.com

I. 正则表达式
来源：http://zlw.aibaodan.cn

================================================================================
来源：http://yox.aizwys.cn

[I01] 判断是否匹配
来源：http://nlk.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mll.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qjt.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://wpo.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://qlg.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://psl.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://diy.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://kqp.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jpw.sysykeji.top

[I02] 提取所有匹配
来源：http://edo.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://rpe.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vuy.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jjn.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://utd.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hut.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rxh.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://sfz.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xcm.dianchejie.cn

[I03] 提取捕获分组
来源：http://ptl.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ojl.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rtj.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zay.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mkr.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://evg.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uyb.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jem.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zmt.hnxiangtu.top

[I04] 正则替换
来源：http://irg.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://giq.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lqu.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://mqr.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://ern.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://qvs.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://gda.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://cbm.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://duo.yfazqb.com

[I05] 按正则拆分
来源：http://bmi.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ucp.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uji.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://cek.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://fab.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://qrg.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jlh.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ilr.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dkt.meibo888.top


<!-- 参考信息 -->