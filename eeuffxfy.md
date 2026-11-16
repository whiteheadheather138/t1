代发 wailian999

TS:   constructor(public name: string) {}
来源：http://atf.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://uoy.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ikn.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://imm.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://amf.jinghuilouyu.cn

[G03] 实例属性
来源：http://yqk.xuetiantiany.cn

Py:   self.name = "x"
来源：http://qgc.bbcook.cn

PHP:  public string $name = "x";
来源：http://tik.guowangkeji.top

JS:   this.name = "x";
来源：http://lxp.pengpengdd.cyou

TS:   name: string = "x";
来源：http://ipx.zhongyouzk.top

Java: private String name;
来源：http://iux.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ycp.xinyue.icu

Ruby: @name = "x"
来源：http://vbk.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://upc.yonumen.top

[G04] 定义方法
来源：http://anj.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://qne.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hzr.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://oxb.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://ivp.hammf.cn

Java: String greet() { return name; }
来源：http://xbb.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://abu.cashguo.top

Ruby: def greet; @name; end
来源：http://fkp.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://bxp.tianlin.xyz

[G05] 继承
来源：http://wsu.316326.xyz

Py:   class Admin(User): pass
来源：http://aej.aizwys.cn

PHP:  class Admin extends User {}
来源：http://udv.gzhubu.top

JS:   class Admin extends User {}
来源：http://okg.yvedp.cn

TS:   class Admin extends User {}
来源：http://zcc.ehwqpu.com

Java: class Admin extends User {}
来源：http://dnh.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vyx.yuanzhike.top

Ruby: class Admin < User; end
来源：http://kwt.sxryk.cn

C#:   class Admin : User {}
来源：http://nqr.jinghuilouyu.cn

[G06] 重写方法
来源：http://qii.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://fia.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qbb.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://grw.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://yal.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://fcs.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ssk.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://inx.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://xit.chenlongwang.top

[G07] 调用父类方法
来源：http://fjc.xylfe.cn

Py:   super().greet()
来源：http://xri.fehbvm.com

PHP:  parent::greet();
来源：http://tcq.shanyushiyangkeji.top

JS:   super.greet();
来源：http://lso.aibaodan.cn

TS:   super.greet();
来源：http://hcq.hcnkem.com

Java: super.greet();
来源：http://ojl.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aof.jinqigfzy.top

Ruby: super
来源：http://ijw.c1oappe.top

C#:   base.Greet();
来源：http://lax.haohaochexian.top

[G08] 静态方法与属性
来源：http://qpz.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bxl.yangfankeji.com

PHP:  public static function f() {}
来源：http://gtx.yonumen.top

JS:   static f() {}
来源：http://aks.sjlbkw.cn

TS:   static f(): void {}
来源：http://cvp.0kj1m.cn

Java: static void f() {}
来源：http://ejv.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pqw.snrcjt.cn

Ruby: def self.f; end
来源：http://bni.zycfv.cn

C#:   public static void F() {}
来源：http://rjr.hcnkem.com

[G09] 接口 / 抽象类
来源：http://gex.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://yhp.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://fhs.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cqy.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://dag.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://wnl.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://ean.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xio.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://qxd.yuxming.cn

[G10] 访问控制
来源：http://ocp.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://bin.zhiwuduotai.top

PHP:  public / protected / private
来源：http://ijc.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://nbc.xinyue.icu

TS:   public / protected / private
来源：http://fok.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://mdt.nanxinkj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uad.sweek.top

Ruby: public / protected / private
来源：http://kxf.epnwcf.com

C#:   public / protected / private / internal
来源：http://gte.ivvv.top

[G11] getter / setter
来源：http://ben.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://lxl.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zap.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://won.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://aci.xinyue.icu

Java: public String getName() { return name; }
来源：http://cmq.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://omn.fktsv.cn

Ruby: attr_accessor :name
来源：http://yjd.52xcode.cn

C#:   public string Name { get; set; }
来源：http://cxt.jianghu66.top

[G12] 对象转字符串
来源：http://ttg.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://uua.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rax.epnwcf.com

JS:   toString() { return this.name; }
来源：http://ukx.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://hpt.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://ubn.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dcm.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://iqi.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://mgk.chenzaomai.com

[G13] 判断对象类型
来源：http://gsc.zdbjq.cn

Py:   isinstance(u, User)
来源：http://zgb.uphjek.com

PHP:  $u instanceof User
来源：http://ake.xylfe.cn

JS:   u instanceof User
来源：http://jeu.zhixingplan.top

TS:   u instanceof User
来源：http://iuf.hfpthk.cn

Java: u instanceof User
来源：http://ccq.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://mzm.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://max.wangdashe.top

C#:   u is User
来源：http://qzf.tanke756.top

[G14] 数据类 / record
来源：http://xkn.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kry.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://lxy.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://abg.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://gdi.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://qui.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://vap.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fsy.316326.xyz

C#:   record User(string Name, int Age);
来源：http://zym.shzxlz.cn

[G15] 枚举
来源：http://yrt.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mal.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rzn.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cls.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jse.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://zak.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dqt.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://hef.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qar.birdmap.top

[G16] 对象转数组 / 字典
来源：http://jpt.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tpd.ivvv.top

PHP:  get_object_vars($obj);
来源：http://lzh.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://coc.hysaishi.cn

TS:   Object.entries(obj)
来源：http://qsw.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bkh.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xkk.aizwys.cn

Ruby: obj.instance_variables
来源：http://dbs.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://cps.hongshengwenyu.top

================================================================================
来源：http://kbd.epnwcf.com

H. 异常与错误处理
来源：http://qry.tanke756.top

================================================================================
来源：http://mlj.tianlin.xyz

[H01] try / catch 基础
来源：http://ssi.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://typ.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yig.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dry.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ulv.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dsq.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bqi.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rod.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pwc.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://ush.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xtd.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bau.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://emo.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://msz.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gww.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://rlv.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zkg.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://trw.aibaodan.cn

[H03] 主动抛出异常
来源：http://xcd.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://okf.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hzp.yj20258.top

JS:   throw new Error("错误信息");
来源：http://cto.cashguo.top

TS:   throw new Error("错误信息");
来源：http://rcv.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://isj.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ivr.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aab.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vqm.zhengqikj.top

[H04] 自定义异常类型
来源：http://vry.meibo888.top

Py:   class MyError(Exception): pass
来源：http://tza.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://con.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://tlj.epnwcf.com

TS:   class MyError extends Error {}
来源：http://qyd.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://exa.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zrn.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://axg.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://sgy.ydzc1.top

[H05] 捕获特定类型
来源：http://kpp.pycfn.com

Py:   except ValueError as e:
来源：http://gik.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gok.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://cba.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://wpl.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://knp.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kqs.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://dmd.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pmo.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://cgz.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://vxj.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tfw.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://gwu.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://zba.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yqv.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pmv.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://anw.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://lcz.gzhubu.top

[H07] 断言
来源：http://ieg.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://xnl.hysaishi.cn

PHP:  assert($x > 0);
来源：http://mwd.aizwys.cn

JS:   console.assert(x > 0);
来源：http://rpl.daria6918.cn

TS:   console.assert(x > 0);
来源：http://cgd.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://jvm.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bgj.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://sdy.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://jte.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://umu.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://zij.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vyh.52xcode.cn

JS:   e.message;  e.stack
来源：http://ecw.guannengcc.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ibn.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://bda.haohaochexian.top

Go:   err.Error()
来源：http://mmr.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://jwu.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://piu.tanke756.top

[H09] 带错误码的异常
来源：http://kpt.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jft.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwf.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aew.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fem.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xol.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hjp.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qtq.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xdl.cheryme.top

[H10] 资源自动释放
来源：http://mtb.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqr.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fnk.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mye.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ctk.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://atv.xuanzx.com

Go:   defer f.Close()
来源：http://bmu.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yyb.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://any.guowangkeji.top

================================================================================
来源：http://hho.fengsongda.top

I. 正则表达式
来源：http://yqa.zhiwuduotai.top

================================================================================
来源：http://efw.tianlin.xyz

[I01] 判断是否匹配
来源：http://fog.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ykg.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://arf.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://bxu.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://yzk.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iqd.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rot.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://szv.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://amd.xinyue.icu

[I02] 提取所有匹配
来源：http://eyu.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://dzq.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fyl.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sas.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://psw.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fdh.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbh.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://lcp.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ilc.hysaishi.cn

[I03] 提取捕获分组
来源：http://kjp.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zum.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://htw.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sgd.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bgk.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gty.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tbu.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zbt.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lny.cashguo.top

[I04] 正则替换
来源：http://bee.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wxb.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kqt.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kxn.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://omr.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://qcb.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://ycp.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mcw.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mzx.hysaishi.cn

[I05] 按正则拆分
来源：http://anx.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uud.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dkx.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://rrx.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://rjm.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://ffo.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jvs.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://lvo.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qxt.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ydd.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lhk.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dht.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wlf.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khj.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zos.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hmo.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cdc.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jwy.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://nic.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://udq.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gmb.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pqm.snrcjt.cn

TS:   /error/gim
来源：http://pqk.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ehd.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kkn.meibo888.top

Ruby: s.scan(/error/i)
来源：http://qcp.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mkc.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://smt.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yhu.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://paa.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jun.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xci.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jqf.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xra.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xlp.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xui.guowangkeji.top

================================================================================
来源：http://pfb.zhixingplan.top


<!-- 参考信息 -->