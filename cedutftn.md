代发 wailian999

[G02] 构造函数
来源：http://nep.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://mal.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://thb.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://lmi.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://qet.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://bnf.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aaj.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://dpc.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://amq.zhongyouzk.top

[G03] 实例属性
来源：http://qxp.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://vpq.0kj1m.cn

PHP:  public string $name = "x";
来源：http://ide.ydjk.org.cn

JS:   this.name = "x";
来源：http://zsv.zhijiandao.cn

TS:   name: string = "x";
来源：http://fwt.smart0.xyz

Java: private String name;
来源：http://yri.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jmt.cdnleiting.top

Ruby: @name = "x"
来源：http://gzo.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://duf.ywan-chungtsiang.top

[G04] 定义方法
来源：http://vqq.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://tdk.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://emc.zhixingplan.top

JS:   greet() { return this.name; }
来源：http://mjc.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://jvr.sysykeji.top

Java: String greet() { return name; }
来源：http://xlc.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://alx.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://rei.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://hmd.zhijiandao.cn

[G05] 继承
来源：http://gfb.hysaishi.cn

Py:   class Admin(User): pass
来源：http://kyu.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://zzt.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://fex.haohaochexian.top

TS:   class Admin extends User {}
来源：http://uru.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://ngm.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hek.xylfe.cn

Ruby: class Admin < User; end
来源：http://bif.bbcook.cn

C#:   class Admin : User {}
来源：http://mmy.jinyuanbaomall.cn

[G06] 重写方法
来源：http://sar.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://bil.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://tnl.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://lgk.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://oog.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://hnk.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://myu.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://bqr.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://ahq.meibo888.top

[G07] 调用父类方法
来源：http://yrd.yangfankeji.com

Py:   super().greet()
来源：http://mmg.yj202588.top

PHP:  parent::greet();
来源：http://oks.chenjidiqi.icu

JS:   super.greet();
来源：http://upc.sysykeji.top

TS:   super.greet();
来源：http://eea.wangshuangyany.cn

Java: super.greet();
来源：http://byx.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bwa.hnqzz.top

Ruby: super
来源：http://nod.chenlongwang.top

C#:   base.Greet();
来源：http://dmp.gzhubu.top

[G08] 静态方法与属性
来源：http://oeb.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gix.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://vew.ydjk.org.cn

JS:   static f() {}
来源：http://jqk.wangdashe.top

TS:   static f(): void {}
来源：http://jxd.ppjwa.cn

Java: static void f() {}
来源：http://zxq.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mbp.mhx1999.top

Ruby: def self.f; end
来源：http://xra.gaohongyu789.top

C#:   public static void F() {}
来源：http://pqi.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://clh.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://smr.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xga.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jfh.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://cvf.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://fms.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://khf.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://piz.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://ojx.xuetiantiany.cn

[G10] 访问控制
来源：http://ywb.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://tbr.jinqigfzy.top

PHP:  public / protected / private
来源：http://zyy.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://hbe.sweek.top

TS:   public / protected / private
来源：http://bhp.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://kdi.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zyf.316326.xyz

Ruby: public / protected / private
来源：http://gpu.sweek.top

C#:   public / protected / private / internal
来源：http://moz.fktsv.cn

[G11] getter / setter
来源：http://uir.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://yge.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jnc.uphjek.com

JS:   get name() { return this._name; }
来源：http://tuf.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://wcn.zdbjq.cn

Java: public String getName() { return name; }
来源：http://bje.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ddi.tarul.cn

Ruby: attr_accessor :name
来源：http://paj.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://vmn.yanxiufei.cn

[G12] 对象转字符串
来源：http://evu.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://gwn.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kbg.ybcxt.top

JS:   toString() { return this.name; }
来源：http://ueb.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://ldj.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://qff.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://man.tian-w.cn

Ruby: def to_s; @name; end
来源：http://pkg.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://ehl.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://tuu.chenzaomai.com

Py:   isinstance(u, User)
来源：http://ari.cashguo.top

PHP:  $u instanceof User
来源：http://gix.52xcode.cn

JS:   u instanceof User
来源：http://jim.sysykeji.top

TS:   u instanceof User
来源：http://ozs.xziqi.cn

Java: u instanceof User
来源：http://har.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vmz.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://zsb.yfazqb.com

C#:   u is User
来源：http://sez.hnxiangtu.top

[G14] 数据类 / record
来源：http://huy.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tbo.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://haq.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://pgd.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://jlu.ivvv.top

Java: record User(String name, int age) {}
来源：http://jvu.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://nlh.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zrp.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://gzd.316326.xyz

[G15] 枚举
来源：http://mkf.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://scg.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wlp.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hkj.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rtt.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://hak.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zez.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://ynb.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dsw.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://hvv.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pat.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://vmb.bjfxy.top

JS:   Object.entries(obj)
来源：http://owc.zhengqikj.top

TS:   Object.entries(obj)
来源：http://dgp.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wrp.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://exn.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://bsy.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://kdj.chenjidiqi.icu

================================================================================
来源：http://yvx.aizwys.cn

H. 异常与错误处理
来源：http://czb.guowangkeji.top

================================================================================
来源：http://kwp.fzhhl.top

[H01] try / catch 基础
来源：http://gkz.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gyv.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mst.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lht.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wgy.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rlj.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nhf.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fif.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://opi.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://duy.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://wbx.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uao.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wpj.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iee.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vxf.mhx1999.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hdc.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dgg.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://pyf.quarkkingdee.top

[H03] 主动抛出异常
来源：http://nql.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://tao.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ewt.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://kie.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://cxf.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aip.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tdj.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://mem.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://rjp.yj20258.top

[H04] 自定义异常类型
来源：http://yza.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://yjq.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://ubp.daxiang520.top

JS:   class MyError extends Error {}
来源：http://sba.epnwcf.com

TS:   class MyError extends Error {}
来源：http://gbr.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://ekf.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zix.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://kmr.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://wmz.sxryk.cn

[H05] 捕获特定类型
来源：http://skq.vehdjk.com

Py:   except ValueError as e:
来源：http://vri.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hao.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://wqk.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://gbz.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://slw.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kiy.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://scy.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tsp.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://xkv.uphjek.com

Py:   value = d.get("k") or default
来源：http://nav.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://twr.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hwl.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://dsz.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nrp.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uko.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://xce.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://eat.zhongyouzk.top

[H07] 断言
来源：http://uhv.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://iit.cucudq.cn

PHP:  assert($x > 0);
来源：http://zjm.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://odw.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://vxy.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://kif.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ktc.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://wll.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://ihb.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://fal.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://voe.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ceo.yonumen.top

JS:   e.message;  e.stack
来源：http://ath.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pec.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lfn.zdbjq.cn

Go:   err.Error()
来源：http://bsp.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://omd.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://zrc.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://xsf.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://axt.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dsf.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pks.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mej.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xdh.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nie.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bru.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eby.pycfn.com

[H10] 资源自动释放
来源：http://ymu.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lxr.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://drd.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ghs.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ibw.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yuc.pycfn.com

Go:   defer f.Close()
来源：http://fiv.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ssq.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hmp.jiagoushi.top

================================================================================
来源：http://odm.sysykeji.top

I. 正则表达式
来源：http://qls.meibo888.top

================================================================================
来源：http://kfu.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://nzf.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ebm.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xvk.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://yus.guannengcc.top

TS:   /\d+/.test(s)
来源：http://sow.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lft.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iox.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://gfp.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rkx.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://jth.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://srp.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zet.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pop.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://wxs.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tfn.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wwh.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://oor.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://efn.0kj1m.cn

[I03] 提取捕获分组
来源：http://dos.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gjr.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ywl.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://prf.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nbc.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ufj.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://emo.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ofo.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pht.havefunace.top

[I04] 正则替换
来源：http://uvm.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jsc.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cbh.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://pns.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://qja.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vho.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gnx.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uxl.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://icp.birdmap.top

[I05] 按正则拆分
来源：http://xcg.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mkh.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uci.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://kix.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://dyk.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://ppj.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aye.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jnr.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hqy.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rpu.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zzx.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oce.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pny.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fpi.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://adn.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yge.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jrc.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fil.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://nbd.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fir.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wyy.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gaz.jiagoushi.top

TS:   /error/gim
来源：http://iwf.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://foz.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://opu.havefunace.top

Ruby: s.scan(/error/i)
来源：http://jds.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hub.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://dyi.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xwg.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oom.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kjl.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://khz.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vhh.sufxvd.cn


<!-- 参考信息 -->