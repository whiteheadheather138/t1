代发 wailian999

Py:   class User: pass
来源：http://kgu.zycfv.cn

PHP:  class User {}
来源：http://gzy.c1oappe.top

JS:   class User {}
来源：http://nzb.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://uai.pengpengdd.cyou

Java: class User {}
来源：http://ggt.shuidangran.top

Go:   type User struct { Name string }
来源：http://nhr.xuetiantiany.cn

Ruby: class User; end
来源：http://trb.xingfuxueyuan.xyz

C#:   class User {}
来源：http://rzk.c1oappe.top

[G02] 构造函数
来源：http://yeo.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://ovn.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://crw.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://gyv.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://ohl.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://akm.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zfj.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://jtn.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://egy.jinqigfzy.top

[G03] 实例属性
来源：http://yjm.cqqwz.cn

Py:   self.name = "x"
来源：http://stw.yvedp.cn

PHP:  public string $name = "x";
来源：http://xhe.shangyingyoupin.top

JS:   this.name = "x";
来源：http://jel.ehwqpu.com

TS:   name: string = "x";
来源：http://xxk.jyoumei.cn

Java: private String name;
来源：http://nyk.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ars.meibo888.top

Ruby: @name = "x"
来源：http://mrk.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://kvr.zdqjudy.top

[G04] 定义方法
来源：http://tqz.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://yuj.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zoz.xziqi.cn

JS:   greet() { return this.name; }
来源：http://jql.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://rtj.zhongyouzk.top

Java: String greet() { return name; }
来源：http://cca.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://trd.jiagoushi.top

Ruby: def greet; @name; end
来源：http://njl.ydzc1.top

C#:   public string Greet() => Name;
来源：http://sgl.redwolf501.top

[G05] 继承
来源：http://jnl.bjfxy.top

Py:   class Admin(User): pass
来源：http://ygo.ybcxt.top

PHP:  class Admin extends User {}
来源：http://vmk.yj20258888.top

JS:   class Admin extends User {}
来源：http://cxa.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://ybu.zhongyouzk.top

Java: class Admin extends User {}
来源：http://fxd.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iir.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://ubu.yuanzhike.top

C#:   class Admin : User {}
来源：http://ble.jinghuilouyu.cn

[G06] 重写方法
来源：http://jso.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://wdj.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://llp.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://lag.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://rjm.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://nre.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dnv.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://ugi.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://hgc.ydjk.org.cn

[G07] 调用父类方法
来源：http://mdi.meibo888.top

Py:   super().greet()
来源：http://lok.fzhhl.top

PHP:  parent::greet();
来源：http://vdl.ybcxt.top

JS:   super.greet();
来源：http://ctz.cdnleiting.top

TS:   super.greet();
来源：http://jih.zycfv.cn

Java: super.greet();
来源：http://mji.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://egz.zhixingplan.top

Ruby: super
来源：http://nze.xinyue.icu

C#:   base.Greet();
来源：http://zqc.vqdsnc.cn

[G08] 静态方法与属性
来源：http://syv.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gqb.daria6918.cn

PHP:  public static function f() {}
来源：http://zds.jqgufenzy.top

JS:   static f() {}
来源：http://wag.vehdjk.com

TS:   static f(): void {}
来源：http://vqz.daria6918.cn

Java: static void f() {}
来源：http://yuu.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://yen.epnwcf.com

Ruby: def self.f; end
来源：http://axy.hnxiangtu.top

C#:   public static void F() {}
来源：http://lgz.shuidangran.top

[G09] 接口 / 抽象类
来源：http://jkn.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://hgb.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://vqx.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://kfz.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://tlq.xylfe.cn

Java: interface Shape { double area(); }
来源：http://mkr.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://rdb.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cel.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://etp.pycfn.com

[G10] 访问控制
来源：http://boh.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://axn.smart0.xyz

PHP:  public / protected / private
来源：http://knv.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://tve.ybcxt.top

TS:   public / protected / private
来源：http://msz.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://bbs.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aju.pycfn.com

Ruby: public / protected / private
来源：http://nky.aibaodan.cn

C#:   public / protected / private / internal
来源：http://ruc.hcnkem.com

[G11] getter / setter
来源：http://nxm.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://iwf.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ovp.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://puq.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://frr.wangdashe.top

Java: public String getName() { return name; }
来源：http://pih.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://diq.chenzaomai.com

Ruby: attr_accessor :name
来源：http://oex.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://qxj.gogol.net.cn

[G12] 对象转字符串
来源：http://lgy.tarul.cn

Py:   def __str__(self): return self.name
来源：http://dxw.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bhs.zycfv.cn

JS:   toString() { return this.name; }
来源：http://csm.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://kyi.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://hju.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://vap.fengsongda.top

Ruby: def to_s; @name; end
来源：http://jhk.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://sxh.jinqigufen.top

[G13] 判断对象类型
来源：http://bjx.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://yck.yfazqb.com

PHP:  $u instanceof User
来源：http://inq.meibo888.top

JS:   u instanceof User
来源：http://zdb.haohaochexian.top

TS:   u instanceof User
来源：http://hjg.yangfankeji.com

Java: u instanceof User
来源：http://rlh.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ada.redwolf501.top

Ruby: u.is_a?(User)
来源：http://dai.daria6918.cn

C#:   u is User
来源：http://nkd.quarkkingdee.top

[G14] 数据类 / record
来源：http://eyn.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cje.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://gdq.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jds.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://mlf.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://ixg.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://tqs.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xbw.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://qiq.zhengqikj.top

[G15] 枚举
来源：http://skx.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wcm.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nhi.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xmw.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tjt.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://zxs.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zrc.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://dzj.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djh.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://age.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tpa.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://scb.hfpthk.cn

JS:   Object.entries(obj)
来源：http://yjo.cqqwz.cn

TS:   Object.entries(obj)
来源：http://nqw.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mgo.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pew.aizwys.cn

Ruby: obj.instance_variables
来源：http://vms.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://ohf.snrcjt.cn

================================================================================
来源：http://ske.hongshengwenyu.top

H. 异常与错误处理
来源：http://clk.xinyue.icu

================================================================================
来源：http://rvg.9152youxi.cn

[H01] try / catch 基础
来源：http://oaj.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://esg.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ckr.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dly.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://grj.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wnz.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lur.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nwg.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fnh.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://huy.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ebs.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uii.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mff.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wff.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://sfl.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://otk.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rvp.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jzb.ppjwa.cn

[H03] 主动抛出异常
来源：http://kps.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://rds.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ovp.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://shr.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://afc.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lvs.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://azy.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kpi.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://maf.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://jhk.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://wmy.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://jeb.fehbvm.com

JS:   class MyError extends Error {}
来源：http://vyr.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://dkt.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://yvr.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bqk.zycfv.cn

Ruby: class MyError < StandardError; end
来源：http://dls.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://ckw.zhengqikj.top

[H05] 捕获特定类型
来源：http://gzb.gotoacloud.top

Py:   except ValueError as e:
来源：http://vjr.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yac.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://bga.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://pmh.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://kej.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mbv.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://ldg.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iqu.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://lrq.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://nsc.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rla.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kej.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://moh.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yjx.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xbj.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://jmw.dianchejie.cn

C#:   obj?.A?.B ?? default
来源：http://ian.yuxming.cn

[H07] 断言
来源：http://lhq.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://reb.redwolf501.top

PHP:  assert($x > 0);
来源：http://gww.daxiang520.top

JS:   console.assert(x > 0);
来源：http://qzk.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://pjm.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://jvx.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ocj.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://hwc.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://kog.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://her.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://zpo.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uja.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://tcy.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hzs.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jye.iojbl.cn

Go:   err.Error()
来源：http://bgy.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://xur.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://vtb.yuxming.cn

[H09] 带错误码的异常
来源：http://hgb.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qwl.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dtr.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eii.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hwn.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cqq.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://duq.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://yqh.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ggg.nanxuanxn.top

[H10] 资源自动释放
来源：http://cba.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ltb.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iia.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://spd.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nyb.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wpg.ehwqpu.com

Go:   defer f.Close()
来源：http://xbz.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qkb.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ein.jianghu66.top

================================================================================
来源：http://nzm.jqgfzy.top

I. 正则表达式
来源：http://yau.chenlongwang.top

================================================================================
来源：http://fmh.uphjek.com

[I01] 判断是否匹配
来源：http://fug.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vyi.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://jon.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://aqy.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://kch.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://azv.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mqo.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://bwo.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hbc.nanxuanxn.top

[I02] 提取所有匹配
来源：http://pna.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://xdp.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://trh.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cgl.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://ksb.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ppe.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://otm.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://rrq.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ena.jqgfzy.top

[I03] 提取捕获分组
来源：http://gry.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://crv.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rxq.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://psl.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xev.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tqd.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cup.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qiu.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fnm.jinghuilouyu.cn

[I04] 正则替换
来源：http://qyd.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uez.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wxt.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://nnd.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ias.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://emo.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://olm.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bvc.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ssi.yuanzhike.top

[I05] 按正则拆分
来源：http://whs.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://utv.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://grm.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://hhp.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://ayo.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://cxb.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfn.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://fta.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://igj.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lzr.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://muq.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jiu.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uov.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dvo.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gmb.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tja.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uaq.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gjp.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://kgk.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yhq.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xlu.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rqg.0kj1m.cn

TS:   /error/gim
来源：http://pql.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gwd.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ogf.uphjek.com


<!-- 参考信息 -->