代发 wailian999

================================================================================
来源：http://jht.shanyushiyangtech.top

G. 面向对象
来源：http://fci.tarul.cn

================================================================================
来源：http://zba.hysaishi.cn

[G01] 定义类
来源：http://ydz.havefunace.top

Py:   class User: pass
来源：http://tzv.ctjpmb.com

PHP:  class User {}
来源：http://ffw.nwbrower.top

JS:   class User {}
来源：http://uyt.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://slq.cucudq.cn

Java: class User {}
来源：http://czs.hcnkem.com

Go:   type User struct { Name string }
来源：http://vsa.nanxuanxn.top

Ruby: class User; end
来源：http://qkj.ydjk.org.cn

C#:   class User {}
来源：http://vzf.cucudq.cn

[G02] 构造函数
来源：http://lmn.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://lem.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://vrx.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://agg.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://egt.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://bhz.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wya.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://pme.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://beu.jqgufenzy.top

[G03] 实例属性
来源：http://yhe.fengsongda.top

Py:   self.name = "x"
来源：http://sen.yueranfly.top

PHP:  public string $name = "x";
来源：http://bxb.hongshengwenyu.top

JS:   this.name = "x";
来源：http://wmz.chenjidiqi.icu

TS:   name: string = "x";
来源：http://cfk.hcnkem.com

Java: private String name;
来源：http://gyh.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://neo.yonumen.top

Ruby: @name = "x"
来源：http://fem.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://ieo.jinqigfzy.top

[G04] 定义方法
来源：http://vmj.bbcook.cn

Py:   def greet(self): return self.name
来源：http://kqd.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://szq.redwolf501.top

JS:   greet() { return this.name; }
来源：http://uvx.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://peq.ctjpmb.com

Java: String greet() { return name; }
来源：http://aoo.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wxp.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://fhx.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://vbh.bbcook.cn

[G05] 继承
来源：http://eop.hfpthk.cn

Py:   class Admin(User): pass
来源：http://kzc.yueranfly.top

PHP:  class Admin extends User {}
来源：http://eqm.fzhhl.top

JS:   class Admin extends User {}
来源：http://yps.aizwys.cn

TS:   class Admin extends User {}
来源：http://clb.jinqigfzy.top

Java: class Admin extends User {}
来源：http://bda.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ivi.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://lsk.tian-w.cn

C#:   class Admin : User {}
来源：http://ghm.sysykeji.top

[G06] 重写方法
来源：http://kht.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://epi.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ptj.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://hfu.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://dpv.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://uvi.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xip.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://zbf.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://azn.sysykeji.top

[G07] 调用父类方法
来源：http://nxd.jiagoushi.top

Py:   super().greet()
来源：http://vlg.jianghu66.top

PHP:  parent::greet();
来源：http://esj.epnwcf.com

JS:   super.greet();
来源：http://rkd.zhiwuduotai.top

TS:   super.greet();
来源：http://dnl.sxryk.cn

Java: super.greet();
来源：http://vhu.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nip.yangfankeji.com

Ruby: super
来源：http://qkj.hnqzz.top

C#:   base.Greet();
来源：http://bki.bbcook.cn

[G08] 静态方法与属性
来源：http://tps.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pqo.cheryme.top

PHP:  public static function f() {}
来源：http://eux.fehbvm.com

JS:   static f() {}
来源：http://bpl.jianghu66.top

TS:   static f(): void {}
来源：http://toh.iojbl.cn

Java: static void f() {}
来源：http://kgc.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iqg.yongpay.top

Ruby: def self.f; end
来源：http://efd.aizwys.cn

C#:   public static void F() {}
来源：http://raa.yj20258.top

[G09] 接口 / 抽象类
来源：http://zwh.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://ouf.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://esq.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hmx.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://nil.tarul.cn

Java: interface Shape { double area(); }
来源：http://cfw.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://rce.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pfe.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://qod.0kj1m.cn

[G10] 访问控制
来源：http://hhf.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://myk.zhongyouzk.top

PHP:  public / protected / private
来源：http://nqm.gzhubu.top

JS:   #private 字段；其余公开
来源：http://ibm.cheryme.top

TS:   public / protected / private
来源：http://yvt.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://gru.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lgd.gzhubu.top

Ruby: public / protected / private
来源：http://jqe.yvedp.cn

C#:   public / protected / private / internal
来源：http://jfn.vqdsnc.cn

[G11] getter / setter
来源：http://lss.xziqi.cn

Py:   @property 与 @x.setter
来源：http://mdr.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jck.daria6918.cn

JS:   get name() { return this._name; }
来源：http://jub.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://dkg.ppjwa.cn

Java: public String getName() { return name; }
来源：http://ifi.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fsk.sysykeji.top

Ruby: attr_accessor :name
来源：http://tpe.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://itb.dianchejie.cn

[G12] 对象转字符串
来源：http://hlw.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://qeo.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://euy.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://fnq.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://pln.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://gpm.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://wop.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://alk.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://wam.fehbvm.com

[G13] 判断对象类型
来源：http://hfm.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://ofq.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://dxu.zdqjudy.top

JS:   u instanceof User
来源：http://wcl.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://pvd.ydjk.org.cn

Java: u instanceof User
来源：http://pws.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lnw.ybcxt.top

Ruby: u.is_a?(User)
来源：http://heq.ctjpmb.com

C#:   u is User
来源：http://dfc.jianghu66.top

[G14] 数据类 / record
来源：http://gow.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ghs.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://zfm.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tun.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://req.jianghu66.top

Java: record User(String name, int age) {}
来源：http://fdi.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://lnp.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jwi.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://blc.sysykeji.top

[G15] 枚举
来源：http://pav.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lpc.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://uxe.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kys.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ovk.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://bmy.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fqj.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://aeh.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qav.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://fph.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yeu.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://qqp.hnxiangtu.top

JS:   Object.entries(obj)
来源：http://qtj.c1oappe.top

TS:   Object.entries(obj)
来源：http://ffi.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fth.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lhm.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://nsr.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://qaw.ywan-chungtsiang.top

================================================================================
来源：http://xxh.jyoumei.cn

H. 异常与错误处理
来源：http://tis.jqgfzy.top

================================================================================
来源：http://bju.birdmap.top

[H01] try / catch 基础
来源：http://nkd.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://njv.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kzh.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xbz.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vxh.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ieg.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dil.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wxm.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wzm.ivvv.top

[H02] finally / ensure 收尾
来源：http://boe.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://qcg.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nmh.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://muk.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jmu.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bhd.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dza.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vow.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eia.cheryme.top

[H03] 主动抛出异常
来源：http://bdg.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://reb.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cfu.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://vgr.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://wqn.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hgi.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nbm.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jpj.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://atp.sjlbkw.cn

[H04] 自定义异常类型
来源：http://gwq.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://khy.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://hvb.epnwcf.com

JS:   class MyError extends Error {}
来源：http://gws.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://iex.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://oum.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aim.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://msi.xuanzx.com

C#:   class MyException : Exception {}
来源：http://ifl.52xcode.cn

[H05] 捕获特定类型
来源：http://sdn.yangfankeji.com

Py:   except ValueError as e:
来源：http://fgk.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ynq.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://htt.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://aax.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://dos.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fdb.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://cfs.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eqt.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://ybe.sweek.top

Py:   value = d.get("k") or default
来源：http://dzr.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://duq.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://mau.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yys.shzxlz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ttq.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dyv.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://eas.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://jcb.daria6918.cn

[H07] 断言
来源：http://fjf.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://yfo.fktsv.cn

PHP:  assert($x > 0);
来源：http://xyk.yueranfly.top

JS:   console.assert(x > 0);
来源：http://wlv.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://xln.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://ifp.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rsy.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://jgq.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://adt.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://kuw.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://nhh.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zun.tianlin.xyz

JS:   e.message;  e.stack
来源：http://qsj.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ovu.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dgo.hfpthk.cn

Go:   err.Error()
来源：http://xoj.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://ogv.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://dqx.sweek.top

[H09] 带错误码的异常
来源：http://pio.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jwj.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ivt.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qnx.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tqy.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pok.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hgb.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://oti.ywan-chungtsiang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://czt.hammf.cn

[H10] 资源自动释放
来源：http://qhg.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://saf.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jpi.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ydw.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kpk.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xkh.9152youxi.cn

Go:   defer f.Close()
来源：http://ysh.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lvw.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jdw.zhaomingkeji.xyz

================================================================================
来源：http://oos.xuanzx.com

I. 正则表达式
来源：http://zjn.epnwcf.com

================================================================================
来源：http://mun.zdbjq.cn

[I01] 判断是否匹配
来源：http://qiv.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iai.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://iiz.yueranfly.top

JS:   /\d+/.test(s)
来源：http://uvw.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://lte.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uvh.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qkk.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://ykp.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gnc.bjfxy.top

[I02] 提取所有匹配
来源：http://vim.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://tww.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ent.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cdc.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://qin.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fja.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pzr.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://yms.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jqa.dianchejie.cn

[I03] 提取捕获分组
来源：http://qcl.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://irm.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vjt.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sto.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ogk.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jic.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://igl.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vah.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xyz.tarul.cn

[I04] 正则替换
来源：http://foq.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mth.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ffd.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://bec.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://dpz.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://sfb.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sxs.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iwu.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ymu.dashuyun.cn

[I05] 按正则拆分
来源：http://ltr.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gem.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gho.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://jsj.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://prz.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://rko.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wil.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://oit.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qdi.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nvp.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tso.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lug.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ukx.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hxa.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://azd.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ehn.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rrw.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://chk.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://tlo.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kwh.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hes.aibaodan.cn


<!-- 参考信息 -->