代发 wailian999

================================================================================
来源：http://kqt.fehbvm.com

G. 面向对象
来源：http://jop.yuxming.cn

================================================================================
来源：http://sds.jinyuanbaomall.cn

[G01] 定义类
来源：http://sio.zhixingplan.top

Py:   class User: pass
来源：http://rwi.yj20258888.top

PHP:  class User {}
来源：http://mjw.snrcjt.cn

JS:   class User {}
来源：http://lss.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://xdx.yueranfly.top

Java: class User {}
来源：http://vzp.tanke756.top

Go:   type User struct { Name string }
来源：http://qla.fehbvm.com

Ruby: class User; end
来源：http://yiu.daria6918.cn

C#:   class User {}
来源：http://lhy.0kj1m.cn

[G02] 构造函数
来源：http://kke.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://tup.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://loy.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://oam.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://xiw.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://xtk.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://glx.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://dng.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://tsu.yuanzhike.top

[G03] 实例属性
来源：http://fhv.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://wvz.9152youxi.cn

PHP:  public string $name = "x";
来源：http://cme.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://wac.zhiwuduotai.top

TS:   name: string = "x";
来源：http://lxu.nwbrower.top

Java: private String name;
来源：http://zvk.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rtj.52xcode.cn

Ruby: @name = "x"
来源：http://yos.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://fyq.snrcjt.cn

[G04] 定义方法
来源：http://efe.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://lqf.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iux.sxryk.cn

JS:   greet() { return this.name; }
来源：http://qnq.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://zsm.andypj.xyz

Java: String greet() { return name; }
来源：http://tgo.kuanghao11.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wcw.yfazqb.com

Ruby: def greet; @name; end
来源：http://pxu.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://php.zhiwuduotai.top

[G05] 继承
来源：http://bex.bjfxy.top

Py:   class Admin(User): pass
来源：http://grq.vehdjk.com

PHP:  class Admin extends User {}
来源：http://zxr.yonumen.top

JS:   class Admin extends User {}
来源：http://ixg.mhx1999.top

TS:   class Admin extends User {}
来源：http://eze.yfazqb.com

Java: class Admin extends User {}
来源：http://ren.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ohi.jianghu66.top

Ruby: class Admin < User; end
来源：http://wdp.zycfv.cn

C#:   class Admin : User {}
来源：http://fkn.hcnkem.com

[G06] 重写方法
来源：http://kas.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://nlp.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://qqq.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://iki.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://cny.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://twn.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://alk.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://ptd.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://skf.shangyingyoupin.top

[G07] 调用父类方法
来源：http://gzm.snrcjt.cn

Py:   super().greet()
来源：http://wvm.nanxinkj.top

PHP:  parent::greet();
来源：http://sqv.gzhubu.top

JS:   super.greet();
来源：http://wuk.cucudq.cn

TS:   super.greet();
来源：http://ftd.ybcxt.top

Java: super.greet();
来源：http://eja.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xhk.hcnkem.com

Ruby: super
来源：http://kpp.yj202588.top

C#:   base.Greet();
来源：http://gic.jqgufenzy.top

[G08] 静态方法与属性
来源：http://hut.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wwo.zhixingplan.top

PHP:  public static function f() {}
来源：http://ffq.cheryme.top

JS:   static f() {}
来源：http://fiy.yangfankeji.com

TS:   static f(): void {}
来源：http://jsh.fanxiaobao.xyz

Java: static void f() {}
来源：http://cnb.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ahs.aizwys.cn

Ruby: def self.f; end
来源：http://djp.bbcook.cn

C#:   public static void F() {}
来源：http://npd.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://bib.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://pqh.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://juv.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ikh.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://hdj.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://plx.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://plf.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cdz.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://wof.ydjk.org.cn

[G10] 访问控制
来源：http://qpn.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://mel.yj202588.top

PHP:  public / protected / private
来源：http://iqp.tian-w.cn

JS:   #private 字段；其余公开
来源：http://jhg.pengpengdd.cyou

TS:   public / protected / private
来源：http://ruk.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://kxv.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://aei.nanxuanxn.top

Ruby: public / protected / private
来源：http://iuc.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://loc.zhongyouzk.top

[G11] getter / setter
来源：http://ihj.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://juj.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ctm.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://ius.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://rvv.zycfv.cn

Java: public String getName() { return name; }
来源：http://piy.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://omn.yvedp.cn

Ruby: attr_accessor :name
来源：http://zdx.cheryme.top

C#:   public string Name { get; set; }
来源：http://xfl.zhengqikj.top

[G12] 对象转字符串
来源：http://gss.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://jda.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qmm.316326.xyz

JS:   toString() { return this.name; }
来源：http://zga.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://jtx.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://soj.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://yzm.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://iua.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://kjz.uphjek.com

[G13] 判断对象类型
来源：http://dpc.haohaochexian.top

Py:   isinstance(u, User)
来源：http://lgw.yongpay.top

PHP:  $u instanceof User
来源：http://gdb.zhijiandao.cn

JS:   u instanceof User
来源：http://dza.52xcode.cn

TS:   u instanceof User
来源：http://quq.gaohongyu789.top

Java: u instanceof User
来源：http://rqh.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vci.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://hfq.sweek.top

C#:   u is User
来源：http://juw.feifeiyinyue.top

[G14] 数据类 / record
来源：http://tdr.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zxm.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://vwv.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://svn.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://wfa.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://jdy.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://dun.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ohx.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://jjn.fzhhl.top

[G15] 枚举
来源：http://urg.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lub.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://suj.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gol.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://del.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://csg.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ehb.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://tgl.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uji.316326.xyz

[G16] 对象转数组 / 字典
来源：http://yqz.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bcj.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://lxs.hesvh.cn

JS:   Object.entries(obj)
来源：http://val.316326.xyz

TS:   Object.entries(obj)
来源：http://qlr.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pjs.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ncs.jinqigufen.top

Ruby: obj.instance_variables
来源：http://xwg.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://inb.ehwqpu.com

================================================================================
来源：http://bjj.jianghu66.top

H. 异常与错误处理
来源：http://ioj.yj20258888.top

================================================================================
来源：http://pha.pycfn.com

[H01] try / catch 基础
来源：http://dkd.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mjs.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kby.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jer.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wmb.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fci.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uot.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tpp.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xyl.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://zei.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://kpw.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qkx.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uvq.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oqk.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://koo.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://glg.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vqv.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://utn.bjfxy.top

[H03] 主动抛出异常
来源：http://cuz.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://iys.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://guj.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://jct.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://gtg.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://izh.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ltm.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tyk.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://bhl.nwbrower.top

[H04] 自定义异常类型
来源：http://ahf.cashguo.top

Py:   class MyError(Exception): pass
来源：http://jwo.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://msr.guannengcc.top

JS:   class MyError extends Error {}
来源：http://jov.yj20258888.top

TS:   class MyError extends Error {}
来源：http://kmd.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://pye.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mfj.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://bkn.yvedp.cn

C#:   class MyException : Exception {}
来源：http://maf.jqgfzy.top

[H05] 捕获特定类型
来源：http://ttd.epnwcf.com

Py:   except ValueError as e:
来源：http://kzg.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ocz.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://kll.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://ajg.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://wez.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qas.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://nuc.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://khg.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://svx.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://cux.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://seo.zhaomingkeji.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://geh.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://sek.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gcv.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zvp.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://yss.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://bny.chenlongwang.top

[H07] 断言
来源：http://ney.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://dat.nanxinkj.top

PHP:  assert($x > 0);
来源：http://gac.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://xaz.52xcode.cn

TS:   console.assert(x > 0);
来源：http://ypm.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://pcd.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://muw.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://cee.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://xpa.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://iwf.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://ihn.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rlt.hnqzz.top

JS:   e.message;  e.stack
来源：http://xdv.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ecs.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ggs.zycfv.cn

Go:   err.Error()
来源：http://xas.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://hcw.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://qoj.jyoumei.cn

[H09] 带错误码的异常
来源：http://dkv.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tnv.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://izz.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kdb.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bgo.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://elb.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rgp.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yrs.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lfu.yangfankeji.com

[H10] 资源自动释放
来源：http://ckp.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://jby.tarul.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dbz.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bat.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xme.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://efb.dashuyun.cn

Go:   defer f.Close()
来源：http://tei.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bpj.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sog.uphjek.com

================================================================================
来源：http://tfu.hnqzz.top

I. 正则表达式
来源：http://lzs.bbcook.cn

================================================================================
来源：http://wnl.zdbjq.cn

[I01] 判断是否匹配
来源：http://psh.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dzh.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://dew.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://wbw.meibo888.top

TS:   /\d+/.test(s)
来源：http://xud.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qqm.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zto.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://mzi.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hyp.316326.xyz

[I02] 提取所有匹配
来源：http://mrg.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://dnj.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lgp.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aoh.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://rqg.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://esf.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ytg.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://scm.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hsa.iojbl.cn

[I03] 提取捕获分组
来源：http://mwa.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hmt.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vnr.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ovc.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sqw.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bqt.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hsz.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tfc.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nkt.ivvv.top

[I04] 正则替换
来源：http://fhi.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gee.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gan.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rjt.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fss.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xsu.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://nul.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ikk.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ito.pengpengdd.cyou

[I05] 按正则拆分
来源：http://buu.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://zqb.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pow.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://ldz.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://iaa.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://yfy.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hzk.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://ouc.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hel.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ler.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://phr.snrcjt.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zut.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://npf.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xhd.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hiu.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dcx.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://szy.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zqx.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://wli.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gbk.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zxu.jinqigfzy.top


<!-- 参考信息 -->