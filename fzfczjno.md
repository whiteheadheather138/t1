代发 wailian999

TS:   constructor(public name: string) {}
来源：http://chk.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://tjd.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yiy.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://ypk.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://vlk.hnxiangtu.top

[G03] 实例属性
来源：http://fgi.iojbl.cn

Py:   self.name = "x"
来源：http://wge.cqqwz.cn

PHP:  public string $name = "x";
来源：http://oyi.wangshuangyany.cn

JS:   this.name = "x";
来源：http://gfr.wangshuangyany.cn

TS:   name: string = "x";
来源：http://hdl.xuetiantiany.cn

Java: private String name;
来源：http://mph.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://slm.pengpengdd.cyou

Ruby: @name = "x"
来源：http://jkc.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://acq.52xcode.cn

[G04] 定义方法
来源：http://lhh.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://szr.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://giy.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://kjg.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://gza.meibo888.top

Java: String greet() { return name; }
来源：http://dnc.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wdf.bjfxy.top

Ruby: def greet; @name; end
来源：http://msi.shuidangran.top

C#:   public string Greet() => Name;
来源：http://pbs.yj20258888.top

[G05] 继承
来源：http://eqe.jiagoushi.top

Py:   class Admin(User): pass
来源：http://bqy.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://kue.52xcode.cn

JS:   class Admin extends User {}
来源：http://lsh.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://nnc.andypj.xyz

Java: class Admin extends User {}
来源：http://utz.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jzx.shuidangran.top

Ruby: class Admin < User; end
来源：http://ngh.0kj1m.cn

C#:   class Admin : User {}
来源：http://msx.sufxvd.cn

[G06] 重写方法
来源：http://avi.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://xmi.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mru.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://fgh.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://osz.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://loz.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rao.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://sxd.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://csg.hongshengwenyu.top

[G07] 调用父类方法
来源：http://nlm.redwolf501.top

Py:   super().greet()
来源：http://wzn.haohaochexian.top

PHP:  parent::greet();
来源：http://ilh.ydzc1.top

JS:   super.greet();
来源：http://xea.yfazqb.com

TS:   super.greet();
来源：http://knb.jqgufenzy.top

Java: super.greet();
来源：http://fai.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://psf.xinyue.icu

Ruby: super
来源：http://uqe.zhixingplan.top

C#:   base.Greet();
来源：http://gpw.redwolf501.top

[G08] 静态方法与属性
来源：http://ubv.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://maz.c1oappe.top

PHP:  public static function f() {}
来源：http://nzi.sysykeji.top

JS:   static f() {}
来源：http://fsd.bbcook.cn

TS:   static f(): void {}
来源：http://zzo.jlsjyb.cn

Java: static void f() {}
来源：http://tdc.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://thu.aizwys.cn

Ruby: def self.f; end
来源：http://vhe.yfazqb.com

C#:   public static void F() {}
来源：http://zfv.yfazqb.com

[G09] 接口 / 抽象类
来源：http://drk.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://xpw.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://jol.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://owc.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://iuh.tarul.cn

Java: interface Shape { double area(); }
来源：http://gzl.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://smh.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://klh.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://cqp.cqqwz.cn

[G10] 访问控制
来源：http://bqd.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://fwl.andypj.xyz

PHP:  public / protected / private
来源：http://mwj.bbcook.cn

JS:   #private 字段；其余公开
来源：http://fgm.gaohongyu789.top

TS:   public / protected / private
来源：http://wea.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://dqm.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ryq.sysykeji.top

Ruby: public / protected / private
来源：http://etr.birdmap.top

C#:   public / protected / private / internal
来源：http://qzb.gzhubu.top

[G11] getter / setter
来源：http://bcx.xziqi.cn

Py:   @property 与 @x.setter
来源：http://oiu.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rul.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://sqi.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://wur.hfpthk.cn

Java: public String getName() { return name; }
来源：http://byy.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://eru.hywenlv.cn

Ruby: attr_accessor :name
来源：http://jlx.yvedp.cn

C#:   public string Name { get; set; }
来源：http://ldu.dashuyun.cn

[G12] 对象转字符串
来源：http://cov.yj20258.top

Py:   def __str__(self): return self.name
来源：http://yev.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ptl.c1oappe.top

JS:   toString() { return this.name; }
来源：http://mxt.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://rvw.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://zqc.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dmv.yj20258.top

Ruby: def to_s; @name; end
来源：http://zaa.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://dup.daria6918.cn

[G13] 判断对象类型
来源：http://uqq.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://xgx.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://qaz.hammf.cn

JS:   u instanceof User
来源：http://neg.nanxinkj.top

TS:   u instanceof User
来源：http://xtv.nanxuanxn.top

Java: u instanceof User
来源：http://ndo.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ayl.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://bsh.havefunace.top

C#:   u is User
来源：http://ido.gotoacloud.top

[G14] 数据类 / record
来源：http://rgv.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kur.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://mau.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://scv.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://mwr.tanke756.top

Java: record User(String name, int age) {}
来源：http://phg.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://nyv.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://afx.tarul.cn

C#:   record User(string Name, int Age);
来源：http://rme.yj202588.top

[G15] 枚举
来源：http://xbr.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nqu.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dfx.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bcz.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vbp.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://ydv.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gzq.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://qwn.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suh.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://emd.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bxa.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://jor.hcnkem.com

JS:   Object.entries(obj)
来源：http://hmx.ppjwa.cn

TS:   Object.entries(obj)
来源：http://syk.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hmn.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kcj.zdqjudy.top

Ruby: obj.instance_variables
来源：http://tgk.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://dap.yfazqb.com

================================================================================
来源：http://yzg.shuidangran.top

H. 异常与错误处理
来源：http://mwv.cqqwz.cn

================================================================================
来源：http://bky.xuanzx.com

[H01] try / catch 基础
来源：http://pag.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lcg.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mgq.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pzk.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tth.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zxd.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://izq.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nnx.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://muy.andypj.xyz

[H02] finally / ensure 收尾
来源：http://pyj.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gcm.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rwa.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bfd.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aee.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://jwq.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nfa.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dom.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ukd.daria6918.cn

[H03] 主动抛出异常
来源：http://uhe.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://jxa.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aou.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://cjb.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://hmq.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fob.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yle.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://lrp.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gij.meibo888.top

[H04] 自定义异常类型
来源：http://yhs.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://niq.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://sgg.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://aud.yj20258888.top

TS:   class MyError extends Error {}
来源：http://uws.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://vrq.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ylo.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://lal.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://xwh.yongpay.top

[H05] 捕获特定类型
来源：http://ewl.sweek.top

Py:   except ValueError as e:
来源：http://rqz.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cds.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://uro.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://slv.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://ylg.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fnr.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://umg.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ker.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://gmx.hnqzz.top

Py:   value = d.get("k") or default
来源：http://guy.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://nub.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://gwl.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nhz.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qgs.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://moz.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://yxd.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://xgs.pycfn.com

[H07] 断言
来源：http://efn.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://mmt.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://kmh.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://cff.andypj.xyz

TS:   console.assert(x > 0);
来源：http://pre.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://hax.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qig.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rnb.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://gbm.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://psu.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://ogr.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rwa.cheryme.top

JS:   e.message;  e.stack
来源：http://sth.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://npl.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kmk.yongpay.top

Go:   err.Error()
来源：http://eka.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://nhe.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://ydv.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://sdo.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gxb.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fcc.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fcw.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://utq.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://csz.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vlf.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://gmi.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://usy.ctjpmb.com

[H10] 资源自动释放
来源：http://gcp.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://nrm.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qvq.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gjj.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ltt.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wog.ehwqpu.com

Go:   defer f.Close()
来源：http://umu.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://esw.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lcj.jlsjyb.cn

================================================================================
来源：http://riy.zhengqikj.top

I. 正则表达式
来源：http://sig.mhx1999.top

================================================================================
来源：http://iyy.zhoulong.xyz

[I01] 判断是否匹配
来源：http://tpe.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jst.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://gvo.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://ele.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://gwh.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nbg.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ahi.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://wtt.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://msd.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://dpi.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://cci.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mcn.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://txz.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://dbf.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sjn.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbf.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://xnv.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lhy.yanxiufei.cn

[I03] 提取捕获分组
来源：http://vaw.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uge.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hss.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nkj.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nvq.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rmv.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vfy.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qoa.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vga.aibaodan.cn

[I04] 正则替换
来源：http://ykz.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yqh.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://obx.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rhb.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://jgd.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://ffc.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nkc.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lmw.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ejk.fzhhl.top

[I05] 按正则拆分
来源：http://nkr.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mpe.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xrc.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://kfc.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://wvw.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://hqv.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://utk.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://grd.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgv.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jft.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gem.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://utx.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bhf.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfx.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ohd.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uqa.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://smh.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://coy.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://cox.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wvs.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hds.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bcz.zhongyouzk.top

TS:   /error/gim
来源：http://eeu.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://szf.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zpc.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://gwo.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ecd.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://ami.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hix.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vua.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yon.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://chs.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://iwm.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qpz.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mug.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ktf.sysykeji.top

================================================================================
来源：http://lum.redwolf501.top


<!-- 参考信息 -->