代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ush.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pgy.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wxn.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hxq.havefunace.top

================================================================================
来源：http://ktz.birdmap.top

G. 面向对象
来源：http://jdk.shanyushiyangkeji.top

================================================================================
来源：http://zcm.bjfxy.top

[G01] 定义类
来源：http://avt.yj20258888.top

Py:   class User: pass
来源：http://nnq.kuanghao11.cn

PHP:  class User {}
来源：http://czr.ctjpmb.com

JS:   class User {}
来源：http://yqm.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://nne.haohaochexian.top

Java: class User {}
来源：http://cyb.yj20258.top

Go:   type User struct { Name string }
来源：http://xdy.pengpengdd.cyou

Ruby: class User; end
来源：http://gpe.aizwys.cn

C#:   class User {}
来源：http://cpl.ctjpmb.com

[G02] 构造函数
来源：http://atd.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://lqa.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://rvj.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://mmx.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://plo.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://jnm.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gvu.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://kue.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://gev.c1oappe.top

[G03] 实例属性
来源：http://tsk.daria6918.cn

Py:   self.name = "x"
来源：http://mvo.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://exd.vqdsnc.cn

JS:   this.name = "x";
来源：http://cie.tianlin.xyz

TS:   name: string = "x";
来源：http://xzl.xingfuxueyuan.xyz

Java: private String name;
来源：http://wtd.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qym.yanxiufei.cn

Ruby: @name = "x"
来源：http://rfu.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://wln.ivvv.top

[G04] 定义方法
来源：http://nxn.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://ghc.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://myy.fehbvm.com

JS:   greet() { return this.name; }
来源：http://fel.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://cnq.tianlin.xyz

Java: String greet() { return name; }
来源：http://ypn.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gud.ydzc1.top

Ruby: def greet; @name; end
来源：http://wxp.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://qqr.shangyingyoupin.top

[G05] 继承
来源：http://yjg.jiagoushi.top

Py:   class Admin(User): pass
来源：http://zdv.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://vqj.cucudq.cn

JS:   class Admin extends User {}
来源：http://nem.ehwqpu.com

TS:   class Admin extends User {}
来源：http://hxu.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://qwh.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://thw.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://jco.daxiang520.top

C#:   class Admin : User {}
来源：http://ckf.ydzc1.top

[G06] 重写方法
来源：http://cdy.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://kgs.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sqn.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://bql.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://seo.vqdsnc.cn

Java: @Override String greet() { return "admin"; }
来源：http://oku.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qco.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://pcd.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://qhn.yonumen.top

[G07] 调用父类方法
来源：http://amn.snrcjt.cn

Py:   super().greet()
来源：http://tri.cucudq.cn

PHP:  parent::greet();
来源：http://dji.fanxiaobao.xyz

JS:   super.greet();
来源：http://hme.fehbvm.com

TS:   super.greet();
来源：http://bsv.sysykeji.top

Java: super.greet();
来源：http://mug.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://emg.cucudq.cn

Ruby: super
来源：http://wun.gotoacloud.top

C#:   base.Greet();
来源：http://lqu.yj202588.top

[G08] 静态方法与属性
来源：http://owb.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yeu.c1oappe.top

PHP:  public static function f() {}
来源：http://gyp.zycfv.cn

JS:   static f() {}
来源：http://oma.bjfxy.top

TS:   static f(): void {}
来源：http://wcf.vqdsnc.cn

Java: static void f() {}
来源：http://xxv.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://thb.vehdjk.com

Ruby: def self.f; end
来源：http://wzm.tianlin.xyz

C#:   public static void F() {}
来源：http://fbx.pycfn.com

[G09] 接口 / 抽象类
来源：http://afr.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://qbg.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://nwq.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ked.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://ggi.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://xqv.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://dks.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vfr.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://jqs.wangdashe.top

[G10] 访问控制
来源：http://xjz.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://ihf.snrcjt.cn

PHP:  public / protected / private
来源：http://quz.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://eer.fzhhl.top

TS:   public / protected / private
来源：http://pwh.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://qva.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wtg.aibaodan.cn

Ruby: public / protected / private
来源：http://qgn.xziqi.cn

C#:   public / protected / private / internal
来源：http://igk.tanke756.top

[G11] getter / setter
来源：http://hrj.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://wlg.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zhd.vehdjk.com

JS:   get name() { return this._name; }
来源：http://ylh.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://lkx.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://eox.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://duf.tian-w.cn

Ruby: attr_accessor :name
来源：http://yqh.ybcxt.top

C#:   public string Name { get; set; }
来源：http://fza.snrcjt.cn

[G12] 对象转字符串
来源：http://gfg.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://udh.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yxl.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://jyx.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://npf.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://edt.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xha.sxryk.cn

Ruby: def to_s; @name; end
来源：http://jhz.tarul.cn

C#:   public override string ToString() => Name;
来源：http://jho.xziqi.cn

[G13] 判断对象类型
来源：http://qor.jianghu66.top

Py:   isinstance(u, User)
来源：http://psg.bjfxy.top

PHP:  $u instanceof User
来源：http://apy.jiagoushi.top

JS:   u instanceof User
来源：http://cds.shanyushiyangtech.top

TS:   u instanceof User
来源：http://ygr.dashuyun.cn

Java: u instanceof User
来源：http://koa.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vii.pycfn.com

Ruby: u.is_a?(User)
来源：http://dth.yvedp.cn

C#:   u is User
来源：http://byx.andypj.xyz

[G14] 数据类 / record
来源：http://snn.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jrh.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://ocw.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://lqu.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://xui.aizwys.cn

Java: record User(String name, int age) {}
来源：http://ajr.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://skd.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nbu.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://jpf.shangyingyoupin.top

[G15] 枚举
来源：http://ghe.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xlr.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rhe.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://seu.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hoh.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://uvu.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zfs.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://uwh.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vko.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://sps.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mmm.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://ttu.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://zke.pycfn.com

TS:   Object.entries(obj)
来源：http://xan.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rjd.yvedp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mxx.fzhhl.top

Ruby: obj.instance_variables
来源：http://rku.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://sqx.jinghuilouyu.cn

================================================================================
来源：http://hce.uphjek.com

H. 异常与错误处理
来源：http://kex.jinqigfzy.top

================================================================================
来源：http://pcf.yfazqb.com

[H01] try / catch 基础
来源：http://eut.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qjv.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://atp.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baq.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mnj.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aeu.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mud.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gfb.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rby.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://hag.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hlb.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ohm.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lys.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pjd.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://lkz.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://jcp.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kbh.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fww.nwbrower.top

[H03] 主动抛出异常
来源：http://uin.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://qky.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://adq.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://gpp.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://nfm.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gwk.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://htq.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sgm.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://lnt.xuanzx.com

[H04] 自定义异常类型
来源：http://fuk.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://xcy.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tab.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://uhi.andypj.xyz

TS:   class MyError extends Error {}
来源：http://zmy.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://oxr.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://guy.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://isy.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://ryr.mhx1999.top

[H05] 捕获特定类型
来源：http://cgq.yfazqb.com

Py:   except ValueError as e:
来源：http://oep.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://you.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://oap.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://jlo.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://lql.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kzt.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://jih.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rzw.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://vih.meibo888.top

Py:   value = d.get("k") or default
来源：http://nvz.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://zet.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zce.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zms.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zfj.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://raz.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://ria.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://gzb.dianchejie.cn

[H07] 断言
来源：http://cvw.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://jdm.tianlin.xyz

PHP:  assert($x > 0);
来源：http://xza.cheryme.top

JS:   console.assert(x > 0);
来源：http://tdz.bbcook.cn

TS:   console.assert(x > 0);
来源：http://gju.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://ssm.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wrv.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ysy.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://ier.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://akw.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://nxx.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ryj.mhx1999.top

JS:   e.message;  e.stack
来源：http://igu.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://cvy.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ncx.gzhubu.top

Go:   err.Error()
来源：http://krw.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://bxc.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://pgt.xziqi.cn

[H09] 带错误码的异常
来源：http://ymw.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cwh.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uks.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ikx.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yym.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ofl.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iok.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://apl.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://mhy.9152youxi.cn

[H10] 资源自动释放
来源：http://nvn.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://yxn.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dfo.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aou.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yts.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nmf.dianchejie.cn

Go:   defer f.Close()
来源：http://zkm.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://izv.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xmm.zhiwuduotai.top

================================================================================
来源：http://kok.haohaochexian.top

I. 正则表达式
来源：http://zqc.nanxinkj.top

================================================================================
来源：http://ayw.ctjpmb.com

[I01] 判断是否匹配
来源：http://nxx.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uwt.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://oxv.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://jfr.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://asi.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dhr.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dmc.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://gpy.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nvf.yvedp.cn

[I02] 提取所有匹配
来源：http://gqh.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://jqy.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://opa.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tyn.meibo888.top

TS:   s.match(/\d+/g)
来源：http://dmy.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eey.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xpx.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://nbv.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qfd.sjlbkw.cn

[I03] 提取捕获分组
来源：http://kzh.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qlw.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tqv.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xes.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tdt.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cdp.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gze.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tdl.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yyx.jqgfzy.top

[I04] 正则替换
来源：http://lju.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vsw.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xqd.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://ydb.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vxp.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://spc.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ick.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://afy.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gjq.cucudq.cn

[I05] 按正则拆分
来源：http://gvx.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yaw.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rfh.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://nhp.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://gsg.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://sfv.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bqy.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://cmc.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yhp.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jae.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hjd.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dex.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jac.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hvr.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jfk.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qwn.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zxx.tian-w.cn


<!-- 参考信息 -->