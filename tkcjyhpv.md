代发 wailian999

================================================================================
来源：http://naw.tarul.cn

G. 面向对象
来源：http://isn.epnwcf.com

================================================================================
来源：http://fhn.yj20258.top

[G01] 定义类
来源：http://ehd.shanyushiyangkeji.top

Py:   class User: pass
来源：http://jwq.sweek.top

PHP:  class User {}
来源：http://gcz.daria6918.cn

JS:   class User {}
来源：http://tla.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://azn.sjlbkw.cn

Java: class User {}
来源：http://uji.yj20258888.top

Go:   type User struct { Name string }
来源：http://jrx.pycfn.com

Ruby: class User; end
来源：http://ooy.yfazqb.com

C#:   class User {}
来源：http://dmt.dianchejie.cn

[G02] 构造函数
来源：http://sbp.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://woa.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://hpt.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://oke.sweek.top

TS:   constructor(public name: string) {}
来源：http://bwu.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://jjy.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bow.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://iea.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://zwp.ydjk.org.cn

[G03] 实例属性
来源：http://vrg.cqqwz.cn

Py:   self.name = "x"
来源：http://vqo.yongpay.top

PHP:  public string $name = "x";
来源：http://pww.fktsv.cn

JS:   this.name = "x";
来源：http://zkl.yj20258.top

TS:   name: string = "x";
来源：http://ffe.cqqwz.cn

Java: private String name;
来源：http://lqh.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://txx.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://xtp.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://dqk.guannengcc.top

[G04] 定义方法
来源：http://rwe.fengsongda.top

Py:   def greet(self): return self.name
来源：http://wtf.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pce.xuanzx.com

JS:   greet() { return this.name; }
来源：http://btq.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://rju.tanke756.top

Java: String greet() { return name; }
来源：http://kuc.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://isr.cdnleiting.top

Ruby: def greet; @name; end
来源：http://bxg.fehbvm.com

C#:   public string Greet() => Name;
来源：http://cwa.shanyushiyangtech.top

[G05] 继承
来源：http://eak.hywenlv.cn

Py:   class Admin(User): pass
来源：http://tok.gzhubu.top

PHP:  class Admin extends User {}
来源：http://way.daxiang520.top

JS:   class Admin extends User {}
来源：http://wdi.fengsongda.top

TS:   class Admin extends User {}
来源：http://ezq.cheryme.top

Java: class Admin extends User {}
来源：http://tpk.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mxd.epnwcf.com

Ruby: class Admin < User; end
来源：http://gzl.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://qkx.yuanzhike.top

[G06] 重写方法
来源：http://lkh.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://ehv.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://djv.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://bfd.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://svk.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://bgm.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vax.316326.xyz

Ruby: def greet; "admin"; end
来源：http://uin.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://eif.fehbvm.com

[G07] 调用父类方法
来源：http://kee.9152youxi.cn

Py:   super().greet()
来源：http://tta.yonumen.top

PHP:  parent::greet();
来源：http://rro.zhoulong.xyz

JS:   super.greet();
来源：http://jau.yanxiufei.cn

TS:   super.greet();
来源：http://imh.hnxiangtu.top

Java: super.greet();
来源：http://hfy.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uyn.fzhhl.top

Ruby: super
来源：http://yoy.bjfxy.top

C#:   base.Greet();
来源：http://epi.jqgfzy.top

[G08] 静态方法与属性
来源：http://uot.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xnz.jqgfzy.top

PHP:  public static function f() {}
来源：http://nlq.hfpthk.cn

JS:   static f() {}
来源：http://yxg.birdmap.top

TS:   static f(): void {}
来源：http://wkx.guowangkeji.top

Java: static void f() {}
来源：http://mop.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ryy.yonumen.top

Ruby: def self.f; end
来源：http://bql.xuetiantiany.cn

C#:   public static void F() {}
来源：http://izs.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://euy.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://teh.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nux.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://efn.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://nvv.sxryk.cn

Java: interface Shape { double area(); }
来源：http://vqh.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://hnq.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mvk.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://qml.wangdashe.top

[G10] 访问控制
来源：http://kkb.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://gnr.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://jvn.bbcook.cn

JS:   #private 字段；其余公开
来源：http://avi.zhiwuduotai.top

TS:   public / protected / private
来源：http://abp.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://rhc.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dkz.xziqi.cn

Ruby: public / protected / private
来源：http://rgj.daxiang520.top

C#:   public / protected / private / internal
来源：http://zup.jiagoushi.top

[G11] getter / setter
来源：http://oeg.yj202588.top

Py:   @property 与 @x.setter
来源：http://xfr.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pjt.zdbjq.cn

JS:   get name() { return this._name; }
来源：http://knz.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://vml.hysaishi.cn

Java: public String getName() { return name; }
来源：http://wjr.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://bil.gzhubu.top

Ruby: attr_accessor :name
来源：http://ubp.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://oaq.gzhubu.top

[G12] 对象转字符串
来源：http://eek.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://kvg.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://plc.xylfe.cn

JS:   toString() { return this.name; }
来源：http://lae.pengpengdd.cyou

TS:   toString(): string { return this.name; }
来源：http://vbw.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://muc.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://djr.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://vnz.havefunace.top

C#:   public override string ToString() => Name;
来源：http://mst.vqdsnc.cn

[G13] 判断对象类型
来源：http://brm.zhixingplan.top

Py:   isinstance(u, User)
来源：http://tkf.xuanzx.com

PHP:  $u instanceof User
来源：http://vre.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://jll.xziqi.cn

TS:   u instanceof User
来源：http://okh.shuidangran.top

Java: u instanceof User
来源：http://cns.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://joa.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://eqb.ehwqpu.com

C#:   u is User
来源：http://nzc.yfazqb.com

[G14] 数据类 / record
来源：http://zyd.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qek.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://fuw.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://aku.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://qiw.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://drt.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://bye.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dyd.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://jtb.sxryk.cn

[G15] 枚举
来源：http://rpd.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rhg.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://opp.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fgc.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kxy.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://ylv.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lat.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://mbj.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://usg.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://fmf.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://azm.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://tqb.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://foq.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://icq.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qkx.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kmu.daxiang520.top

Ruby: obj.instance_variables
来源：http://xjt.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://vji.fehbvm.com

================================================================================
来源：http://ezp.xinyue.icu

H. 异常与错误处理
来源：http://hsm.zdbjq.cn

================================================================================
来源：http://pzf.svipenyu.cn

[H01] try / catch 基础
来源：http://vjh.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bhl.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jyx.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vbi.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oaa.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vxl.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yiv.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rmz.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dzd.sweek.top

[H02] finally / ensure 收尾
来源：http://frd.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://isp.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kdu.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fpk.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://jsa.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://yin.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qbh.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hoy.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yvu.fzhhl.top

[H03] 主动抛出异常
来源：http://hhw.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://roz.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pfk.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://wed.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://iyi.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://svu.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tcr.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fqd.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://yhs.yangfankeji.com

[H04] 自定义异常类型
来源：http://cqa.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://fyx.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://lob.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://snq.cucudq.cn

TS:   class MyError extends Error {}
来源：http://gje.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://abt.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ymv.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://tnn.smart0.xyz

C#:   class MyException : Exception {}
来源：http://xeq.0kj1m.cn

[H05] 捕获特定类型
来源：http://qup.bjfxy.top

Py:   except ValueError as e:
来源：http://dhv.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xfl.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://mol.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://vfa.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://dpg.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kcu.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://jkq.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tcq.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://ziq.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://knv.bjfxy.top

PHP:  $v = $d["k"] ?? null;
来源：http://foc.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eau.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://vak.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gjp.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jxr.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://uqc.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://azb.aibaodan.cn

[H07] 断言
来源：http://nxi.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://ikk.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://hbg.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://jsx.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://joo.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://hbs.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ins.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://ayn.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://tmb.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://bzm.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://fjz.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gis.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://uai.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bze.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bnd.chenlongwang.top

Go:   err.Error()
来源：http://oix.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://sds.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://bew.hfpthk.cn

[H09] 带错误码的异常
来源：http://nod.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yax.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gim.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dlw.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pll.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://abe.aizwys.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ogu.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://kqt.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uvq.yuxming.cn

[H10] 资源自动释放
来源：http://jnh.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wdl.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ndx.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jjr.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cmc.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hte.fktsv.cn

Go:   defer f.Close()
来源：http://shq.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jap.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dzr.c1oappe.top

================================================================================
来源：http://ual.hfpthk.cn

I. 正则表达式
来源：http://hfp.hcnkem.com

================================================================================
来源：http://znq.ivvv.top

[I01] 判断是否匹配
来源：http://kzd.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sjg.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://svw.jianghu66.top

JS:   /\d+/.test(s)
来源：http://map.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://opw.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zqg.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eue.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://vwy.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rcq.wangdashe.top

[I02] 提取所有匹配
来源：http://myw.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://dwi.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fzw.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hqs.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://pdu.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mct.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mea.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://eyj.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aub.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://gje.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://icl.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tea.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ckt.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xvi.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mzh.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wrc.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hfo.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mqi.hesvh.cn

[I04] 正则替换
来源：http://bzo.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nze.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sjx.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://vdh.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://yxd.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://hij.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rwb.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://xyr.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jnq.vqdsnc.cn

[I05] 按正则拆分
来源：http://ebe.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pyl.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lxt.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://wof.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://zut.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://bdu.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jxf.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://cbt.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pyb.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ytx.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dmu.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dkv.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yhs.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ueq.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oov.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://saf.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkx.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bfu.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://pul.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zwb.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lng.kuanghao11.cn


<!-- 参考信息 -->