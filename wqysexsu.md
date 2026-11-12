代发 wailian999

Py:   class User: pass
来源：http://zmd.cashguo.top

PHP:  class User {}
来源：http://mhd.jinyuanbaomall.cn

JS:   class User {}
来源：http://dck.tanke756.top

TS:   class User { name: string = ""; }
来源：http://ujh.jinyuanbaomall.cn

Java: class User {}
来源：http://lad.fktsv.cn

Go:   type User struct { Name string }
来源：http://qpb.hammf.cn

Ruby: class User; end
来源：http://jtw.xingfuxueyuan.xyz

C#:   class User {}
来源：http://mej.fzhhl.top

[G02] 构造函数
来源：http://ysl.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://lym.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://sjy.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://mxg.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://jlw.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://igw.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rnz.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://pth.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://fhe.fehbvm.com

[G03] 实例属性
来源：http://vzk.hcnkem.com

Py:   self.name = "x"
来源：http://zbt.sysykeji.top

PHP:  public string $name = "x";
来源：http://dlo.316326.xyz

JS:   this.name = "x";
来源：http://cld.tianlin.xyz

TS:   name: string = "x";
来源：http://dfn.jinghuilouyu.cn

Java: private String name;
来源：http://uxd.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aeg.hammf.cn

Ruby: @name = "x"
来源：http://ouw.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://gqs.yj20258888.top

[G04] 定义方法
来源：http://kui.fehbvm.com

Py:   def greet(self): return self.name
来源：http://tbg.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://foj.ybcxt.top

JS:   greet() { return this.name; }
来源：http://aba.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://nit.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://oul.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://npb.vehdjk.com

Ruby: def greet; @name; end
来源：http://eoi.xuanzx.com

C#:   public string Greet() => Name;
来源：http://zga.nwbrower.top

[G05] 继承
来源：http://wwa.andypj.xyz

Py:   class Admin(User): pass
来源：http://dzr.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://lis.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://oqp.cqqwz.cn

TS:   class Admin extends User {}
来源：http://qux.guannengcc.top

Java: class Admin extends User {}
来源：http://iut.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vaf.0kj1m.cn

Ruby: class Admin < User; end
来源：http://nqp.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://pzz.316326.xyz

[G06] 重写方法
来源：http://nvi.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://kpk.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://vkq.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://sga.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://bra.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://psx.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nyh.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://uph.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://bmy.guowangkeji.top

[G07] 调用父类方法
来源：http://zsy.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://bwg.svipenyu.cn

PHP:  parent::greet();
来源：http://uwj.hesvh.cn

JS:   super.greet();
来源：http://evy.xinyue.icu

TS:   super.greet();
来源：http://ams.gogol.net.cn

Java: super.greet();
来源：http://ivw.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ljm.zdqjudy.top

Ruby: super
来源：http://pms.xylfe.cn

C#:   base.Greet();
来源：http://rwe.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://dqj.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nmp.daria6918.cn

PHP:  public static function f() {}
来源：http://exq.nanxuanxn.top

JS:   static f() {}
来源：http://rqs.wangshuangyany.cn

TS:   static f(): void {}
来源：http://vpq.gzhubu.top

Java: static void f() {}
来源：http://onl.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ngi.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://fal.yuxming.cn

C#:   public static void F() {}
来源：http://muf.cheryme.top

[G09] 接口 / 抽象类
来源：http://nwr.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://zhv.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://tdq.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://aah.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://nah.mhx1999.top

Java: interface Shape { double area(); }
来源：http://fji.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://xqb.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ctn.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://jtu.nwbrower.top

[G10] 访问控制
来源：http://vac.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://vaa.uphjek.com

PHP:  public / protected / private
来源：http://aoo.uphjek.com

JS:   #private 字段；其余公开
来源：http://twv.ydjk.org.cn

TS:   public / protected / private
来源：http://svu.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://kfi.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pga.daria6918.cn

Ruby: public / protected / private
来源：http://qjb.wangdashe.top

C#:   public / protected / private / internal
来源：http://mhj.cashguo.top

[G11] getter / setter
来源：http://lqi.aizwys.cn

Py:   @property 与 @x.setter
来源：http://osj.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://laj.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://ejh.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://svd.redwolf501.top

Java: public String getName() { return name; }
来源：http://nkh.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://kdk.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://hqe.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://wyp.pengpengdd.cyou

[G12] 对象转字符串
来源：http://mma.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://xdx.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://swx.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://qsk.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://prp.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://jcw.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ppk.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://poy.tanke756.top

C#:   public override string ToString() => Name;
来源：http://oku.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://yjh.daxiang520.top

Py:   isinstance(u, User)
来源：http://odn.52xcode.cn

PHP:  $u instanceof User
来源：http://cbo.shuidangran.top

JS:   u instanceof User
来源：http://zes.jiagoushi.top

TS:   u instanceof User
来源：http://eyx.gogol.net.cn

Java: u instanceof User
来源：http://ony.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oof.xinyue.icu

Ruby: u.is_a?(User)
来源：http://uiq.yj20258888.top

C#:   u is User
来源：http://arm.jlsjyb.cn

[G14] 数据类 / record
来源：http://fmu.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fjc.zhoulong.xyz

PHP:  // 用 readonly 属性模拟
来源：http://vtc.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://yxt.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://itu.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://bga.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://gor.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sjg.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://ucs.daria6918.cn

[G15] 枚举
来源：http://ebp.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wrd.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uba.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fnz.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xqe.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://usj.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nbq.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://fkd.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yde.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://pxo.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mfd.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://bfz.yj20258888.top

JS:   Object.entries(obj)
来源：http://ydc.0kj1m.cn

TS:   Object.entries(obj)
来源：http://koo.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://duv.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vgd.0kj1m.cn

Ruby: obj.instance_variables
来源：http://uqi.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://tvc.zhixingplan.top

================================================================================
来源：http://nhn.jinqigufen.top

H. 异常与错误处理
来源：http://osa.hesvh.cn

================================================================================
来源：http://ois.c1oappe.top

[H01] try / catch 基础
来源：http://aoi.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ais.shanyushiyangtech.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nmd.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vtp.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xev.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qbx.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ydn.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lqe.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fli.316326.xyz

[H02] finally / ensure 收尾
来源：http://ndl.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://vrs.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ock.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zjd.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xap.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ykq.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kjd.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qmi.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vmz.zhengqikj.top

[H03] 主动抛出异常
来源：http://mje.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://iyo.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ojd.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://bgk.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://tqx.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qyb.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qta.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://job.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://zhx.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://qiz.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://eve.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://vgn.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://hms.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://jbh.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://swc.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wve.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://kqb.daria6918.cn

C#:   class MyException : Exception {}
来源：http://zgi.daria6918.cn

[H05] 捕获特定类型
来源：http://qes.epnwcf.com

Py:   except ValueError as e:
来源：http://qld.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nfi.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://xha.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://lnx.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://kvp.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bzp.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://hwu.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qks.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://jpl.yj20258888.top

Py:   value = d.get("k") or default
来源：http://zdp.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zhs.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://olo.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://rux.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vpk.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vcu.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://jja.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://css.fengsongda.top

[H07] 断言
来源：http://fpq.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://obw.xziqi.cn

PHP:  assert($x > 0);
来源：http://mve.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://dpt.nwbrower.top

TS:   console.assert(x > 0);
来源：http://ujx.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://vtu.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kmj.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vps.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://vvx.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://djj.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://pjz.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sag.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://bqw.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ixp.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://nyk.xziqi.cn

Go:   err.Error()
来源：http://rzf.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://iww.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://pln.chenzaomai.com

[H09] 带错误码的异常
来源：http://wfw.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yto.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdn.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blh.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bfv.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://suf.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qbu.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://lwn.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://apo.hfpthk.cn

[H10] 资源自动释放
来源：http://doo.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ods.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ifh.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yrk.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pdz.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dmy.jinqigfzy.top

Go:   defer f.Close()
来源：http://gko.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://edn.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jpe.zhoulong.xyz

================================================================================
来源：http://vck.kuanghao11.cn

I. 正则表达式
来源：http://svw.tanke756.top

================================================================================
来源：http://jjn.jianghu66.top

[I01] 判断是否匹配
来源：http://iru.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zgt.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://yii.fktsv.cn

JS:   /\d+/.test(s)
来源：http://zqs.epnwcf.com

TS:   /\d+/.test(s)
来源：http://lvr.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eyj.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wjp.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://yiu.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mot.uphjek.com

[I02] 提取所有匹配
来源：http://iph.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://vld.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rze.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ppi.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://oez.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fst.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nyc.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://sku.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nrq.aizwys.cn

[I03] 提取捕获分组
来源：http://txl.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yjt.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://osl.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rws.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oep.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sok.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eol.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rsq.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vsl.9152youxi.cn

[I04] 正则替换
来源：http://xlv.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lww.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://llk.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yce.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xfx.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fup.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://irh.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ayv.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dzy.smart0.xyz

[I05] 按正则拆分
来源：http://zvs.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hco.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rne.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://ixd.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://wcl.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://gbz.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sro.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tui.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tmk.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ovz.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ymz.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aqb.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iek.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bgr.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yoo.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xms.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vgl.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pjy.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://jkg.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ztw.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fqd.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://roi.cheryme.top

TS:   /error/gim
来源：http://dlt.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xlj.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zuf.sjlbkw.cn


<!-- 参考信息 -->