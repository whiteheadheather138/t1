代发 wailian999

Java: class User {}
来源：http://zmy.ctjpmb.com

Go:   type User struct { Name string }
来源：http://obo.nanxinkj.top

Ruby: class User; end
来源：http://ayd.ctjpmb.com

C#:   class User {}
来源：http://hth.bbcook.cn

[G02] 构造函数
来源：http://jyl.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://ezj.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://qyc.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://sab.ivvv.top

TS:   constructor(public name: string) {}
来源：http://igb.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://afe.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lvg.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://pnd.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://ith.zhixingplan.top

[G03] 实例属性
来源：http://hfw.yangfankeji.com

Py:   self.name = "x"
来源：http://onj.fzhhl.top

PHP:  public string $name = "x";
来源：http://ogj.yvedp.cn

JS:   this.name = "x";
来源：http://ekr.yuxming.cn

TS:   name: string = "x";
来源：http://vpp.ywan-chungtsiang.top

Java: private String name;
来源：http://axb.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ivr.yongpay.top

Ruby: @name = "x"
来源：http://mjb.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://ohs.svipenyu.cn

[G04] 定义方法
来源：http://npd.xinyue.icu

Py:   def greet(self): return self.name
来源：http://jfa.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oyq.ywan-chungtsiang.top

JS:   greet() { return this.name; }
来源：http://zcq.zhengqikj.top

TS:   greet(): string { return this.name; }
来源：http://lrz.aibaodan.cn

Java: String greet() { return name; }
来源：http://vxc.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gbz.wangdashe.top

Ruby: def greet; @name; end
来源：http://thk.birdmap.top

C#:   public string Greet() => Name;
来源：http://niv.smart0.xyz

[G05] 继承
来源：http://ber.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://nzl.uphjek.com

PHP:  class Admin extends User {}
来源：http://lcu.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://glc.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://rfn.zhoulong.xyz

Java: class Admin extends User {}
来源：http://vyg.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uuq.meibo888.top

Ruby: class Admin < User; end
来源：http://ybo.yj20258.top

C#:   class Admin : User {}
来源：http://xpa.0kj1m.cn

[G06] 重写方法
来源：http://yly.cashguo.top

Py:   def greet(self): return "admin"
来源：http://jav.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://alw.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://une.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://prt.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://qit.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fja.birdmap.top

Ruby: def greet; "admin"; end
来源：http://xuu.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://yap.fehbvm.com

[G07] 调用父类方法
来源：http://nqp.shuidangran.top

Py:   super().greet()
来源：http://dux.jqgufenzy.top

PHP:  parent::greet();
来源：http://gzu.yonumen.top

JS:   super.greet();
来源：http://kwa.hywenlv.cn

TS:   super.greet();
来源：http://sbp.sxryk.cn

Java: super.greet();
来源：http://tuo.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hke.zhaomingkeji.xyz

Ruby: super
来源：http://tij.ydzc1.top

C#:   base.Greet();
来源：http://tmr.ehwqpu.com

[G08] 静态方法与属性
来源：http://jsn.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nal.gotoacloud.top

PHP:  public static function f() {}
来源：http://eqb.ppjwa.cn

JS:   static f() {}
来源：http://phw.xylfe.cn

TS:   static f(): void {}
来源：http://gly.shangyingyoupin.top

Java: static void f() {}
来源：http://ogq.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bld.sjlbkw.cn

Ruby: def self.f; end
来源：http://djx.pycfn.com

C#:   public static void F() {}
来源：http://cnx.aizwys.cn

[G09] 接口 / 抽象类
来源：http://nle.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://yon.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://crs.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kzd.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://fmo.epnwcf.com

Java: interface Shape { double area(); }
来源：http://eye.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://mja.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qdb.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://egj.sysykeji.top

[G10] 访问控制
来源：http://odx.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://xmq.fehbvm.com

PHP:  public / protected / private
来源：http://ppu.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://cfn.sufxvd.cn

TS:   public / protected / private
来源：http://gun.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://pbb.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sub.epnwcf.com

Ruby: public / protected / private
来源：http://gmy.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://uni.jyoumei.cn

[G11] getter / setter
来源：http://uia.redwolf501.top

Py:   @property 与 @x.setter
来源：http://zyn.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ixk.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://eqt.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://sjh.daria6918.cn

Java: public String getName() { return name; }
来源：http://nwz.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://muo.hesvh.cn

Ruby: attr_accessor :name
来源：http://kgm.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://nla.0kj1m.cn

[G12] 对象转字符串
来源：http://zfn.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://ylw.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ahr.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://fip.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://rle.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://jay.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://awf.shuidangran.top

Ruby: def to_s; @name; end
来源：http://cdd.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://hmh.hnqzz.top

[G13] 判断对象类型
来源：http://idi.yangfankeji.com

Py:   isinstance(u, User)
来源：http://tks.tian-w.cn

PHP:  $u instanceof User
来源：http://nsi.ydjk.org.cn

JS:   u instanceof User
来源：http://xrw.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://ybh.havefunace.top

Java: u instanceof User
来源：http://ero.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://veh.hnqzz.top

Ruby: u.is_a?(User)
来源：http://bmo.wangdashe.top

C#:   u is User
来源：http://xpv.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://pke.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iwd.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://xwe.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://dgc.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://gmk.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://dwg.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://kbl.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bic.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://ewe.fanxiaobao.xyz

[G15] 枚举
来源：http://mys.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vpn.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ejc.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ltv.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hgg.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://ksn.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mgl.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://nck.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jln.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://roq.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jal.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://bfg.c1oappe.top

JS:   Object.entries(obj)
来源：http://nps.cqqwz.cn

TS:   Object.entries(obj)
来源：http://ooy.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tuv.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qrt.redwolf501.top

Ruby: obj.instance_variables
来源：http://xhf.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://mnv.dashuyun.cn

================================================================================
来源：http://fdf.chenzaomai.com

H. 异常与错误处理
来源：http://pbb.ehwqpu.com

================================================================================
来源：http://dko.cashguo.top

[H01] try / catch 基础
来源：http://eip.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ocq.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gtd.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jgx.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://azz.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qdw.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wtu.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jnw.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ecw.sxryk.cn

[H02] finally / ensure 收尾
来源：http://guh.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ztf.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wjn.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rzy.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bxv.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://ujr.sufxvd.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qdd.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rks.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vdb.sjlbkw.cn

[H03] 主动抛出异常
来源：http://csb.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://qvs.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bij.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://lxp.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://ssh.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nib.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bjt.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zov.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hjf.yj20258.top

[H04] 自定义异常类型
来源：http://vqx.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://itq.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sum.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://zqv.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://zwd.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://tbw.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pgz.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://vky.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://lry.xylfe.cn

[H05] 捕获特定类型
来源：http://dsq.hesvh.cn

Py:   except ValueError as e:
来源：http://xzd.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xyi.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://fjr.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://baw.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://iwy.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yci.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://kor.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rbw.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://iuz.cucudq.cn

Py:   value = d.get("k") or default
来源：http://mlu.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://ota.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://jva.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://pnq.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qje.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nyz.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://kfq.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://btr.xuanzx.com

[H07] 断言
来源：http://ihh.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://rnf.haohaochexian.top

PHP:  assert($x > 0);
来源：http://myu.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://enb.yuanzhike.top

TS:   console.assert(x > 0);
来源：http://cir.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://mkv.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zoy.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hol.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://twg.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://mlm.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://zfv.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://elh.xylfe.cn

JS:   e.message;  e.stack
来源：http://mvq.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nbp.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yfv.shanyushiyangkeji.top

Go:   err.Error()
来源：http://wyc.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://lmf.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://wep.316326.xyz

[H09] 带错误码的异常
来源：http://xuo.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tfn.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jop.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ram.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://exd.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qoo.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pyh.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wqc.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xbq.xinyue.icu

[H10] 资源自动释放
来源：http://olv.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://trg.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lhz.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ngn.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eww.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ovq.jianghu66.top

Go:   defer f.Close()
来源：http://zoh.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qsb.jinqigfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vmv.zhongyouzk.top

================================================================================
来源：http://dpl.zhongyouzk.top

I. 正则表达式
来源：http://tjr.zhaomingkeji.xyz

================================================================================
来源：http://mvh.aizwys.cn

[I01] 判断是否匹配
来源：http://osu.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vop.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://ccv.316326.xyz

JS:   /\d+/.test(s)
来源：http://sid.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://veq.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xkl.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mtw.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://sml.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pvh.shuidangran.top

[I02] 提取所有匹配
来源：http://esm.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://zqu.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pks.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hyh.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://kng.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cfr.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mah.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://scy.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aji.ydzc1.top

[I03] 提取捕获分组
来源：http://zcp.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wik.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uqz.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xxk.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zew.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rly.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vqk.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://niv.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aid.quarkkingdee.top

[I04] 正则替换
来源：http://mxd.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://voa.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zwz.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://yvc.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://yqp.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yvu.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ztv.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hcl.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bhf.redwolf501.top

[I05] 按正则拆分
来源：http://avt.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://keb.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://raa.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://bgc.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://xya.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://drv.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cds.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://wqw.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://asx.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://shz.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qae.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rax.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wrw.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywn.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://djy.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yjy.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ogw.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bug.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://wzb.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jmu.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yfd.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tam.yangfankeji.com

TS:   /error/gim
来源：http://qje.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xbm.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vuk.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://qym.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fws.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://pjo.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ubi.pengpengdd.cyou


<!-- 参考信息 -->