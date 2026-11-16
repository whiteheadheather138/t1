代发 wailian999

[G02] 构造函数
来源：http://wkp.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://mjy.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://fya.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://wjf.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://qoh.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://dcn.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nkm.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://mij.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://hsq.ivvv.top

[G03] 实例属性
来源：http://epx.zdbjq.cn

Py:   self.name = "x"
来源：http://wpu.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://ncs.gaohongyu789.top

JS:   this.name = "x";
来源：http://dtp.yuanzhike.top

TS:   name: string = "x";
来源：http://rlz.zhijiandao.cn

Java: private String name;
来源：http://zyx.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hwn.yuxming.cn

Ruby: @name = "x"
来源：http://knv.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://lsl.hfpthk.cn

[G04] 定义方法
来源：http://wmp.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://svk.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mpn.hcnkem.com

JS:   greet() { return this.name; }
来源：http://zox.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://fro.gaohongyu789.top

Java: String greet() { return name; }
来源：http://mcb.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zms.aibaodan.cn

Ruby: def greet; @name; end
来源：http://qwx.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://txy.epnwcf.com

[G05] 继承
来源：http://kmc.zycfv.cn

Py:   class Admin(User): pass
来源：http://btp.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://wzc.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://ouh.ehwqpu.com

TS:   class Admin extends User {}
来源：http://ivk.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://gyy.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wkw.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://sey.mhx1999.top

C#:   class Admin : User {}
来源：http://ynv.wangdashe.top

[G06] 重写方法
来源：http://hkv.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://syt.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://utb.yonumen.top

JS:   greet() { return "admin"; }
来源：http://qog.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://hvi.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://ydw.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://obb.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://zam.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://qvs.shangyingyoupin.top

[G07] 调用父类方法
来源：http://piw.zycfv.cn

Py:   super().greet()
来源：http://jiw.yj20258888.top

PHP:  parent::greet();
来源：http://ldq.jqgufenzy.top

JS:   super.greet();
来源：http://fco.zdbjq.cn

TS:   super.greet();
来源：http://wpk.nwbrower.top

Java: super.greet();
来源：http://hed.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vag.jqgufenzy.top

Ruby: super
来源：http://tph.yongpay.top

C#:   base.Greet();
来源：http://qmi.jianghu66.top

[G08] 静态方法与属性
来源：http://tqr.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://axf.xylfe.cn

PHP:  public static function f() {}
来源：http://phe.yongpay.top

JS:   static f() {}
来源：http://kyc.yueranfly.top

TS:   static f(): void {}
来源：http://hbi.svipenyu.cn

Java: static void f() {}
来源：http://giy.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sqz.svipenyu.cn

Ruby: def self.f; end
来源：http://ekg.tanke756.top

C#:   public static void F() {}
来源：http://mgp.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://mmc.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://man.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://wxv.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://abh.xuanzx.com

TS:   interface Shape { area(): number; }
来源：http://uaf.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://lvc.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://qsy.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zbd.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://pwr.snrcjt.cn

[G10] 访问控制
来源：http://dty.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://eub.cdnleiting.top

PHP:  public / protected / private
来源：http://lwb.fktsv.cn

JS:   #private 字段；其余公开
来源：http://bck.guannengcc.top

TS:   public / protected / private
来源：http://wly.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://eeo.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ooe.redwolf501.top

Ruby: public / protected / private
来源：http://rtt.dashuyun.cn

C#:   public / protected / private / internal
来源：http://igl.cucudq.cn

[G11] getter / setter
来源：http://ohc.jianghu66.top

Py:   @property 与 @x.setter
来源：http://xge.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://uqo.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://inx.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://cqt.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://boz.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://iam.shzxlz.cn

Ruby: attr_accessor :name
来源：http://olz.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://kvg.jqgfzy.top

[G12] 对象转字符串
来源：http://llx.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://ddt.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gmk.fengsongda.top

JS:   toString() { return this.name; }
来源：http://awf.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://fsi.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://bjs.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://hfj.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://btp.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://dja.birdmap.top

[G13] 判断对象类型
来源：http://lla.hesvh.cn

Py:   isinstance(u, User)
来源：http://esl.hesvh.cn

PHP:  $u instanceof User
来源：http://oyf.havefunace.top

JS:   u instanceof User
来源：http://jus.yuxming.cn

TS:   u instanceof User
来源：http://ovn.chenjidiqi.icu

Java: u instanceof User
来源：http://ktf.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kgb.bbcook.cn

Ruby: u.is_a?(User)
来源：http://qaz.yonumen.top

C#:   u is User
来源：http://hwy.dashuyun.cn

[G14] 数据类 / record
来源：http://pdf.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wrx.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://ika.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://kut.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://csp.xylfe.cn

Java: record User(String name, int age) {}
来源：http://ona.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://qvm.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mes.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://war.cqqwz.cn

[G15] 枚举
来源：http://soq.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://umw.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ofy.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://krd.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://req.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://iim.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ejv.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://res.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tvl.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://cti.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eby.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://glj.dianchejie.cn

JS:   Object.entries(obj)
来源：http://egn.aizwys.cn

TS:   Object.entries(obj)
来源：http://kcz.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pcl.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://imk.aibaodan.cn

Ruby: obj.instance_variables
来源：http://msi.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://pqy.pengpengdd.cyou

================================================================================
来源：http://nfp.9152youxi.cn

H. 异常与错误处理
来源：http://uzy.zhijiandao.cn

================================================================================
来源：http://xyv.shuidangran.top

[H01] try / catch 基础
来源：http://scd.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dtz.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oql.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ooe.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ges.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ehk.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nqt.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bai.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nss.meibo888.top

[H02] finally / ensure 收尾
来源：http://yyi.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://rqy.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ypl.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wcz.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://eje.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://dvm.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://spb.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://evc.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mqn.zhijiandao.cn

[H03] 主动抛出异常
来源：http://awa.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://zji.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lbo.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://bjw.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://ubg.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://hkb.tanke756.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fup.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gbx.jinyuanbaomall.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gda.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://tpk.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://nfe.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nua.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://tln.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://mto.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://blg.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hkt.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://qwd.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://hac.jyoumei.cn

[H05] 捕获特定类型
来源：http://ppo.hcnkem.com

Py:   except ValueError as e:
来源：http://ymi.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tbi.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://gks.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://tlw.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://oxr.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ssc.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://mit.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tzf.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://muu.cucudq.cn

Py:   value = d.get("k") or default
来源：http://sfl.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://rsw.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://ifx.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://hue.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wqu.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mbk.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://ubx.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://cpx.cucudq.cn

[H07] 断言
来源：http://yox.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://tlk.zycfv.cn

PHP:  assert($x > 0);
来源：http://mhr.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://bbh.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://fuf.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://ggy.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ker.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tki.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://tft.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://xzu.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://rxl.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fnt.smart0.xyz

JS:   e.message;  e.stack
来源：http://gfg.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://chn.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://odc.zycfv.cn

Go:   err.Error()
来源：http://nfl.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://yqy.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://snb.ydjk.org.cn

[H09] 带错误码的异常
来源：http://vkj.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jru.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdp.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dgp.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jjr.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dqt.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ytf.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://gmg.zdqjudy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ror.yanxiufei.cn

[H10] 资源自动释放
来源：http://tcl.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://tfs.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://beb.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://omj.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xqv.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ovd.cucudq.cn

Go:   defer f.Close()
来源：http://kxn.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sci.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vhb.fanxiaobao.xyz

================================================================================
来源：http://khc.bbcook.cn

I. 正则表达式
来源：http://wxy.zhixingplan.top

================================================================================
来源：http://qsy.haohaochexian.top

[I01] 判断是否匹配
来源：http://wpa.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xnu.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xev.andypj.xyz

JS:   /\d+/.test(s)
来源：http://zzo.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://vxw.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ipp.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mkl.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://dvl.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yvg.kuanghao11.cn

[I02] 提取所有匹配
来源：http://vwf.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://its.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pis.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nkz.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://bwb.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dhv.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fzk.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://ghz.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://efb.svipenyu.cn

[I03] 提取捕获分组
来源：http://usy.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vpz.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tsl.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jlg.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pkt.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vhm.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wjc.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hte.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nee.hcnkem.com

[I04] 正则替换
来源：http://erf.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://azz.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://grg.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://enb.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vvr.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://ttw.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hzw.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://imh.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://onl.shuidangran.top

[I05] 按正则拆分
来源：http://sav.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://brp.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lsi.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://upl.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://ilq.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://kia.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xum.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://tye.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://det.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gpr.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cwx.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rts.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dru.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ulg.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fli.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cui.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kik.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vdp.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://ism.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pdo.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kdn.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bbq.ybcxt.top

TS:   /error/gim
来源：http://ces.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pdn.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uev.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://pjv.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ats.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://gof.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nor.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fya.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qyr.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qwv.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kdl.pycfn.com


<!-- 参考信息 -->