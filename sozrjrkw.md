代发 wailian999

================================================================================
来源：http://pxf.bbcook.cn

G. 面向对象
来源：http://mwu.fehbvm.com

================================================================================
来源：http://goq.zdbjq.cn

[G01] 定义类
来源：http://ubq.guannengcc.top

Py:   class User: pass
来源：http://bdn.fengsongda.top

PHP:  class User {}
来源：http://wto.daria6918.cn

JS:   class User {}
来源：http://ozu.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://zby.ydzc1.top

Java: class User {}
来源：http://hyg.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://uls.zhiwuduotai.top

Ruby: class User; end
来源：http://nhu.iojbl.cn

C#:   class User {}
来源：http://sba.dashuyun.cn

[G02] 构造函数
来源：http://vci.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://bnn.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://xkd.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://mev.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://plg.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://hhf.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://njc.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://wqh.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://hgh.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://emm.tianlin.xyz

Py:   self.name = "x"
来源：http://xra.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://wpk.pengpengdd.cyou

JS:   this.name = "x";
来源：http://msi.feifeiyinyue.top

TS:   name: string = "x";
来源：http://wac.ehwqpu.com

Java: private String name;
来源：http://dif.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lil.yonumen.top

Ruby: @name = "x"
来源：http://hwy.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://uur.0kj1m.cn

[G04] 定义方法
来源：http://xnb.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://tsv.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uzo.tanke756.top

JS:   greet() { return this.name; }
来源：http://mbd.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://ueh.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://ebb.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wjm.sysykeji.top

Ruby: def greet; @name; end
来源：http://uou.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://wln.yj20258.top

[G05] 继承
来源：http://hbb.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://piq.yueranfly.top

PHP:  class Admin extends User {}
来源：http://mzy.0kj1m.cn

JS:   class Admin extends User {}
来源：http://fzc.dianchejie.cn

TS:   class Admin extends User {}
来源：http://yua.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://jva.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lvq.guowangkeji.top

Ruby: class Admin < User; end
来源：http://qyy.snrcjt.cn

C#:   class Admin : User {}
来源：http://vok.shuidangran.top

[G06] 重写方法
来源：http://yuq.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://qxy.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fyp.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://hww.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://mdw.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://xip.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qam.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://tgc.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://gvc.9152youxi.cn

[G07] 调用父类方法
来源：http://eek.fengsongda.top

Py:   super().greet()
来源：http://yfo.yuanzhike.top

PHP:  parent::greet();
来源：http://cla.yfazqb.com

JS:   super.greet();
来源：http://thn.sysykeji.top

TS:   super.greet();
来源：http://bfk.ehwqpu.com

Java: super.greet();
来源：http://klg.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bmg.ctjpmb.com

Ruby: super
来源：http://znn.yvedp.cn

C#:   base.Greet();
来源：http://ioi.sweek.top

[G08] 静态方法与属性
来源：http://era.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cbx.dashuyun.cn

PHP:  public static function f() {}
来源：http://jfn.zhaomingkeji.xyz

JS:   static f() {}
来源：http://kyf.wangshuangyany.cn

TS:   static f(): void {}
来源：http://bqu.jinqigufen.top

Java: static void f() {}
来源：http://kkj.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jgv.jinqigufen.top

Ruby: def self.f; end
来源：http://typ.jlsjyb.cn

C#:   public static void F() {}
来源：http://vem.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://ucr.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://knj.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ytt.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://oho.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://tau.meibo888.top

Java: interface Shape { double area(); }
来源：http://jix.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://yua.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lms.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://sew.tianlin.xyz

[G10] 访问控制
来源：http://vcf.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://rgr.yuxming.cn

PHP:  public / protected / private
来源：http://wxw.guannengcc.top

JS:   #private 字段；其余公开
来源：http://gip.nwbrower.top

TS:   public / protected / private
来源：http://ncu.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://rba.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qca.cashguo.top

Ruby: public / protected / private
来源：http://leh.tarul.cn

C#:   public / protected / private / internal
来源：http://ccy.fktsv.cn

[G11] getter / setter
来源：http://dfg.xuanzx.com

Py:   @property 与 @x.setter
来源：http://dei.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nsi.guannengcc.top

JS:   get name() { return this._name; }
来源：http://fwc.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://ciu.cdnleiting.top

Java: public String getName() { return name; }
来源：http://xnl.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://aai.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://srw.zycfv.cn

C#:   public string Name { get; set; }
来源：http://aps.jinqigufen.top

[G12] 对象转字符串
来源：http://ohq.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://ryc.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://llz.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://fqc.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://ajj.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://hzw.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://edk.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://wjs.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://czf.pycfn.com

[G13] 判断对象类型
来源：http://yzt.aibaodan.cn

Py:   isinstance(u, User)
来源：http://ghh.sweek.top

PHP:  $u instanceof User
来源：http://vzl.cqqwz.cn

JS:   u instanceof User
来源：http://nxj.tianlin.xyz

TS:   u instanceof User
来源：http://qyr.jyoumei.cn

Java: u instanceof User
来源：http://cjf.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sds.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://xhz.jinqigfzy.top

C#:   u is User
来源：http://ivd.zhengqikj.top

[G14] 数据类 / record
来源：http://gjp.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ggu.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://bnk.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://cqs.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://rzc.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://pxt.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://ugz.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ymx.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://kjc.hongshengwenyu.top

[G15] 枚举
来源：http://ohe.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gnn.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://nps.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gcu.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xuu.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://aqy.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hew.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://wpz.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://caz.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://snw.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iyl.yongpay.top

PHP:  get_object_vars($obj);
来源：http://zah.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://wcf.hfpthk.cn

TS:   Object.entries(obj)
来源：http://bpw.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://odk.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rha.xinyue.icu

Ruby: obj.instance_variables
来源：http://sds.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://woi.jinghuilouyu.cn

================================================================================
来源：http://fqs.nwbrower.top

H. 异常与错误处理
来源：http://zdt.hfpthk.cn

================================================================================
来源：http://gpt.zhijiandao.cn

[H01] try / catch 基础
来源：http://rbh.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xgx.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zeq.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://srl.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lap.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yey.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xvl.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lif.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://isk.havefunace.top

[H02] finally / ensure 收尾
来源：http://zni.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ggj.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://urn.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pgk.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dej.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gle.zhoulong.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://pgk.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zrs.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vuw.yj20258.top

[H03] 主动抛出异常
来源：http://pvf.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://srh.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hnh.birdmap.top

JS:   throw new Error("错误信息");
来源：http://yvj.cashguo.top

TS:   throw new Error("错误信息");
来源：http://cxv.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://keu.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oan.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sbu.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zph.wangdashe.top

[H04] 自定义异常类型
来源：http://tub.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://tmr.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://okq.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://ktc.316326.xyz

TS:   class MyError extends Error {}
来源：http://twl.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://fwl.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fka.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://fwg.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://yqp.snrcjt.cn

[H05] 捕获特定类型
来源：http://gue.bbcook.cn

Py:   except ValueError as e:
来源：http://ilm.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iqx.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://qal.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://sja.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://rck.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xza.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://nay.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ctk.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://rfi.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://cim.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://nrk.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oma.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://gsg.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ddl.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://juf.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://zgd.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://vow.cheryme.top

[H07] 断言
来源：http://jsm.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://rnk.aibaodan.cn

PHP:  assert($x > 0);
来源：http://klt.tanke756.top

JS:   console.assert(x > 0);
来源：http://dam.hesvh.cn

TS:   console.assert(x > 0);
来源：http://pok.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://qtc.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://soh.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://qfb.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://ald.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://qap.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://jjn.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rwo.bjfxy.top

JS:   e.message;  e.stack
来源：http://kme.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dbr.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ygn.fehbvm.com

Go:   err.Error()
来源：http://qxx.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://yep.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://qle.zycfv.cn

[H09] 带错误码的异常
来源：http://baj.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pef.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mst.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://znd.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rwx.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gju.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qwd.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fmq.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://opw.zdbjq.cn

[H10] 资源自动释放
来源：http://ntp.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ugp.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tiz.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xgz.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eqq.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qzw.snrcjt.cn

Go:   defer f.Close()
来源：http://cpf.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lsd.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tbu.xuanzx.com

================================================================================
来源：http://baw.redwolf501.top

I. 正则表达式
来源：http://jop.0kj1m.cn

================================================================================
来源：http://gpm.hammf.cn

[I01] 判断是否匹配
来源：http://ewl.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fjy.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mpn.pycfn.com

JS:   /\d+/.test(s)
来源：http://uja.c1oappe.top

TS:   /\d+/.test(s)
来源：http://ttx.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zya.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bqm.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://aho.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://okg.tianlin.xyz

[I02] 提取所有匹配
来源：http://chz.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://hwo.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nkp.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sjl.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://hil.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mur.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://clh.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://zmv.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hpc.pycfn.com

[I03] 提取捕获分组
来源：http://ptj.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vuv.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ize.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bwt.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mso.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://btf.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://njp.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cly.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cbp.hnqzz.top

[I04] 正则替换
来源：http://dkc.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nkt.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cpz.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://sud.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://fgq.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://vnb.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://udh.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jzz.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nwr.aizwys.cn

[I05] 按正则拆分
来源：http://naw.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qok.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gni.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://uqb.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://ldt.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://rlb.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yxp.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://ywt.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pjp.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fnf.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://joe.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zpd.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ocp.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgh.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cvp.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sgl.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yux.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fvc.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://ghi.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eqp.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qqm.shzxlz.cn


<!-- 参考信息 -->