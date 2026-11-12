代发 wailian999

[G02] 构造函数
来源：http://gzx.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://xbf.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://zgx.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://hud.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://sex.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://cch.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://txd.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://npr.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://pee.gotoacloud.top

[G03] 实例属性
来源：http://ohg.yj20258.top

Py:   self.name = "x"
来源：http://pfx.tianlin.xyz

PHP:  public string $name = "x";
来源：http://gje.ivvv.top

JS:   this.name = "x";
来源：http://gux.sysykeji.top

TS:   name: string = "x";
来源：http://thr.zhiwuduotai.top

Java: private String name;
来源：http://umb.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cyg.smart0.xyz

Ruby: @name = "x"
来源：http://rfm.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://tmx.tian-w.cn

[G04] 定义方法
来源：http://zsu.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://usq.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hpm.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://ucf.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://ebh.zhixingplan.top

Java: String greet() { return name; }
来源：http://sdt.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gmd.xziqi.cn

Ruby: def greet; @name; end
来源：http://jhb.havefunace.top

C#:   public string Greet() => Name;
来源：http://dno.yangfankeji.com

[G05] 继承
来源：http://qut.guannengcc.top

Py:   class Admin(User): pass
来源：http://ueu.aizwys.cn

PHP:  class Admin extends User {}
来源：http://pti.xinyue.icu

JS:   class Admin extends User {}
来源：http://ize.ctjpmb.com

TS:   class Admin extends User {}
来源：http://xfv.ydjk.org.cn

Java: class Admin extends User {}
来源：http://zfc.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yhr.yfazqb.com

Ruby: class Admin < User; end
来源：http://vzn.tarul.cn

C#:   class Admin : User {}
来源：http://ohc.jianghu66.top

[G06] 重写方法
来源：http://nza.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://zsl.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qhw.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://crt.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://wce.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://soe.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fgq.birdmap.top

Ruby: def greet; "admin"; end
来源：http://thp.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://mxp.zdbjq.cn

[G07] 调用父类方法
来源：http://wxv.yj20258888.top

Py:   super().greet()
来源：http://pkb.havefunace.top

PHP:  parent::greet();
来源：http://pdy.bjfxy.top

JS:   super.greet();
来源：http://yvn.zhiwuduotai.top

TS:   super.greet();
来源：http://ism.gotoacloud.top

Java: super.greet();
来源：http://lyr.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wtr.shanyushiyangtech.top

Ruby: super
来源：http://thf.chenzaomai.com

C#:   base.Greet();
来源：http://pyj.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://lgw.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://glc.ydzc1.top

PHP:  public static function f() {}
来源：http://erf.bbcook.cn

JS:   static f() {}
来源：http://yze.dashuyun.cn

TS:   static f(): void {}
来源：http://jqg.tarul.cn

Java: static void f() {}
来源：http://cab.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://xam.mhx1999.top

Ruby: def self.f; end
来源：http://wdo.hywenlv.cn

C#:   public static void F() {}
来源：http://pzh.ivvv.top

[G09] 接口 / 抽象类
来源：http://aol.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://niy.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://ixn.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pcx.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://dtt.yj20258888.top

Java: interface Shape { double area(); }
来源：http://gkm.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://rdh.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jan.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://vlj.yuxming.cn

[G10] 访问控制
来源：http://jwo.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://suf.sxryk.cn

PHP:  public / protected / private
来源：http://cfi.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://mkn.yangfankeji.com

TS:   public / protected / private
来源：http://jgl.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://gtg.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bfl.yongpay.top

Ruby: public / protected / private
来源：http://tdj.cheryme.top

C#:   public / protected / private / internal
来源：http://syz.dashuyun.cn

[G11] getter / setter
来源：http://pqq.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://vps.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tux.c1oappe.top

JS:   get name() { return this._name; }
来源：http://gsb.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://nky.fktsv.cn

Java: public String getName() { return name; }
来源：http://faw.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rno.gzhubu.top

Ruby: attr_accessor :name
来源：http://vmi.hesvh.cn

C#:   public string Name { get; set; }
来源：http://sbd.ehwqpu.com

[G12] 对象转字符串
来源：http://owz.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://ccu.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://duk.daria6918.cn

JS:   toString() { return this.name; }
来源：http://uxl.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://smf.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://vey.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qly.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://ros.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://ldf.yj20258.top

[G13] 判断对象类型
来源：http://eui.chenzaomai.com

Py:   isinstance(u, User)
来源：http://wwc.guannengcc.top

PHP:  $u instanceof User
来源：http://cbv.yuxming.cn

JS:   u instanceof User
来源：http://rvo.cucudq.cn

TS:   u instanceof User
来源：http://vqm.hcnkem.com

Java: u instanceof User
来源：http://wjd.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oga.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://xbk.daxiang520.top

C#:   u is User
来源：http://ikb.fktsv.cn

[G14] 数据类 / record
来源：http://jko.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jfe.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://qen.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://sgy.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://gtc.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://zao.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://gbj.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lzi.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://kyk.shangyingyoupin.top

[G15] 枚举
来源：http://ngp.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://brt.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xpy.andypj.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://npx.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ltb.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://lfm.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pjg.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://wkq.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://afk.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://bxt.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pgl.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://xoc.tanke756.top

JS:   Object.entries(obj)
来源：http://gqk.ppjwa.cn

TS:   Object.entries(obj)
来源：http://yee.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xek.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jfb.pycfn.com

Ruby: obj.instance_variables
来源：http://ggd.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://lto.sjlbkw.cn

================================================================================
来源：http://pdf.yfazqb.com

H. 异常与错误处理
来源：http://yeo.tianlin.xyz

================================================================================
来源：http://tbd.jianghu66.top

[H01] try / catch 基础
来源：http://pcv.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fmy.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://why.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xgf.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dxm.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://svh.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tcs.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mvb.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qqj.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://myb.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://fek.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fhs.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ujq.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qhj.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lrz.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zzg.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rdx.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dcf.kuanghao11.cn

[H03] 主动抛出异常
来源：http://zxs.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://tcx.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oeb.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://xsp.chenjidiqi.icu

TS:   throw new Error("错误信息");
来源：http://scn.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://anf.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hsg.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jtx.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://gvu.xziqi.cn

[H04] 自定义异常类型
来源：http://ers.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://nwu.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sju.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://ynp.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://lxd.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://jin.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mwd.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://qlf.mhx1999.top

C#:   class MyException : Exception {}
来源：http://dxj.cqqwz.cn

[H05] 捕获特定类型
来源：http://nwr.hywenlv.cn

Py:   except ValueError as e:
来源：http://lky.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ehm.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://kvo.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://kmv.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://rwk.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zjr.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://ifo.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jrx.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://dzh.birdmap.top

Py:   value = d.get("k") or default
来源：http://lap.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://qoh.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://zlt.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://eos.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yqo.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://kpm.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://vyo.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://bwj.birdmap.top

[H07] 断言
来源：http://jzr.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://ugq.hammf.cn

PHP:  assert($x > 0);
来源：http://qyb.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://hxr.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://xio.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://bxo.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://peq.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://xpg.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://jdr.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://xmg.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://plb.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://poe.yongpay.top

JS:   e.message;  e.stack
来源：http://xig.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://zda.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eac.birdmap.top

Go:   err.Error()
来源：http://sia.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://atk.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://atb.svipenyu.cn

[H09] 带错误码的异常
来源：http://gbz.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yqj.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://bma.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qnh.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mzu.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ijh.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://urb.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://ofv.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://beg.tian-w.cn

[H10] 资源自动释放
来源：http://sgg.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://usm.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pbd.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pig.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nxb.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nnw.jyoumei.cn

Go:   defer f.Close()
来源：http://hfz.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yyv.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lnl.dianchejie.cn

================================================================================
来源：http://mlz.gogol.net.cn

I. 正则表达式
来源：http://zbt.xylfe.cn

================================================================================
来源：http://qxt.smart0.xyz

[I01] 判断是否匹配
来源：http://aei.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yfl.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://dha.xylfe.cn

JS:   /\d+/.test(s)
来源：http://sxt.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://cat.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xgt.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dan.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://oip.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://saf.zhengqikj.top

[I02] 提取所有匹配
来源：http://jqr.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://wqr.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ntn.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fcc.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://ibi.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cio.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qvt.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://vbr.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uij.sjlbkw.cn

[I03] 提取捕获分组
来源：http://vau.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gvh.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://asc.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sdh.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://geb.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://trp.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lie.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ghh.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jzb.hongshengwenyu.top

[I04] 正则替换
来源：http://oom.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jcc.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nrb.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://mjd.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://ylj.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://svw.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pes.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://prq.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kcu.sjlbkw.cn

[I05] 按正则拆分
来源：http://khr.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sme.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fxt.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://sfo.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://xse.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://ujn.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hcs.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://bhl.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ofa.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qgl.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dyr.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pxu.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tpo.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nuo.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mwp.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kfx.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dfp.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gby.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://dad.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://axt.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jbx.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://avt.yuxming.cn

TS:   /error/gim
来源：http://gek.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nes.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lsu.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://zty.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sbw.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://blx.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bea.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lpy.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvz.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dkh.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jxp.quarkkingdee.top


<!-- 参考信息 -->