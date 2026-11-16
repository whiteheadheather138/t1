代发 wailian999

================================================================================
来源：http://ufv.yj202588.top

G. 面向对象
来源：http://bma.yongpay.top

================================================================================
来源：http://hxt.tianlin.xyz

[G01] 定义类
来源：http://sub.yj20258.top

Py:   class User: pass
来源：http://uod.chenzaomai.com

PHP:  class User {}
来源：http://wqe.fktsv.cn

JS:   class User {}
来源：http://opw.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://bte.sweek.top

Java: class User {}
来源：http://fkx.hywenlv.cn

Go:   type User struct { Name string }
来源：http://gjh.wangdashe.top

Ruby: class User; end
来源：http://dnk.sysykeji.top

C#:   class User {}
来源：http://zhj.fktsv.cn

[G02] 构造函数
来源：http://hti.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://muw.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://qei.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://bnq.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://pyi.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://sru.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lmh.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://mmn.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://pfy.aizwys.cn

[G03] 实例属性
来源：http://gmr.jqgfzy.top

Py:   self.name = "x"
来源：http://ria.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://qxm.svipenyu.cn

JS:   this.name = "x";
来源：http://lpg.uphjek.com

TS:   name: string = "x";
来源：http://jnk.xziqi.cn

Java: private String name;
来源：http://ugx.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wfn.svipenyu.cn

Ruby: @name = "x"
来源：http://rqt.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://qij.yangfankeji.com

[G04] 定义方法
来源：http://qcg.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://fvg.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://oih.daria6918.cn

JS:   greet() { return this.name; }
来源：http://zgh.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://dkw.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://qcw.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://uzo.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://rgv.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://vuv.sjlbkw.cn

[G05] 继承
来源：http://lqc.zhengqikj.top

Py:   class Admin(User): pass
来源：http://fie.316326.xyz

PHP:  class Admin extends User {}
来源：http://omd.meibo888.top

JS:   class Admin extends User {}
来源：http://joa.yuxming.cn

TS:   class Admin extends User {}
来源：http://bed.zdbjq.cn

Java: class Admin extends User {}
来源：http://xro.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pwb.iojbl.cn

Ruby: class Admin < User; end
来源：http://fxo.sjlbkw.cn

C#:   class Admin : User {}
来源：http://ufv.guannengcc.top

[G06] 重写方法
来源：http://sau.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://jkj.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://giw.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://lls.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://cyc.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://tyi.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aju.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://ttw.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://dxr.guowangkeji.top

[G07] 调用父类方法
来源：http://igw.yonumen.top

Py:   super().greet()
来源：http://qmd.nanxuanxn.top

PHP:  parent::greet();
来源：http://ywi.sweek.top

JS:   super.greet();
来源：http://mdn.xziqi.cn

TS:   super.greet();
来源：http://qwy.xuanzx.com

Java: super.greet();
来源：http://lve.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ntp.shanyushiyangkeji.top

Ruby: super
来源：http://orw.jianghu66.top

C#:   base.Greet();
来源：http://gky.hysaishi.cn

[G08] 静态方法与属性
来源：http://qma.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kjr.ydzc1.top

PHP:  public static function f() {}
来源：http://zxu.meibo888.top

JS:   static f() {}
来源：http://ovm.tanke756.top

TS:   static f(): void {}
来源：http://tfp.haohaochexian.top

Java: static void f() {}
来源：http://mha.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mwr.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://fuw.sweek.top

C#:   public static void F() {}
来源：http://prm.jianghu66.top

[G09] 接口 / 抽象类
来源：http://oba.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://lki.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://ugq.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kdb.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://plp.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://ucn.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://svm.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fhe.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://ipm.nwbrower.top

[G10] 访问控制
来源：http://dnk.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://nuf.cucudq.cn

PHP:  public / protected / private
来源：http://gov.sysykeji.top

JS:   #private 字段；其余公开
来源：http://hiw.bbcook.cn

TS:   public / protected / private
来源：http://uvy.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://aeb.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qsc.yuanzhike.top

Ruby: public / protected / private
来源：http://cck.aibaodan.cn

C#:   public / protected / private / internal
来源：http://ixj.zdbjq.cn

[G11] getter / setter
来源：http://jgd.vehdjk.com

Py:   @property 与 @x.setter
来源：http://jvw.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://pof.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://pxk.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://yzr.aibaodan.cn

Java: public String getName() { return name; }
来源：http://cdt.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://deo.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://huh.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://opv.52xcode.cn

[G12] 对象转字符串
来源：http://byo.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://dke.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dsc.bjfxy.top

JS:   toString() { return this.name; }
来源：http://ats.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://zkm.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://qrl.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ixl.sxryk.cn

Ruby: def to_s; @name; end
来源：http://kaq.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://onh.mhx1999.top

[G13] 判断对象类型
来源：http://egm.aizwys.cn

Py:   isinstance(u, User)
来源：http://wvv.tarul.cn

PHP:  $u instanceof User
来源：http://nqy.9152youxi.cn

JS:   u instanceof User
来源：http://hfl.aizwys.cn

TS:   u instanceof User
来源：http://gqv.vqdsnc.cn

Java: u instanceof User
来源：http://vtv.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nyi.yueranfly.top

Ruby: u.is_a?(User)
来源：http://mpp.yangfankeji.com

C#:   u is User
来源：http://nlo.yongpay.top

[G14] 数据类 / record
来源：http://hcz.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qhv.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://mpe.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://ait.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://ijn.sweek.top

Java: record User(String name, int age) {}
来源：http://cai.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://exq.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jqt.meibo888.top

C#:   record User(string Name, int Age);
来源：http://tup.316326.xyz

[G15] 枚举
来源：http://hqq.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dzn.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xdf.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sct.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://edq.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://hjj.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://old.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://wcr.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xwk.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://ohs.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hpi.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://vfh.haohaochexian.top

JS:   Object.entries(obj)
来源：http://mpd.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://zoj.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ajn.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kzs.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://tks.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://gxm.sysykeji.top

================================================================================
来源：http://bun.9152youxi.cn

H. 异常与错误处理
来源：http://eph.dashuyun.cn

================================================================================
来源：http://vrc.cqqwz.cn

[H01] try / catch 基础
来源：http://moc.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ups.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ssf.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://exi.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rjk.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://edn.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cry.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wkv.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nct.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://qaa.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qge.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://wku.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ysi.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lhi.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://xop.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zwp.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fxn.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iwh.shzxlz.cn

[H03] 主动抛出异常
来源：http://sxa.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://jha.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://prj.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://osw.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://dpc.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jfw.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gjg.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://irr.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://rhb.hnqzz.top

[H04] 自定义异常类型
来源：http://pwb.sweek.top

Py:   class MyError(Exception): pass
来源：http://yzk.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://uxq.ydzc1.top

JS:   class MyError extends Error {}
来源：http://zlx.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://ufg.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://mla.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zyt.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://uzt.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://zdf.iojbl.cn

[H05] 捕获特定类型
来源：http://aav.jlsjyb.cn

Py:   except ValueError as e:
来源：http://uwz.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nho.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://dga.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://pgr.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://vck.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pxy.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://jkp.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://czb.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://jgq.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://qql.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://zzu.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://fup.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://fix.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aew.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yjo.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://xtr.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://apz.ydjk.org.cn

[H07] 断言
来源：http://kkq.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://vmv.jiagoushi.top

PHP:  assert($x > 0);
来源：http://iak.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://rut.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://sum.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://pkb.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yvv.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://oum.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://ukx.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://lof.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://tjc.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iof.meibo888.top

JS:   e.message;  e.stack
来源：http://ech.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tpm.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nsq.c1oappe.top

Go:   err.Error()
来源：http://xph.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://qjy.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://giu.vqdsnc.cn

[H09] 带错误码的异常
来源：http://xxz.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gut.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ptb.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zog.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ipx.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bqg.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://byv.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://gjw.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://how.yuxming.cn

[H10] 资源自动释放
来源：http://udk.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kkv.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fdt.yangfankeji.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ced.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://geq.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ufh.zhiwuduotai.top

Go:   defer f.Close()
来源：http://hda.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bwy.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://suw.gzhubu.top

================================================================================
来源：http://bwq.tianlin.xyz

I. 正则表达式
来源：http://zlz.ydjk.org.cn

================================================================================
来源：http://qif.jianghu66.top

[I01] 判断是否匹配
来源：http://snp.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oje.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://kin.daxiang520.top

JS:   /\d+/.test(s)
来源：http://joi.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://wiu.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lyu.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xip.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://mfp.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://roh.hywenlv.cn

[I02] 提取所有匹配
来源：http://ukt.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://dni.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://poh.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sib.hysaishi.cn

TS:   s.match(/\d+/g)
来源：http://tlz.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://faj.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xat.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://pbn.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iqd.zhijiandao.cn

[I03] 提取捕获分组
来源：http://jzd.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://adv.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wgf.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pjt.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zxz.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dmt.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hbk.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://syn.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uky.52xcode.cn

[I04] 正则替换
来源：http://mtn.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lkp.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tzy.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://dmu.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://diu.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://sqk.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hkk.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wic.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mve.feifeiyinyue.top

[I05] 按正则拆分
来源：http://ljn.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://sng.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://prx.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://myj.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://dbj.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://tax.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sjc.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://ony.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://smb.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://imt.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hdy.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ozu.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lei.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhz.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cma.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://puw.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lma.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kkm.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://iud.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sej.tianlin.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jox.fengsongda.top


<!-- 参考信息 -->