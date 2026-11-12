代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wsv.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tdd.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bbp.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kab.jlsjyb.cn

================================================================================
来源：http://qcc.hysaishi.cn

G. 面向对象
来源：http://zec.hesvh.cn

================================================================================
来源：http://jqw.svipenyu.cn

[G01] 定义类
来源：http://fup.havefunace.top

Py:   class User: pass
来源：http://bxo.gogol.net.cn

PHP:  class User {}
来源：http://oyb.redwolf501.top

JS:   class User {}
来源：http://sgm.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://drp.bbcook.cn

Java: class User {}
来源：http://oxy.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://cqe.fehbvm.com

Ruby: class User; end
来源：http://vnl.daria6918.cn

C#:   class User {}
来源：http://zbu.shuidangran.top

[G02] 构造函数
来源：http://cbc.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://egk.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://wrs.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://wag.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://fsg.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://zcq.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pzj.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://ela.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://fjw.cashguo.top

[G03] 实例属性
来源：http://xaj.zhoulong.xyz

Py:   self.name = "x"
来源：http://whn.fktsv.cn

PHP:  public string $name = "x";
来源：http://rlp.fzhhl.top

JS:   this.name = "x";
来源：http://sly.tianlin.xyz

TS:   name: string = "x";
来源：http://dxc.nwbrower.top

Java: private String name;
来源：http://eph.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://afe.ctjpmb.com

Ruby: @name = "x"
来源：http://qjm.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://vde.hcnkem.com

[G04] 定义方法
来源：http://eby.birdmap.top

Py:   def greet(self): return self.name
来源：http://jok.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dfx.xinyue.icu

JS:   greet() { return this.name; }
来源：http://bof.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://pds.ctjpmb.com

Java: String greet() { return name; }
来源：http://rht.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://oly.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://mxo.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://fod.wangdashe.top

[G05] 继承
来源：http://rkg.ctjpmb.com

Py:   class Admin(User): pass
来源：http://ste.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://beg.tianlin.xyz

JS:   class Admin extends User {}
来源：http://xlg.yj202588.top

TS:   class Admin extends User {}
来源：http://ajq.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://rrt.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eeb.iojbl.cn

Ruby: class Admin < User; end
来源：http://miz.daxiang520.top

C#:   class Admin : User {}
来源：http://xtu.shzxlz.cn

[G06] 重写方法
来源：http://ran.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://auc.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dbl.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://qca.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://pip.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://gzy.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ltj.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://yki.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://wrm.shzxlz.cn

[G07] 调用父类方法
来源：http://nnx.zhongyouzk.top

Py:   super().greet()
来源：http://qgi.guowangkeji.top

PHP:  parent::greet();
来源：http://hmb.hysaishi.cn

JS:   super.greet();
来源：http://kdu.jyoumei.cn

TS:   super.greet();
来源：http://hal.hongshengwenyu.top

Java: super.greet();
来源：http://kkd.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lar.uphjek.com

Ruby: super
来源：http://avi.yongpay.top

C#:   base.Greet();
来源：http://ctn.iojbl.cn

[G08] 静态方法与属性
来源：http://cea.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dlk.zdbjq.cn

PHP:  public static function f() {}
来源：http://uom.snrcjt.cn

JS:   static f() {}
来源：http://zne.zhijiandao.cn

TS:   static f(): void {}
来源：http://hsx.cdnleiting.top

Java: static void f() {}
来源：http://zqx.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pap.yangfankeji.com

Ruby: def self.f; end
来源：http://fpx.zhijiandao.cn

C#:   public static void F() {}
来源：http://kgr.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://utj.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://xyj.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jih.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fww.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://cht.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://kze.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://szg.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aex.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://gpn.cqqwz.cn

[G10] 访问控制
来源：http://hnq.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://vha.yuanzhike.top

PHP:  public / protected / private
来源：http://xio.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://vwo.daria6918.cn

TS:   public / protected / private
来源：http://qah.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://rlh.tanke756.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ror.hesvh.cn

Ruby: public / protected / private
来源：http://jbw.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://fkk.jinyuanbaomall.cn

[G11] getter / setter
来源：http://uwa.hesvh.cn

Py:   @property 与 @x.setter
来源：http://kdq.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://dzq.sysykeji.top

JS:   get name() { return this._name; }
来源：http://jzk.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://uxk.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://ced.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hym.jianghu66.top

Ruby: attr_accessor :name
来源：http://dox.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://yfy.bjfxy.top

[G12] 对象转字符串
来源：http://lyi.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://qpg.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ciq.nwbrower.top

JS:   toString() { return this.name; }
来源：http://bvh.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://mqy.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://mke.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://qec.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://qgw.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://wom.aizwys.cn

[G13] 判断对象类型
来源：http://awu.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://xcv.9152youxi.cn

PHP:  $u instanceof User
来源：http://vvl.daria6918.cn

JS:   u instanceof User
来源：http://bpf.hnxiangtu.top

TS:   u instanceof User
来源：http://rxr.jianghu66.top

Java: u instanceof User
来源：http://lmg.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vcz.guannengcc.top

Ruby: u.is_a?(User)
来源：http://elr.zycfv.cn

C#:   u is User
来源：http://kvx.meibo888.top

[G14] 数据类 / record
来源：http://kvw.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pxs.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://lcf.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://syx.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://gil.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://rye.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://vmt.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lov.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://xnr.xylfe.cn

[G15] 枚举
来源：http://fov.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dtf.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ncu.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vqq.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mom.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://oyz.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yiu.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://bpn.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://who.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://cew.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bwr.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://nej.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://gle.yj20258.top

TS:   Object.entries(obj)
来源：http://ilq.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://poz.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rof.cashguo.top

Ruby: obj.instance_variables
来源：http://eqn.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://kck.sweek.top

================================================================================
来源：http://hce.quarkkingdee.top

H. 异常与错误处理
来源：http://zym.hnqzz.top

================================================================================
来源：http://uxu.dashuyun.cn

[H01] try / catch 基础
来源：http://pez.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nec.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hav.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ris.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nns.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tdp.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qho.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oxm.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ydt.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://hyn.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://obx.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ldm.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ria.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vns.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://lto.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nrh.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://rnp.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://dqp.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://reo.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://cxw.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wzk.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://aie.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://xnr.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://dnu.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zry.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pek.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://zrd.jiagoushi.top

[H04] 自定义异常类型
来源：http://ngr.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://jyo.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://wza.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://gsd.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://kkf.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://lca.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ztw.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://fjp.yvedp.cn

C#:   class MyException : Exception {}
来源：http://xqu.gogol.net.cn

[H05] 捕获特定类型
来源：http://qte.bbcook.cn

Py:   except ValueError as e:
来源：http://hhc.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ytr.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://ygy.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://mpl.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://eei.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kat.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://slz.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mmo.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://sjn.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://ajl.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://kdl.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://unb.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ziq.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hhu.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vrh.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://rbs.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://mjp.andypj.xyz

[H07] 断言
来源：http://upu.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://vzo.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://yst.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://ura.jianghu66.top

TS:   console.assert(x > 0);
来源：http://njp.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://arr.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mxb.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pru.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://kkg.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://kde.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://yar.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lil.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://yli.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wop.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://xun.ywan-chungtsiang.top

Go:   err.Error()
来源：http://aov.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://bdd.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://uke.hcnkem.com

[H09] 带错误码的异常
来源：http://hwh.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pha.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wxl.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yye.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aag.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yrc.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vrk.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://nfj.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://wsc.hfpthk.cn

[H10] 资源自动释放
来源：http://tmb.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://atk.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wai.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xtp.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bvx.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uzs.yfazqb.com

Go:   defer f.Close()
来源：http://rmk.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tvo.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gti.zhaomingkeji.xyz

================================================================================
来源：http://ipf.fehbvm.com

I. 正则表达式
来源：http://cyt.pengpengdd.cyou

================================================================================
来源：http://mcn.haohaochexian.top

[I01] 判断是否匹配
来源：http://sue.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kzl.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://yia.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://zbn.sysykeji.top

TS:   /\d+/.test(s)
来源：http://gpm.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://trc.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qof.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://vyl.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dnt.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://twe.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://zsr.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yjw.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zvm.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://rgi.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zmb.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://osy.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://aiq.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wkr.yfazqb.com

[I03] 提取捕获分组
来源：http://smg.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yko.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cvj.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gvs.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vzi.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ddw.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://prn.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eqd.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jwz.52xcode.cn

[I04] 正则替换
来源：http://wnx.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kzy.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cha.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://wkh.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://kac.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xul.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://qqw.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://otq.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fpo.xylfe.cn

[I05] 按正则拆分
来源：http://jgy.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qpl.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qie.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://ymz.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://jyb.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://ghl.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://phs.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://ryr.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ajw.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://psb.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ktl.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vgl.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwi.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://slh.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gxs.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iel.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cmb.sufxvd.cn


<!-- 参考信息 -->