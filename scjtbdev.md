代发 wailian999

Py:   class User: pass
来源：http://obx.nanxuanxn.top

PHP:  class User {}
来源：http://zxx.chenjidiqi.icu

JS:   class User {}
来源：http://khm.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://uft.feifeiyinyue.top

Java: class User {}
来源：http://vnb.yfazqb.com

Go:   type User struct { Name string }
来源：http://tdk.fzhhl.top

Ruby: class User; end
来源：http://hta.tarul.cn

C#:   class User {}
来源：http://szr.gaohongyu789.top

[G02] 构造函数
来源：http://fdl.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://dwo.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://xja.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://gng.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://wuh.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://fyu.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kye.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://sqx.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://plq.vehdjk.com

[G03] 实例属性
来源：http://rgd.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://wyg.jyoumei.cn

PHP:  public string $name = "x";
来源：http://tht.yuxming.cn

JS:   this.name = "x";
来源：http://wgr.chenjidiqi.icu

TS:   name: string = "x";
来源：http://tua.shangyingyoupin.top

Java: private String name;
来源：http://jyo.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pvo.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://wya.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://qaw.chenlongwang.top

[G04] 定义方法
来源：http://gim.fktsv.cn

Py:   def greet(self): return self.name
来源：http://ijj.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://avw.daxiang520.top

JS:   greet() { return this.name; }
来源：http://cui.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://vyj.zhoulong.xyz

Java: String greet() { return name; }
来源：http://kqu.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bbx.yj20258888.top

Ruby: def greet; @name; end
来源：http://ctn.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://eux.uphjek.com

[G05] 继承
来源：http://crk.guannengcc.top

Py:   class Admin(User): pass
来源：http://zzv.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://gda.ctjpmb.com

JS:   class Admin extends User {}
来源：http://hzj.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://ecc.52xcode.cn

Java: class Admin extends User {}
来源：http://jdv.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dmq.yongpay.top

Ruby: class Admin < User; end
来源：http://dme.vqdsnc.cn

C#:   class Admin : User {}
来源：http://qtc.316326.xyz

[G06] 重写方法
来源：http://tbo.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://ert.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zed.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://msu.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://pxz.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://isp.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mxv.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://pnc.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://kwe.gzhubu.top

[G07] 调用父类方法
来源：http://wec.hnqzz.top

Py:   super().greet()
来源：http://nva.dashuyun.cn

PHP:  parent::greet();
来源：http://ier.tanke756.top

JS:   super.greet();
来源：http://dqu.havefunace.top

TS:   super.greet();
来源：http://xiz.pengpengdd.cyou

Java: super.greet();
来源：http://lad.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kmz.mhx1999.top

Ruby: super
来源：http://rkm.yonumen.top

C#:   base.Greet();
来源：http://qvu.fktsv.cn

[G08] 静态方法与属性
来源：http://vox.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://usd.zhengqikj.top

PHP:  public static function f() {}
来源：http://dbx.yueranfly.top

JS:   static f() {}
来源：http://ppd.zhoulong.xyz

TS:   static f(): void {}
来源：http://jlp.xuanzx.com

Java: static void f() {}
来源：http://ict.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oas.hnqzz.top

Ruby: def self.f; end
来源：http://vwg.yj202588.top

C#:   public static void F() {}
来源：http://npd.wangdashe.top

[G09] 接口 / 抽象类
来源：http://ykb.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://omh.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://vhk.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://kdp.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://igv.bjfxy.top

Java: interface Shape { double area(); }
来源：http://ebr.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://jch.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cvj.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://tre.chenlongwang.top

[G10] 访问控制
来源：http://svy.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://qlb.birdmap.top

PHP:  public / protected / private
来源：http://sya.daria6918.cn

JS:   #private 字段；其余公开
来源：http://lke.shzxlz.cn

TS:   public / protected / private
来源：http://inb.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://vru.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://jol.jiagoushi.top

Ruby: public / protected / private
来源：http://dxr.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://uuq.nwbrower.top

[G11] getter / setter
来源：http://eok.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://jgn.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fpj.yj202588.top

JS:   get name() { return this._name; }
来源：http://ncv.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://ayi.xylfe.cn

Java: public String getName() { return name; }
来源：http://hiy.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://wgn.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://mub.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://bif.nanxinkj.top

[G12] 对象转字符串
来源：http://qtj.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://eow.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ahk.yongpay.top

JS:   toString() { return this.name; }
来源：http://xqo.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://tbp.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://szv.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://ixo.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://eht.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://iey.yanxiufei.cn

[G13] 判断对象类型
来源：http://nsh.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://kme.epnwcf.com

PHP:  $u instanceof User
来源：http://mqz.epnwcf.com

JS:   u instanceof User
来源：http://sdu.meibo888.top

TS:   u instanceof User
来源：http://wgq.jinqigufen.top

Java: u instanceof User
来源：http://jho.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pia.sweek.top

Ruby: u.is_a?(User)
来源：http://aup.jianghu66.top

C#:   u is User
来源：http://nhm.pycfn.com

[G14] 数据类 / record
来源：http://npg.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aod.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://bfb.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://fig.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://lyo.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://ebb.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://gyk.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qru.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://qxg.quarkkingdee.top

[G15] 枚举
来源：http://mgb.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dwf.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rdc.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xyv.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://htq.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://rdp.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wfv.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://gpx.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rnk.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://jsc.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ucd.hammf.cn

PHP:  get_object_vars($obj);
来源：http://pgp.andypj.xyz

JS:   Object.entries(obj)
来源：http://rxf.ydzc1.top

TS:   Object.entries(obj)
来源：http://iqw.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mlu.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ipm.316326.xyz

Ruby: obj.instance_variables
来源：http://cgg.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://lqj.guannengcc.top

================================================================================
来源：http://wti.cucudq.cn

H. 异常与错误处理
来源：http://iks.shzxlz.cn

================================================================================
来源：http://iqf.gaohongyu789.top

[H01] try / catch 基础
来源：http://ylo.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ahr.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hdg.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ncv.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfc.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xgd.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zcx.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://egq.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dir.yuxming.cn

[H02] finally / ensure 收尾
来源：http://kvp.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://qyw.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nas.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mur.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zup.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://mho.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://rar.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uif.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lsf.ydzc1.top

[H03] 主动抛出异常
来源：http://yfh.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://gmk.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yyj.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://ooy.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://avg.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mbp.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zei.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://rwy.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://hkl.hesvh.cn

[H04] 自定义异常类型
来源：http://scy.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://amo.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xrx.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://bxj.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://qee.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://ekk.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cwe.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://tne.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://uxe.bbcook.cn

[H05] 捕获特定类型
来源：http://svl.fzhhl.top

Py:   except ValueError as e:
来源：http://lxl.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ruj.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://jbx.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://hvh.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://udl.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rkm.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://wwd.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bur.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://hdz.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://hxu.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rmh.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://dwb.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lbq.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yqx.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yhs.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://ham.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://uvp.shanyushiyangkeji.top

[H07] 断言
来源：http://jap.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://dbf.yuanzhike.top

PHP:  assert($x > 0);
来源：http://fas.xylfe.cn

JS:   console.assert(x > 0);
来源：http://mji.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://clh.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://qvq.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pbp.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://xdb.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://ixn.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://ogb.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://nqv.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xvr.jinqigufen.top

JS:   e.message;  e.stack
来源：http://ioa.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mhy.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://wtd.epnwcf.com

Go:   err.Error()
来源：http://dbg.quarkkingdee.top

Ruby: e.message;  e.backtrace
来源：http://fsh.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://phe.mhx1999.top

[H09] 带错误码的异常
来源：http://epr.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bbh.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qeb.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jsi.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iij.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lmy.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qeg.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://aof.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yvy.yangfankeji.com

[H10] 资源自动释放
来源：http://fvt.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fmy.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ejt.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eqn.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://egk.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bpf.zhoulong.xyz

Go:   defer f.Close()
来源：http://eaw.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xju.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nml.ppjwa.cn

================================================================================
来源：http://fec.dianchejie.cn

I. 正则表达式
来源：http://yjf.aibaodan.cn

================================================================================
来源：http://zdv.nwbrower.top

[I01] 判断是否匹配
来源：http://vpa.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xoc.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pbq.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://oor.jianghu66.top

TS:   /\d+/.test(s)
来源：http://rzt.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kjy.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ctz.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://wlg.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pqk.hnxiangtu.top

[I02] 提取所有匹配
来源：http://rgs.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://gow.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zlk.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zvu.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://kjz.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kxz.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bdq.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://tiu.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sqx.fktsv.cn

[I03] 提取捕获分组
来源：http://ymk.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cep.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dql.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rlg.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://upw.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hhp.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://puf.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iqp.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uwk.jqgufenzy.top

[I04] 正则替换
来源：http://tkf.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tci.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rqb.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xjb.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ezr.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://kni.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dxn.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://hhx.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tfl.tian-w.cn

[I05] 按正则拆分
来源：http://weh.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://seg.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zsg.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://kul.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://qzg.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://zch.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nbg.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wer.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mfi.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pkm.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wpe.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xwu.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zpm.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eff.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lba.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nxq.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://syw.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hdq.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://dxb.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://weo.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bte.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sfi.wangdashe.top

TS:   /error/gim
来源：http://yid.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ewa.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xgz.ehwqpu.com


<!-- 参考信息 -->