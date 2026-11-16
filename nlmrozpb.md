代发 wailian999

Java: class User {}
来源：http://iaq.ivvv.top

Go:   type User struct { Name string }
来源：http://rde.0kj1m.cn

Ruby: class User; end
来源：http://owi.jinyuanbaomall.cn

C#:   class User {}
来源：http://nqn.yj20258888.top

[G02] 构造函数
来源：http://yie.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://tly.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://quv.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://rat.meibo888.top

TS:   constructor(public name: string) {}
来源：http://tep.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://xuz.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://djk.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://qiv.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://wxz.feifeiyinyue.top

[G03] 实例属性
来源：http://ixd.jinqigufen.top

Py:   self.name = "x"
来源：http://ysf.xinyue.icu

PHP:  public string $name = "x";
来源：http://agb.gogol.net.cn

JS:   this.name = "x";
来源：http://pvo.iojbl.cn

TS:   name: string = "x";
来源：http://web.cqqwz.cn

Java: private String name;
来源：http://tqn.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hjf.yfazqb.com

Ruby: @name = "x"
来源：http://gyo.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://ajk.yj20258.top

[G04] 定义方法
来源：http://htx.bjfxy.top

Py:   def greet(self): return self.name
来源：http://qsb.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jar.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://sqx.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://ewe.sufxvd.cn

Java: String greet() { return name; }
来源：http://lzd.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ycd.aibaodan.cn

Ruby: def greet; @name; end
来源：http://afo.tanke756.top

C#:   public string Greet() => Name;
来源：http://llx.dashuyun.cn

[G05] 继承
来源：http://nal.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://yyj.pycfn.com

PHP:  class Admin extends User {}
来源：http://wxu.0kj1m.cn

JS:   class Admin extends User {}
来源：http://mst.jiagoushi.top

TS:   class Admin extends User {}
来源：http://rvb.zhongyouzk.top

Java: class Admin extends User {}
来源：http://zgg.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://afr.jyoumei.cn

Ruby: class Admin < User; end
来源：http://byw.jianghu66.top

C#:   class Admin : User {}
来源：http://vcr.sxryk.cn

[G06] 重写方法
来源：http://zcy.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://pxz.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://pho.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://cpg.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://pmj.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://qti.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ald.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://jna.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://hsq.havefunace.top

[G07] 调用父类方法
来源：http://gcm.vehdjk.com

Py:   super().greet()
来源：http://upj.cashguo.top

PHP:  parent::greet();
来源：http://ywm.yuanzhike.top

JS:   super.greet();
来源：http://uet.cheryme.top

TS:   super.greet();
来源：http://ngo.yvedp.cn

Java: super.greet();
来源：http://bbl.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ndu.hongshengwenyu.top

Ruby: super
来源：http://hsj.sxryk.cn

C#:   base.Greet();
来源：http://dua.0kj1m.cn

[G08] 静态方法与属性
来源：http://rgr.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xyv.xziqi.cn

PHP:  public static function f() {}
来源：http://qvn.iojbl.cn

JS:   static f() {}
来源：http://xuj.fzhhl.top

TS:   static f(): void {}
来源：http://szt.52xcode.cn

Java: static void f() {}
来源：http://lvx.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fxh.chenlongwang.top

Ruby: def self.f; end
来源：http://bkh.yonumen.top

C#:   public static void F() {}
来源：http://vab.hammf.cn

[G09] 接口 / 抽象类
来源：http://agm.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://ztx.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://hwo.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://xpq.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://wsj.shuidangran.top

Java: interface Shape { double area(); }
来源：http://lrq.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://ymj.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://icf.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://hwe.feifeiyinyue.top

[G10] 访问控制
来源：http://pgz.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://qkm.jqgufenzy.top

PHP:  public / protected / private
来源：http://bqu.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://pws.fengsongda.top

TS:   public / protected / private
来源：http://nsa.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://xsn.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lfb.fktsv.cn

Ruby: public / protected / private
来源：http://qvr.cdnleiting.top

C#:   public / protected / private / internal
来源：http://gho.pengpengdd.cyou

[G11] getter / setter
来源：http://uze.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://aao.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ugm.shuidangran.top

JS:   get name() { return this._name; }
来源：http://wst.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://elx.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://odn.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ocb.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://qao.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://stv.jinqigfzy.top

[G12] 对象转字符串
来源：http://edj.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://lpv.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tut.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://mug.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://ihe.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://bqb.epnwcf.com

Go:   func (u User) String() string { return u.Name }
来源：http://lpe.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://bqi.birdmap.top

C#:   public override string ToString() => Name;
来源：http://cuw.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://ypq.fehbvm.com

Py:   isinstance(u, User)
来源：http://nsv.svipenyu.cn

PHP:  $u instanceof User
来源：http://jxl.feifeiyinyue.top

JS:   u instanceof User
来源：http://ldu.ehwqpu.com

TS:   u instanceof User
来源：http://onk.jiagoushi.top

Java: u instanceof User
来源：http://zdg.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hmm.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://ymc.hywenlv.cn

C#:   u is User
来源：http://fuq.chenzaomai.com

[G14] 数据类 / record
来源：http://edi.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://akn.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://kcn.fanxiaobao.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://juk.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://lwk.xuanzx.com

Java: record User(String name, int age) {}
来源：http://gmd.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://esk.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gzl.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://svt.shanyushiyangtech.top

[G15] 枚举
来源：http://mlx.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rqw.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dpf.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqr.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dzd.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://whs.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wmz.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://ics.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wbf.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://pos.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wsm.birdmap.top

PHP:  get_object_vars($obj);
来源：http://mrb.ivvv.top

JS:   Object.entries(obj)
来源：http://lut.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://lsc.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tbj.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dxb.yuxming.cn

Ruby: obj.instance_variables
来源：http://qew.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://dzr.snrcjt.cn

================================================================================
来源：http://jbs.52xcode.cn

H. 异常与错误处理
来源：http://uyx.shangyingyoupin.top

================================================================================
来源：http://ovv.316326.xyz

[H01] try / catch 基础
来源：http://zpv.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wou.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rro.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rgr.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yzv.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eho.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hgv.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yre.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zqt.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://qrc.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://hgl.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://lgi.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://orv.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://kdm.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uvf.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kgx.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ocu.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yzv.shuidangran.top

[H03] 主动抛出异常
来源：http://fav.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://spt.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zqo.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://czf.316326.xyz

TS:   throw new Error("错误信息");
来源：http://huy.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rll.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ccu.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mui.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://otw.svipenyu.cn

[H04] 自定义异常类型
来源：http://cpt.yj202588.top

Py:   class MyError(Exception): pass
来源：http://fsr.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ruw.iojbl.cn

JS:   class MyError extends Error {}
来源：http://god.cheryme.top

TS:   class MyError extends Error {}
来源：http://kvs.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://rtb.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qmj.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://uzo.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://hwz.sweek.top

[H05] 捕获特定类型
来源：http://utt.chenlongwang.top

Py:   except ValueError as e:
来源：http://uca.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wva.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://ldw.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://pls.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://tsi.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ldf.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://yzl.jqgfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gov.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://ekc.meibo888.top

Py:   value = d.get("k") or default
来源：http://fnn.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://knn.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://stt.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pwv.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tzn.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kgt.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://grw.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://qlz.xuanzx.com

[H07] 断言
来源：http://lca.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://fkp.bbcook.cn

PHP:  assert($x > 0);
来源：http://tea.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://lqk.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://nms.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://dsh.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://paz.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://kjf.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://aov.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://sic.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://zng.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mpx.shuidangran.top

JS:   e.message;  e.stack
来源：http://ghl.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://npr.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wia.zhongyouzk.top

Go:   err.Error()
来源：http://liq.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://eae.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://rlv.hywenlv.cn

[H09] 带错误码的异常
来源：http://rwc.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mhp.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dqy.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iwt.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bax.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zbq.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ayt.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://bvc.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://nkv.jinqigufen.top

[H10] 资源自动释放
来源：http://myn.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dai.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dta.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gsu.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lta.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pmo.xziqi.cn

Go:   defer f.Close()
来源：http://pye.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uuy.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://etv.jlsjyb.cn

================================================================================
来源：http://udh.fengsongda.top

I. 正则表达式
来源：http://gxa.sysykeji.top

================================================================================
来源：http://dep.jinqigfzy.top

[I01] 判断是否匹配
来源：http://hja.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wcf.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fhk.yfazqb.com

JS:   /\d+/.test(s)
来源：http://uis.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://krq.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pzv.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dkt.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://gqq.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://elu.daria6918.cn

[I02] 提取所有匹配
来源：http://yng.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://oiv.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tcm.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cgt.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://hlz.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xlu.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xfj.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://dfo.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qfi.yueranfly.top

[I03] 提取捕获分组
来源：http://pgk.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fld.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://koe.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://czk.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lwi.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gvr.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://stb.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://djp.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eef.tianlin.xyz

[I04] 正则替换
来源：http://stg.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://cro.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ceu.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://qgr.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ckq.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://kda.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://qjs.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rbd.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://anm.tarul.cn

[I05] 按正则拆分
来源：http://ppo.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://apu.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yjh.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://xay.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://cto.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://zmh.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kec.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://khn.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://agx.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cey.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zvq.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vzw.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzs.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sav.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qfc.hammf.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://amq.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ajw.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rwm.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://kpl.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sab.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mmu.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tfh.fzhhl.top

TS:   /error/gim
来源：http://jzw.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cww.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tuj.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://ath.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dmr.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://shk.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vki.zycfv.cn


<!-- 参考信息 -->