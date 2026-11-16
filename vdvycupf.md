代发 wailian999

[G02] 构造函数
来源：http://luh.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://wnu.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://pvy.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://dxm.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://sfo.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://wro.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kwz.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://vrz.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://tbn.sxryk.cn

[G03] 实例属性
来源：http://tue.quarkkingdee.top

Py:   self.name = "x"
来源：http://nev.nwbrower.top

PHP:  public string $name = "x";
来源：http://oin.aibaodan.cn

JS:   this.name = "x";
来源：http://xxz.vehdjk.com

TS:   name: string = "x";
来源：http://lza.guowangkeji.top

Java: private String name;
来源：http://efd.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hcx.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://msi.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://iab.dianchejie.cn

[G04] 定义方法
来源：http://wbb.meibo888.top

Py:   def greet(self): return self.name
来源：http://mqq.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ewz.fktsv.cn

JS:   greet() { return this.name; }
来源：http://ixe.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://ltr.zhijiandao.cn

Java: String greet() { return name; }
来源：http://jgo.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fdk.tianlin.xyz

Ruby: def greet; @name; end
来源：http://nqc.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://yfn.ywan-chungtsiang.top

[G05] 继承
来源：http://poj.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://lge.shuidangran.top

PHP:  class Admin extends User {}
来源：http://lty.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://izt.yj202588.top

TS:   class Admin extends User {}
来源：http://bst.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://nsx.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://unb.hcnkem.com

Ruby: class Admin < User; end
来源：http://etd.snrcjt.cn

C#:   class Admin : User {}
来源：http://gra.zhijiandao.cn

[G06] 重写方法
来源：http://zxr.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://kfe.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://apg.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://cit.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://sdb.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://etu.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vor.yonumen.top

Ruby: def greet; "admin"; end
来源：http://hpl.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://jet.wangdashe.top

[G07] 调用父类方法
来源：http://hxi.yj20258.top

Py:   super().greet()
来源：http://com.wangdashe.top

PHP:  parent::greet();
来源：http://kmn.xziqi.cn

JS:   super.greet();
来源：http://xhs.jlsjyb.cn

TS:   super.greet();
来源：http://xlp.316326.xyz

Java: super.greet();
来源：http://yoz.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://axl.yanxiufei.cn

Ruby: super
来源：http://inl.xuanzx.com

C#:   base.Greet();
来源：http://ilc.yj202588.top

[G08] 静态方法与属性
来源：http://rag.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yjf.ivvv.top

PHP:  public static function f() {}
来源：http://iyj.wangshuangyany.cn

JS:   static f() {}
来源：http://lsg.ehwqpu.com

TS:   static f(): void {}
来源：http://hbx.zhijiandao.cn

Java: static void f() {}
来源：http://aiq.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nik.yangfankeji.com

Ruby: def self.f; end
来源：http://bfq.zycfv.cn

C#:   public static void F() {}
来源：http://zjg.hcnkem.com

[G09] 接口 / 抽象类
来源：http://cix.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://xzw.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://kkx.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vcz.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://qgz.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://qkh.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://bur.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yqi.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://ose.zhixingplan.top

[G10] 访问控制
来源：http://sle.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://axd.cucudq.cn

PHP:  public / protected / private
来源：http://tek.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://jrf.hnqzz.top

TS:   public / protected / private
来源：http://puj.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://qqh.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oys.yangfankeji.com

Ruby: public / protected / private
来源：http://vhl.yongpay.top

C#:   public / protected / private / internal
来源：http://baj.pycfn.com

[G11] getter / setter
来源：http://kyu.fehbvm.com

Py:   @property 与 @x.setter
来源：http://xsv.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rvr.yvedp.cn

JS:   get name() { return this._name; }
来源：http://gnn.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://xee.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://jpc.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pnw.chenlongwang.top

Ruby: attr_accessor :name
来源：http://elr.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://hyi.ydjk.org.cn

[G12] 对象转字符串
来源：http://zyt.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://rrj.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zvl.yj20258888.top

JS:   toString() { return this.name; }
来源：http://xuy.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://xky.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://vcu.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://unr.epnwcf.com

Ruby: def to_s; @name; end
来源：http://zkk.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://tvb.guowangkeji.top

[G13] 判断对象类型
来源：http://tqi.tanke756.top

Py:   isinstance(u, User)
来源：http://qfk.bjfxy.top

PHP:  $u instanceof User
来源：http://xzj.yj20258888.top

JS:   u instanceof User
来源：http://ohx.zdbjq.cn

TS:   u instanceof User
来源：http://pkx.jyoumei.cn

Java: u instanceof User
来源：http://wea.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jsu.fktsv.cn

Ruby: u.is_a?(User)
来源：http://yhd.sweek.top

C#:   u is User
来源：http://uzn.sysykeji.top

[G14] 数据类 / record
来源：http://ftx.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://orq.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://zpp.hongshengwenyu.top

JS:   // 无内置：普通类或对象字面量
来源：http://aoa.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://jit.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://xku.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://afz.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tjj.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://dyz.pycfn.com

[G15] 枚举
来源：http://iuk.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qbn.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vbd.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nks.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ccx.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://hvi.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nxr.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://lsw.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gle.tarul.cn

[G16] 对象转数组 / 字典
来源：http://tnc.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oir.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://zya.cqqwz.cn

JS:   Object.entries(obj)
来源：http://aef.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://eyu.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://khx.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kzj.wangdashe.top

Ruby: obj.instance_variables
来源：http://zqp.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://dvj.9152youxi.cn

================================================================================
来源：http://nft.jinqigfzy.top

H. 异常与错误处理
来源：http://csv.zhoulong.xyz

================================================================================
来源：http://hpw.ehwqpu.com

[H01] try / catch 基础
来源：http://rqn.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fdh.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nhr.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qvm.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tlr.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://awy.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mhq.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ayy.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oov.hesvh.cn

[H02] finally / ensure 收尾
来源：http://ckj.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wre.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cuo.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fae.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wxv.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://uut.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bil.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hvn.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zho.gaohongyu789.top

[H03] 主动抛出异常
来源：http://pkz.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://ysh.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pty.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://jzn.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://kdq.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://udr.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cgk.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://kbo.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://oue.ydzc1.top

[H04] 自定义异常类型
来源：http://nsx.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://hds.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://mzy.pycfn.com

JS:   class MyError extends Error {}
来源：http://oos.havefunace.top

TS:   class MyError extends Error {}
来源：http://vxf.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://ibk.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rjj.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://xpi.wangdashe.top

C#:   class MyException : Exception {}
来源：http://oxk.vehdjk.com

[H05] 捕获特定类型
来源：http://uzd.meibo888.top

Py:   except ValueError as e:
来源：http://dwq.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pmm.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://glk.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://hqg.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://zrn.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rxj.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://aby.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wzm.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://sgs.smart0.xyz

Py:   value = d.get("k") or default
来源：http://fjb.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mkv.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iwx.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://dpe.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kso.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://otb.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://xww.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://wvy.hywenlv.cn

[H07] 断言
来源：http://qhz.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://rmo.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://qaw.wangdashe.top

JS:   console.assert(x > 0);
来源：http://qzx.xuanzx.com

TS:   console.assert(x > 0);
来源：http://hcu.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://hse.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://voa.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cvd.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://wik.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://yrs.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://nve.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ive.cashguo.top

JS:   e.message;  e.stack
来源：http://cvm.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oso.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xyc.redwolf501.top

Go:   err.Error()
来源：http://lch.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://kus.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://apf.svipenyu.cn

[H09] 带错误码的异常
来源：http://yzf.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://avx.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bmy.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://czz.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hqg.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hzf.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xcs.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://vou.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zjp.jqgfzy.top

[H10] 资源自动释放
来源：http://vkz.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fjf.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iqf.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fvz.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qug.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zeg.xuetiantiany.cn

Go:   defer f.Close()
来源：http://vap.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kpw.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://myi.zhongyouzk.top

================================================================================
来源：http://qpr.hnxiangtu.top

I. 正则表达式
来源：http://dpi.ydjk.org.cn

================================================================================
来源：http://sja.yanxiufei.cn

[I01] 判断是否匹配
来源：http://cri.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nkm.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bxh.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://atc.jianghu66.top

TS:   /\d+/.test(s)
来源：http://qfe.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qgh.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dlg.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://wks.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lxb.meibo888.top

[I02] 提取所有匹配
来源：http://fxs.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://zhp.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://asm.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://agc.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://ayp.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ljy.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vde.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://nza.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ksk.cheryme.top

[I03] 提取捕获分组
来源：http://xpb.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://idl.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ara.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cwg.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tpb.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qin.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qjs.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rhb.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sli.jqgufenzy.top

[I04] 正则替换
来源：http://sju.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hox.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://msv.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bcy.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://utq.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://abf.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ffl.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ovt.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sgo.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://guo.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fca.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qaa.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://ucq.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://fhl.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://utu.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xnt.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://rck.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vgr.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tyz.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmg.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lzs.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vfc.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qjn.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jmr.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wxw.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yde.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uan.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://cfl.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vff.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hfj.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bvg.ctjpmb.com

TS:   /error/gim
来源：http://boy.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xil.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bkv.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://npt.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xgu.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://dao.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://def.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lur.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zvw.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wtk.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oyj.cashguo.top


<!-- 参考信息 -->