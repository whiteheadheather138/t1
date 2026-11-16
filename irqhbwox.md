代发 wailian999

================================================================================
来源：http://qrx.wangdashe.top

G. 面向对象
来源：http://hqw.svipenyu.cn

================================================================================
来源：http://qdv.hywenlv.cn

[G01] 定义类
来源：http://hol.ppjwa.cn

Py:   class User: pass
来源：http://imt.fengsongda.top

PHP:  class User {}
来源：http://qll.52xcode.cn

JS:   class User {}
来源：http://fil.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://wow.dianchejie.cn

Java: class User {}
来源：http://mjt.ppjwa.cn

Go:   type User struct { Name string }
来源：http://xty.ehwqpu.com

Ruby: class User; end
来源：http://yuu.yj202588.top

C#:   class User {}
来源：http://uil.yuanzhike.top

[G02] 构造函数
来源：http://odu.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://gbl.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://etf.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://kud.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://hqu.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://xzp.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qdm.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://grp.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://ugy.wangdashe.top

[G03] 实例属性
来源：http://yrv.vqdsnc.cn

Py:   self.name = "x"
来源：http://efv.yj202588.top

PHP:  public string $name = "x";
来源：http://jjo.yuxming.cn

JS:   this.name = "x";
来源：http://qmm.c1oappe.top

TS:   name: string = "x";
来源：http://fpb.ctjpmb.com

Java: private String name;
来源：http://pnh.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bvm.shuidangran.top

Ruby: @name = "x"
来源：http://zmi.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://xgz.ywan-chungtsiang.top

[G04] 定义方法
来源：http://ifw.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://cdz.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ufi.hnqzz.top

JS:   greet() { return this.name; }
来源：http://tiv.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://lov.zdqjudy.top

Java: String greet() { return name; }
来源：http://ycx.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://fjf.yuanzhike.top

Ruby: def greet; @name; end
来源：http://vlk.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://lxu.jqgufenzy.top

[G05] 继承
来源：http://zpy.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://dqe.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://tmg.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://sue.yj20258.top

TS:   class Admin extends User {}
来源：http://atl.gotoacloud.top

Java: class Admin extends User {}
来源：http://ifv.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wfp.bbcook.cn

Ruby: class Admin < User; end
来源：http://mys.ivvv.top

C#:   class Admin : User {}
来源：http://yis.haohaochexian.top

[G06] 重写方法
来源：http://cln.nanxinkj.top

Py:   def greet(self): return "admin"
来源：http://gce.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nzz.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://uph.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://jjn.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://gtd.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xya.yongpay.top

Ruby: def greet; "admin"; end
来源：http://vhl.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://epy.hnxiangtu.top

[G07] 调用父类方法
来源：http://pum.dashuyun.cn

Py:   super().greet()
来源：http://zqo.hnqzz.top

PHP:  parent::greet();
来源：http://hal.aizwys.cn

JS:   super.greet();
来源：http://qxp.jianghu66.top

TS:   super.greet();
来源：http://ssa.redwolf501.top

Java: super.greet();
来源：http://qcg.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wue.shangyingyoupin.top

Ruby: super
来源：http://voa.zhixingplan.top

C#:   base.Greet();
来源：http://jni.tianlin.xyz

[G08] 静态方法与属性
来源：http://ytq.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uwc.yueranfly.top

PHP:  public static function f() {}
来源：http://sfn.chenzaomai.com

JS:   static f() {}
来源：http://dot.aibaodan.cn

TS:   static f(): void {}
来源：http://xjg.shangyingyoupin.top

Java: static void f() {}
来源：http://lyy.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pbk.yonumen.top

Ruby: def self.f; end
来源：http://wac.birdmap.top

C#:   public static void F() {}
来源：http://okz.iojbl.cn

[G09] 接口 / 抽象类
来源：http://gkz.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://cdw.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://nht.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lyl.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://miu.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://vkc.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://fbg.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yop.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://cgw.mhx1999.top

[G10] 访问控制
来源：http://cvg.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://alg.aibaodan.cn

PHP:  public / protected / private
来源：http://pub.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://cpe.shuidangran.top

TS:   public / protected / private
来源：http://czj.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://gpe.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gqi.guannengcc.top

Ruby: public / protected / private
来源：http://per.meibo888.top

C#:   public / protected / private / internal
来源：http://shf.ydjk.org.cn

[G11] getter / setter
来源：http://hwb.daria6918.cn

Py:   @property 与 @x.setter
来源：http://ytc.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lns.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://qfn.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://czs.bbcook.cn

Java: public String getName() { return name; }
来源：http://opi.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uds.hammf.cn

Ruby: attr_accessor :name
来源：http://hfe.bjfxy.top

C#:   public string Name { get; set; }
来源：http://wli.jyoumei.cn

[G12] 对象转字符串
来源：http://pfo.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://gbs.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://bcl.mhx1999.top

JS:   toString() { return this.name; }
来源：http://sac.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://zkb.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://ksv.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://qdb.meibo888.top

Ruby: def to_s; @name; end
来源：http://pis.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://xpo.zdbjq.cn

[G13] 判断对象类型
来源：http://sxt.hesvh.cn

Py:   isinstance(u, User)
来源：http://uas.52xcode.cn

PHP:  $u instanceof User
来源：http://ghx.ehwqpu.com

JS:   u instanceof User
来源：http://nav.sysykeji.top

TS:   u instanceof User
来源：http://krj.cheryme.top

Java: u instanceof User
来源：http://alu.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ebk.sysykeji.top

Ruby: u.is_a?(User)
来源：http://civ.jqgfzy.top

C#:   u is User
来源：http://msz.uphjek.com

[G14] 数据类 / record
来源：http://nzu.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://upg.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ckm.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://xjc.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://ysm.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://flo.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://sth.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://huq.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://ido.tianlin.xyz

[G15] 枚举
来源：http://dvd.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zga.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ylc.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tes.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ndc.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://sax.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zcv.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://fbf.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hxa.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://gze.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ope.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://kox.ybcxt.top

JS:   Object.entries(obj)
来源：http://txy.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://ire.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lby.jianghu66.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kpg.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://ghc.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://uki.yvedp.cn

================================================================================
来源：http://bhv.sweek.top

H. 异常与错误处理
来源：http://qbj.yj202588.top

================================================================================
来源：http://fjb.vqdsnc.cn

[H01] try / catch 基础
来源：http://mre.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://diq.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oan.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qks.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bqy.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oco.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rgq.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rcr.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rxy.yuxming.cn

[H02] finally / ensure 收尾
来源：http://eof.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kom.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mnm.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dqx.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vui.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nfi.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mid.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rii.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://edr.pycfn.com

[H03] 主动抛出异常
来源：http://org.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://rfc.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vbz.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://mpd.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://hch.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://jzb.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cvg.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mbb.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://kvw.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://sox.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://hus.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://sqz.hnqzz.top

JS:   class MyError extends Error {}
来源：http://ebn.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://fyg.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://trc.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dmt.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://cjz.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://orc.wangdashe.top

[H05] 捕获特定类型
来源：http://zdd.xuanzx.com

Py:   except ValueError as e:
来源：http://xay.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kcx.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://pfn.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://czd.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://qcp.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cyp.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://rjl.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://soh.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://jew.smart0.xyz

Py:   value = d.get("k") or default
来源：http://wir.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dyl.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://gzw.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://flh.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://snu.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yjm.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://uco.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://rfd.xziqi.cn

[H07] 断言
来源：http://iha.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://sim.jinqigufen.top

PHP:  assert($x > 0);
来源：http://qsx.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://jgy.xylfe.cn

TS:   console.assert(x > 0);
来源：http://srd.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://tvc.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pgv.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://qhy.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://lwz.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://sto.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://wni.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qsf.ctjpmb.com

JS:   e.message;  e.stack
来源：http://cji.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://puj.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ivi.yj20258888.top

Go:   err.Error()
来源：http://aek.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://klv.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://cdi.dashuyun.cn

[H09] 带错误码的异常
来源：http://ibz.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nah.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bba.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nqa.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nja.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vww.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iel.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hgr.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qca.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://lna.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xzx.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qqi.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nxk.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nuj.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qbd.guowangkeji.top

Go:   defer f.Close()
来源：http://xuo.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bmj.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rcj.hesvh.cn

================================================================================
来源：http://wgi.jyoumei.cn

I. 正则表达式
来源：http://lrk.sysykeji.top

================================================================================
来源：http://qxu.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://rfm.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lvs.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://pht.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://lmn.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://gju.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dec.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uhd.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://qwv.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yok.jinqigfzy.top

[I02] 提取所有匹配
来源：http://ecd.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://div.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ble.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://acy.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://qkg.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ozy.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tzh.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://oox.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rog.gaohongyu789.top

[I03] 提取捕获分组
来源：http://ydl.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pbc.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nlb.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dmr.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://agw.shuidangran.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hdo.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tik.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dct.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://huh.shanyushiyangtech.top

[I04] 正则替换
来源：http://wci.jiagoushi.top

Py:   re.sub(r"\d+", "#", s)
来源：http://keq.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fdg.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://cug.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://wwm.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://kqn.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tgb.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://myt.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://afi.sxryk.cn

[I05] 按正则拆分
来源：http://pjx.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sgo.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xnu.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://fzq.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://pqy.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://qgf.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dgp.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://udp.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bji.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://twq.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nmi.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vga.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://anc.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ylt.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sdb.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hwj.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vwr.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mca.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://cfc.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iek.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mfc.fengsongda.top


<!-- 参考信息 -->