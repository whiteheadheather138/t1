代发 wailian999

[G02] 构造函数
来源：http://btf.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://ful.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://lph.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://pop.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://tmk.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://swy.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jko.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://xig.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://bqe.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://clz.hammf.cn

Py:   self.name = "x"
来源：http://zwe.zdbjq.cn

PHP:  public string $name = "x";
来源：http://acm.jiagoushi.top

JS:   this.name = "x";
来源：http://khf.dianchejie.cn

TS:   name: string = "x";
来源：http://muh.guannengcc.top

Java: private String name;
来源：http://bgd.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nor.yueranfly.top

Ruby: @name = "x"
来源：http://rhy.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://jmr.fzhhl.top

[G04] 定义方法
来源：http://utx.iojbl.cn

Py:   def greet(self): return self.name
来源：http://oos.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://oys.fzhhl.top

JS:   greet() { return this.name; }
来源：http://zsl.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://fja.chenlongwang.top

Java: String greet() { return name; }
来源：http://gla.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cla.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://yjk.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://phm.xziqi.cn

[G05] 继承
来源：http://wir.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://jdx.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://tjn.yvedp.cn

JS:   class Admin extends User {}
来源：http://mlg.wangdashe.top

TS:   class Admin extends User {}
来源：http://oqp.ivvv.top

Java: class Admin extends User {}
来源：http://mgp.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ulb.bbcook.cn

Ruby: class Admin < User; end
来源：http://bnc.zhoulong.xyz

C#:   class Admin : User {}
来源：http://pgy.hywenlv.cn

[G06] 重写方法
来源：http://csl.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://evz.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://kxa.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://zlj.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://nkf.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://ggx.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qkn.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://urc.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://ysc.nanxinkj.top

[G07] 调用父类方法
来源：http://aow.zhixingplan.top

Py:   super().greet()
来源：http://erg.tianlin.xyz

PHP:  parent::greet();
来源：http://jtp.pycfn.com

JS:   super.greet();
来源：http://aoh.snrcjt.cn

TS:   super.greet();
来源：http://gjf.shuidangran.top

Java: super.greet();
来源：http://ayj.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iwq.svipenyu.cn

Ruby: super
来源：http://cux.jiagoushi.top

C#:   base.Greet();
来源：http://qao.ivvv.top

[G08] 静态方法与属性
来源：http://nld.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://otw.bbcook.cn

PHP:  public static function f() {}
来源：http://uot.sweek.top

JS:   static f() {}
来源：http://fyo.jqgufenzy.top

TS:   static f(): void {}
来源：http://gxs.316326.xyz

Java: static void f() {}
来源：http://htb.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rax.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://zzv.cashguo.top

C#:   public static void F() {}
来源：http://bck.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://fuh.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://lol.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://onc.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bpi.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://zsa.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://bcn.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://vid.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wok.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://zsc.yongpay.top

[G10] 访问控制
来源：http://qbw.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ufg.ybcxt.top

PHP:  public / protected / private
来源：http://qlv.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://oen.gogol.net.cn

TS:   public / protected / private
来源：http://rxq.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://xiv.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tvu.xinyue.icu

Ruby: public / protected / private
来源：http://wnc.nwbrower.top

C#:   public / protected / private / internal
来源：http://bkq.guannengcc.top

[G11] getter / setter
来源：http://dmw.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://jep.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://zgm.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://nff.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://dqa.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://rkt.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://roq.xziqi.cn

Ruby: attr_accessor :name
来源：http://oyx.fengsongda.top

C#:   public string Name { get; set; }
来源：http://mvy.epnwcf.com

[G12] 对象转字符串
来源：http://fre.hammf.cn

Py:   def __str__(self): return self.name
来源：http://zth.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rxb.tanke756.top

JS:   toString() { return this.name; }
来源：http://gdz.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://ovx.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://nli.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hos.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://rfn.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://oas.zhoulong.xyz

[G13] 判断对象类型
来源：http://hxp.sysykeji.top

Py:   isinstance(u, User)
来源：http://aqa.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://ude.nwbrower.top

JS:   u instanceof User
来源：http://tni.zhongyouzk.top

TS:   u instanceof User
来源：http://eoe.yanxiufei.cn

Java: u instanceof User
来源：http://jem.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rcb.bbcook.cn

Ruby: u.is_a?(User)
来源：http://tma.snrcjt.cn

C#:   u is User
来源：http://mcq.gogol.net.cn

[G14] 数据类 / record
来源：http://vlw.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ysa.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://tyv.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://oyn.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://ucu.zycfv.cn

Java: record User(String name, int age) {}
来源：http://zmk.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://esn.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zrm.tanke756.top

C#:   record User(string Name, int Age);
来源：http://fji.nwbrower.top

[G15] 枚举
来源：http://ykq.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ktm.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://krw.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qbe.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bjl.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://dwb.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jqy.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://sti.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://owr.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://mfd.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kax.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://hks.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://umz.yuanzhike.top

TS:   Object.entries(obj)
来源：http://hvy.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://prb.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wpb.cashguo.top

Ruby: obj.instance_variables
来源：http://kvx.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://vqn.fzhhl.top

================================================================================
来源：http://rdk.hesvh.cn

H. 异常与错误处理
来源：http://vvh.fzhhl.top

================================================================================
来源：http://cxy.nwbrower.top

[H01] try / catch 基础
来源：http://bld.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cmq.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xxh.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fwz.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zwq.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ztj.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://klv.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pcs.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lca.tarul.cn

[H02] finally / ensure 收尾
来源：http://jck.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://pjl.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://yjz.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aoz.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://wux.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vgz.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mrj.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bye.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://zaf.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://olf.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://rqq.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://agv.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://axj.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://irf.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ihp.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bnb.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://neq.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://uxg.fengsongda.top

[H04] 自定义异常类型
来源：http://fcp.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://cxj.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ylr.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://hed.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://ltx.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://ncn.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://teh.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://vdq.yj20258.top

C#:   class MyException : Exception {}
来源：http://ewl.yvedp.cn

[H05] 捕获特定类型
来源：http://stg.aizwys.cn

Py:   except ValueError as e:
来源：http://qzd.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://edz.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://zbz.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://ojr.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://knm.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tyc.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://cht.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rno.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://wmr.iojbl.cn

Py:   value = d.get("k") or default
来源：http://rwf.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://zns.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aij.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://sgh.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ncg.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://scd.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://rss.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://yfj.jinqigufen.top

[H07] 断言
来源：http://eyz.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://zfr.yj20258.top

PHP:  assert($x > 0);
来源：http://htw.uphjek.com

JS:   console.assert(x > 0);
来源：http://qap.fzhhl.top

TS:   console.assert(x > 0);
来源：http://zji.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://oug.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgh.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jzz.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://xzq.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://rdf.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://tlv.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jcp.hfpthk.cn

JS:   e.message;  e.stack
来源：http://inh.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ojk.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nkl.yuanzhike.top

Go:   err.Error()
来源：http://hib.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://htc.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://sao.yueranfly.top

[H09] 带错误码的异常
来源：http://jmu.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ges.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://obx.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qpj.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jey.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://snv.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lhx.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://pea.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bng.feifeiyinyue.top

[H10] 资源自动释放
来源：http://wkr.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://niy.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dcx.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mqe.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aun.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gzd.sysykeji.top

Go:   defer f.Close()
来源：http://mil.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rpf.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qbn.kuanghao11.cn

================================================================================
来源：http://zbi.yanxiufei.cn

I. 正则表达式
来源：http://piq.shzxlz.cn

================================================================================
来源：http://dsm.vqdsnc.cn

[I01] 判断是否匹配
来源：http://ndi.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://frk.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://eon.316326.xyz

JS:   /\d+/.test(s)
来源：http://bqs.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://jfo.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nos.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nbz.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://mvi.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fey.ctjpmb.com

[I02] 提取所有匹配
来源：http://nbf.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://eys.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wtu.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mvu.hysaishi.cn

TS:   s.match(/\d+/g)
来源：http://pkn.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tir.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vtg.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://vab.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yxw.hesvh.cn

[I03] 提取捕获分组
来源：http://fuy.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://njd.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lzd.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wir.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fvu.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gzm.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ble.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uer.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bxj.pengpengdd.cyou

[I04] 正则替换
来源：http://fjr.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zns.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kii.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://arv.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://aiu.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ttt.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hhi.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://kei.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zvv.zhoulong.xyz

[I05] 按正则拆分
来源：http://zrr.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hnp.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xwy.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://dji.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://evz.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://nvg.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fpy.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fuk.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wut.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ozg.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jyd.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://owf.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwe.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vau.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://odq.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mdr.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qmb.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vty.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://lsa.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lnf.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ils.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iyh.xylfe.cn

TS:   /error/gim
来源：http://hmt.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lji.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cff.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://rkf.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tpl.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://vyt.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lde.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fvo.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bbg.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://law.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gut.hesvh.cn


<!-- 参考信息 -->