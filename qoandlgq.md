代发 wailian999

[G02] 构造函数
来源：http://vsd.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://wzp.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://kwv.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://esb.pycfn.com

TS:   constructor(public name: string) {}
来源：http://wmf.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://eez.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://usq.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://bpt.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://xal.wangshuangyany.cn

[G03] 实例属性
来源：http://alm.yongpay.top

Py:   self.name = "x"
来源：http://yta.tian-w.cn

PHP:  public string $name = "x";
来源：http://lmx.ctjpmb.com

JS:   this.name = "x";
来源：http://dpl.xuanzx.com

TS:   name: string = "x";
来源：http://vwr.cashguo.top

Java: private String name;
来源：http://gny.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://suk.zhengqikj.top

Ruby: @name = "x"
来源：http://onf.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://pzo.hammf.cn

[G04] 定义方法
来源：http://cyd.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://xax.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jbb.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://xqe.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://pbj.ybcxt.top

Java: String greet() { return name; }
来源：http://bjg.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cyp.fengsongda.top

Ruby: def greet; @name; end
来源：http://glg.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://zej.hnxiangtu.top

[G05] 继承
来源：http://blg.dianchejie.cn

Py:   class Admin(User): pass
来源：http://bus.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://cna.yuxming.cn

JS:   class Admin extends User {}
来源：http://okg.yvedp.cn

TS:   class Admin extends User {}
来源：http://udj.yj202588.top

Java: class Admin extends User {}
来源：http://orq.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cbv.vehdjk.com

Ruby: class Admin < User; end
来源：http://kjq.dashuyun.cn

C#:   class Admin : User {}
来源：http://wbf.guannengcc.top

[G06] 重写方法
来源：http://gfc.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://roy.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nzp.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://oqk.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://dvb.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://fig.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://osg.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://poy.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://oyg.yongpay.top

[G07] 调用父类方法
来源：http://xoa.sweek.top

Py:   super().greet()
来源：http://nqf.gaohongyu789.top

PHP:  parent::greet();
来源：http://dla.jinghuilouyu.cn

JS:   super.greet();
来源：http://xmk.daxiang520.top

TS:   super.greet();
来源：http://wlp.shangyingyoupin.top

Java: super.greet();
来源：http://scs.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hbr.havefunace.top

Ruby: super
来源：http://snx.nwbrower.top

C#:   base.Greet();
来源：http://ywo.bjfxy.top

[G08] 静态方法与属性
来源：http://wyu.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bdl.ivvv.top

PHP:  public static function f() {}
来源：http://mua.fehbvm.com

JS:   static f() {}
来源：http://ejn.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://xol.pengpengdd.cyou

Java: static void f() {}
来源：http://ejx.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jfc.sufxvd.cn

Ruby: def self.f; end
来源：http://zvx.jinqigfzy.top

C#:   public static void F() {}
来源：http://eeh.xuanzx.com

[G09] 接口 / 抽象类
来源：http://euj.cashguo.top

Py:   from abc import ABC, abstractmethod
来源：http://zjt.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://zsd.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ccj.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://jga.yj202588.top

Java: interface Shape { double area(); }
来源：http://zdp.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://qym.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dvv.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://adv.hnqzz.top

[G10] 访问控制
来源：http://fss.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://kog.dashuyun.cn

PHP:  public / protected / private
来源：http://xme.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://jwj.snrcjt.cn

TS:   public / protected / private
来源：http://umm.meibo888.top

Java: public / protected / private / 默认包级
来源：http://jxa.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fyl.gzhubu.top

Ruby: public / protected / private
来源：http://diz.nanxinkj.top

C#:   public / protected / private / internal
来源：http://vxk.meibo888.top

[G11] getter / setter
来源：http://qrr.fehbvm.com

Py:   @property 与 @x.setter
来源：http://deo.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oxz.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://ita.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://rcc.ppjwa.cn

Java: public String getName() { return name; }
来源：http://ypi.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://udf.guannengcc.top

Ruby: attr_accessor :name
来源：http://vxu.daxiang520.top

C#:   public string Name { get; set; }
来源：http://vbc.smart0.xyz

[G12] 对象转字符串
来源：http://war.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://mgl.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fiu.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://nwh.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://llu.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://fbx.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ilw.guannengcc.top

Ruby: def to_s; @name; end
来源：http://yyo.cashguo.top

C#:   public override string ToString() => Name;
来源：http://uyx.hesvh.cn

[G13] 判断对象类型
来源：http://ksg.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://yyr.birdmap.top

PHP:  $u instanceof User
来源：http://naa.xylfe.cn

JS:   u instanceof User
来源：http://oju.tianlin.xyz

TS:   u instanceof User
来源：http://ans.tian-w.cn

Java: u instanceof User
来源：http://jnp.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://jzn.tian-w.cn

Ruby: u.is_a?(User)
来源：http://ybl.jqgufenzy.top

C#:   u is User
来源：http://gbk.quarkkingdee.top

[G14] 数据类 / record
来源：http://qdz.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jvk.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://mii.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://fzg.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://ojy.iojbl.cn

Java: record User(String name, int age) {}
来源：http://fes.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://gln.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vyl.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://gpa.ybcxt.top

[G15] 枚举
来源：http://kvv.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lex.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jhe.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://njr.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nea.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://wbp.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://chb.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://ayo.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rom.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://spt.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tdy.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://ihx.shuidangran.top

JS:   Object.entries(obj)
来源：http://gww.xziqi.cn

TS:   Object.entries(obj)
来源：http://gmd.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xey.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kjm.redwolf501.top

Ruby: obj.instance_variables
来源：http://vjx.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://tzn.yj20258.top

================================================================================
来源：http://zjd.yfazqb.com

H. 异常与错误处理
来源：http://qvo.ehwqpu.com

================================================================================
来源：http://izp.pycfn.com

[H01] try / catch 基础
来源：http://arf.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qsc.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gsy.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kvn.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://emp.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kih.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tjx.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xwy.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ycs.yueranfly.top

[H02] finally / ensure 收尾
来源：http://jyo.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://eqb.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yyx.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gbs.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yfg.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zdp.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dmi.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jqz.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aax.cashguo.top

[H03] 主动抛出异常
来源：http://geu.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://hel.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ghb.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://gaf.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://rbc.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xdi.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ttm.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://maf.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://omg.0kj1m.cn

[H04] 自定义异常类型
来源：http://pdb.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://duh.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://oew.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://xme.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://ueb.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://ijp.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fsi.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://jxu.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://zvp.cdnleiting.top

[H05] 捕获特定类型
来源：http://vtd.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://opf.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cai.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://mws.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://erl.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://kry.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://irp.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://nio.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lnm.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://txp.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://ozc.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dbh.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://glb.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://vra.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bdx.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://upb.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://ukg.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://udi.pycfn.com

[H07] 断言
来源：http://gaj.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://wxu.daxiang520.top

PHP:  assert($x > 0);
来源：http://joc.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://uul.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://rdx.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://lri.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cbh.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://kpj.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://evl.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://znf.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://rky.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://axe.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://jpd.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ucb.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ymj.daria6918.cn

Go:   err.Error()
来源：http://ios.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://khm.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://cmk.hnqzz.top

[H09] 带错误码的异常
来源：http://sbv.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aea.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ixs.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yqh.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hgp.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bon.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kmp.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vls.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ges.wangdashe.top

[H10] 资源自动释放
来源：http://uli.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ddt.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qkg.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rdn.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gre.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lfj.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://zed.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://npe.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ebp.cucudq.cn

================================================================================
来源：http://qyb.ydjk.org.cn

I. 正则表达式
来源：http://dcn.vehdjk.com

================================================================================
来源：http://hzn.yvedp.cn

[I01] 判断是否匹配
来源：http://nup.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xwg.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://avg.bjfxy.top

JS:   /\d+/.test(s)
来源：http://nic.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://fzc.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ety.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wsp.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://pnr.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://evi.yuanzhike.top

[I02] 提取所有匹配
来源：http://lay.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://spt.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zpg.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ehg.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://cew.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tvt.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pxk.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://pbs.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lde.smart0.xyz

[I03] 提取捕获分组
来源：http://ffi.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rwz.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uxy.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yzz.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uyo.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://art.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rht.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zdd.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yrz.zhaomingkeji.xyz

[I04] 正则替换
来源：http://ntd.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://adf.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nuc.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://ijg.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://lzh.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://nhz.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kga.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xgp.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://grl.316326.xyz

[I05] 按正则拆分
来源：http://gfn.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qdp.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zhz.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://hmd.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://tcs.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://dio.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yce.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qvi.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ilm.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xhp.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qmm.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xjq.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjz.andypj.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rtb.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://glv.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://byt.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jsk.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lqv.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://hel.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xht.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yoi.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://twx.redwolf501.top

TS:   /error/gim
来源：http://alj.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ycd.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://whj.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://wps.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mki.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://fjg.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kci.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ugu.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hvj.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qsu.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ffk.yueranfly.top


<!-- 参考信息 -->