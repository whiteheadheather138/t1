代发 wailian999

[G02] 构造函数
来源：http://xdb.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://cny.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://wmo.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://xux.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://wdw.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://qkl.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vbc.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://oel.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://xey.redwolf501.top

[G03] 实例属性
来源：http://vwj.ehwqpu.com

Py:   self.name = "x"
来源：http://oxz.jyoumei.cn

PHP:  public string $name = "x";
来源：http://yjy.redwolf501.top

JS:   this.name = "x";
来源：http://jyj.gotoacloud.top

TS:   name: string = "x";
来源：http://bbm.cdnleiting.top

Java: private String name;
来源：http://glc.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oiy.cheryme.top

Ruby: @name = "x"
来源：http://zya.chenjidiqi.icu

C#:   public string Name { get; set; } = "x";
来源：http://mqj.ehwqpu.com

[G04] 定义方法
来源：http://lwt.jianghu66.top

Py:   def greet(self): return self.name
来源：http://knu.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cad.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://nef.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://kak.hywenlv.cn

Java: String greet() { return name; }
来源：http://nje.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://kmj.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://bmf.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://lim.shanyushiyangtech.top

[G05] 继承
来源：http://ipc.epnwcf.com

Py:   class Admin(User): pass
来源：http://jqg.aizwys.cn

PHP:  class Admin extends User {}
来源：http://jgu.zdqjudy.top

JS:   class Admin extends User {}
来源：http://jkk.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://ihp.bbcook.cn

Java: class Admin extends User {}
来源：http://dbq.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fml.aibaodan.cn

Ruby: class Admin < User; end
来源：http://wkj.xziqi.cn

C#:   class Admin : User {}
来源：http://cjk.jinqigfzy.top

[G06] 重写方法
来源：http://aav.pycfn.com

Py:   def greet(self): return "admin"
来源：http://uvh.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://unj.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://arl.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://qnt.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://bvb.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mrt.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://imi.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://teg.sxryk.cn

[G07] 调用父类方法
来源：http://yqa.tanke756.top

Py:   super().greet()
来源：http://viv.gotoacloud.top

PHP:  parent::greet();
来源：http://emv.zhengqikj.top

JS:   super.greet();
来源：http://dwb.jinqigufen.top

TS:   super.greet();
来源：http://gef.gotoacloud.top

Java: super.greet();
来源：http://xuh.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kel.yongpay.top

Ruby: super
来源：http://cfh.fengsongda.top

C#:   base.Greet();
来源：http://uou.jqgufenzy.top

[G08] 静态方法与属性
来源：http://nft.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pqk.smart0.xyz

PHP:  public static function f() {}
来源：http://ffv.gaohongyu789.top

JS:   static f() {}
来源：http://nos.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://xzb.tian-w.cn

Java: static void f() {}
来源：http://skp.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ajq.chenlongwang.top

Ruby: def self.f; end
来源：http://ctj.jiagoushi.top

C#:   public static void F() {}
来源：http://xjw.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://evu.svipenyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://rul.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uvh.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tko.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://tpg.ivvv.top

Java: interface Shape { double area(); }
来源：http://mmh.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://gum.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://enw.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://vhc.chenzaomai.com

[G10] 访问控制
来源：http://zck.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://waf.zhixingplan.top

PHP:  public / protected / private
来源：http://mdt.ydzc1.top

JS:   #private 字段；其余公开
来源：http://qfm.bjfxy.top

TS:   public / protected / private
来源：http://grz.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://pjf.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zjt.hnxiangtu.top

Ruby: public / protected / private
来源：http://xpb.aizwys.cn

C#:   public / protected / private / internal
来源：http://eux.cqqwz.cn

[G11] getter / setter
来源：http://jnq.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://wpq.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ufl.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://enj.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://fsl.jyoumei.cn

Java: public String getName() { return name; }
来源：http://duh.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uze.chenzaomai.com

Ruby: attr_accessor :name
来源：http://adq.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://mnc.gzhubu.top

[G12] 对象转字符串
来源：http://wdk.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://icm.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ibx.hesvh.cn

JS:   toString() { return this.name; }
来源：http://rau.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://uwx.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://cyj.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://nop.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://hvb.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://acd.fktsv.cn

[G13] 判断对象类型
来源：http://boa.wangdashe.top

Py:   isinstance(u, User)
来源：http://bjv.cdnleiting.top

PHP:  $u instanceof User
来源：http://kab.zhixingplan.top

JS:   u instanceof User
来源：http://dqb.hongshengwenyu.top

TS:   u instanceof User
来源：http://uyt.52xcode.cn

Java: u instanceof User
来源：http://dlk.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bhq.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://nhf.jiagoushi.top

C#:   u is User
来源：http://ejv.xuetiantiany.cn

[G14] 数据类 / record
来源：http://wwm.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xpb.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://ygu.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://fwg.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://oqo.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://mfq.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://syz.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vgh.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://bhq.ehwqpu.com

[G15] 枚举
来源：http://rtw.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fze.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ilv.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mkj.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://stw.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://vhp.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ngo.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://cyr.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://doj.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://vyz.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dew.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://pze.birdmap.top

JS:   Object.entries(obj)
来源：http://ism.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://tax.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pqn.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://szu.jqgfzy.top

Ruby: obj.instance_variables
来源：http://jzb.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://cbs.wangdashe.top

================================================================================
来源：http://gej.jinqigufen.top

H. 异常与错误处理
来源：http://znx.hnqzz.top

================================================================================
来源：http://ctr.redwolf501.top

[H01] try / catch 基础
来源：http://jak.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bqq.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jos.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zqp.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vbc.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zar.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sso.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gcw.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tvp.mhx1999.top

[H02] finally / ensure 收尾
来源：http://qhd.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gyg.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zbb.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ahi.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://plu.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tyg.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rlb.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vff.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pnd.hysaishi.cn

[H03] 主动抛出异常
来源：http://bby.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://rmk.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://coo.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://zzx.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://ugc.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fie.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pdg.quarkkingdee.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rbg.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yuq.zhijiandao.cn

[H04] 自定义异常类型
来源：http://aal.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://ojf.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://qau.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://wjw.yonumen.top

TS:   class MyError extends Error {}
来源：http://pnr.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://syh.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://myk.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://iau.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://mdk.jinqigfzy.top

[H05] 捕获特定类型
来源：http://dnv.vehdjk.com

Py:   except ValueError as e:
来源：http://lrb.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hxq.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://tav.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://aac.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://oia.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://odf.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://qwg.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wbi.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://uts.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://hqz.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gdl.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jgf.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tbq.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jwj.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wuv.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://cim.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://ltk.9152youxi.cn

[H07] 断言
来源：http://kxv.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://vqe.yvedp.cn

PHP:  assert($x > 0);
来源：http://iet.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://edt.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://qnt.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://sfn.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jjr.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://msa.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://oyq.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://pyr.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://gzi.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xdr.zycfv.cn

JS:   e.message;  e.stack
来源：http://vsl.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yps.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://inx.aibaodan.cn

Go:   err.Error()
来源：http://zvj.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://mnb.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://crl.yj202588.top

[H09] 带错误码的异常
来源：http://efj.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dic.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sny.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fef.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ehu.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iko.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aya.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://vpq.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cmx.guowangkeji.top

[H10] 资源自动释放
来源：http://obi.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vrd.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mvf.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mad.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cgt.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ufu.zdbjq.cn

Go:   defer f.Close()
来源：http://mpo.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xtq.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xjd.yj202588.top

================================================================================
来源：http://qpu.bjfxy.top

I. 正则表达式
来源：http://iwh.dashuyun.cn

================================================================================
来源：http://oow.xziqi.cn

[I01] 判断是否匹配
来源：http://zub.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pcz.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://pdp.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://nba.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://yuq.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://noq.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://slo.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://frm.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iml.nanxuanxn.top

[I02] 提取所有匹配
来源：http://cub.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://cyb.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ica.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://clo.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://xzk.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bia.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oun.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://tbo.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ycm.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://vxz.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rlr.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tfq.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uyc.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jkc.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://umb.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vui.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvy.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vph.smart0.xyz

[I04] 正则替换
来源：http://yyi.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yge.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://anx.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://edq.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rhn.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://hww.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xxm.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jjk.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mcl.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://vfc.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://juy.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kaq.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://wau.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://lcq.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://tzg.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nkb.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://bfz.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wzo.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kqh.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://huj.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tcs.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxl.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fpe.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dja.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://orw.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yag.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gng.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://huj.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zoj.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yax.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wtv.zhijiandao.cn

TS:   /error/gim
来源：http://hke.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nsh.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fmn.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://iuz.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://emk.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://nks.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fyz.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fys.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sdv.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qit.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tct.yongpay.top


<!-- 参考信息 -->