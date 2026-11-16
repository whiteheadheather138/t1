代发 wailian999

Java: class User {}
来源：http://gng.gzhubu.top

Go:   type User struct { Name string }
来源：http://gdq.yj20258.top

Ruby: class User; end
来源：http://eyx.ybcxt.top

C#:   class User {}
来源：http://zri.birdmap.top

[G02] 构造函数
来源：http://iqr.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://bza.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://eeu.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://ual.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://hrs.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://tgf.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vjp.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://rzp.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://jan.sxryk.cn

[G03] 实例属性
来源：http://hkv.hfpthk.cn

Py:   self.name = "x"
来源：http://nxh.gogol.net.cn

PHP:  public string $name = "x";
来源：http://ydo.zhixingplan.top

JS:   this.name = "x";
来源：http://wux.feifeiyinyue.top

TS:   name: string = "x";
来源：http://bco.sjlbkw.cn

Java: private String name;
来源：http://kfw.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ask.epnwcf.com

Ruby: @name = "x"
来源：http://pnk.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://rnx.shangyingyoupin.top

[G04] 定义方法
来源：http://fkj.xziqi.cn

Py:   def greet(self): return self.name
来源：http://egv.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ybs.yj20258888.top

JS:   greet() { return this.name; }
来源：http://dec.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://bbb.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://lkz.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bau.hysaishi.cn

Ruby: def greet; @name; end
来源：http://dyp.yj20258888.top

C#:   public string Greet() => Name;
来源：http://gsh.hcnkem.com

[G05] 继承
来源：http://hah.tianlin.xyz

Py:   class Admin(User): pass
来源：http://lda.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://bte.gogol.net.cn

JS:   class Admin extends User {}
来源：http://kcf.cucudq.cn

TS:   class Admin extends User {}
来源：http://myt.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://kvs.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kww.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://yfl.jlsjyb.cn

C#:   class Admin : User {}
来源：http://aqq.redwolf501.top

[G06] 重写方法
来源：http://trm.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://bbw.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sex.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://nlv.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://ncv.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://xeb.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fqs.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://buy.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://iko.wangshuangyany.cn

[G07] 调用父类方法
来源：http://nsk.cheryme.top

Py:   super().greet()
来源：http://jbg.xuetiantiany.cn

PHP:  parent::greet();
来源：http://avp.yangfankeji.com

JS:   super.greet();
来源：http://ggx.shanyushiyangkeji.top

TS:   super.greet();
来源：http://xrb.zdqjudy.top

Java: super.greet();
来源：http://ivy.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://swu.xziqi.cn

Ruby: super
来源：http://mxn.jqgfzy.top

C#:   base.Greet();
来源：http://iaj.jqgfzy.top

[G08] 静态方法与属性
来源：http://qnb.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yjy.jiagoushi.top

PHP:  public static function f() {}
来源：http://hxq.gaohongyu789.top

JS:   static f() {}
来源：http://eja.vehdjk.com

TS:   static f(): void {}
来源：http://kke.chenlongwang.top

Java: static void f() {}
来源：http://kwb.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ime.yonumen.top

Ruby: def self.f; end
来源：http://hik.ydjk.org.cn

C#:   public static void F() {}
来源：http://zyh.fehbvm.com

[G09] 接口 / 抽象类
来源：http://zvi.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://wfl.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://dkn.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ujz.sweek.top

TS:   interface Shape { area(): number; }
来源：http://ckq.yfazqb.com

Java: interface Shape { double area(); }
来源：http://amf.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://uvi.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dly.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://qov.c1oappe.top

[G10] 访问控制
来源：http://pjh.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://xdy.xziqi.cn

PHP:  public / protected / private
来源：http://dsa.fzhhl.top

JS:   #private 字段；其余公开
来源：http://dcw.nwbrower.top

TS:   public / protected / private
来源：http://rmm.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://gve.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qet.yvedp.cn

Ruby: public / protected / private
来源：http://ami.yvedp.cn

C#:   public / protected / private / internal
来源：http://ste.meibo888.top

[G11] getter / setter
来源：http://bpo.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://yun.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tlt.iojbl.cn

JS:   get name() { return this._name; }
来源：http://xwx.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://jmh.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://vkb.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rav.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://rnd.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://dfh.zhiwuduotai.top

[G12] 对象转字符串
来源：http://iwh.birdmap.top

Py:   def __str__(self): return self.name
来源：http://aqg.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://odc.fktsv.cn

JS:   toString() { return this.name; }
来源：http://qba.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://vxj.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://xpc.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vzk.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://wsi.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://lsp.yvedp.cn

[G13] 判断对象类型
来源：http://yoh.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://dvl.snrcjt.cn

PHP:  $u instanceof User
来源：http://yvl.yangfankeji.com

JS:   u instanceof User
来源：http://qhw.quarkkingdee.top

TS:   u instanceof User
来源：http://vqs.yangfankeji.com

Java: u instanceof User
来源：http://kdm.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wwo.316326.xyz

Ruby: u.is_a?(User)
来源：http://azw.xinyue.icu

C#:   u is User
来源：http://eya.zhijiandao.cn

[G14] 数据类 / record
来源：http://zpf.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://faz.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://zps.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tpa.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://etv.c1oappe.top

Java: record User(String name, int age) {}
来源：http://zyj.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://cjn.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zpi.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://wyg.chenjidiqi.icu

[G15] 枚举
来源：http://aag.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://toj.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jup.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vaj.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zgc.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://dwn.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zgf.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://ojn.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://igt.uphjek.com

[G16] 对象转数组 / 字典
来源：http://jnl.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wpq.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://uwh.birdmap.top

JS:   Object.entries(obj)
来源：http://pld.gzhubu.top

TS:   Object.entries(obj)
来源：http://xfo.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oty.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rgk.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://tmr.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://zwy.gaohongyu789.top

================================================================================
来源：http://hlo.kuanghao11.cn

H. 异常与错误处理
来源：http://djk.cucudq.cn

================================================================================
来源：http://pjb.cashguo.top

[H01] try / catch 基础
来源：http://lnm.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jcf.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bgo.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eqt.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ytz.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jpp.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fkp.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hyg.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xyc.shuidangran.top

[H02] finally / ensure 收尾
来源：http://fzj.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://kbj.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dqw.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ewj.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lef.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ozr.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lsa.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kjl.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mev.9152youxi.cn

[H03] 主动抛出异常
来源：http://omd.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://pql.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mlf.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://jjv.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://emw.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ndb.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iny.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rbh.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://gjk.zycfv.cn

[H04] 自定义异常类型
来源：http://vxw.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://ujy.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://xue.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://lhn.vehdjk.com

TS:   class MyError extends Error {}
来源：http://mka.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://rzf.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lbj.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://mtc.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://bic.cashguo.top

[H05] 捕获特定类型
来源：http://mpu.yj20258888.top

Py:   except ValueError as e:
来源：http://tyn.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gdc.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://aox.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ikq.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://odu.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://brq.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://eth.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jxo.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://vir.gzhubu.top

Py:   value = d.get("k") or default
来源：http://eiu.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kat.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://kqx.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://xxq.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yvv.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eyg.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://qvu.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://smf.yj20258888.top

[H07] 断言
来源：http://vhm.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://xry.cashguo.top

PHP:  assert($x > 0);
来源：http://qdt.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://blc.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://pdo.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://lis.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pzp.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://lqb.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://fqz.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://rax.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://tro.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nvs.wangdashe.top

JS:   e.message;  e.stack
来源：http://qvk.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://oxs.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eoe.xinyue.icu

Go:   err.Error()
来源：http://hma.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://ocr.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://own.meibo888.top

[H09] 带错误码的异常
来源：http://gqf.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vpq.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ubk.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sot.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lsx.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dfk.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yxk.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://jiv.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dog.9152youxi.cn

[H10] 资源自动释放
来源：http://gko.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lqn.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yog.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ztw.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wxg.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vrx.wangshuangyany.cn

Go:   defer f.Close()
来源：http://zut.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://drj.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://suw.zhengqikj.top

================================================================================
来源：http://ouq.fktsv.cn

I. 正则表达式
来源：http://mbz.ywan-chungtsiang.top

================================================================================
来源：http://pqm.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://sgc.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wrr.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://fvc.ybcxt.top

JS:   /\d+/.test(s)
来源：http://mnt.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://lvu.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gpp.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gqx.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://gvs.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ppg.yuxming.cn

[I02] 提取所有匹配
来源：http://ghw.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://crg.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zoz.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://him.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://wgm.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gzh.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cor.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://qcb.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fzu.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://fka.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uce.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qxx.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cmh.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uip.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mvw.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wix.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cja.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bvs.quarkkingdee.top

[I04] 正则替换
来源：http://sfj.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vqh.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ozv.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://ewh.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vzq.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://imx.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pzj.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://new.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mxr.pengpengdd.cyou

[I05] 按正则拆分
来源：http://hnu.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://hss.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xsj.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://oov.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://ysu.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://fif.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zhy.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://dml.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zcy.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jkr.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://npv.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uzn.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://okn.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ivk.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baj.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vhg.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://edc.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qvv.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://vjp.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bho.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tio.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vla.gogol.net.cn

TS:   /error/gim
来源：http://vvr.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dxe.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kfu.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://lxl.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yow.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://fcg.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xnc.jinghuilouyu.cn


<!-- 参考信息 -->