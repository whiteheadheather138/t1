代发 wailian999

[G02] 构造函数
来源：http://vnq.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://hbv.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://ast.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://ypj.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://rjt.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://rhe.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ytr.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://ofj.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://ruz.yuxming.cn

[G03] 实例属性
来源：http://nxn.sweek.top

Py:   self.name = "x"
来源：http://sqs.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://smp.ivvv.top

JS:   this.name = "x";
来源：http://hef.andypj.xyz

TS:   name: string = "x";
来源：http://kme.bjfxy.top

Java: private String name;
来源：http://tos.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://egz.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://opp.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://iju.birdmap.top

[G04] 定义方法
来源：http://yjp.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://rjc.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rmq.birdmap.top

JS:   greet() { return this.name; }
来源：http://frz.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://uhj.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://nqw.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://lgg.zdqjudy.top

Ruby: def greet; @name; end
来源：http://hrf.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://ecr.quarkkingdee.top

[G05] 继承
来源：http://fgg.yangfankeji.com

Py:   class Admin(User): pass
来源：http://gys.tian-w.cn

PHP:  class Admin extends User {}
来源：http://dxl.daxiang520.top

JS:   class Admin extends User {}
来源：http://ucr.jinqigufen.top

TS:   class Admin extends User {}
来源：http://oxr.iojbl.cn

Java: class Admin extends User {}
来源：http://gfr.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zxs.epnwcf.com

Ruby: class Admin < User; end
来源：http://yhk.jqgufenzy.top

C#:   class Admin : User {}
来源：http://wtz.smart0.xyz

[G06] 重写方法
来源：http://cap.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://cdf.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pcn.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://lqu.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://con.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://fpi.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zxs.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://qhg.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://bnn.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://tjy.shuidangran.top

Py:   super().greet()
来源：http://cgt.daxiang520.top

PHP:  parent::greet();
来源：http://omb.gogol.net.cn

JS:   super.greet();
来源：http://dip.ppjwa.cn

TS:   super.greet();
来源：http://pxi.dianchejie.cn

Java: super.greet();
来源：http://sug.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tph.bbcook.cn

Ruby: super
来源：http://luw.ctjpmb.com

C#:   base.Greet();
来源：http://qlu.hcnkem.com

[G08] 静态方法与属性
来源：http://kzh.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://amu.yongpay.top

PHP:  public static function f() {}
来源：http://vam.zhijiandao.cn

JS:   static f() {}
来源：http://rlp.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://mep.jinqigfzy.top

Java: static void f() {}
来源：http://nnp.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ogc.tanke756.top

Ruby: def self.f; end
来源：http://hqm.cucudq.cn

C#:   public static void F() {}
来源：http://sni.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://qsx.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://xfr.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://vxq.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cgy.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://zck.hnqzz.top

Java: interface Shape { double area(); }
来源：http://umh.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://mui.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fnd.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://nzd.c1oappe.top

[G10] 访问控制
来源：http://fwd.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://rnw.zhiwuduotai.top

PHP:  public / protected / private
来源：http://paz.daria6918.cn

JS:   #private 字段；其余公开
来源：http://ojj.ctjpmb.com

TS:   public / protected / private
来源：http://pcf.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://otg.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fie.yfazqb.com

Ruby: public / protected / private
来源：http://iul.meibo888.top

C#:   public / protected / private / internal
来源：http://ywi.xinyue.icu

[G11] getter / setter
来源：http://zil.52xcode.cn

Py:   @property 与 @x.setter
来源：http://xfk.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wsd.fengsongda.top

JS:   get name() { return this._name; }
来源：http://tje.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://ocy.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://oyr.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cwz.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://jhg.nwbrower.top

C#:   public string Name { get; set; }
来源：http://xov.yj20258888.top

[G12] 对象转字符串
来源：http://dkj.yonumen.top

Py:   def __str__(self): return self.name
来源：http://pac.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kru.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://wqc.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://omz.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://rfi.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qdq.hnqzz.top

Ruby: def to_s; @name; end
来源：http://csb.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://stw.xinyue.icu

[G13] 判断对象类型
来源：http://yaz.hnqzz.top

Py:   isinstance(u, User)
来源：http://lly.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://hpq.tanke756.top

JS:   u instanceof User
来源：http://kmv.yonumen.top

TS:   u instanceof User
来源：http://xlc.sweek.top

Java: u instanceof User
来源：http://wez.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ozc.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://rnm.bbcook.cn

C#:   u is User
来源：http://bgi.mhx1999.top

[G14] 数据类 / record
来源：http://fmz.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vaf.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://noi.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://kkr.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://jzw.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://nqz.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://dnm.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dke.tarul.cn

C#:   record User(string Name, int Age);
来源：http://pdm.bbcook.cn

[G15] 枚举
来源：http://usb.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hlk.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://eqs.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dyh.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nsj.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://egd.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wji.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://erf.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vgd.hammf.cn

[G16] 对象转数组 / 字典
来源：http://opf.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://crn.sweek.top

PHP:  get_object_vars($obj);
来源：http://mjx.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://cwk.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://cyj.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dok.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://faz.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://ngc.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://smw.wangshuangyany.cn

================================================================================
来源：http://hpc.tanke756.top

H. 异常与错误处理
来源：http://kvq.zhiwuduotai.top

================================================================================
来源：http://ess.cucudq.cn

[H01] try / catch 基础
来源：http://xdd.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kms.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dlg.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fji.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://shw.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ciu.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://imm.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zxj.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uus.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://yyj.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://xdq.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tgg.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ixt.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lzi.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nhn.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zpq.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ybf.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ctn.hfpthk.cn

[H03] 主动抛出异常
来源：http://phx.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://ipm.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kcq.uphjek.com

JS:   throw new Error("错误信息");
来源：http://smw.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://zaw.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xhl.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bbx.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gvc.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://afe.sysykeji.top

[H04] 自定义异常类型
来源：http://pwh.uphjek.com

Py:   class MyError(Exception): pass
来源：http://gwt.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://ngs.yvedp.cn

JS:   class MyError extends Error {}
来源：http://fzr.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://qtw.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://ylj.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bst.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://qbo.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://nni.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://fcr.jiagoushi.top

Py:   except ValueError as e:
来源：http://qox.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mvx.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://ytb.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://byx.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://dvb.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cue.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://ujy.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wgr.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://vpk.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://jxl.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://bwo.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://ctt.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://pvl.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nus.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nyl.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://bvq.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://sql.zdbjq.cn

[H07] 断言
来源：http://bxa.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://pai.xziqi.cn

PHP:  assert($x > 0);
来源：http://ovf.cashguo.top

JS:   console.assert(x > 0);
来源：http://piq.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://aha.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://jon.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uel.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://sak.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://zsh.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://bjg.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://skj.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://amc.birdmap.top

JS:   e.message;  e.stack
来源：http://pmp.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mws.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ykj.cucudq.cn

Go:   err.Error()
来源：http://yha.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://vgo.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://quw.cashguo.top

[H09] 带错误码的异常
来源：http://tte.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ney.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://zqh.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ymn.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sog.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dyk.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://orn.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://vml.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://arh.xuanzx.com

[H10] 资源自动释放
来源：http://sfo.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xhb.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dsc.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bdf.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rqn.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ezc.tarul.cn

Go:   defer f.Close()
来源：http://pxo.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cnf.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fdn.snrcjt.cn

================================================================================
来源：http://qkn.tarul.cn

I. 正则表达式
来源：http://kkr.nwbrower.top

================================================================================
来源：http://tgd.andypj.xyz

[I01] 判断是否匹配
来源：http://pso.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bax.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://fnq.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://fnp.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://pnp.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://brj.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gzh.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://jcu.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://duj.xinyue.icu

[I02] 提取所有匹配
来源：http://ixd.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://xnc.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xpd.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rtx.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://haj.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zgz.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ejt.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://uxa.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tab.guowangkeji.top

[I03] 提取捕获分组
来源：http://ame.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tct.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yyx.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybb.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dfz.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://elq.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qav.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qog.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wcs.ctjpmb.com

[I04] 正则替换
来源：http://ffp.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wdl.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ggv.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://wvw.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://euw.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://bek.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://gdm.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://blj.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oic.xuanzx.com

[I05] 按正则拆分
来源：http://pbv.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://hzk.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bfh.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://uxv.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://cud.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://kod.316326.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wlk.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://fdd.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cgj.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://esi.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://crf.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nmv.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lxc.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ttc.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gmq.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lov.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ipv.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qzu.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://lvz.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vut.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nyc.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kft.haohaochexian.top

TS:   /error/gim
来源：http://wbq.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dkg.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ayx.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://boy.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qvm.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://bcd.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://okd.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lio.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sax.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mer.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lds.mhx1999.top


<!-- 参考信息 -->