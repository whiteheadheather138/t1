代发 wailian999

================================================================================
来源：http://eyw.jiagoushi.top

G. 面向对象
来源：http://rwt.uphjek.com

================================================================================
来源：http://qri.xuetiantiany.cn

[G01] 定义类
来源：http://dux.birdmap.top

Py:   class User: pass
来源：http://oqp.hywenlv.cn

PHP:  class User {}
来源：http://ndv.shangyingyoupin.top

JS:   class User {}
来源：http://lnr.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://kfs.chenlongwang.top

Java: class User {}
来源：http://wsi.gzhubu.top

Go:   type User struct { Name string }
来源：http://mma.ivvv.top

Ruby: class User; end
来源：http://ddr.316326.xyz

C#:   class User {}
来源：http://nxo.daxiang520.top

[G02] 构造函数
来源：http://pjo.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://asd.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://lft.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://exy.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://hgc.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://zui.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qgj.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://hrw.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://opg.ehwqpu.com

[G03] 实例属性
来源：http://fvv.jinqigfzy.top

Py:   self.name = "x"
来源：http://xqw.fktsv.cn

PHP:  public string $name = "x";
来源：http://mcy.jiagoushi.top

JS:   this.name = "x";
来源：http://dtn.daxiang520.top

TS:   name: string = "x";
来源：http://ozd.yongpay.top

Java: private String name;
来源：http://qas.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pog.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://vld.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://ray.fanxiaobao.xyz

[G04] 定义方法
来源：http://txm.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://xxk.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uta.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://wwt.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://gcj.ctjpmb.com

Java: String greet() { return name; }
来源：http://imf.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tky.fengsongda.top

Ruby: def greet; @name; end
来源：http://dkm.tian-w.cn

C#:   public string Greet() => Name;
来源：http://nqu.aizwys.cn

[G05] 继承
来源：http://oav.xziqi.cn

Py:   class Admin(User): pass
来源：http://kwe.tanke756.top

PHP:  class Admin extends User {}
来源：http://oxe.hesvh.cn

JS:   class Admin extends User {}
来源：http://zag.gzhubu.top

TS:   class Admin extends User {}
来源：http://mff.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://zax.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://amu.bjfxy.top

Ruby: class Admin < User; end
来源：http://nbc.zdbjq.cn

C#:   class Admin : User {}
来源：http://pbp.yueranfly.top

[G06] 重写方法
来源：http://taa.hammf.cn

Py:   def greet(self): return "admin"
来源：http://nrt.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wwb.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://vwx.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://oha.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://isr.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://onr.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://vgk.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://qfr.9152youxi.cn

[G07] 调用父类方法
来源：http://heq.jinyuanbaomall.cn

Py:   super().greet()
来源：http://fqa.svipenyu.cn

PHP:  parent::greet();
来源：http://iyg.feifeiyinyue.top

JS:   super.greet();
来源：http://vem.yangfankeji.com

TS:   super.greet();
来源：http://vnc.sjlbkw.cn

Java: super.greet();
来源：http://gfk.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fdi.nwbrower.top

Ruby: super
来源：http://eun.kuanghao11.cn

C#:   base.Greet();
来源：http://njf.vqdsnc.cn

[G08] 静态方法与属性
来源：http://nqb.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kxh.tianlin.xyz

PHP:  public static function f() {}
来源：http://vmw.gzhubu.top

JS:   static f() {}
来源：http://csm.sufxvd.cn

TS:   static f(): void {}
来源：http://pke.pycfn.com

Java: static void f() {}
来源：http://yeg.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://srz.yfazqb.com

Ruby: def self.f; end
来源：http://xvh.52xcode.cn

C#:   public static void F() {}
来源：http://txn.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://etv.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://xbq.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dpg.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fmp.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://npx.gzhubu.top

Java: interface Shape { double area(); }
来源：http://auu.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://bgs.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://prs.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://uhp.52xcode.cn

[G10] 访问控制
来源：http://spw.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://dza.zhengqikj.top

PHP:  public / protected / private
来源：http://ayg.tarul.cn

JS:   #private 字段；其余公开
来源：http://ycx.yj20258.top

TS:   public / protected / private
来源：http://pfu.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://zda.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://new.hcnkem.com

Ruby: public / protected / private
来源：http://zax.zycfv.cn

C#:   public / protected / private / internal
来源：http://pgj.c1oappe.top

[G11] getter / setter
来源：http://wod.c1oappe.top

Py:   @property 与 @x.setter
来源：http://xhz.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cbh.yfazqb.com

JS:   get name() { return this._name; }
来源：http://onk.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://rsi.yj20258888.top

Java: public String getName() { return name; }
来源：http://qej.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bnz.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://rxp.daria6918.cn

C#:   public string Name { get; set; }
来源：http://suo.cucudq.cn

[G12] 对象转字符串
来源：http://eds.pycfn.com

Py:   def __str__(self): return self.name
来源：http://opd.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ltb.yuxming.cn

JS:   toString() { return this.name; }
来源：http://mxo.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://xkf.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://llr.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://wev.meibo888.top

Ruby: def to_s; @name; end
来源：http://lkr.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://kxm.0kj1m.cn

[G13] 判断对象类型
来源：http://wye.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://dyq.mhx1999.top

PHP:  $u instanceof User
来源：http://edz.shuidangran.top

JS:   u instanceof User
来源：http://uag.haohaochexian.top

TS:   u instanceof User
来源：http://ead.yj20258.top

Java: u instanceof User
来源：http://egf.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xqr.cucudq.cn

Ruby: u.is_a?(User)
来源：http://uva.52xcode.cn

C#:   u is User
来源：http://sqd.yj202588.top

[G14] 数据类 / record
来源：http://hwr.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sbi.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://kxo.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hhz.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://izz.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://eak.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://vse.jianghu66.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bzg.yonumen.top

C#:   record User(string Name, int Age);
来源：http://qpo.yj202588.top

[G15] 枚举
来源：http://lsj.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://igi.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rvg.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qff.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uwg.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://mgd.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jif.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://uxs.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rmy.yj202588.top

[G16] 对象转数组 / 字典
来源：http://mum.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ylm.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://uch.cheryme.top

JS:   Object.entries(obj)
来源：http://nrz.yonumen.top

TS:   Object.entries(obj)
来源：http://awv.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://phb.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vpk.gotoacloud.top

Ruby: obj.instance_variables
来源：http://grt.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://wcu.zhixingplan.top

================================================================================
来源：http://loj.zhiwuduotai.top

H. 异常与错误处理
来源：http://lse.wangshuangyany.cn

================================================================================
来源：http://aln.chenlongwang.top

[H01] try / catch 基础
来源：http://uxy.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hxg.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dtp.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jdr.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lvr.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mlz.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ygj.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tdi.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dro.yonumen.top

[H02] finally / ensure 收尾
来源：http://ngz.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://gxs.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qoj.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fta.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://jjw.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mdl.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gdr.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hnn.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hnh.sufxvd.cn

[H03] 主动抛出异常
来源：http://lcg.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://nsp.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qot.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://lyu.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://mxm.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cwg.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kut.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ooj.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://gkr.jqgfzy.top

[H04] 自定义异常类型
来源：http://dpc.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://nis.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://mhg.cucudq.cn

JS:   class MyError extends Error {}
来源：http://clg.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://iwg.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://cjq.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ick.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://dvx.shuidangran.top

C#:   class MyException : Exception {}
来源：http://edm.hesvh.cn

[H05] 捕获特定类型
来源：http://zej.cqqwz.cn

Py:   except ValueError as e:
来源：http://kro.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sia.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://lzf.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://ism.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://nyz.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qat.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://qbl.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hdi.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://piv.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://kcu.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://tdn.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://eag.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gyu.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dty.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://cls.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://wxa.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://pfx.yj202588.top

[H07] 断言
来源：http://ika.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://nic.zhixingplan.top

PHP:  assert($x > 0);
来源：http://gfh.cheryme.top

JS:   console.assert(x > 0);
来源：http://qij.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://dvy.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://sso.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xnc.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://sbn.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://mog.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://qcw.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://vao.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mxe.gogol.net.cn

JS:   e.message;  e.stack
来源：http://rzg.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uby.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gdu.zdqjudy.top

Go:   err.Error()
来源：http://hxz.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://idl.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://jvt.jianghu66.top

[H09] 带错误码的异常
来源：http://png.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qjt.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://idx.snrcjt.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://efa.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iii.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kao.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lve.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://mjt.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xsc.yj20258888.top

[H10] 资源自动释放
来源：http://mjr.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iak.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kza.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rla.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fvd.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ugl.yj20258.top

Go:   defer f.Close()
来源：http://mvv.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fis.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yja.xziqi.cn

================================================================================
来源：http://pxe.redwolf501.top

I. 正则表达式
来源：http://aqi.jinqigufen.top

================================================================================
来源：http://xhi.ctjpmb.com

[I01] 判断是否匹配
来源：http://pjz.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bno.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://anz.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://ghe.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://esl.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dcv.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bcw.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://ljb.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pjf.uphjek.com

[I02] 提取所有匹配
来源：http://imb.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://hpt.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wix.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zsl.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://ckb.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rvi.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://imc.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://nnc.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bzb.fktsv.cn

[I03] 提取捕获分组
来源：http://dny.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ozf.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vkn.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qeh.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oct.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ywk.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gwg.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fvq.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ssk.jinqigufen.top

[I04] 正则替换
来源：http://avn.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gdy.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uzh.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ffa.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dqt.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://olw.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dzp.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://quw.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fyz.shangyingyoupin.top

[I05] 按正则拆分
来源：http://igi.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://njw.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lsm.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://ksh.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://kto.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://ywu.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yta.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://fgj.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nym.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xzc.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uar.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vza.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jaf.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnw.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ogg.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ayg.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lwk.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ava.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://bii.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pod.tianlin.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fxi.shzxlz.cn


<!-- 参考信息 -->