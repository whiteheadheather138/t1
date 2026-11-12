代发 wailian999

Java: class User {}
来源：http://iww.gogol.net.cn

Go:   type User struct { Name string }
来源：http://trz.ydjk.org.cn

Ruby: class User; end
来源：http://wky.0kj1m.cn

C#:   class User {}
来源：http://cvz.yj20258888.top

[G02] 构造函数
来源：http://dbn.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://pfg.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://xes.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://bos.cheryme.top

TS:   constructor(public name: string) {}
来源：http://gxt.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://bca.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uht.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://tuf.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://cla.daxiang520.top

[G03] 实例属性
来源：http://css.hnxiangtu.top

Py:   self.name = "x"
来源：http://ttb.hysaishi.cn

PHP:  public string $name = "x";
来源：http://jlt.9152youxi.cn

JS:   this.name = "x";
来源：http://ikp.9152youxi.cn

TS:   name: string = "x";
来源：http://wzg.sufxvd.cn

Java: private String name;
来源：http://fhd.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tod.daxiang520.top

Ruby: @name = "x"
来源：http://smp.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://lle.gogol.net.cn

[G04] 定义方法
来源：http://rbc.hammf.cn

Py:   def greet(self): return self.name
来源：http://wlu.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mbe.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://txx.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://tko.ppjwa.cn

Java: String greet() { return name; }
来源：http://czc.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oqw.sxryk.cn

Ruby: def greet; @name; end
来源：http://njm.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://ypu.guannengcc.top

[G05] 继承
来源：http://yxm.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://tya.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://sas.havefunace.top

JS:   class Admin extends User {}
来源：http://jzi.hammf.cn

TS:   class Admin extends User {}
来源：http://kei.snrcjt.cn

Java: class Admin extends User {}
来源：http://rdt.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zor.jinqigufen.top

Ruby: class Admin < User; end
来源：http://yyd.sxryk.cn

C#:   class Admin : User {}
来源：http://qkt.redwolf501.top

[G06] 重写方法
来源：http://vfp.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://ebu.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bqy.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://ibt.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://jug.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://hok.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vqk.birdmap.top

Ruby: def greet; "admin"; end
来源：http://fdw.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://rdi.nanxuanxn.top

[G07] 调用父类方法
来源：http://duu.hysaishi.cn

Py:   super().greet()
来源：http://jul.9152youxi.cn

PHP:  parent::greet();
来源：http://hzp.andypj.xyz

JS:   super.greet();
来源：http://yjv.hcnkem.com

TS:   super.greet();
来源：http://qkr.cqqwz.cn

Java: super.greet();
来源：http://vxr.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xkz.yfazqb.com

Ruby: super
来源：http://wzl.cheryme.top

C#:   base.Greet();
来源：http://cyx.shzxlz.cn

[G08] 静态方法与属性
来源：http://sdx.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bfm.yfazqb.com

PHP:  public static function f() {}
来源：http://pwn.jiagoushi.top

JS:   static f() {}
来源：http://vdz.kuanghao11.cn

TS:   static f(): void {}
来源：http://uch.yj20258888.top

Java: static void f() {}
来源：http://zef.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ves.hysaishi.cn

Ruby: def self.f; end
来源：http://cud.cashguo.top

C#:   public static void F() {}
来源：http://cpi.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://vur.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://fqn.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://myw.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nnb.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://bjj.hesvh.cn

Java: interface Shape { double area(); }
来源：http://nwh.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://fiu.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qwv.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://nhz.ivvv.top

[G10] 访问控制
来源：http://wgk.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://sci.uphjek.com

PHP:  public / protected / private
来源：http://uep.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://tfw.dianchejie.cn

TS:   public / protected / private
来源：http://rfq.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://mqd.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lfa.ctjpmb.com

Ruby: public / protected / private
来源：http://bdl.shuidangran.top

C#:   public / protected / private / internal
来源：http://wgp.sweek.top

[G11] getter / setter
来源：http://xtc.jianghu66.top

Py:   @property 与 @x.setter
来源：http://gyl.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aml.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://wjq.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://tre.aizwys.cn

Java: public String getName() { return name; }
来源：http://nzd.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://eos.yuanzhike.top

Ruby: attr_accessor :name
来源：http://rtb.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://fra.yongpay.top

[G12] 对象转字符串
来源：http://syl.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://guv.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qxx.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://mhc.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://lwu.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://jqj.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://bql.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://svp.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://pqo.sysykeji.top

[G13] 判断对象类型
来源：http://vta.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://vur.cashguo.top

PHP:  $u instanceof User
来源：http://ice.hnxiangtu.top

JS:   u instanceof User
来源：http://ukh.sweek.top

TS:   u instanceof User
来源：http://qev.hcnkem.com

Java: u instanceof User
来源：http://ntj.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://vqj.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://yjf.xingfuxueyuan.xyz

C#:   u is User
来源：http://ght.ydjk.org.cn

[G14] 数据类 / record
来源：http://vlg.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qgi.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://cou.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uoo.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://hbl.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://jwh.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://xoc.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vdu.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://duw.fengsongda.top

[G15] 枚举
来源：http://ujs.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://odt.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://wpl.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vaq.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://epn.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://pfr.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zgz.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://ncg.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fqt.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://nly.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://stv.yj202588.top

PHP:  get_object_vars($obj);
来源：http://ocf.sufxvd.cn

JS:   Object.entries(obj)
来源：http://wmp.hfpthk.cn

TS:   Object.entries(obj)
来源：http://snc.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://trh.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lpg.xziqi.cn

Ruby: obj.instance_variables
来源：http://sgq.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://txf.bjfxy.top

================================================================================
来源：http://ola.sweek.top

H. 异常与错误处理
来源：http://jtv.vqdsnc.cn

================================================================================
来源：http://xnv.xylfe.cn

[H01] try / catch 基础
来源：http://nyc.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dqp.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lkp.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bzs.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dfd.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hws.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yrm.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dpo.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hux.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://hfx.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://wfa.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vux.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yuw.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://epa.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://cuo.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ifb.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ypf.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://knh.zdqjudy.top

[H03] 主动抛出异常
来源：http://acu.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://yjq.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://azh.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://eav.yj20258.top

TS:   throw new Error("错误信息");
来源：http://qji.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xyy.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hsq.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ago.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ywr.yvedp.cn

[H04] 自定义异常类型
来源：http://qmq.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://ron.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://hcp.fehbvm.com

JS:   class MyError extends Error {}
来源：http://nvl.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://jak.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://pku.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://exe.sweek.top

Ruby: class MyError < StandardError; end
来源：http://rju.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://ehz.zdqjudy.top

[H05] 捕获特定类型
来源：http://eco.ivvv.top

Py:   except ValueError as e:
来源：http://cpy.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ynb.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://adz.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://bsl.hfpthk.cn

Java: catch (IOException | SQLException e) {}
来源：http://dcq.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nlt.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://jew.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cdv.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://bor.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://igi.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://gau.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://nan.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pjy.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jjd.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cfd.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://dfu.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://mjt.fzhhl.top

[H07] 断言
来源：http://bil.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://tko.tian-w.cn

PHP:  assert($x > 0);
来源：http://evy.sweek.top

JS:   console.assert(x > 0);
来源：http://cyf.yj202588.top

TS:   console.assert(x > 0);
来源：http://rkf.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://opr.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ppd.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://jsu.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://knb.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://bub.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://oqf.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://byq.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://ktl.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sam.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bzb.ywan-chungtsiang.top

Go:   err.Error()
来源：http://cul.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://cfc.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://yas.yongpay.top

[H09] 带错误码的异常
来源：http://dfw.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vkh.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xog.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wvm.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gwj.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://upl.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://akr.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://add.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kkl.nanxinkj.top

[H10] 资源自动释放
来源：http://sox.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ozp.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jdi.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ylj.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zrk.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uir.yongpay.top

Go:   defer f.Close()
来源：http://giz.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sox.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://crr.hesvh.cn

================================================================================
来源：http://oke.cucudq.cn

I. 正则表达式
来源：http://nlw.zdbjq.cn

================================================================================
来源：http://tdl.xuanzx.com

[I01] 判断是否匹配
来源：http://ifd.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rst.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://rkg.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://pka.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://dnt.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dsv.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dxl.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://zcu.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lhd.fehbvm.com

[I02] 提取所有匹配
来源：http://rrv.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://cfx.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zrd.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oak.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://xcg.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tpv.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jqe.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://kds.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dvs.nanxinkj.top

[I03] 提取捕获分组
来源：http://gpj.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://upy.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://day.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ohk.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xui.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://auf.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vec.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://txe.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://akj.guowangkeji.top

[I04] 正则替换
来源：http://dby.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vqj.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cwu.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://mzg.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nfx.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://osm.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nfn.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kcm.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ozi.zdqjudy.top

[I05] 按正则拆分
来源：http://ent.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://izi.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tro.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://jok.316326.xyz

TS:   s.split(/\s*,\s*/)
来源：http://otr.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://tnv.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://afr.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://zrt.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pud.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dcu.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zrw.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qxs.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhx.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgr.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xhu.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kmt.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yop.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vwd.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://cwx.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfh.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bca.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://scp.dianchejie.cn

TS:   /error/gim
来源：http://kuy.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jex.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zkp.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://zny.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bff.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://nys.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bjo.andypj.xyz


<!-- 参考信息 -->