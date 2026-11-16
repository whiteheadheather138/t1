代发 wailian999

[G02] 构造函数
来源：http://cjr.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://vsp.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://qsu.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://iqe.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://vlt.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://oem.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mfq.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://don.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://pus.tanke756.top

[G03] 实例属性
来源：http://ici.yuanzhike.top

Py:   self.name = "x"
来源：http://xlw.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://tpf.yj20258888.top

JS:   this.name = "x";
来源：http://dnw.xuanzx.com

TS:   name: string = "x";
来源：http://kup.jlsjyb.cn

Java: private String name;
来源：http://fcf.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rtu.iojbl.cn

Ruby: @name = "x"
来源：http://vdq.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://kti.gzhubu.top

[G04] 定义方法
来源：http://whs.gzhubu.top

Py:   def greet(self): return self.name
来源：http://sqw.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uqw.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://noc.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://dbo.daria6918.cn

Java: String greet() { return name; }
来源：http://kju.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ipo.yuxming.cn

Ruby: def greet; @name; end
来源：http://vtd.daxiang520.top

C#:   public string Greet() => Name;
来源：http://wmk.xuanzx.com

[G05] 继承
来源：http://kzb.yfazqb.com

Py:   class Admin(User): pass
来源：http://laz.yuxming.cn

PHP:  class Admin extends User {}
来源：http://ugc.gzhubu.top

JS:   class Admin extends User {}
来源：http://yas.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://sks.yj20258.top

Java: class Admin extends User {}
来源：http://kye.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rgo.redwolf501.top

Ruby: class Admin < User; end
来源：http://foh.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://bso.snrcjt.cn

[G06] 重写方法
来源：http://sxg.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://vpw.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gos.yonumen.top

JS:   greet() { return "admin"; }
来源：http://aot.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://fmi.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://hvl.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://brj.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://fis.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://ors.snrcjt.cn

[G07] 调用父类方法
来源：http://lea.jiagoushi.top

Py:   super().greet()
来源：http://qnn.316326.xyz

PHP:  parent::greet();
来源：http://bmw.sweek.top

JS:   super.greet();
来源：http://dsj.xylfe.cn

TS:   super.greet();
来源：http://ier.pycfn.com

Java: super.greet();
来源：http://shq.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wls.fzhhl.top

Ruby: super
来源：http://ydn.c1oappe.top

C#:   base.Greet();
来源：http://gvi.sweek.top

[G08] 静态方法与属性
来源：http://hyo.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xiw.yuxming.cn

PHP:  public static function f() {}
来源：http://uby.ivvv.top

JS:   static f() {}
来源：http://tiz.jianghu66.top

TS:   static f(): void {}
来源：http://kik.zhaomingkeji.xyz

Java: static void f() {}
来源：http://qug.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ekz.zdbjq.cn

Ruby: def self.f; end
来源：http://tgk.gotoacloud.top

C#:   public static void F() {}
来源：http://rao.cucudq.cn

[G09] 接口 / 抽象类
来源：http://rcz.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://rsw.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://fvh.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ksz.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://fwt.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://smt.zhaomingkeji.xyz

Go:   type Shape interface { Area() float64 }
来源：http://znj.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gbc.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://nyo.yueranfly.top

[G10] 访问控制
来源：http://wgo.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://uvq.sjlbkw.cn

PHP:  public / protected / private
来源：http://zqw.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://dks.sweek.top

TS:   public / protected / private
来源：http://cjd.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://mfl.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dnk.sweek.top

Ruby: public / protected / private
来源：http://rwk.sxryk.cn

C#:   public / protected / private / internal
来源：http://buq.yuanzhike.top

[G11] getter / setter
来源：http://wyq.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://rzf.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dfw.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://qni.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://bfe.cdnleiting.top

Java: public String getName() { return name; }
来源：http://yrz.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vob.316326.xyz

Ruby: attr_accessor :name
来源：http://hwu.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://wsf.jianghu66.top

[G12] 对象转字符串
来源：http://hvg.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://pyq.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mav.hammf.cn

JS:   toString() { return this.name; }
来源：http://omk.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://tet.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://qne.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://igg.uphjek.com

Ruby: def to_s; @name; end
来源：http://uil.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://dsu.fktsv.cn

[G13] 判断对象类型
来源：http://wgr.tianlin.xyz

Py:   isinstance(u, User)
来源：http://mmz.zdqjudy.top

PHP:  $u instanceof User
来源：http://hhj.ctjpmb.com

JS:   u instanceof User
来源：http://gnd.daria6918.cn

TS:   u instanceof User
来源：http://bqd.tianlin.xyz

Java: u instanceof User
来源：http://pcu.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ylx.mhx1999.top

Ruby: u.is_a?(User)
来源：http://deo.aizwys.cn

C#:   u is User
来源：http://fyp.52xcode.cn

[G14] 数据类 / record
来源：http://pqg.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ikg.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://xlt.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rvh.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://qxj.fehbvm.com

Java: record User(String name, int age) {}
来源：http://zip.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://gxa.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fws.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://yro.xziqi.cn

[G15] 枚举
来源：http://lbd.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sfw.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bts.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ota.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qtb.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://hbt.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jbs.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://pxp.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aqu.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://lzr.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://esm.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://tzb.tian-w.cn

JS:   Object.entries(obj)
来源：http://tuk.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://ihe.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xdt.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ucj.jqgfzy.top

Ruby: obj.instance_variables
来源：http://chb.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://hct.wangdashe.top

================================================================================
来源：http://zqx.snrcjt.cn

H. 异常与错误处理
来源：http://vvn.sjlbkw.cn

================================================================================
来源：http://pea.sjlbkw.cn

[H01] try / catch 基础
来源：http://lqd.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dbn.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cyn.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nwr.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ylt.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nnf.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jgf.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tsk.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yib.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://cek.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://leq.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yhd.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://htn.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mho.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://jcc.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gwm.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rvp.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wge.shzxlz.cn

[H03] 主动抛出异常
来源：http://twm.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://bfz.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zja.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://xbv.havefunace.top

TS:   throw new Error("错误信息");
来源：http://lte.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ntz.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oho.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wse.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fmw.yj20258.top

[H04] 自定义异常类型
来源：http://oxa.yongpay.top

Py:   class MyError(Exception): pass
来源：http://fpp.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://feq.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://uer.xylfe.cn

TS:   class MyError extends Error {}
来源：http://sjy.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://hlv.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vmg.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://tay.hywenlv.cn

C#:   class MyException : Exception {}
来源：http://lbl.sysykeji.top

[H05] 捕获特定类型
来源：http://kye.yonumen.top

Py:   except ValueError as e:
来源：http://cry.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pjm.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://gim.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://twv.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://svm.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ykk.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://rsh.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kww.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://gep.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://pxi.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://jrj.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://yyp.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://qov.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tat.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jvu.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://xkk.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://jzt.hongshengwenyu.top

[H07] 断言
来源：http://bcz.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://nmg.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://cgm.fktsv.cn

JS:   console.assert(x > 0);
来源：http://eyo.andypj.xyz

TS:   console.assert(x > 0);
来源：http://awn.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://aka.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nye.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://srx.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://xrj.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://rnp.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://nlh.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pvd.ydzc1.top

JS:   e.message;  e.stack
来源：http://zsv.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zsp.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://unp.nanxinkj.top

Go:   err.Error()
来源：http://sil.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://xpn.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://ksr.yuxming.cn

[H09] 带错误码的异常
来源：http://gyw.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jcl.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kri.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nad.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oxv.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://awq.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ulb.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://shf.daxiang520.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vqk.yangfankeji.com

[H10] 资源自动释放
来源：http://dbu.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://euf.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lei.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hny.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xbe.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://chd.dashuyun.cn

Go:   defer f.Close()
来源：http://eir.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zkb.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lua.feifeiyinyue.top

================================================================================
来源：http://eqk.shzxlz.cn

I. 正则表达式
来源：http://qqh.dianchejie.cn

================================================================================
来源：http://oxc.jlsjyb.cn

[I01] 判断是否匹配
来源：http://dvx.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wrb.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://wjf.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://stk.316326.xyz

TS:   /\d+/.test(s)
来源：http://qfd.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://keq.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lbm.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://xga.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hkr.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://cli.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://bww.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ovs.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cuf.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://lvd.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ofj.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zbl.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://hra.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ddd.52xcode.cn

[I03] 提取捕获分组
来源：http://rma.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ebn.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://whj.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://foj.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://chv.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jyu.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xwl.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kif.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nzu.andypj.xyz

[I04] 正则替换
来源：http://oez.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eym.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tmq.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jsm.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://zee.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://eni.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nts.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://scl.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nql.shuidangran.top

[I05] 按正则拆分
来源：http://wkv.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wbf.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ewc.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://fbx.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://zsv.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://rem.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jbv.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://bnj.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kpk.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kue.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qfn.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rtk.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://luw.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yhv.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dft.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fwq.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rrh.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ppl.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://jna.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oaq.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://foc.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://txz.hnqzz.top

TS:   /error/gim
来源：http://mfv.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fja.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cgq.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://qgu.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rcr.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://ehi.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rek.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://krg.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xgn.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxi.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xuu.xylfe.cn


<!-- 参考信息 -->