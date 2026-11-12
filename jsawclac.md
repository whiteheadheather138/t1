代发 wailian999

Py:   class User: pass
来源：http://teb.gogol.net.cn

PHP:  class User {}
来源：http://vsb.meibo888.top

JS:   class User {}
来源：http://tzf.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://ehi.jinghuilouyu.cn

Java: class User {}
来源：http://rsh.svipenyu.cn

Go:   type User struct { Name string }
来源：http://eel.chenlongwang.top

Ruby: class User; end
来源：http://fpw.birdmap.top

C#:   class User {}
来源：http://btd.cashguo.top

[G02] 构造函数
来源：http://jqg.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://ooj.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://lma.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://val.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://zne.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://wjd.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://onf.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://zcs.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://qex.smart0.xyz

[G03] 实例属性
来源：http://hxd.aizwys.cn

Py:   self.name = "x"
来源：http://esi.xylfe.cn

PHP:  public string $name = "x";
来源：http://ftp.gotoacloud.top

JS:   this.name = "x";
来源：http://rnk.bjfxy.top

TS:   name: string = "x";
来源：http://tco.sysykeji.top

Java: private String name;
来源：http://vnz.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tqo.zhengqikj.top

Ruby: @name = "x"
来源：http://vhz.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://kql.sysykeji.top

[G04] 定义方法
来源：http://ybm.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://xyr.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bln.yj20258.top

JS:   greet() { return this.name; }
来源：http://mid.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://onz.hysaishi.cn

Java: String greet() { return name; }
来源：http://waf.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://jap.52xcode.cn

Ruby: def greet; @name; end
来源：http://njt.epnwcf.com

C#:   public string Greet() => Name;
来源：http://hux.gzhubu.top

[G05] 继承
来源：http://kxr.hammf.cn

Py:   class Admin(User): pass
来源：http://inf.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://wrc.dianchejie.cn

JS:   class Admin extends User {}
来源：http://nwp.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://pfh.tanke756.top

Java: class Admin extends User {}
来源：http://zko.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ffx.jianghu66.top

Ruby: class Admin < User; end
来源：http://rwt.zhijiandao.cn

C#:   class Admin : User {}
来源：http://tmi.sxryk.cn

[G06] 重写方法
来源：http://rmz.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://ajh.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lvj.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://wnp.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://dgl.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://lob.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rek.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://hgz.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://kpy.hongshengwenyu.top

[G07] 调用父类方法
来源：http://ead.guannengcc.top

Py:   super().greet()
来源：http://epi.jqgufenzy.top

PHP:  parent::greet();
来源：http://fqe.wangdashe.top

JS:   super.greet();
来源：http://aon.zhijiandao.cn

TS:   super.greet();
来源：http://wzx.yj20258888.top

Java: super.greet();
来源：http://qpa.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eqe.zdqjudy.top

Ruby: super
来源：http://lmr.jiagoushi.top

C#:   base.Greet();
来源：http://yjq.guowangkeji.top

[G08] 静态方法与属性
来源：http://fma.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zsm.epnwcf.com

PHP:  public static function f() {}
来源：http://zpa.sysykeji.top

JS:   static f() {}
来源：http://iga.hnqzz.top

TS:   static f(): void {}
来源：http://hzd.sweek.top

Java: static void f() {}
来源：http://njl.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vsn.snrcjt.cn

Ruby: def self.f; end
来源：http://fto.yfazqb.com

C#:   public static void F() {}
来源：http://kdm.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://yun.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://kvf.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://ztf.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yyr.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://grt.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://uzp.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://ajg.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qjd.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://qek.xziqi.cn

[G10] 访问控制
来源：http://uqz.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://kad.hysaishi.cn

PHP:  public / protected / private
来源：http://ndv.jianghu66.top

JS:   #private 字段；其余公开
来源：http://fmt.hesvh.cn

TS:   public / protected / private
来源：http://due.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://max.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qts.kuanghao11.cn

Ruby: public / protected / private
来源：http://ouv.jinqigufen.top

C#:   public / protected / private / internal
来源：http://woo.sufxvd.cn

[G11] getter / setter
来源：http://crk.fehbvm.com

Py:   @property 与 @x.setter
来源：http://dpc.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ahs.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://iuo.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://oog.jinqigufen.top

Java: public String getName() { return name; }
来源：http://iuf.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzc.sweek.top

Ruby: attr_accessor :name
来源：http://gtc.fktsv.cn

C#:   public string Name { get; set; }
来源：http://xkq.sufxvd.cn

[G12] 对象转字符串
来源：http://hsg.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://ydg.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ofu.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://muo.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://ece.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://rxg.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jxm.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://xgb.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://emi.redwolf501.top

[G13] 判断对象类型
来源：http://dgj.pycfn.com

Py:   isinstance(u, User)
来源：http://jch.quarkkingdee.top

PHP:  $u instanceof User
来源：http://yok.iojbl.cn

JS:   u instanceof User
来源：http://kvg.wangdashe.top

TS:   u instanceof User
来源：http://rig.yvedp.cn

Java: u instanceof User
来源：http://ipm.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://krs.xylfe.cn

Ruby: u.is_a?(User)
来源：http://uis.xziqi.cn

C#:   u is User
来源：http://vyj.ybcxt.top

[G14] 数据类 / record
来源：http://fah.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dfd.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://pyl.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://kjc.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://krw.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://jxw.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://uga.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sle.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://qnd.cdnleiting.top

[G15] 枚举
来源：http://zja.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mxh.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bne.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nsa.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zhz.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://kzh.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://myv.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://aye.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hck.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://skk.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://juh.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://bww.ivvv.top

JS:   Object.entries(obj)
来源：http://ews.ydzc1.top

TS:   Object.entries(obj)
来源：http://usq.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bxx.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gcy.cdnleiting.top

Ruby: obj.instance_variables
来源：http://wvu.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://hoi.jiagoushi.top

================================================================================
来源：http://zos.fktsv.cn

H. 异常与错误处理
来源：http://aww.yueranfly.top

================================================================================
来源：http://cwq.cdnleiting.top

[H01] try / catch 基础
来源：http://ssu.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://whc.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pnv.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bnt.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jic.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://agq.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fwa.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iqi.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qzg.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://ojj.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://rmn.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bni.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://znh.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://zge.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://bxr.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eji.hysaishi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bym.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://msw.yonumen.top

[H03] 主动抛出异常
来源：http://jgh.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://trl.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ysq.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://wou.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://evq.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zqb.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hjo.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://sjv.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dro.gaohongyu789.top

[H04] 自定义异常类型
来源：http://cly.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://enj.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://tva.iojbl.cn

JS:   class MyError extends Error {}
来源：http://gbb.cashguo.top

TS:   class MyError extends Error {}
来源：http://yuw.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://vnc.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xsv.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://xbl.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://rik.jlsjyb.cn

[H05] 捕获特定类型
来源：http://gqu.meibo888.top

Py:   except ValueError as e:
来源：http://wdk.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zkn.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://wfs.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://yfs.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://htq.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jig.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://jgb.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dpx.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://kfq.shuidangran.top

Py:   value = d.get("k") or default
来源：http://ldz.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://aol.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://rae.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://jmk.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zip.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://deq.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://cby.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://zdc.fehbvm.com

[H07] 断言
来源：http://dfu.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://hyz.sweek.top

PHP:  assert($x > 0);
来源：http://maz.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://fuj.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://qds.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://iuy.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cju.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hpr.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://ngj.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://ipj.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://bwj.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nwr.svipenyu.cn

JS:   e.message;  e.stack
来源：http://nov.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://tyx.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cnv.smart0.xyz

Go:   err.Error()
来源：http://fgo.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://gkg.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://aui.daxiang520.top

[H09] 带错误码的异常
来源：http://gpw.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qcc.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://apu.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gnr.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kek.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vba.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ayv.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://zzl.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gem.chenzaomai.com

[H10] 资源自动释放
来源：http://fva.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oht.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wlj.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://epm.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wow.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mgk.yj202588.top

Go:   defer f.Close()
来源：http://zth.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dli.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdu.xuetiantiany.cn

================================================================================
来源：http://fck.jiagoushi.top

I. 正则表达式
来源：http://jyw.tanke756.top

================================================================================
来源：http://scy.0kj1m.cn

[I01] 判断是否匹配
来源：http://kxv.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oxr.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cvu.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://joy.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://wnw.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aaz.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fqf.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://lrb.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ven.chenzaomai.com

[I02] 提取所有匹配
来源：http://vrp.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://qyf.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lnh.yvedp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hpa.meibo888.top

TS:   s.match(/\d+/g)
来源：http://ogt.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iuh.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gtc.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://svw.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uxy.sweek.top

[I03] 提取捕获分组
来源：http://tqg.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ucr.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qnw.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://egf.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kfw.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ggx.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ypk.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rlf.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kgp.yj202588.top

[I04] 正则替换
来源：http://hcy.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wfd.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nxh.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kqn.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://alu.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://aaa.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vzz.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://idt.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jrj.gaohongyu789.top

[I05] 按正则拆分
来源：http://dsx.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://spi.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fir.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://dmm.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://pks.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://whg.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gym.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://aww.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sja.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yol.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zyh.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ajg.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cla.zhongyouzk.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzp.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ugb.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://inv.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kyk.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xdh.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://oan.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ukb.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sro.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nvx.nanxinkj.top

TS:   /error/gim
来源：http://tfb.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bmo.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bue.zhiwuduotai.top


<!-- 参考信息 -->