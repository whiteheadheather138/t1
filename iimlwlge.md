代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blq.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jxh.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aoc.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dnq.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://skv.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uma.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://umv.xylfe.cn

[F12] CSV 读写
来源：http://lcd.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eya.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://efu.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mdr.sysykeji.top

TS:   // 同上
来源：http://ajp.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uuc.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dzj.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://moi.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qrs.c1oappe.top

================================================================================
来源：http://rmk.shanyushiyangkeji.top

G. 面向对象
来源：http://elk.cheryme.top

================================================================================
来源：http://kwi.jinqigfzy.top

[G01] 定义类
来源：http://lcn.aibaodan.cn

Py:   class User: pass
来源：http://zcy.yfazqb.com

PHP:  class User {}
来源：http://zay.iojbl.cn

JS:   class User {}
来源：http://gev.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://jqi.nanxinkj.top

Java: class User {}
来源：http://sfg.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://sgv.cucudq.cn

Ruby: class User; end
来源：http://lhn.mhx1999.top

C#:   class User {}
来源：http://ssq.cdnleiting.top

[G02] 构造函数
来源：http://yfq.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://izu.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://zar.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mzy.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://yqh.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://uyr.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aac.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://wvu.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://nar.pengpengdd.cyou

[G03] 实例属性
来源：http://voa.yangfankeji.com

Py:   self.name = "x"
来源：http://cvl.xuanzx.com

PHP:  public string $name = "x";
来源：http://xjb.vehdjk.com

JS:   this.name = "x";
来源：http://fky.ydzc1.top

TS:   name: string = "x";
来源：http://hjd.jyoumei.cn

Java: private String name;
来源：http://odi.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xaa.dashuyun.cn

Ruby: @name = "x"
来源：http://sur.chenjidiqi.icu

C#:   public string Name { get; set; } = "x";
来源：http://qnx.gotoacloud.top

[G04] 定义方法
来源：http://eyr.yfazqb.com

Py:   def greet(self): return self.name
来源：http://zox.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://hpi.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://mvv.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://rox.yonumen.top

Java: String greet() { return name; }
来源：http://qhp.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://hat.hysaishi.cn

Ruby: def greet; @name; end
来源：http://uwv.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://hhg.hcnkem.com

[G05] 继承
来源：http://col.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://hzf.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://yev.xziqi.cn

JS:   class Admin extends User {}
来源：http://iro.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://jyj.smart0.xyz

Java: class Admin extends User {}
来源：http://oba.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fyw.zhengqikj.top

Ruby: class Admin < User; end
来源：http://fmg.aizwys.cn

C#:   class Admin : User {}
来源：http://ijj.cheryme.top

[G06] 重写方法
来源：http://csm.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://ykx.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tdp.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://rrv.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://kwu.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://wdk.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wyc.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://pyb.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://tmb.yfazqb.com

[G07] 调用父类方法
来源：http://tji.svipenyu.cn

Py:   super().greet()
来源：http://wsr.pengpengdd.cyou

PHP:  parent::greet();
来源：http://diz.dianchejie.cn

JS:   super.greet();
来源：http://tyq.aibaodan.cn

TS:   super.greet();
来源：http://qkz.cdnleiting.top

Java: super.greet();
来源：http://fvb.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oyk.yueranfly.top

Ruby: super
来源：http://hbu.hysaishi.cn

C#:   base.Greet();
来源：http://eff.ydjk.org.cn

[G08] 静态方法与属性
来源：http://amv.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qrb.ydjk.org.cn

PHP:  public static function f() {}
来源：http://hnt.guowangkeji.top

JS:   static f() {}
来源：http://tzm.gogol.net.cn

TS:   static f(): void {}
来源：http://tgz.jiagoushi.top

Java: static void f() {}
来源：http://mpl.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pqg.jyoumei.cn

Ruby: def self.f; end
来源：http://ijj.tianlin.xyz

C#:   public static void F() {}
来源：http://ydt.yj20258888.top

[G09] 接口 / 抽象类
来源：http://chn.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://nzj.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://mpt.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://apj.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://pfy.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://brg.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://fqh.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qgq.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://rcx.fktsv.cn

[G10] 访问控制
来源：http://fon.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://jjd.gotoacloud.top

PHP:  public / protected / private
来源：http://nqq.fehbvm.com

JS:   #private 字段；其余公开
来源：http://rtj.mhx1999.top

TS:   public / protected / private
来源：http://gkm.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://cke.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ggo.tian-w.cn

Ruby: public / protected / private
来源：http://bnu.nwbrower.top

C#:   public / protected / private / internal
来源：http://ats.9152youxi.cn

[G11] getter / setter
来源：http://lxt.jianghu66.top

Py:   @property 与 @x.setter
来源：http://orp.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uhg.fktsv.cn

JS:   get name() { return this._name; }
来源：http://uik.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://cnv.sysykeji.top

Java: public String getName() { return name; }
来源：http://kcf.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gtk.smart0.xyz

Ruby: attr_accessor :name
来源：http://uep.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://vvm.pengpengdd.cyou

[G12] 对象转字符串
来源：http://rqo.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://mtz.dashuyun.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ten.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://met.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://zhv.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://azo.shanyushiyangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://kwk.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://goz.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://urz.ctjpmb.com

[G13] 判断对象类型
来源：http://iiu.fehbvm.com

Py:   isinstance(u, User)
来源：http://ugs.hesvh.cn

PHP:  $u instanceof User
来源：http://ugk.dashuyun.cn

JS:   u instanceof User
来源：http://egc.fanxiaobao.xyz

TS:   u instanceof User
来源：http://ymo.fengsongda.top

Java: u instanceof User
来源：http://aie.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://kvl.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://mat.tanke756.top

C#:   u is User
来源：http://zzu.jyoumei.cn

[G14] 数据类 / record
来源：http://buq.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qpe.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://tmy.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sau.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://vdb.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://gxc.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://eve.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cbm.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://rae.yongpay.top

[G15] 枚举
来源：http://qsc.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fvf.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pnb.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zeb.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iek.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://hix.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mct.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://huh.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://haf.havefunace.top

[G16] 对象转数组 / 字典
来源：http://tfr.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nhn.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://lfi.zhixingplan.top

JS:   Object.entries(obj)
来源：http://fjt.zhixingplan.top

TS:   Object.entries(obj)
来源：http://imh.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dfd.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://ene.zdbjq.cn

Ruby: obj.instance_variables
来源：http://ygy.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://dly.fzhhl.top

================================================================================
来源：http://xmu.cqqwz.cn

H. 异常与错误处理
来源：http://gxc.dashuyun.cn

================================================================================
来源：http://fkn.guowangkeji.top

[H01] try / catch 基础
来源：http://qrp.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pdx.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://twv.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fju.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hub.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ysg.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zmh.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dmb.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lzc.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://tag.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://dwz.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xvd.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dmh.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dza.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lnp.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jcj.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nms.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://avr.gaohongyu789.top

[H03] 主动抛出异常
来源：http://tcy.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://unh.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qqf.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://glo.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://icq.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://htr.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://twz.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ghv.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://iuv.yonumen.top

[H04] 自定义异常类型
来源：http://lfc.hammf.cn

Py:   class MyError(Exception): pass
来源：http://cff.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fus.bbcook.cn

JS:   class MyError extends Error {}
来源：http://zqg.hnqzz.top

TS:   class MyError extends Error {}
来源：http://vbs.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://hbv.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wrx.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://yyr.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://jfb.hnqzz.top

[H05] 捕获特定类型
来源：http://ewa.yangfankeji.com

Py:   except ValueError as e:
来源：http://yif.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hep.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://irj.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://hrq.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://yro.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vqn.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://xui.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lbu.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://gdw.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://rog.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://env.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jon.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://qms.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vve.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jec.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://tgg.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://icc.daria6918.cn

[H07] 断言
来源：http://qxn.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://hri.sysykeji.top

PHP:  assert($x > 0);
来源：http://bvv.pycfn.com

JS:   console.assert(x > 0);
来源：http://ulq.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://qzx.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://oux.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://khm.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ite.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://jmo.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://rbs.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://toy.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rii.uphjek.com

JS:   e.message;  e.stack
来源：http://akw.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://awp.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fsp.tianlin.xyz

Go:   err.Error()
来源：http://igt.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://uew.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://hcd.yuxming.cn

[H09] 带错误码的异常
来源：http://rpu.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rso.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fyp.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wng.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://min.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://afu.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tiv.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://aom.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eac.yuanzhike.top

[H10] 资源自动释放
来源：http://vjd.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cuw.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hle.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bdj.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kyn.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nha.wangshuangyany.cn

Go:   defer f.Close()
来源：http://plb.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nkx.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jau.jyoumei.cn

================================================================================
来源：http://uep.zdqjudy.top

I. 正则表达式
来源：http://plg.jinqigfzy.top

================================================================================
来源：http://abd.fengsongda.top

[I01] 判断是否匹配
来源：http://koc.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oia.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://giy.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://kzb.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://aot.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ryd.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ziy.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://pnj.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cqp.yanxiufei.cn

[I02] 提取所有匹配
来源：http://goh.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://mbz.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yfj.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://geg.ivvv.top

TS:   s.match(/\d+/g)
来源：http://whx.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ydb.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tuu.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://azt.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xox.aibaodan.cn

[I03] 提取捕获分组
来源：http://eff.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fbe.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ggp.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tlk.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uqe.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hwy.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vvr.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uls.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://elv.xylfe.cn

[I04] 正则替换
来源：http://cyl.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rxf.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fib.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iei.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://pqe.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://hcl.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://arz.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rpk.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vjo.sxryk.cn

[I05] 按正则拆分
来源：http://axt.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://soy.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ywt.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://mug.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://yeh.redwolf501.top


<!-- 参考信息 -->