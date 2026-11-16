代发 wailian999

Java: class User {}
来源：http://ucq.fehbvm.com

Go:   type User struct { Name string }
来源：http://mzs.yuxming.cn

Ruby: class User; end
来源：http://fcr.zdqjudy.top

C#:   class User {}
来源：http://wct.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://mcu.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://pbs.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://kzy.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://six.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://mvb.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://och.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rkk.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://tbm.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://ocz.yj20258.top

[G03] 实例属性
来源：http://omr.sjlbkw.cn

Py:   self.name = "x"
来源：http://uuk.guowangkeji.top

PHP:  public string $name = "x";
来源：http://dvx.mhx1999.top

JS:   this.name = "x";
来源：http://hja.kuanghao11.cn

TS:   name: string = "x";
来源：http://rqy.kuanghao11.cn

Java: private String name;
来源：http://fcv.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dau.quarkkingdee.top

Ruby: @name = "x"
来源：http://frq.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://yet.zdbjq.cn

[G04] 定义方法
来源：http://dty.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://hap.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rux.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://ttd.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://yrz.zhoulong.xyz

Java: String greet() { return name; }
来源：http://ksf.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://gtx.svipenyu.cn

Ruby: def greet; @name; end
来源：http://ncx.zycfv.cn

C#:   public string Greet() => Name;
来源：http://shw.bbcook.cn

[G05] 继承
来源：http://sin.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://koe.xylfe.cn

PHP:  class Admin extends User {}
来源：http://tpb.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://fiu.zdqjudy.top

TS:   class Admin extends User {}
来源：http://hgz.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://kst.ppjwa.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ppr.havefunace.top

Ruby: class Admin < User; end
来源：http://gcw.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://ewa.nanxuanxn.top

[G06] 重写方法
来源：http://oxo.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://atq.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kfl.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://hji.cheryme.top

TS:   greet(): string { return "admin"; }
来源：http://aux.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://zxp.jinyuanbaomall.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zyb.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://kps.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://lxd.nwbrower.top

[G07] 调用父类方法
来源：http://oul.zhaomingkeji.xyz

Py:   super().greet()
来源：http://mhu.dianchejie.cn

PHP:  parent::greet();
来源：http://iyl.bjfxy.top

JS:   super.greet();
来源：http://hcu.meibo888.top

TS:   super.greet();
来源：http://muf.xinyue.icu

Java: super.greet();
来源：http://ngv.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xus.tianlin.xyz

Ruby: super
来源：http://ugy.havefunace.top

C#:   base.Greet();
来源：http://cxk.fehbvm.com

[G08] 静态方法与属性
来源：http://for.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kek.tian-w.cn

PHP:  public static function f() {}
来源：http://psz.hnqzz.top

JS:   static f() {}
来源：http://lrc.vqdsnc.cn

TS:   static f(): void {}
来源：http://lrm.shanyushiyangkeji.top

Java: static void f() {}
来源：http://ytz.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://beu.xuetiantiany.cn

Ruby: def self.f; end
来源：http://zou.xuanzx.com

C#:   public static void F() {}
来源：http://ifs.uphjek.com

[G09] 接口 / 抽象类
来源：http://qis.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://fic.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yuh.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://feg.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://pqg.bbcook.cn

Java: interface Shape { double area(); }
来源：http://bpu.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://uvv.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zzk.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://wba.fzhhl.top

[G10] 访问控制
来源：http://ptq.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://eeh.pycfn.com

PHP:  public / protected / private
来源：http://gne.havefunace.top

JS:   #private 字段；其余公开
来源：http://qrg.cheryme.top

TS:   public / protected / private
来源：http://bwa.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://ryr.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fxt.epnwcf.com

Ruby: public / protected / private
来源：http://zzb.jinqigufen.top

C#:   public / protected / private / internal
来源：http://ikw.yonumen.top

[G11] getter / setter
来源：http://dbd.ivvv.top

Py:   @property 与 @x.setter
来源：http://vli.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hje.yvedp.cn

JS:   get name() { return this._name; }
来源：http://zaz.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://asi.xylfe.cn

Java: public String getName() { return name; }
来源：http://epf.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://gvi.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://xjd.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://rlj.gzhubu.top

[G12] 对象转字符串
来源：http://fft.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://cem.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://uua.bjfxy.top

JS:   toString() { return this.name; }
来源：http://vlj.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://htk.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://lkj.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jov.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://hak.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://bwt.guowangkeji.top

[G13] 判断对象类型
来源：http://tzs.meibo888.top

Py:   isinstance(u, User)
来源：http://usm.sysykeji.top

PHP:  $u instanceof User
来源：http://xso.sufxvd.cn

JS:   u instanceof User
来源：http://ojs.9152youxi.cn

TS:   u instanceof User
来源：http://dft.zhengqikj.top

Java: u instanceof User
来源：http://sdn.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lss.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://wtm.gogol.net.cn

C#:   u is User
来源：http://nla.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://sxn.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hsz.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://orb.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://baf.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://ach.xylfe.cn

Java: record User(String name, int age) {}
来源：http://lsp.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://xly.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://poa.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://hgo.hywenlv.cn

[G15] 枚举
来源：http://rbs.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cyk.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://skh.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xdz.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vyq.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://exm.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pya.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://umf.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xub.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://xqo.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mmb.yonumen.top

PHP:  get_object_vars($obj);
来源：http://fdw.bbcook.cn

JS:   Object.entries(obj)
来源：http://ewv.andypj.xyz

TS:   Object.entries(obj)
来源：http://cxm.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dan.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://qnw.gotoacloud.top

Ruby: obj.instance_variables
来源：http://rao.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://zjk.fehbvm.com

================================================================================
来源：http://jyu.yvedp.cn

H. 异常与错误处理
来源：http://rjq.jinyuanbaomall.cn

================================================================================
来源：http://zqo.shzxlz.cn

[H01] try / catch 基础
来源：http://nfi.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tcr.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://axt.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nya.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ejb.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nuh.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ddo.cqqwz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://owh.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mum.guannengcc.top

[H02] finally / ensure 收尾
来源：http://kve.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://spi.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://csk.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gnv.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sst.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://bix.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ekg.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ksj.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xaf.pycfn.com

[H03] 主动抛出异常
来源：http://vgl.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://jnm.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oid.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://tdg.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://vni.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://tad.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sfx.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jtm.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://qni.fehbvm.com

[H04] 自定义异常类型
来源：http://wpm.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://ciz.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://sgc.xuanzx.com

JS:   class MyError extends Error {}
来源：http://ucs.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://zxb.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://sfb.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qsx.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://vef.meibo888.top

C#:   class MyException : Exception {}
来源：http://aqu.svipenyu.cn

[H05] 捕获特定类型
来源：http://zqv.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://qjz.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ucn.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://rvk.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://tik.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://ecq.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zdo.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://lii.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xpx.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://qaq.sweek.top

Py:   value = d.get("k") or default
来源：http://mpv.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://coc.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://ubw.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://tkw.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hib.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kxt.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://sck.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://klb.zhijiandao.cn

[H07] 断言
来源：http://szh.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://acx.xziqi.cn

PHP:  assert($x > 0);
来源：http://zsv.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://olv.mhx1999.top

TS:   console.assert(x > 0);
来源：http://kju.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://pbj.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gnb.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://djv.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://hsu.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://jpt.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://vqf.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kdx.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://tmt.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rfo.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rzv.jyoumei.cn

Go:   err.Error()
来源：http://gmr.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://jmg.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://tto.hcnkem.com

[H09] 带错误码的异常
来源：http://pgz.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qdi.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iid.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rpy.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dfa.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dro.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rzm.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://qbl.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gob.zycfv.cn

[H10] 资源自动释放
来源：http://zou.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jhk.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tjw.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://chh.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wda.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kgi.sxryk.cn

Go:   defer f.Close()
来源：http://vvc.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iwm.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hcp.haohaochexian.top

================================================================================
来源：http://qvd.zhiwuduotai.top

I. 正则表达式
来源：http://yhu.fengsongda.top

================================================================================
来源：http://eqd.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://nne.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zmd.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fjw.mhx1999.top

JS:   /\d+/.test(s)
来源：http://uqz.jianghu66.top

TS:   /\d+/.test(s)
来源：http://iqo.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ecl.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ogq.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://wkv.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nil.sjlbkw.cn

[I02] 提取所有匹配
来源：http://fth.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://jxi.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ylz.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nqy.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://vis.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lug.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lcp.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://pbv.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bvl.cucudq.cn

[I03] 提取捕获分组
来源：http://saf.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yji.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gtd.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jtk.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zgz.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oow.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://psv.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cvr.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zyu.ppjwa.cn

[I04] 正则替换
来源：http://wnu.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uqd.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oae.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ejn.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://ydl.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yly.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hxj.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hns.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://krx.gogol.net.cn

[I05] 按正则拆分
来源：http://eui.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ywq.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gtv.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://jnd.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://ujo.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://hce.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vxi.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://yrh.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ylz.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cdh.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://agf.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pop.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iwt.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://imq.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mml.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fea.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pmu.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vde.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://hxn.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hyu.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rdl.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mum.ywan-chungtsiang.top

TS:   /error/gim
来源：http://iyj.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fkl.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rdn.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://xll.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://usl.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://zfp.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gkg.zhiwuduotai.top


<!-- 参考信息 -->