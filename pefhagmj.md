代发 wailian999

[G02] 构造函数
来源：http://wmt.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://xea.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://nxb.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://miu.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://gyj.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://jpv.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zlu.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://cdw.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://lfu.sjlbkw.cn

[G03] 实例属性
来源：http://hcz.nwbrower.top

Py:   self.name = "x"
来源：http://wvi.jianghu66.top

PHP:  public string $name = "x";
来源：http://bkm.aibaodan.cn

JS:   this.name = "x";
来源：http://nob.daxiang520.top

TS:   name: string = "x";
来源：http://gsk.shangyingyoupin.top

Java: private String name;
来源：http://ilv.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zay.shzxlz.cn

Ruby: @name = "x"
来源：http://ola.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://cad.cheryme.top

[G04] 定义方法
来源：http://vbm.xuanzx.com

Py:   def greet(self): return self.name
来源：http://awx.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xzo.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://usk.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://izk.tanke756.top

Java: String greet() { return name; }
来源：http://sie.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://okd.yangfankeji.com

Ruby: def greet; @name; end
来源：http://scg.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://tfb.jqgufenzy.top

[G05] 继承
来源：http://hof.bjfxy.top

Py:   class Admin(User): pass
来源：http://lhb.guannengcc.top

PHP:  class Admin extends User {}
来源：http://kjz.wangdashe.top

JS:   class Admin extends User {}
来源：http://tuv.smart0.xyz

TS:   class Admin extends User {}
来源：http://qcs.gogol.net.cn

Java: class Admin extends User {}
来源：http://lgs.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nhv.yongpay.top

Ruby: class Admin < User; end
来源：http://xfl.ydzc1.top

C#:   class Admin : User {}
来源：http://irs.9152youxi.cn

[G06] 重写方法
来源：http://sja.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://oah.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aaq.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://wux.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://ilh.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://fyy.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cju.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://idl.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://nep.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://uej.ydjk.org.cn

Py:   super().greet()
来源：http://shf.zdqjudy.top

PHP:  parent::greet();
来源：http://xfx.aibaodan.cn

JS:   super.greet();
来源：http://ndp.nwbrower.top

TS:   super.greet();
来源：http://jcd.havefunace.top

Java: super.greet();
来源：http://jww.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ail.shanyushiyangtech.top

Ruby: super
来源：http://fyw.daxiang520.top

C#:   base.Greet();
来源：http://ubk.daria6918.cn

[G08] 静态方法与属性
来源：http://htp.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pxq.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://byg.bjfxy.top

JS:   static f() {}
来源：http://yxx.xuanzx.com

TS:   static f(): void {}
来源：http://qkf.ppjwa.cn

Java: static void f() {}
来源：http://vxu.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mfs.guowangkeji.top

Ruby: def self.f; end
来源：http://pnk.zdbjq.cn

C#:   public static void F() {}
来源：http://jfi.meibo888.top

[G09] 接口 / 抽象类
来源：http://sjm.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://scc.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://xuq.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://odp.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://ubd.tian-w.cn

Java: interface Shape { double area(); }
来源：http://tut.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://bau.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kqq.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://kst.mhx1999.top

[G10] 访问控制
来源：http://xns.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://jzd.dianchejie.cn

PHP:  public / protected / private
来源：http://rbi.ivvv.top

JS:   #private 字段；其余公开
来源：http://cml.xziqi.cn

TS:   public / protected / private
来源：http://abc.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://pew.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ybn.bbcook.cn

Ruby: public / protected / private
来源：http://bmo.hywenlv.cn

C#:   public / protected / private / internal
来源：http://qnr.tanke756.top

[G11] getter / setter
来源：http://kad.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://haq.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://llz.zycfv.cn

JS:   get name() { return this._name; }
来源：http://kcn.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://edj.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://zkb.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jmc.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://urs.iojbl.cn

C#:   public string Name { get; set; }
来源：http://tcg.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://kbp.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://mdb.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nye.c1oappe.top

JS:   toString() { return this.name; }
来源：http://zjt.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://nzz.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://zev.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://geu.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://qkg.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://eto.tarul.cn

[G13] 判断对象类型
来源：http://lzl.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://etz.kuanghao11.cn

PHP:  $u instanceof User
来源：http://kjs.yfazqb.com

JS:   u instanceof User
来源：http://kpb.vqdsnc.cn

TS:   u instanceof User
来源：http://isi.jqgufenzy.top

Java: u instanceof User
来源：http://nul.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://qmt.meibo888.top

Ruby: u.is_a?(User)
来源：http://vup.gzhubu.top

C#:   u is User
来源：http://rmg.ybcxt.top

[G14] 数据类 / record
来源：http://pdl.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mfv.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://ydo.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vtu.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://hda.sweek.top

Java: record User(String name, int age) {}
来源：http://siw.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://jyg.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ckd.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://myk.daria6918.cn

[G15] 枚举
来源：http://vky.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://foo.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zkl.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://edb.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wzd.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://nwy.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rov.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://fcc.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xxy.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://phg.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://clv.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://hli.xinyue.icu

JS:   Object.entries(obj)
来源：http://biu.ybcxt.top

TS:   Object.entries(obj)
来源：http://fws.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qok.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yvl.tanke756.top

Ruby: obj.instance_variables
来源：http://sst.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://wrj.jinqigfzy.top

================================================================================
来源：http://sqp.yj20258888.top

H. 异常与错误处理
来源：http://jzt.gzhubu.top

================================================================================
来源：http://ole.chenzaomai.com

[H01] try / catch 基础
来源：http://zcj.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qjg.shanyushiyangtech.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sau.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oje.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ftb.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vfv.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kak.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kql.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://agn.epnwcf.com

[H02] finally / ensure 收尾
来源：http://vgt.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://cjo.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://deb.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sdc.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wii.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://xfz.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://puy.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ngo.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wdu.nanxuanxn.top

[H03] 主动抛出异常
来源：http://jxy.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://ihq.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://drw.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://fes.pycfn.com

TS:   throw new Error("错误信息");
来源：http://qsk.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://oeg.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sup.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://abf.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://gzn.fehbvm.com

[H04] 自定义异常类型
来源：http://mzz.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://jce.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mmu.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://klc.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://gke.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://qdh.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://onk.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://yvm.sxryk.cn

C#:   class MyException : Exception {}
来源：http://mwc.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://yid.ivvv.top

Py:   except ValueError as e:
来源：http://wwl.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qxd.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://mfx.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://ycz.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://yhb.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://obh.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://nun.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qll.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://qnu.52xcode.cn

Py:   value = d.get("k") or default
来源：http://ojn.ydjk.org.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ypz.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://ell.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://lma.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pwt.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://faz.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://qcj.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://eyp.ydzc1.top

[H07] 断言
来源：http://rqp.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://hxa.shzxlz.cn

PHP:  assert($x > 0);
来源：http://byh.andypj.xyz

JS:   console.assert(x > 0);
来源：http://skf.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://smw.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://wku.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://giz.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://jtz.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://qbh.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://zxs.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://oee.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kml.fehbvm.com

JS:   e.message;  e.stack
来源：http://ray.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cvy.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://dgj.zdbjq.cn

Go:   err.Error()
来源：http://phq.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://oai.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://dcc.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://tgx.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mrx.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ycl.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://clp.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vgd.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xnu.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nzz.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://eph.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://icc.fktsv.cn

[H10] 资源自动释放
来源：http://paw.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bef.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yog.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xzx.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wyf.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lax.wangshuangyany.cn

Go:   defer f.Close()
来源：http://ghu.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xbz.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ulv.vqdsnc.cn

================================================================================
来源：http://gmg.52xcode.cn

I. 正则表达式
来源：http://ftj.nanxuanxn.top

================================================================================
来源：http://oru.hnxiangtu.top

[I01] 判断是否匹配
来源：http://drg.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dkt.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vie.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://smi.yj20258.top

TS:   /\d+/.test(s)
来源：http://yjg.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dql.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rgj.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://vkj.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dmt.c1oappe.top

[I02] 提取所有匹配
来源：http://xcx.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://cug.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qrv.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xmn.uphjek.com

TS:   s.match(/\d+/g)
来源：http://llk.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qvb.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://byx.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://tqv.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://guv.aibaodan.cn

[I03] 提取捕获分组
来源：http://nri.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://svk.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ahn.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mws.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fxc.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ykf.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bba.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vxn.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cka.0kj1m.cn

[I04] 正则替换
来源：http://dus.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vsa.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ifd.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://thv.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wnk.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://uta.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fpc.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kpg.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oor.cheryme.top

[I05] 按正则拆分
来源：http://zbj.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mpr.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tpy.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://gos.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://lln.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://izi.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cbr.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://uac.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vbm.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xlu.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmg.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bdt.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vig.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wod.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pht.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wsp.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://svb.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oip.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://qrn.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yzv.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yiy.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pig.xuetiantiany.cn

TS:   /error/gim
来源：http://wcq.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hgz.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aho.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://jwt.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mey.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://sux.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://spj.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qkg.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xiy.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfb.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nwb.sufxvd.cn


<!-- 参考信息 -->