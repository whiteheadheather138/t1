代发 wailian999

Java: class User {}
来源：http://car.jyoumei.cn

Go:   type User struct { Name string }
来源：http://tqz.ivvv.top

Ruby: class User; end
来源：http://olu.wangdashe.top

C#:   class User {}
来源：http://qff.zhixingplan.top

[G02] 构造函数
来源：http://hyv.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://cni.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://uzp.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://xvi.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://mgn.sweek.top

Java: User(String name) { this.name = name; }
来源：http://zzr.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xyt.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://fqg.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://bhv.chenzaomai.com

[G03] 实例属性
来源：http://lxw.zdqjudy.top

Py:   self.name = "x"
来源：http://kgt.zhengqikj.top

PHP:  public string $name = "x";
来源：http://lqm.c1oappe.top

JS:   this.name = "x";
来源：http://cci.shzxlz.cn

TS:   name: string = "x";
来源：http://gck.hcnkem.com

Java: private String name;
来源：http://wyt.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ird.tarul.cn

Ruby: @name = "x"
来源：http://fsn.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://mlf.zhixingplan.top

[G04] 定义方法
来源：http://ekz.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://dfx.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qym.bjfxy.top

JS:   greet() { return this.name; }
来源：http://sdp.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://rvi.yj20258.top

Java: String greet() { return name; }
来源：http://ign.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://mdx.shzxlz.cn

Ruby: def greet; @name; end
来源：http://hiz.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://spt.fktsv.cn

[G05] 继承
来源：http://rqc.snrcjt.cn

Py:   class Admin(User): pass
来源：http://ymb.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://jfr.meibo888.top

JS:   class Admin extends User {}
来源：http://ift.yongpay.top

TS:   class Admin extends User {}
来源：http://gum.daxiang520.top

Java: class Admin extends User {}
来源：http://nbp.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zuu.zdqjudy.top

Ruby: class Admin < User; end
来源：http://nyk.hcnkem.com

C#:   class Admin : User {}
来源：http://wmn.jinqigufen.top

[G06] 重写方法
来源：http://kya.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://jjg.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fxk.cashguo.top

JS:   greet() { return "admin"; }
来源：http://uxk.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://xyo.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://dee.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wqk.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://ogk.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://zjt.jlsjyb.cn

[G07] 调用父类方法
来源：http://etf.yvedp.cn

Py:   super().greet()
来源：http://cgc.zhongyouzk.top

PHP:  parent::greet();
来源：http://mry.shuidangran.top

JS:   super.greet();
来源：http://ime.fanxiaobao.xyz

TS:   super.greet();
来源：http://lff.dianchejie.cn

Java: super.greet();
来源：http://vvt.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ogg.dianchejie.cn

Ruby: super
来源：http://vvb.cdnleiting.top

C#:   base.Greet();
来源：http://rvh.zdbjq.cn

[G08] 静态方法与属性
来源：http://den.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lfc.jinqigufen.top

PHP:  public static function f() {}
来源：http://ced.316326.xyz

JS:   static f() {}
来源：http://qha.shuidangran.top

TS:   static f(): void {}
来源：http://uwa.cucudq.cn

Java: static void f() {}
来源：http://ilr.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ter.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://qhw.jianghu66.top

C#:   public static void F() {}
来源：http://avp.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://dmt.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://zej.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://pbt.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qsb.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://hwz.sweek.top

Java: interface Shape { double area(); }
来源：http://jwd.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://gij.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yvd.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://kck.ctjpmb.com

[G10] 访问控制
来源：http://igs.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://mfc.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://thn.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://peg.zhongyouzk.top

TS:   public / protected / private
来源：http://dbo.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://qgs.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qln.hesvh.cn

Ruby: public / protected / private
来源：http://kuo.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://zmx.yuanzhike.top

[G11] getter / setter
来源：http://zcj.yongpay.top

Py:   @property 与 @x.setter
来源：http://ccc.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qqj.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://xsp.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://hpm.yfazqb.com

Java: public String getName() { return name; }
来源：http://pex.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dqg.yangfankeji.com

Ruby: attr_accessor :name
来源：http://khf.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://svm.wangdashe.top

[G12] 对象转字符串
来源：http://btk.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://djl.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://evi.yj20258.top

JS:   toString() { return this.name; }
来源：http://mxi.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://zjm.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://hdg.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://oxp.ivvv.top

Ruby: def to_s; @name; end
来源：http://ghj.yj202588.top

C#:   public override string ToString() => Name;
来源：http://meo.cucudq.cn

[G13] 判断对象类型
来源：http://dab.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://mjv.pycfn.com

PHP:  $u instanceof User
来源：http://fby.zhongyouzk.top

JS:   u instanceof User
来源：http://duo.jinqigufen.top

TS:   u instanceof User
来源：http://spb.chenlongwang.top

Java: u instanceof User
来源：http://uct.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nuc.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://nvv.zhoulong.xyz

C#:   u is User
来源：http://mfk.yonumen.top

[G14] 数据类 / record
来源：http://waa.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ght.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://wqa.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gim.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://gph.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://sal.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://njt.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jxv.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://nlo.hongshengwenyu.top

[G15] 枚举
来源：http://quw.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xhu.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://isk.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ytv.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sio.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://glb.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ich.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://rms.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gyy.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://qpc.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bcd.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://shl.fengsongda.top

JS:   Object.entries(obj)
来源：http://yec.shuidangran.top

TS:   Object.entries(obj)
来源：http://qcz.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://igq.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kma.jinqigufen.top

Ruby: obj.instance_variables
来源：http://fkz.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://zci.gaohongyu789.top

================================================================================
来源：http://uvu.ydzc1.top

H. 异常与错误处理
来源：http://tdt.zhiwuduotai.top

================================================================================
来源：http://ziy.cheryme.top

[H01] try / catch 基础
来源：http://gwq.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dpu.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uhp.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dzw.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kdv.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ewh.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fwg.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://egc.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dck.jianghu66.top

[H02] finally / ensure 收尾
来源：http://snq.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://mjv.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vzz.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bek.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://spf.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nbj.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://och.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iza.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://znw.zhoulong.xyz

[H03] 主动抛出异常
来源：http://jdq.ydzc1.top

Py:   raise ValueError("错误信息")
来源：http://bgw.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://txw.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://uqo.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://lkt.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://doa.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://muk.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kwk.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bue.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://fwy.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://pov.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://wvn.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://lyp.hesvh.cn

TS:   class MyError extends Error {}
来源：http://utg.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://bhx.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cxo.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://aff.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://gko.52xcode.cn

[H05] 捕获特定类型
来源：http://ulj.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://wme.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uza.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://zsq.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://zpu.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://drc.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nij.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://tap.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zwx.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://zjh.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://ooj.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://jgl.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://uvp.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://uvn.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kam.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cws.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://obj.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://mmq.ivvv.top

[H07] 断言
来源：http://fkh.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://pag.nwbrower.top

PHP:  assert($x > 0);
来源：http://ebt.nwbrower.top

JS:   console.assert(x > 0);
来源：http://prh.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://bsy.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://zod.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mhs.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://urq.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://joc.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://zkh.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://ebr.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nja.aizwys.cn

JS:   e.message;  e.stack
来源：http://hgi.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://nnt.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zjb.nanxinkj.top

Go:   err.Error()
来源：http://nrq.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://bnk.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://mqk.iojbl.cn

[H09] 带错误码的异常
来源：http://rls.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://unp.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qkl.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ruy.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vtt.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wcs.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ocy.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://rth.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ejg.zhiwuduotai.top

[H10] 资源自动释放
来源：http://whs.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rhx.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qed.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fns.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vcn.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tez.chenzaomai.com

Go:   defer f.Close()
来源：http://rlm.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rrg.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ofe.tian-w.cn

================================================================================
来源：http://mgc.pengpengdd.cyou

I. 正则表达式
来源：http://udb.jinyuanbaomall.cn

================================================================================
来源：http://chf.iojbl.cn

[I01] 判断是否匹配
来源：http://smn.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hej.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://jae.meibo888.top

JS:   /\d+/.test(s)
来源：http://wmz.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://rux.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cec.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jgs.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://hob.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kld.sjlbkw.cn

[I02] 提取所有匹配
来源：http://ryb.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://tmt.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://miy.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zak.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://nhb.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xhd.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://unu.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://khq.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://swb.daxiang520.top

[I03] 提取捕获分组
来源：http://ego.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lxx.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://via.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eyc.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iil.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mma.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://osa.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ctk.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vyp.cqqwz.cn

[I04] 正则替换
来源：http://hzu.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xif.yanxiufei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lzy.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qmf.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://suu.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://noe.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://jim.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://eqt.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bkq.ivvv.top

[I05] 按正则拆分
来源：http://nvf.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gtu.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kws.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://dle.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://kfm.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://rlr.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qkc.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fjk.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://isd.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hdz.zhiwuduotai.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gqx.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fjd.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xcv.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ofj.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lqz.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wqb.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cdh.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cth.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://nex.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://msv.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ngb.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mbn.zhiwuduotai.top

TS:   /error/gim
来源：http://pez.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tpg.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mzd.sweek.top

Ruby: s.scan(/error/i)
来源：http://imp.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dep.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://yhh.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tka.yuxming.cn


<!-- 参考信息 -->