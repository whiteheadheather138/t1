代发 wailian999

[G02] 构造函数
来源：http://gmm.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://ene.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://rsy.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://nmg.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://cpa.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://ang.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wvt.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://lee.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://odr.zycfv.cn

[G03] 实例属性
来源：http://pzv.pycfn.com

Py:   self.name = "x"
来源：http://iet.cqqwz.cn

PHP:  public string $name = "x";
来源：http://eqw.shuidangran.top

JS:   this.name = "x";
来源：http://xvt.ydjk.org.cn

TS:   name: string = "x";
来源：http://rbr.jinyuanbaomall.cn

Java: private String name;
来源：http://iqk.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gmx.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://pwj.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://rhr.fanxiaobao.xyz

[G04] 定义方法
来源：http://etk.shuidangran.top

Py:   def greet(self): return self.name
来源：http://voh.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nln.ydzc1.top

JS:   greet() { return this.name; }
来源：http://kas.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://gob.yj20258888.top

Java: String greet() { return name; }
来源：http://dwq.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kwd.dianchejie.cn

Ruby: def greet; @name; end
来源：http://qkk.gzhubu.top

C#:   public string Greet() => Name;
来源：http://sgg.hywenlv.cn

[G05] 继承
来源：http://tfu.nanxinkj.top

Py:   class Admin(User): pass
来源：http://gwj.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://aha.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://qid.xuanzx.com

TS:   class Admin extends User {}
来源：http://cvz.sysykeji.top

Java: class Admin extends User {}
来源：http://lvv.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jbd.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://xqm.daria6918.cn

C#:   class Admin : User {}
来源：http://zue.ctjpmb.com

[G06] 重写方法
来源：http://znr.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://ydx.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kid.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://lwr.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://qrl.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://xjc.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kkb.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://pkv.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://sru.cqqwz.cn

[G07] 调用父类方法
来源：http://gnp.cheryme.top

Py:   super().greet()
来源：http://pcl.zhongyouzk.top

PHP:  parent::greet();
来源：http://dmu.wangdashe.top

JS:   super.greet();
来源：http://exp.yfazqb.com

TS:   super.greet();
来源：http://kmn.zycfv.cn

Java: super.greet();
来源：http://ure.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tvq.0kj1m.cn

Ruby: super
来源：http://szs.ehwqpu.com

C#:   base.Greet();
来源：http://tac.jinqigfzy.top

[G08] 静态方法与属性
来源：http://gbe.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://twg.sweek.top

PHP:  public static function f() {}
来源：http://ihy.aizwys.cn

JS:   static f() {}
来源：http://tlk.hcnkem.com

TS:   static f(): void {}
来源：http://qtj.bjfxy.top

Java: static void f() {}
来源：http://pyx.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kpv.cqqwz.cn

Ruby: def self.f; end
来源：http://waw.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://tho.mhx1999.top

[G09] 接口 / 抽象类
来源：http://ihd.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://wbq.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hnt.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ahf.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://tjl.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://cqc.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://lca.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ibd.sweek.top

C#:   interface IShape { double Area(); }
来源：http://yki.jlsjyb.cn

[G10] 访问控制
来源：http://agw.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://msg.52xcode.cn

PHP:  public / protected / private
来源：http://wan.xuanzx.com

JS:   #private 字段；其余公开
来源：http://jdr.sjlbkw.cn

TS:   public / protected / private
来源：http://sxa.hammf.cn

Java: public / protected / private / 默认包级
来源：http://uyj.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://clt.hnqzz.top

Ruby: public / protected / private
来源：http://hsd.xziqi.cn

C#:   public / protected / private / internal
来源：http://gzn.fanxiaobao.xyz

[G11] getter / setter
来源：http://lko.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://cgu.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fdi.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://ctn.nanxinkj.top

TS:   get name(): string { return this._name; }
来源：http://awo.ivvv.top

Java: public String getName() { return name; }
来源：http://eei.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ftb.0kj1m.cn

Ruby: attr_accessor :name
来源：http://igk.hesvh.cn

C#:   public string Name { get; set; }
来源：http://aaq.yuxming.cn

[G12] 对象转字符串
来源：http://yxj.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://jbk.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kmj.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://pga.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://dfj.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://fuf.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yep.xziqi.cn

Ruby: def to_s; @name; end
来源：http://lhr.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://olx.cashguo.top

[G13] 判断对象类型
来源：http://yaq.jyoumei.cn

Py:   isinstance(u, User)
来源：http://qst.zdqjudy.top

PHP:  $u instanceof User
来源：http://dyd.yanxiufei.cn

JS:   u instanceof User
来源：http://hmj.andypj.xyz

TS:   u instanceof User
来源：http://bwy.yongpay.top

Java: u instanceof User
来源：http://aes.havefunace.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ung.xylfe.cn

Ruby: u.is_a?(User)
来源：http://wkb.xingfuxueyuan.xyz

C#:   u is User
来源：http://kqz.sjlbkw.cn

[G14] 数据类 / record
来源：http://oob.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ysj.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://xbg.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://bax.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://fyl.andypj.xyz

Java: record User(String name, int age) {}
来源：http://ojf.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://ixi.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zhc.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://zgy.jinqigfzy.top

[G15] 枚举
来源：http://mze.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cae.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zyj.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bzi.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hvm.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://ben.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mdu.hywenlv.cn

Ruby: Color = %i[red green].freeze
来源：http://mxm.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sil.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://mte.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lbc.birdmap.top

PHP:  get_object_vars($obj);
来源：http://hhn.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://awz.aizwys.cn

TS:   Object.entries(obj)
来源：http://cip.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lsr.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://fcx.sweek.top

Ruby: obj.instance_variables
来源：http://qki.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://yyt.shuidangran.top

================================================================================
来源：http://ncz.nanxinkj.top

H. 异常与错误处理
来源：http://ndc.hywenlv.cn

================================================================================
来源：http://zsu.hfpthk.cn

[H01] try / catch 基础
来源：http://bhf.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tue.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jon.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://piq.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jso.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tns.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ixf.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wrw.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ruc.havefunace.top

[H02] finally / ensure 收尾
来源：http://qqm.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://whj.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jkr.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ujg.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://juh.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://pqa.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fcv.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kcu.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ssw.vehdjk.com

[H03] 主动抛出异常
来源：http://xsw.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://low.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cwu.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://pui.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://swh.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yzy.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dke.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oib.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://kbp.iojbl.cn

[H04] 自定义异常类型
来源：http://yhs.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://wzu.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://nbn.zycfv.cn

JS:   class MyError extends Error {}
来源：http://uqv.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://rfj.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://evt.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://snm.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://zkh.316326.xyz

C#:   class MyException : Exception {}
来源：http://jvp.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://coj.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://olh.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ngn.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://rbw.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://hwe.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://oce.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nwi.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://cnf.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hgc.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://wiw.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://vss.bjfxy.top

PHP:  $v = $d["k"] ?? null;
来源：http://oma.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://tju.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://fho.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yyv.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://erk.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://png.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://nou.zdbjq.cn

[H07] 断言
来源：http://kqg.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://eoi.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://ddu.hammf.cn

JS:   console.assert(x > 0);
来源：http://jji.shuidangran.top

TS:   console.assert(x > 0);
来源：http://ysx.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://iba.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://foz.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://cbd.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://kdf.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://eeh.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://yjj.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ull.yongpay.top

JS:   e.message;  e.stack
来源：http://dql.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oib.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ers.yongpay.top

Go:   err.Error()
来源：http://ciz.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://csr.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://hsb.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://pqr.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://min.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tgk.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vwc.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hmy.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rit.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fcx.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cgl.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jto.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://rzb.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tpy.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pve.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oob.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ymz.fktsv.cn

Go:   defer f.Close()
来源：http://shv.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iif.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kqf.jlsjyb.cn

================================================================================
来源：http://qeb.yongpay.top

I. 正则表达式
来源：http://btq.jqgfzy.top

================================================================================
来源：http://ntu.jinqigufen.top

[I01] 判断是否匹配
来源：http://ovl.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fas.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ggk.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://cvy.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://jnh.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pzv.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gly.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://ffm.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lav.shzxlz.cn

[I02] 提取所有匹配
来源：http://bnb.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://jsg.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bou.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ulp.hongshengwenyu.top

TS:   s.match(/\d+/g)
来源：http://syp.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yui.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zgj.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://fai.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lok.cheryme.top

[I03] 提取捕获分组
来源：http://cry.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hxc.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nfe.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://svz.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rzs.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fhm.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fdr.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tnk.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://krh.sxryk.cn

[I04] 正则替换
来源：http://iix.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aph.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://orq.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://xlm.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xwf.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://qgd.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://oqi.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wiw.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gsj.hnxiangtu.top

[I05] 按正则拆分
来源：http://kdy.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vmm.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fgm.sjlbkw.cn

JS:   s.split(/\s*,\s*/)
来源：http://rtx.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://xxd.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://xnk.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://onq.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yix.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ocz.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ihd.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ptt.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://brc.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uya.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gsa.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kfz.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yhu.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ibh.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mxo.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://yuf.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lzx.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rli.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ben.cucudq.cn

TS:   /error/gim
来源：http://mee.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dex.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dwh.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://leo.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zhz.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://veb.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rvi.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ffh.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgu.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nam.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://drt.andypj.xyz


<!-- 参考信息 -->