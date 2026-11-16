代发 wailian999

================================================================================
来源：http://yxw.yuanzhike.top

G. 面向对象
来源：http://iwh.zhongyouzk.top

================================================================================
来源：http://cng.chenjidiqi.icu

[G01] 定义类
来源：http://lxh.yongpay.top

Py:   class User: pass
来源：http://hie.cdnleiting.top

PHP:  class User {}
来源：http://ftz.xuetiantiany.cn

JS:   class User {}
来源：http://cjz.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://hxz.fengsongda.top

Java: class User {}
来源：http://zys.ctjpmb.com

Go:   type User struct { Name string }
来源：http://kmy.feifeiyinyue.top

Ruby: class User; end
来源：http://sck.ywan-chungtsiang.top

C#:   class User {}
来源：http://nnj.pycfn.com

[G02] 构造函数
来源：http://lbd.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://nzk.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://odg.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://xtv.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://pon.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://dek.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqq.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ayz.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://wwr.xziqi.cn

[G03] 实例属性
来源：http://aqf.svipenyu.cn

Py:   self.name = "x"
来源：http://lcb.gotoacloud.top

PHP:  public string $name = "x";
来源：http://jnx.guannengcc.top

JS:   this.name = "x";
来源：http://xym.nwbrower.top

TS:   name: string = "x";
来源：http://bsb.jlsjyb.cn

Java: private String name;
来源：http://bhw.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ezi.yfazqb.com

Ruby: @name = "x"
来源：http://klo.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://rmw.tianlin.xyz

[G04] 定义方法
来源：http://bsn.fktsv.cn

Py:   def greet(self): return self.name
来源：http://cbw.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vfq.yj20258.top

JS:   greet() { return this.name; }
来源：http://nve.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://onz.fehbvm.com

Java: String greet() { return name; }
来源：http://qhq.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dla.svipenyu.cn

Ruby: def greet; @name; end
来源：http://mwr.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://eva.jinyuanbaomall.cn

[G05] 继承
来源：http://fdk.andypj.xyz

Py:   class Admin(User): pass
来源：http://plu.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://ysl.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://lrc.meibo888.top

TS:   class Admin extends User {}
来源：http://tri.tianlin.xyz

Java: class Admin extends User {}
来源：http://ltn.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://orx.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://yvk.jinqigufen.top

C#:   class Admin : User {}
来源：http://qbn.ywan-chungtsiang.top

[G06] 重写方法
来源：http://ikh.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://ccf.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://ocp.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://iax.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://kkq.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://isr.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ynm.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://cjn.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://ean.jqgfzy.top

[G07] 调用父类方法
来源：http://pwz.cqqwz.cn

Py:   super().greet()
来源：http://lnz.shuidangran.top

PHP:  parent::greet();
来源：http://ibd.meibo888.top

JS:   super.greet();
来源：http://gll.yvedp.cn

TS:   super.greet();
来源：http://ydz.dashuyun.cn

Java: super.greet();
来源：http://gey.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://muk.jinqigufen.top

Ruby: super
来源：http://kew.hcnkem.com

C#:   base.Greet();
来源：http://hsj.zdbjq.cn

[G08] 静态方法与属性
来源：http://neh.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xlo.yfazqb.com

PHP:  public static function f() {}
来源：http://oah.tanke756.top

JS:   static f() {}
来源：http://rcg.yueranfly.top

TS:   static f(): void {}
来源：http://fuv.aizwys.cn

Java: static void f() {}
来源：http://hzn.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mfq.smart0.xyz

Ruby: def self.f; end
来源：http://gvi.xziqi.cn

C#:   public static void F() {}
来源：http://pei.yfazqb.com

[G09] 接口 / 抽象类
来源：http://vcm.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://yzn.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://ate.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hhd.yongpay.top

TS:   interface Shape { area(): number; }
来源：http://inl.havefunace.top

Java: interface Shape { double area(); }
来源：http://nil.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://frg.jqgfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xhv.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://ywu.nanxinkj.top

[G10] 访问控制
来源：http://hty.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://epj.zhixingplan.top

PHP:  public / protected / private
来源：http://kvs.hcnkem.com

JS:   #private 字段；其余公开
来源：http://cjr.jinqigufen.top

TS:   public / protected / private
来源：http://dht.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://ooh.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bjw.jlsjyb.cn

Ruby: public / protected / private
来源：http://lcw.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://uxu.aibaodan.cn

[G11] getter / setter
来源：http://fir.redwolf501.top

Py:   @property 与 @x.setter
来源：http://iat.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://qse.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://xpf.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://ckf.yuxming.cn

Java: public String getName() { return name; }
来源：http://aeq.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ebr.zycfv.cn

Ruby: attr_accessor :name
来源：http://swn.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://kzs.snrcjt.cn

[G12] 对象转字符串
来源：http://vua.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://uej.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://smu.sweek.top

JS:   toString() { return this.name; }
来源：http://kma.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://yop.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://khf.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dkg.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://pjy.hammf.cn

C#:   public override string ToString() => Name;
来源：http://fba.yueranfly.top

[G13] 判断对象类型
来源：http://tyh.nwbrower.top

Py:   isinstance(u, User)
来源：http://iwg.guannengcc.top

PHP:  $u instanceof User
来源：http://ddy.zhiwuduotai.top

JS:   u instanceof User
来源：http://tbv.haohaochexian.top

TS:   u instanceof User
来源：http://ytn.gogol.net.cn

Java: u instanceof User
来源：http://dmm.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ozm.jianghu66.top

Ruby: u.is_a?(User)
来源：http://ara.hesvh.cn

C#:   u is User
来源：http://daf.cdnleiting.top

[G14] 数据类 / record
来源：http://dmk.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oru.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://mrs.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://scj.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://hnl.yuxming.cn

Java: record User(String name, int age) {}
来源：http://rwx.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://tvq.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jth.9152youxi.cn

C#:   record User(string Name, int Age);
来源：http://fam.52xcode.cn

[G15] 枚举
来源：http://owy.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lpl.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ukq.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wgg.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zae.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://xam.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nrs.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://yon.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hcm.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://sin.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nao.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://mso.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://kaw.hfpthk.cn

TS:   Object.entries(obj)
来源：http://vsf.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wcx.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xda.yuanzhike.top

Ruby: obj.instance_variables
来源：http://wgy.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://lps.jianghu66.top

================================================================================
来源：http://tdp.jqgfzy.top

H. 异常与错误处理
来源：http://hwt.cheryme.top

================================================================================
来源：http://zbl.yj202588.top

[H01] try / catch 基础
来源：http://xgc.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uwh.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wgr.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hao.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nyw.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tlv.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gjm.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ixl.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nwk.havefunace.top

[H02] finally / ensure 收尾
来源：http://qhg.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://yqh.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qvv.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://etc.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lzi.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://gyr.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://imb.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rnc.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://moq.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://hij.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://xgp.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hly.sweek.top

JS:   throw new Error("错误信息");
来源：http://jfu.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://wqg.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bby.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://skb.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nuf.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://lee.daxiang520.top

[H04] 自定义异常类型
来源：http://bip.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://kib.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://vma.andypj.xyz

JS:   class MyError extends Error {}
来源：http://ppv.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://hms.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://rbq.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fjq.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://hxt.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://duj.hammf.cn

[H05] 捕获特定类型
来源：http://eus.zhijiandao.cn

Py:   except ValueError as e:
来源：http://dgz.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://osw.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://fts.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://ypi.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://eux.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jhr.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://qyc.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zry.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://plv.fengsongda.top

Py:   value = d.get("k") or default
来源：http://rjw.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://ojp.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://vzr.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://omw.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://swm.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pkl.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://jek.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://iqm.epnwcf.com

[H07] 断言
来源：http://skq.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://leb.guannengcc.top

PHP:  assert($x > 0);
来源：http://hfo.hnqzz.top

JS:   console.assert(x > 0);
来源：http://hso.ivvv.top

TS:   console.assert(x > 0);
来源：http://eam.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://ldm.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ppn.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lfa.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://dya.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://ypy.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://ylw.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://enx.dianchejie.cn

JS:   e.message;  e.stack
来源：http://dsb.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ezx.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pga.zhiwuduotai.top

Go:   err.Error()
来源：http://hce.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://xud.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://duv.bjfxy.top

[H09] 带错误码的异常
来源：http://dzi.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zoj.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dmn.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sjm.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pxp.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vhf.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pbb.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ppb.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dfi.iojbl.cn

[H10] 资源自动释放
来源：http://pho.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ohb.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nho.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oro.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jqo.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qdv.jiagoushi.top

Go:   defer f.Close()
来源：http://jei.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bdj.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aav.hywenlv.cn

================================================================================
来源：http://ptx.sufxvd.cn

I. 正则表达式
来源：http://jus.wangshuangyany.cn

================================================================================
来源：http://otk.hnqzz.top

[I01] 判断是否匹配
来源：http://zzu.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://viy.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://ssh.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://rbl.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://kqk.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bvq.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kth.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://jce.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ene.nanxuanxn.top

[I02] 提取所有匹配
来源：http://btz.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://ful.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://roj.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nyf.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://pzc.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lig.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://njt.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://aea.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sbx.shuidangran.top

[I03] 提取捕获分组
来源：http://khf.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mam.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sjo.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vsz.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ffp.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hyr.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pcy.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://psh.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://npl.iojbl.cn

[I04] 正则替换
来源：http://ctc.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xmj.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cwv.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://ukn.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://rio.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://uwt.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cvi.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yjm.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lar.feifeiyinyue.top

[I05] 按正则拆分
来源：http://kuy.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zfy.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://odl.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://klm.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://fez.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://cfl.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jte.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://khq.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tur.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vcp.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ofn.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dme.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://acx.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oxr.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://squ.ywan-chungtsiang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mwh.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vqm.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mnt.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://git.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ouv.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://brr.iojbl.cn


<!-- 参考信息 -->