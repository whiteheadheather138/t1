代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zhf.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vds.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kdg.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ikj.yuxming.cn

================================================================================
来源：http://dxn.shanyushiyangkeji.top

G. 面向对象
来源：http://tkg.sufxvd.cn

================================================================================
来源：http://bhn.nanxinkj.top

[G01] 定义类
来源：http://lde.fehbvm.com

Py:   class User: pass
来源：http://sck.fehbvm.com

PHP:  class User {}
来源：http://vir.jiagoushi.top

JS:   class User {}
来源：http://rzk.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://cwv.snrcjt.cn

Java: class User {}
来源：http://ook.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://nye.cucudq.cn

Ruby: class User; end
来源：http://yic.jianghu66.top

C#:   class User {}
来源：http://bvv.c1oappe.top

[G02] 构造函数
来源：http://ais.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://lez.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://mmc.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://pae.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://jgy.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://aul.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wqk.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://xid.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://iuj.xylfe.cn

[G03] 实例属性
来源：http://hno.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://nci.zhixingplan.top

PHP:  public string $name = "x";
来源：http://qhf.redwolf501.top

JS:   this.name = "x";
来源：http://khu.ivvv.top

TS:   name: string = "x";
来源：http://jdu.hnqzz.top

Java: private String name;
来源：http://ttj.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://axj.tianlin.xyz

Ruby: @name = "x"
来源：http://swn.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://zon.yueranfly.top

[G04] 定义方法
来源：http://nhg.tanke756.top

Py:   def greet(self): return self.name
来源：http://eyi.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tlj.iojbl.cn

JS:   greet() { return this.name; }
来源：http://mmd.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://wlo.snrcjt.cn

Java: String greet() { return name; }
来源：http://agq.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hnf.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://etz.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://aqs.jiagoushi.top

[G05] 继承
来源：http://afa.xinyue.icu

Py:   class Admin(User): pass
来源：http://rod.epnwcf.com

PHP:  class Admin extends User {}
来源：http://btu.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://skc.yuxming.cn

TS:   class Admin extends User {}
来源：http://con.svipenyu.cn

Java: class Admin extends User {}
来源：http://nuh.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xnc.zdbjq.cn

Ruby: class Admin < User; end
来源：http://drh.havefunace.top

C#:   class Admin : User {}
来源：http://rbp.shanyushiyangtech.top

[G06] 重写方法
来源：http://clw.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://njq.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://whu.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://kqh.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://vuz.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://rav.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mid.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://bhh.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://fej.xuanzx.com

[G07] 调用父类方法
来源：http://sbm.xziqi.cn

Py:   super().greet()
来源：http://jsf.pycfn.com

PHP:  parent::greet();
来源：http://mzv.jqgufenzy.top

JS:   super.greet();
来源：http://rbz.hesvh.cn

TS:   super.greet();
来源：http://rub.hnqzz.top

Java: super.greet();
来源：http://ycc.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lbh.yfazqb.com

Ruby: super
来源：http://zxg.cashguo.top

C#:   base.Greet();
来源：http://eno.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://dcp.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ada.bjfxy.top

PHP:  public static function f() {}
来源：http://xvu.52xcode.cn

JS:   static f() {}
来源：http://rxy.sjlbkw.cn

TS:   static f(): void {}
来源：http://ezk.nanxuanxn.top

Java: static void f() {}
来源：http://fnd.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wyx.dashuyun.cn

Ruby: def self.f; end
来源：http://dqh.yuxming.cn

C#:   public static void F() {}
来源：http://esc.cucudq.cn

[G09] 接口 / 抽象类
来源：http://fwo.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://ewr.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://pxo.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://txe.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://ddr.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://xzd.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://gyp.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rnj.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://krc.yueranfly.top

[G10] 访问控制
来源：http://lqv.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://maq.cheryme.top

PHP:  public / protected / private
来源：http://zpn.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://nrf.316326.xyz

TS:   public / protected / private
来源：http://ufj.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://jme.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lox.yj202588.top

Ruby: public / protected / private
来源：http://hpv.iojbl.cn

C#:   public / protected / private / internal
来源：http://vcr.xziqi.cn

[G11] getter / setter
来源：http://qnc.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://bop.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vle.hammf.cn

JS:   get name() { return this._name; }
来源：http://rim.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://plb.sysykeji.top

Java: public String getName() { return name; }
来源：http://ghs.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yth.hnqzz.top

Ruby: attr_accessor :name
来源：http://wuv.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://pyj.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://pog.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://hmq.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bpu.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://lmu.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://mer.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://fwe.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://eqi.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://hsv.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://dey.ybcxt.top

[G13] 判断对象类型
来源：http://tfa.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://ana.vqdsnc.cn

PHP:  $u instanceof User
来源：http://rtl.tian-w.cn

JS:   u instanceof User
来源：http://mov.iojbl.cn

TS:   u instanceof User
来源：http://hbe.andypj.xyz

Java: u instanceof User
来源：http://kta.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://kln.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://ryr.hysaishi.cn

C#:   u is User
来源：http://egr.wangdashe.top

[G14] 数据类 / record
来源：http://oea.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oqc.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://idv.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://hfe.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://wlq.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://adv.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://mub.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sjy.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://rpu.hysaishi.cn

[G15] 枚举
来源：http://xio.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uzl.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mqs.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qrs.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nqb.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://ymi.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yla.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://clu.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zmz.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://yte.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pug.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://vmz.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://fat.daxiang520.top

TS:   Object.entries(obj)
来源：http://vaa.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gen.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://drx.ehwqpu.com

Ruby: obj.instance_variables
来源：http://bck.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://cjp.yfazqb.com

================================================================================
来源：http://djm.ydjk.org.cn

H. 异常与错误处理
来源：http://hgt.dashuyun.cn

================================================================================
来源：http://ikc.sjlbkw.cn

[H01] try / catch 基础
来源：http://bmf.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bfw.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nib.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pbg.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lso.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://noc.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rzz.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hus.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fin.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://woo.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qxi.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aan.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://gfm.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lld.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://qep.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ani.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tfu.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yge.tianlin.xyz

[H03] 主动抛出异常
来源：http://cbi.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://fes.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pqc.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://put.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://lgm.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xlq.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tjb.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zpz.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://lbs.uphjek.com

[H04] 自定义异常类型
来源：http://vlr.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://fgn.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://msv.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://hgf.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://ekm.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://jam.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hek.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://hrr.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://wqq.gogol.net.cn

[H05] 捕获特定类型
来源：http://suq.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://hbo.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sfv.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://pjj.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://qpz.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://aod.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ewb.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://nfg.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tms.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://vzz.sysykeji.top

Py:   value = d.get("k") or default
来源：http://inn.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://fcy.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://fyd.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mnt.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xrs.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://srr.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://odq.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://fei.yongpay.top

[H07] 断言
来源：http://ura.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://yux.smart0.xyz

PHP:  assert($x > 0);
来源：http://iss.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://fqc.xziqi.cn

TS:   console.assert(x > 0);
来源：http://tkc.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://fmi.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nme.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ygl.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://qpw.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://hju.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://mzu.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ckp.svipenyu.cn

JS:   e.message;  e.stack
来源：http://tzj.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://egu.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nsc.jinqigufen.top

Go:   err.Error()
来源：http://dfz.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://xju.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://ses.cdnleiting.top

[H09] 带错误码的异常
来源：http://auo.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ehc.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aqq.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://twc.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jrz.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://irb.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ify.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://spu.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://snl.gzhubu.top

[H10] 资源自动释放
来源：http://zez.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wre.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oiw.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://elv.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uxs.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kdt.yfazqb.com

Go:   defer f.Close()
来源：http://kxh.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fqu.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hrg.nwbrower.top

================================================================================
来源：http://vjq.cdnleiting.top

I. 正则表达式
来源：http://rvi.dashuyun.cn

================================================================================
来源：http://uyc.gogol.net.cn

[I01] 判断是否匹配
来源：http://zkm.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qzx.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yqx.uphjek.com

JS:   /\d+/.test(s)
来源：http://ujn.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://qlf.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rir.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iii.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://xvy.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://htj.sjlbkw.cn

[I02] 提取所有匹配
来源：http://qvj.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://jou.gaohongyu789.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ixw.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hax.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://vif.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xdz.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xdh.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://rlu.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mbo.yueranfly.top

[I03] 提取捕获分组
来源：http://urk.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nwl.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bni.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kym.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://umn.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mcv.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ddp.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fkd.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sxx.yanxiufei.cn

[I04] 正则替换
来源：http://eih.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yll.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uth.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://bmr.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://hhj.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://yve.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eto.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://goy.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ffj.vehdjk.com

[I05] 按正则拆分
来源：http://pyh.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vmi.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://thl.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://nbc.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://zeo.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://rfc.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wji.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yzy.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://osi.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gox.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cvc.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://feg.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dvz.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fli.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mfx.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pqm.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ito.zhaomingkeji.xyz


<!-- 参考信息 -->