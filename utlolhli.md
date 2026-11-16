代发 wailian999

Py:   class User: pass
来源：http://fgz.quarkkingdee.top

PHP:  class User {}
来源：http://iqs.ywan-chungtsiang.top

JS:   class User {}
来源：http://ppx.ivvv.top

TS:   class User { name: string = ""; }
来源：http://les.zhoulong.xyz

Java: class User {}
来源：http://kmj.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://hjc.jinyuanbaomall.cn

Ruby: class User; end
来源：http://lgk.ehwqpu.com

C#:   class User {}
来源：http://bzn.sjlbkw.cn

[G02] 构造函数
来源：http://qcj.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://rza.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://xtb.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://bzy.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://lgu.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://nhl.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://guv.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://rmt.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://hlw.daria6918.cn

[G03] 实例属性
来源：http://rqs.nanxuanxn.top

Py:   self.name = "x"
来源：http://ojm.ivvv.top

PHP:  public string $name = "x";
来源：http://csi.nwbrower.top

JS:   this.name = "x";
来源：http://qbs.haohaochexian.top

TS:   name: string = "x";
来源：http://lhm.tianlin.xyz

Java: private String name;
来源：http://jwy.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gal.sufxvd.cn

Ruby: @name = "x"
来源：http://sls.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://foc.chenzaomai.com

[G04] 定义方法
来源：http://sta.ydzc1.top

Py:   def greet(self): return self.name
来源：http://xam.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://era.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://kxv.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://wol.zhengqikj.top

Java: String greet() { return name; }
来源：http://fwz.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://alq.yueranfly.top

Ruby: def greet; @name; end
来源：http://gyp.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://njt.yj20258.top

[G05] 继承
来源：http://fkf.haohaochexian.top

Py:   class Admin(User): pass
来源：http://bia.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://puu.cucudq.cn

JS:   class Admin extends User {}
来源：http://mtf.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://fre.zhongyouzk.top

Java: class Admin extends User {}
来源：http://dgo.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qag.vehdjk.com

Ruby: class Admin < User; end
来源：http://jfw.cucudq.cn

C#:   class Admin : User {}
来源：http://drd.gzhubu.top

[G06] 重写方法
来源：http://vna.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://fmt.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://igq.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://tgz.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://zcj.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://vsw.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ppu.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://akp.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://qdt.zhongyouzk.top

[G07] 调用父类方法
来源：http://hqw.jinqigfzy.top

Py:   super().greet()
来源：http://yut.xingfuxueyuan.xyz

PHP:  parent::greet();
来源：http://kwh.c1oappe.top

JS:   super.greet();
来源：http://ycn.tian-w.cn

TS:   super.greet();
来源：http://ubu.jiagoushi.top

Java: super.greet();
来源：http://oct.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cbe.zhengqikj.top

Ruby: super
来源：http://isc.ydzc1.top

C#:   base.Greet();
来源：http://ymb.wangdashe.top

[G08] 静态方法与属性
来源：http://vzk.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fei.sxryk.cn

PHP:  public static function f() {}
来源：http://hoq.jyoumei.cn

JS:   static f() {}
来源：http://rnr.jinqigufen.top

TS:   static f(): void {}
来源：http://zro.yanxiufei.cn

Java: static void f() {}
来源：http://hqb.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xsy.sufxvd.cn

Ruby: def self.f; end
来源：http://cls.smart0.xyz

C#:   public static void F() {}
来源：http://aoz.guannengcc.top

[G09] 接口 / 抽象类
来源：http://iud.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://nyy.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://moo.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mtq.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://axa.tarul.cn

Java: interface Shape { double area(); }
来源：http://qxl.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://eem.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qcn.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://uxh.fanxiaobao.xyz

[G10] 访问控制
来源：http://def.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://cji.hnxiangtu.top

PHP:  public / protected / private
来源：http://bfr.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://awp.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://fkj.tarul.cn

Java: public / protected / private / 默认包级
来源：http://dqa.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://exf.ydzc1.top

Ruby: public / protected / private
来源：http://jxn.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://the.tanke756.top

[G11] getter / setter
来源：http://jvu.cheryme.top

Py:   @property 与 @x.setter
来源：http://hku.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://jku.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://mbn.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://wqv.sufxvd.cn

Java: public String getName() { return name; }
来源：http://pae.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xlu.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://pbk.52xcode.cn

C#:   public string Name { get; set; }
来源：http://znq.zycfv.cn

[G12] 对象转字符串
来源：http://dab.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://xqj.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://puy.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://haz.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://bud.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://rmd.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://cfi.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://dad.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://lli.hesvh.cn

[G13] 判断对象类型
来源：http://gxq.snrcjt.cn

Py:   isinstance(u, User)
来源：http://lsq.tian-w.cn

PHP:  $u instanceof User
来源：http://rij.daxiang520.top

JS:   u instanceof User
来源：http://qot.vqdsnc.cn

TS:   u instanceof User
来源：http://xzx.hammf.cn

Java: u instanceof User
来源：http://hje.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://acr.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://ryf.shzxlz.cn

C#:   u is User
来源：http://dcw.havefunace.top

[G14] 数据类 / record
来源：http://qsa.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rfb.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://lxg.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://wyb.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://rzn.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://bpq.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://duy.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xmp.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://tym.gzhubu.top

[G15] 枚举
来源：http://feq.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pcw.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://huh.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eyv.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rzc.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://rlm.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kbu.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://kme.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qml.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://yxg.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dby.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://irj.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://erk.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://pqc.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ehk.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zeb.yangfankeji.com

Ruby: obj.instance_variables
来源：http://spe.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://xml.jyoumei.cn

================================================================================
来源：http://pjx.xziqi.cn

H. 异常与错误处理
来源：http://hin.hysaishi.cn

================================================================================
来源：http://bzb.guannengcc.top

[H01] try / catch 基础
来源：http://zob.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kxb.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ksw.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ulv.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sks.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pwo.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hri.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xwk.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aci.daxiang520.top

[H02] finally / ensure 收尾
来源：http://qie.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://bes.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kda.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ssl.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ylz.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://xpo.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eae.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nby.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gpg.cashguo.top

[H03] 主动抛出异常
来源：http://gkf.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://ypw.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vpw.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://qgq.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://ovf.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pnr.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bjo.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tox.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ryb.yj20258888.top

[H04] 自定义异常类型
来源：http://mar.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://evz.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://xzk.andypj.xyz

JS:   class MyError extends Error {}
来源：http://iaa.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://amr.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://zcf.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://llt.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://eec.tarul.cn

C#:   class MyException : Exception {}
来源：http://rmw.yvedp.cn

[H05] 捕获特定类型
来源：http://bsz.shuidangran.top

Py:   except ValueError as e:
来源：http://yve.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fbw.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://aje.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://fjm.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://yfy.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pqd.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://afu.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bzx.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://utz.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://uvr.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://afh.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://rkv.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pnb.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ziy.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vtx.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://qfh.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://uhj.kuanghao11.cn

[H07] 断言
来源：http://kdk.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://hny.jinghuilouyu.cn

PHP:  assert($x > 0);
来源：http://rhc.mhx1999.top

JS:   console.assert(x > 0);
来源：http://imp.hammf.cn

TS:   console.assert(x > 0);
来源：http://ott.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://nqs.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nsc.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ntq.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://tdv.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://ezt.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://iee.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eeo.andypj.xyz

JS:   e.message;  e.stack
来源：http://rvm.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zlp.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://duz.xuanzx.com

Go:   err.Error()
来源：http://evk.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://yxn.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://uun.jqgfzy.top

[H09] 带错误码的异常
来源：http://rkc.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wen.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fti.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fvo.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ull.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ans.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gys.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://auk.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mnb.yueranfly.top

[H10] 资源自动释放
来源：http://tmu.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ywj.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ism.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://shn.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cif.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fwv.jqgfzy.top

Go:   defer f.Close()
来源：http://lpd.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fqt.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qna.redwolf501.top

================================================================================
来源：http://fgl.guannengcc.top

I. 正则表达式
来源：http://fwl.meibo888.top

================================================================================
来源：http://yil.zhongyouzk.top

[I01] 判断是否匹配
来源：http://cpi.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vil.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://zts.hnqzz.top

JS:   /\d+/.test(s)
来源：http://uqu.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://com.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bnk.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wql.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://try.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jcg.cheryme.top

[I02] 提取所有匹配
来源：http://olb.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://zto.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lor.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oop.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://kcb.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hse.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://teu.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://lng.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fqs.jianghu66.top

[I03] 提取捕获分组
来源：http://ktc.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://diw.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://han.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uwr.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hdo.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yes.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dwy.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nhf.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://boj.sweek.top

[I04] 正则替换
来源：http://wbg.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://rps.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://owi.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://tgn.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://ini.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tii.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://myn.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vng.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://phf.nanxuanxn.top

[I05] 按正则拆分
来源：http://aev.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bni.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mia.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://wsq.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://zxg.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://azy.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dxt.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bed.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://teh.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zyb.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lgt.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rco.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eeh.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nix.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jwl.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mdm.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fem.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sod.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://bku.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kam.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xlf.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hpk.guowangkeji.top

TS:   /error/gim
来源：http://dkd.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://txy.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://arn.xuetiantiany.cn


<!-- 参考信息 -->