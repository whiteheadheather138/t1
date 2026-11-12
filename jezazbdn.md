代发 wailian999

Java: class User {}
来源：http://rhk.havefunace.top

Go:   type User struct { Name string }
来源：http://bxy.andypj.xyz

Ruby: class User; end
来源：http://nkq.jianghu66.top

C#:   class User {}
来源：http://owg.guowangkeji.top

[G02] 构造函数
来源：http://ajl.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://qyp.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://gqy.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://ibn.tanke756.top

TS:   constructor(public name: string) {}
来源：http://yca.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://hrg.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bbv.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://bum.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://huu.cucudq.cn

[G03] 实例属性
来源：http://sbp.mhx1999.top

Py:   self.name = "x"
来源：http://vjq.hysaishi.cn

PHP:  public string $name = "x";
来源：http://rqs.guannengcc.top

JS:   this.name = "x";
来源：http://ree.wangdashe.top

TS:   name: string = "x";
来源：http://dfj.shanyushiyangkeji.top

Java: private String name;
来源：http://utg.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iaq.sxryk.cn

Ruby: @name = "x"
来源：http://adr.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://iqt.zdbjq.cn

[G04] 定义方法
来源：http://vpl.guannengcc.top

Py:   def greet(self): return self.name
来源：http://lwe.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://fid.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://vgj.cashguo.top

TS:   greet(): string { return this.name; }
来源：http://gpg.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://wvv.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://siw.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://jbl.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://pcg.redwolf501.top

[G05] 继承
来源：http://mjl.nanxinkj.top

Py:   class Admin(User): pass
来源：http://wkr.fzhhl.top

PHP:  class Admin extends User {}
来源：http://hhs.sufxvd.cn

JS:   class Admin extends User {}
来源：http://vlf.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://nvw.yvedp.cn

Java: class Admin extends User {}
来源：http://zee.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://coa.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://ntl.tanke756.top

C#:   class Admin : User {}
来源：http://jdu.sjlbkw.cn

[G06] 重写方法
来源：http://jwe.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://api.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://umq.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://cee.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://rnu.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://jvu.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hqg.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://bjl.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://tid.fengsongda.top

[G07] 调用父类方法
来源：http://pcp.xylfe.cn

Py:   super().greet()
来源：http://jpi.bjfxy.top

PHP:  parent::greet();
来源：http://jtw.hnqzz.top

JS:   super.greet();
来源：http://dhk.zhengqikj.top

TS:   super.greet();
来源：http://oin.gaohongyu789.top

Java: super.greet();
来源：http://nhy.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dxw.mhx1999.top

Ruby: super
来源：http://hmz.316326.xyz

C#:   base.Greet();
来源：http://aey.sxryk.cn

[G08] 静态方法与属性
来源：http://hjy.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rhz.52xcode.cn

PHP:  public static function f() {}
来源：http://qty.hcnkem.com

JS:   static f() {}
来源：http://xgq.jinqigfzy.top

TS:   static f(): void {}
来源：http://wmf.hongshengwenyu.top

Java: static void f() {}
来源：http://dth.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jrc.shuidangran.top

Ruby: def self.f; end
来源：http://pfc.yangfankeji.com

C#:   public static void F() {}
来源：http://yvv.bbcook.cn

[G09] 接口 / 抽象类
来源：http://dfh.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://bte.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nqi.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://frs.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://grk.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://aac.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://xbd.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kcr.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://sjc.fehbvm.com

[G10] 访问控制
来源：http://jkc.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://oes.daria6918.cn

PHP:  public / protected / private
来源：http://qgi.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://czx.sjlbkw.cn

TS:   public / protected / private
来源：http://xkx.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://dwu.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fcv.xziqi.cn

Ruby: public / protected / private
来源：http://jam.yuxming.cn

C#:   public / protected / private / internal
来源：http://kcs.hywenlv.cn

[G11] getter / setter
来源：http://yry.sweek.top

Py:   @property 与 @x.setter
来源：http://lcj.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qlz.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://opl.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://rex.sufxvd.cn

Java: public String getName() { return name; }
来源：http://xhr.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ila.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://lbf.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://dyr.xuanzx.com

[G12] 对象转字符串
来源：http://llh.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://zlj.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oyu.mhx1999.top

JS:   toString() { return this.name; }
来源：http://oep.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://lhl.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://fyf.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dai.epnwcf.com

Ruby: def to_s; @name; end
来源：http://jan.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://yja.epnwcf.com

[G13] 判断对象类型
来源：http://zfg.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://crm.aibaodan.cn

PHP:  $u instanceof User
来源：http://dhc.ydzc1.top

JS:   u instanceof User
来源：http://rsy.zhijiandao.cn

TS:   u instanceof User
来源：http://qlr.shanyushiyangtech.top

Java: u instanceof User
来源：http://qcu.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://fse.gzhubu.top

Ruby: u.is_a?(User)
来源：http://ldb.jqgufenzy.top

C#:   u is User
来源：http://hxm.shanyushiyangtech.top

[G14] 数据类 / record
来源：http://yvd.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vqy.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://wmw.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uca.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://iko.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://grh.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://mgt.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mfz.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://byi.cashguo.top

[G15] 枚举
来源：http://ylw.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nic.vehdjk.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://isk.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wvr.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tnh.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://pvx.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pfh.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://vcm.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bmy.smart0.xyz

[G16] 对象转数组 / 字典
来源：http://yns.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kzp.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://jym.guannengcc.top

JS:   Object.entries(obj)
来源：http://wzy.aibaodan.cn

TS:   Object.entries(obj)
来源：http://miy.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nle.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vgp.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://lwx.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://nsj.shangyingyoupin.top

================================================================================
来源：http://brd.shzxlz.cn

H. 异常与错误处理
来源：http://gag.nanxuanxn.top

================================================================================
来源：http://gbr.haohaochexian.top

[H01] try / catch 基础
来源：http://xet.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kfy.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mcb.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bci.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://foh.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ltu.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uws.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nne.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ktd.hammf.cn

[H02] finally / ensure 收尾
来源：http://kuw.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://spl.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bjq.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://opu.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rmo.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://ogx.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://iky.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fkq.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://cdi.iojbl.cn

[H03] 主动抛出异常
来源：http://njs.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://zyc.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dwo.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://nqa.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://acm.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yrx.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vae.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://elf.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://fbe.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://elx.ivvv.top

Py:   class MyError(Exception): pass
来源：http://hyw.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://qgs.meibo888.top

JS:   class MyError extends Error {}
来源：http://dsa.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://uoe.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://bhb.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sux.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://qvd.52xcode.cn

C#:   class MyException : Exception {}
来源：http://wej.zdqjudy.top

[H05] 捕获特定类型
来源：http://klh.ehwqpu.com

Py:   except ValueError as e:
来源：http://wwp.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ivi.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://ngf.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://see.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://shi.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kih.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://the.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://way.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://vqn.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://kua.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pnx.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://xfu.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://ene.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tet.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dvt.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://cmd.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://bub.jqgfzy.top

[H07] 断言
来源：http://vcq.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://vmn.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://xwd.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://ouy.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://apv.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://exh.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fbn.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://wll.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://rni.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://gab.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://atc.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://luz.yueranfly.top

JS:   e.message;  e.stack
来源：http://ign.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pcu.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bdk.ehwqpu.com

Go:   err.Error()
来源：http://nam.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://ksm.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://cco.zdbjq.cn

[H09] 带错误码的异常
来源：http://qyj.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xvi.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dzz.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vko.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wdp.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zzc.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nsa.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wdw.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kaf.shuidangran.top

[H10] 资源自动释放
来源：http://crk.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uud.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bxq.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xok.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://azm.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fcn.hnxiangtu.top

Go:   defer f.Close()
来源：http://dpx.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yps.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fta.52xcode.cn

================================================================================
来源：http://yft.sxryk.cn

I. 正则表达式
来源：http://ilr.jqgfzy.top

================================================================================
来源：http://gax.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://gpw.c1oappe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ffs.xuetiantiany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dtl.sysykeji.top

JS:   /\d+/.test(s)
来源：http://tmt.hesvh.cn

TS:   /\d+/.test(s)
来源：http://sbq.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iqz.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aud.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://zgg.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://phm.jlsjyb.cn

[I02] 提取所有匹配
来源：http://cme.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://cqy.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xgu.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://frt.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://mrt.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eiy.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://juv.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://maf.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eze.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://tbr.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rar.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bbu.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zvi.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://myq.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rhb.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kgi.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iqz.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hjb.ydzc1.top

[I04] 正则替换
来源：http://mib.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zhs.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ghe.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://sxe.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zum.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://udl.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ejo.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://msd.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fkq.yueranfly.top

[I05] 按正则拆分
来源：http://sdf.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://kmz.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hbx.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://cax.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://pzj.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://itd.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dgz.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://edi.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dlx.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tcc.zhiwuduotai.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mbn.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jtr.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bnk.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tto.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lxb.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qjh.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ppb.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ccy.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://uhp.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jxn.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eae.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://daj.52xcode.cn

TS:   /error/gim
来源：http://tow.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iik.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qwt.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://ksb.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ahm.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://rvy.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gdg.0kj1m.cn


<!-- 参考信息 -->