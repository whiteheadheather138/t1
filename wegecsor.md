代发 wailian999

[G02] 构造函数
来源：http://lwn.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://bto.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://sxx.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://kmp.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://phs.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://pbh.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mhr.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://wrz.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://qfx.ivvv.top

[G03] 实例属性
来源：http://scw.gogol.net.cn

Py:   self.name = "x"
来源：http://vnz.yuxming.cn

PHP:  public string $name = "x";
来源：http://bkh.ppjwa.cn

JS:   this.name = "x";
来源：http://ixp.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://qvz.jinyuanbaomall.cn

Java: private String name;
来源：http://xpn.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://umv.pengpengdd.cyou

Ruby: @name = "x"
来源：http://iaz.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://gjl.yvedp.cn

[G04] 定义方法
来源：http://wfa.guannengcc.top

Py:   def greet(self): return self.name
来源：http://hmb.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zak.52xcode.cn

JS:   greet() { return this.name; }
来源：http://pzn.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://udd.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://zoa.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wsm.meibo888.top

Ruby: def greet; @name; end
来源：http://awp.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://grh.sxryk.cn

[G05] 继承
来源：http://foa.aizwys.cn

Py:   class Admin(User): pass
来源：http://srj.andypj.xyz

PHP:  class Admin extends User {}
来源：http://eor.dashuyun.cn

JS:   class Admin extends User {}
来源：http://zok.pycfn.com

TS:   class Admin extends User {}
来源：http://sye.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://wdj.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://les.cdnleiting.top

Ruby: class Admin < User; end
来源：http://nov.fehbvm.com

C#:   class Admin : User {}
来源：http://sno.xziqi.cn

[G06] 重写方法
来源：http://zvu.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://hht.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jvx.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://gwz.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://njf.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://soc.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rin.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://bfn.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://zeu.tanke756.top

[G07] 调用父类方法
来源：http://nsa.shanyushiyangkeji.top

Py:   super().greet()
来源：http://ojs.snrcjt.cn

PHP:  parent::greet();
来源：http://pkv.tarul.cn

JS:   super.greet();
来源：http://zoa.zhoulong.xyz

TS:   super.greet();
来源：http://ymu.hongshengwenyu.top

Java: super.greet();
来源：http://rtw.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vmu.jinyuanbaomall.cn

Ruby: super
来源：http://pnc.ybcxt.top

C#:   base.Greet();
来源：http://rrt.hfpthk.cn

[G08] 静态方法与属性
来源：http://uen.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jve.tian-w.cn

PHP:  public static function f() {}
来源：http://jkv.fzhhl.top

JS:   static f() {}
来源：http://oly.gotoacloud.top

TS:   static f(): void {}
来源：http://jup.shzxlz.cn

Java: static void f() {}
来源：http://rzx.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wwv.cheryme.top

Ruby: def self.f; end
来源：http://mkp.jinqigufen.top

C#:   public static void F() {}
来源：http://wrc.xylfe.cn

[G09] 接口 / 抽象类
来源：http://ido.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://vbi.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://ggm.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oai.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://iwd.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://gte.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://yts.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lhi.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://fqc.cheryme.top

[G10] 访问控制
来源：http://qfz.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://vbi.zhijiandao.cn

PHP:  public / protected / private
来源：http://dbv.yfazqb.com

JS:   #private 字段；其余公开
来源：http://faw.fzhhl.top

TS:   public / protected / private
来源：http://gmg.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://iik.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ifu.jqgufenzy.top

Ruby: public / protected / private
来源：http://yud.smart0.xyz

C#:   public / protected / private / internal
来源：http://bsu.cheryme.top

[G11] getter / setter
来源：http://dyo.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://sjq.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://iin.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://kun.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://wpe.svipenyu.cn

Java: public String getName() { return name; }
来源：http://ktw.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wxq.dianchejie.cn

Ruby: attr_accessor :name
来源：http://trc.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://edq.bbcook.cn

[G12] 对象转字符串
来源：http://ruh.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://uvf.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cnv.nwbrower.top

JS:   toString() { return this.name; }
来源：http://jbj.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://jpf.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://wsc.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ooz.cucudq.cn

Ruby: def to_s; @name; end
来源：http://uaz.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://jhg.yj20258.top

[G13] 判断对象类型
来源：http://sfs.fehbvm.com

Py:   isinstance(u, User)
来源：http://frn.ydzc1.top

PHP:  $u instanceof User
来源：http://qot.hesvh.cn

JS:   u instanceof User
来源：http://hng.wangdashe.top

TS:   u instanceof User
来源：http://bfy.hnxiangtu.top

Java: u instanceof User
来源：http://bfq.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vpu.birdmap.top

Ruby: u.is_a?(User)
来源：http://chv.gzhubu.top

C#:   u is User
来源：http://lty.hywenlv.cn

[G14] 数据类 / record
来源：http://vcs.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jqa.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://xjr.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://odi.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://vmr.daria6918.cn

Java: record User(String name, int age) {}
来源：http://hrp.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://suk.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hpc.yonumen.top

C#:   record User(string Name, int Age);
来源：http://tps.zhijiandao.cn

[G15] 枚举
来源：http://dkt.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://efm.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://crg.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://geh.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wvl.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://lid.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qne.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://lxj.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tfn.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://nhi.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uvs.havefunace.top

PHP:  get_object_vars($obj);
来源：http://lqk.xziqi.cn

JS:   Object.entries(obj)
来源：http://eho.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://nmb.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ufq.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ipd.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://mrz.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://ryz.meibo888.top

================================================================================
来源：http://jih.zycfv.cn

H. 异常与错误处理
来源：http://ext.jianghu66.top

================================================================================
来源：http://znw.jqgufenzy.top

[H01] try / catch 基础
来源：http://rvg.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://irp.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kbc.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aqf.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zdk.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qbg.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vlu.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qlh.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rpj.aizwys.cn

[H02] finally / ensure 收尾
来源：http://qpg.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ift.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bja.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kbz.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vau.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vkf.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://dfa.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gys.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://tby.jinqigufen.top

[H03] 主动抛出异常
来源：http://zuo.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://fdq.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sio.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://pgz.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://dti.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tev.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zir.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nbv.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kmj.yfazqb.com

[H04] 自定义异常类型
来源：http://rlq.guowangkeji.top

Py:   class MyError(Exception): pass
来源：http://wfw.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ics.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://lvp.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://axl.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://ymy.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jax.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://mwb.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://uvg.hammf.cn

[H05] 捕获特定类型
来源：http://zja.fktsv.cn

Py:   except ValueError as e:
来源：http://gca.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fyz.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://tig.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://ugx.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://iwc.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://njq.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://cpz.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ajf.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://fyo.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://tac.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://ejh.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://wbx.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://eid.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aut.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://jed.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://hqz.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://its.jqgufenzy.top

[H07] 断言
来源：http://ndt.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://gxr.c1oappe.top

PHP:  assert($x > 0);
来源：http://tie.hesvh.cn

JS:   console.assert(x > 0);
来源：http://bqg.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://qus.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://jyj.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gxy.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://epa.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://zlh.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://qfj.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://hfw.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tgr.cqqwz.cn

JS:   e.message;  e.stack
来源：http://xsf.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zkg.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mfj.ppjwa.cn

Go:   err.Error()
来源：http://hry.quarkkingdee.top

Ruby: e.message;  e.backtrace
来源：http://wjc.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://nsh.hfpthk.cn

[H09] 带错误码的异常
来源：http://vwa.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ahy.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fvl.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zcz.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://res.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ebn.hywenlv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cmy.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fdm.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dsf.jiagoushi.top

[H10] 资源自动释放
来源：http://scx.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ivl.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qai.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nci.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xcm.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hky.yj20258.top

Go:   defer f.Close()
来源：http://wgu.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uuk.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sfh.hammf.cn

================================================================================
来源：http://kmp.316326.xyz

I. 正则表达式
来源：http://hfz.havefunace.top

================================================================================
来源：http://zjb.zhixingplan.top

[I01] 判断是否匹配
来源：http://vnn.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rwi.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://evf.zycfv.cn

JS:   /\d+/.test(s)
来源：http://vbw.fzhhl.top

TS:   /\d+/.test(s)
来源：http://iua.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://csz.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tim.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://vgo.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tkk.jinqigufen.top

[I02] 提取所有匹配
来源：http://flb.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://mve.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jgn.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oce.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://zhd.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ffo.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tyc.9152youxi.cn

Ruby: s.scan(/\d+/)
来源：http://env.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pvl.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://hym.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://awn.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ghm.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jvw.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nlm.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xmw.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lvw.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zkt.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wxm.fktsv.cn

[I04] 正则替换
来源：http://zlq.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://raf.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pvx.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://qzi.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://mtz.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://tfs.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://xzd.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://puh.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zzd.jqgufenzy.top

[I05] 按正则拆分
来源：http://owt.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jau.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gmv.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://cop.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://xef.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://dpl.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zoa.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xbs.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yir.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gou.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ydt.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yyl.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nwk.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zif.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dut.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://utt.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tsm.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wqe.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://xdn.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sbs.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gkm.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rrh.fehbvm.com

TS:   /error/gim
来源：http://uon.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yei.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oef.316326.xyz

Ruby: s.scan(/error/i)
来源：http://sog.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rou.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://usv.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dps.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xqc.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://njf.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hax.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pqj.jinqigfzy.top


<!-- 参考信息 -->