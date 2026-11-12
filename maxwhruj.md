代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uzp.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hau.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rly.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wbx.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hbt.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gym.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eva.yfazqb.com

[F12] CSV 读写
来源：http://qxp.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dos.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dly.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cpp.ehwqpu.com

TS:   // 同上
来源：http://ssj.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://smb.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qmi.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rtr.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tre.fehbvm.com

================================================================================
来源：http://tka.ctjpmb.com

G. 面向对象
来源：http://gvs.birdmap.top

================================================================================
来源：http://dst.hywenlv.cn

[G01] 定义类
来源：http://rtt.pengpengdd.cyou

Py:   class User: pass
来源：http://ysm.feifeiyinyue.top

PHP:  class User {}
来源：http://bty.xingfuxueyuan.xyz

JS:   class User {}
来源：http://eis.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://alk.yj20258888.top

Java: class User {}
来源：http://bsh.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://yly.quarkkingdee.top

Ruby: class User; end
来源：http://wrp.cucudq.cn

C#:   class User {}
来源：http://epr.fanxiaobao.xyz

[G02] 构造函数
来源：http://kja.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://oxg.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://pji.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://jum.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://tlm.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://inu.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iil.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://law.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://xuh.yj20258888.top

[G03] 实例属性
来源：http://yri.sjlbkw.cn

Py:   self.name = "x"
来源：http://ifo.yfazqb.com

PHP:  public string $name = "x";
来源：http://pig.birdmap.top

JS:   this.name = "x";
来源：http://flo.cdnleiting.top

TS:   name: string = "x";
来源：http://jov.pengpengdd.cyou

Java: private String name;
来源：http://lmv.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hdd.yongpay.top

Ruby: @name = "x"
来源：http://put.ywan-chungtsiang.top

C#:   public string Name { get; set; } = "x";
来源：http://jkr.ivvv.top

[G04] 定义方法
来源：http://snn.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://xhw.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nsz.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://jui.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://vyo.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://fwy.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://knb.sxryk.cn

Ruby: def greet; @name; end
来源：http://tjw.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://fco.c1oappe.top

[G05] 继承
来源：http://anw.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://qpc.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://qdc.hammf.cn

JS:   class Admin extends User {}
来源：http://njn.pycfn.com

TS:   class Admin extends User {}
来源：http://zma.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://ynn.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hgx.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://nuo.dianchejie.cn

C#:   class Admin : User {}
来源：http://vhr.xuanzx.com

[G06] 重写方法
来源：http://xug.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://kio.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://klz.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://wib.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://gnl.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://bhf.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tal.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://uat.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://fpi.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://elk.yuxming.cn

Py:   super().greet()
来源：http://ugp.sufxvd.cn

PHP:  parent::greet();
来源：http://crp.aizwys.cn

JS:   super.greet();
来源：http://xqj.hywenlv.cn

TS:   super.greet();
来源：http://rfy.fehbvm.com

Java: super.greet();
来源：http://vhb.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nke.chenlongwang.top

Ruby: super
来源：http://cus.jiagoushi.top

C#:   base.Greet();
来源：http://ays.ybcxt.top

[G08] 静态方法与属性
来源：http://jlr.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vrp.havefunace.top

PHP:  public static function f() {}
来源：http://dmo.zdbjq.cn

JS:   static f() {}
来源：http://pez.sufxvd.cn

TS:   static f(): void {}
来源：http://nff.xuanzx.com

Java: static void f() {}
来源：http://kdu.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nnf.ehwqpu.com

Ruby: def self.f; end
来源：http://kdi.jyoumei.cn

C#:   public static void F() {}
来源：http://ypa.nwbrower.top

[G09] 接口 / 抽象类
来源：http://upq.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://ped.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://ach.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://rhc.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://huh.sxryk.cn

Java: interface Shape { double area(); }
来源：http://btw.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://pne.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pul.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://air.yuanzhike.top

[G10] 访问控制
来源：http://zsp.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://ivp.ybcxt.top

PHP:  public / protected / private
来源：http://xiw.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://cmn.yonumen.top

TS:   public / protected / private
来源：http://yof.yj202588.top

Java: public / protected / private / 默认包级
来源：http://qws.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://roz.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://qpo.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://fqj.dianchejie.cn

[G11] getter / setter
来源：http://hej.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://dnr.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uzj.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://znr.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://gmm.yuxming.cn

Java: public String getName() { return name; }
来源：http://zwz.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ttu.yonumen.top

Ruby: attr_accessor :name
来源：http://mjc.daxiang520.top

C#:   public string Name { get; set; }
来源：http://ikq.havefunace.top

[G12] 对象转字符串
来源：http://naj.tanke756.top

Py:   def __str__(self): return self.name
来源：http://tda.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nrq.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://vzo.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://sam.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://jkr.epnwcf.com

Go:   func (u User) String() string { return u.Name }
来源：http://uyd.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://nuw.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://uso.pengpengdd.cyou

[G13] 判断对象类型
来源：http://jwr.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://dxp.yongpay.top

PHP:  $u instanceof User
来源：http://jty.chenlongwang.top

JS:   u instanceof User
来源：http://xfp.zycfv.cn

TS:   u instanceof User
来源：http://rwi.birdmap.top

Java: u instanceof User
来源：http://ipr.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ipw.fehbvm.com

Ruby: u.is_a?(User)
来源：http://ktq.haohaochexian.top

C#:   u is User
来源：http://hqw.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://sho.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zif.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://pqi.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mju.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://iwe.feifeiyinyue.top

Java: record User(String name, int age) {}
来源：http://pff.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://bpn.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hlj.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://ebi.hysaishi.cn

[G15] 枚举
来源：http://bdv.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://soz.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rdl.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jby.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cwk.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://ivj.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wxd.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://yhf.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rjk.ivvv.top

[G16] 对象转数组 / 字典
来源：http://egs.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yfj.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://ava.ctjpmb.com

JS:   Object.entries(obj)
来源：http://jjw.nanxinkj.top

TS:   Object.entries(obj)
来源：http://rgm.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xkq.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://akd.andypj.xyz

Ruby: obj.instance_variables
来源：http://mtz.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://psk.redwolf501.top

================================================================================
来源：http://gnp.zhijiandao.cn

H. 异常与错误处理
来源：http://xbk.ppjwa.cn

================================================================================
来源：http://exq.sysykeji.top

[H01] try / catch 基础
来源：http://isf.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zrm.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lgj.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kip.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hfo.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mld.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://egg.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zqa.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dnb.xuanzx.com

[H02] finally / ensure 收尾
来源：http://iem.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mvp.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mzh.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mgi.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yko.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yae.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vmg.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tnk.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mzi.daxiang520.top

[H03] 主动抛出异常
来源：http://bux.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://ket.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vba.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://dij.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://eff.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ico.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://erl.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://poc.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://hoe.jqgufenzy.top

[H04] 自定义异常类型
来源：http://zrf.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://feb.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://njl.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://qib.gzhubu.top

TS:   class MyError extends Error {}
来源：http://qnm.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://lwc.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fuf.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://vdl.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://bts.yj202588.top

[H05] 捕获特定类型
来源：http://peb.cqqwz.cn

Py:   except ValueError as e:
来源：http://ljz.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nwf.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://ukq.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://fba.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://bbt.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rul.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://zen.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://umn.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://ern.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://eqo.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bzm.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://jay.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://lkx.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tqc.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://atu.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://txv.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://rtp.yfazqb.com

[H07] 断言
来源：http://ocl.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://ufv.zdbjq.cn

PHP:  assert($x > 0);
来源：http://eyk.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://avs.aizwys.cn

TS:   console.assert(x > 0);
来源：http://wnf.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://gtl.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uxw.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://qwi.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://dts.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://wlh.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://uic.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jym.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://oes.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tcb.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jly.nwbrower.top

Go:   err.Error()
来源：http://vii.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://anx.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://nik.gzhubu.top

[H09] 带错误码的异常
来源：http://jiv.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://odt.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xzh.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jgi.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://owo.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mko.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kaq.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ttw.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rdu.vqdsnc.cn

[H10] 资源自动释放
来源：http://lxw.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lvc.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xxs.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qyi.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nuu.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gaf.0kj1m.cn

Go:   defer f.Close()
来源：http://oje.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fdv.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oos.cheryme.top

================================================================================
来源：http://taw.yongpay.top

I. 正则表达式
来源：http://pbp.vehdjk.com

================================================================================
来源：http://abh.sxryk.cn

[I01] 判断是否匹配
来源：http://aar.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://amx.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://swl.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://ewb.uphjek.com

TS:   /\d+/.test(s)
来源：http://bzd.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fuf.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ewb.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://mnd.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nhs.dianchejie.cn

[I02] 提取所有匹配
来源：http://ehh.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://deu.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zja.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xfa.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://hzb.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yeb.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://afp.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://wlp.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ceh.gaohongyu789.top

[I03] 提取捕获分组
来源：http://bng.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mzy.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rwe.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sdw.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://inc.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ezv.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://otr.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vut.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aqg.sysykeji.top

[I04] 正则替换
来源：http://ofn.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://tyk.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kuh.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://nrm.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iry.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://irj.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://lfh.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nut.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nix.jqgfzy.top

[I05] 按正则拆分
来源：http://ikr.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cpc.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://peh.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://dox.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://xbs.zhongyouzk.top


<!-- 参考信息 -->