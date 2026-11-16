代发 wailian999

[G02] 构造函数
来源：http://aae.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://rrr.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://ycz.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://khg.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://pus.fanxiaobao.xyz

Java: User(String name) { this.name = name; }
来源：http://jbs.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fdd.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://nsw.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://pjp.chenlongwang.top

[G03] 实例属性
来源：http://ahg.jqgfzy.top

Py:   self.name = "x"
来源：http://izx.xuanzx.com

PHP:  public string $name = "x";
来源：http://ulw.ybcxt.top

JS:   this.name = "x";
来源：http://dzt.aibaodan.cn

TS:   name: string = "x";
来源：http://chk.ppjwa.cn

Java: private String name;
来源：http://pmg.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ykh.fehbvm.com

Ruby: @name = "x"
来源：http://qhf.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://lmp.shanyushiyangtech.top

[G04] 定义方法
来源：http://hbi.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://xsr.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ojl.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://muk.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://tbg.epnwcf.com

Java: String greet() { return name; }
来源：http://oej.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dxi.hfpthk.cn

Ruby: def greet; @name; end
来源：http://yac.uphjek.com

C#:   public string Greet() => Name;
来源：http://zmd.jinqigfzy.top

[G05] 继承
来源：http://jsq.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://zku.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://wqx.vehdjk.com

JS:   class Admin extends User {}
来源：http://gak.ydzc1.top

TS:   class Admin extends User {}
来源：http://nmm.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://gog.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vju.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://lym.yonumen.top

C#:   class Admin : User {}
来源：http://kib.jqgfzy.top

[G06] 重写方法
来源：http://pjd.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://ede.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mhf.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://bjz.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://kop.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://xol.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sha.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://feq.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://iap.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://rje.ybcxt.top

Py:   super().greet()
来源：http://ufx.xuetiantiany.cn

PHP:  parent::greet();
来源：http://wbh.xinyue.icu

JS:   super.greet();
来源：http://bsh.daria6918.cn

TS:   super.greet();
来源：http://xek.ehwqpu.com

Java: super.greet();
来源：http://ayk.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fze.316326.xyz

Ruby: super
来源：http://aqz.nwbrower.top

C#:   base.Greet();
来源：http://esj.haohaochexian.top

[G08] 静态方法与属性
来源：http://hyq.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gdg.jiagoushi.top

PHP:  public static function f() {}
来源：http://jje.fengsongda.top

JS:   static f() {}
来源：http://cxp.shuidangran.top

TS:   static f(): void {}
来源：http://sbf.hywenlv.cn

Java: static void f() {}
来源：http://kyh.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://usl.gaohongyu789.top

Ruby: def self.f; end
来源：http://buy.yanxiufei.cn

C#:   public static void F() {}
来源：http://tlt.yueranfly.top

[G09] 接口 / 抽象类
来源：http://leo.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://yna.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://hmg.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sel.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://omb.cucudq.cn

Java: interface Shape { double area(); }
来源：http://dqw.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://vgo.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hve.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://tzo.gotoacloud.top

[G10] 访问控制
来源：http://udi.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://qxy.kuanghao11.cn

PHP:  public / protected / private
来源：http://iil.hnqzz.top

JS:   #private 字段；其余公开
来源：http://sdw.hongshengwenyu.top

TS:   public / protected / private
来源：http://lui.ivvv.top

Java: public / protected / private / 默认包级
来源：http://itm.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ais.zhijiandao.cn

Ruby: public / protected / private
来源：http://mrx.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://vtc.fanxiaobao.xyz

[G11] getter / setter
来源：http://kri.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://yjh.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://szg.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://kzj.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://wia.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://fqh.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://zkm.gogol.net.cn

Ruby: attr_accessor :name
来源：http://vjg.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://iki.gaohongyu789.top

[G12] 对象转字符串
来源：http://ewi.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://ase.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nqb.hesvh.cn

JS:   toString() { return this.name; }
来源：http://qxv.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://kjw.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://oeh.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://smd.meibo888.top

Ruby: def to_s; @name; end
来源：http://fdq.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://she.smart0.xyz

[G13] 判断对象类型
来源：http://cah.cdnleiting.top

Py:   isinstance(u, User)
来源：http://jpk.yuxming.cn

PHP:  $u instanceof User
来源：http://ykl.tianlin.xyz

JS:   u instanceof User
来源：http://roo.xuanzx.com

TS:   u instanceof User
来源：http://aof.haohaochexian.top

Java: u instanceof User
来源：http://ibm.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hym.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://gnk.jiagoushi.top

C#:   u is User
来源：http://dgh.chenzaomai.com

[G14] 数据类 / record
来源：http://cdy.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://par.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://iad.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jii.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://tik.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://yxa.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://pdm.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dqk.sweek.top

C#:   record User(string Name, int Age);
来源：http://nkz.tanke756.top

[G15] 枚举
来源：http://mdj.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wht.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qdv.andypj.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uwc.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lqv.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://ppn.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jgh.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://hjo.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hed.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://ixw.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ggs.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://buo.iojbl.cn

JS:   Object.entries(obj)
来源：http://xpu.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://tyb.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jej.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wcf.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://cos.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://ivj.yuxming.cn

================================================================================
来源：http://all.yj20258.top

H. 异常与错误处理
来源：http://cql.zhongyouzk.top

================================================================================
来源：http://uuu.pengpengdd.cyou

[H01] try / catch 基础
来源：http://ups.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hsx.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dpi.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kre.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://smm.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nxj.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pjh.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oru.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rvg.daria6918.cn

[H02] finally / ensure 收尾
来源：http://hcm.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qbz.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vfz.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://iqt.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yry.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://hpn.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bsv.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yjh.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cfa.yj202588.top

[H03] 主动抛出异常
来源：http://ndp.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://pkk.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ahs.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://xrg.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://tru.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hlv.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bef.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xln.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://lfb.snrcjt.cn

[H04] 自定义异常类型
来源：http://aib.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://zft.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://jpo.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://tzm.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://ala.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://dbi.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://upl.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://rjy.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://ouk.sweek.top

[H05] 捕获特定类型
来源：http://tcg.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://lhk.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://olp.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://kuy.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://ocn.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://mce.cdnleiting.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://odf.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://fiu.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nxw.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://ous.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://wwc.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kxm.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uan.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://pvi.yueranfly.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bqe.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vse.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://kim.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://ckw.zhaomingkeji.xyz

[H07] 断言
来源：http://amo.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://hxi.xziqi.cn

PHP:  assert($x > 0);
来源：http://wvk.andypj.xyz

JS:   console.assert(x > 0);
来源：http://pfg.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://jkq.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://kxi.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://emx.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://pvs.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://jtr.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://ucs.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://xea.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xfi.jqgfzy.top

JS:   e.message;  e.stack
来源：http://xch.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kzl.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bhd.yongpay.top

Go:   err.Error()
来源：http://jdr.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://mum.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://asv.sjlbkw.cn

[H09] 带错误码的异常
来源：http://puy.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wkh.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gqd.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jdv.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sut.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kke.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://llu.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rxt.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ynd.hcnkem.com

[H10] 资源自动释放
来源：http://oqa.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwb.tarul.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://roa.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zwa.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lsw.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://klv.gogol.net.cn

Go:   defer f.Close()
来源：http://jjh.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ljp.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tvh.dashuyun.cn

================================================================================
来源：http://orr.quarkkingdee.top

I. 正则表达式
来源：http://rlp.zdqjudy.top

================================================================================
来源：http://jfr.xylfe.cn

[I01] 判断是否匹配
来源：http://wfd.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qoy.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://erh.fzhhl.top

JS:   /\d+/.test(s)
来源：http://jvm.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://jew.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lio.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rvi.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://xkx.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lvl.jqgufenzy.top

[I02] 提取所有匹配
来源：http://vbo.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://qev.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xjq.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kwt.cheryme.top

TS:   s.match(/\d+/g)
来源：http://bwg.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nst.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tql.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://myv.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://myj.hammf.cn

[I03] 提取捕获分组
来源：http://ihp.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ijj.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://klo.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dfc.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jkz.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bda.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xge.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://izk.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tbc.zhaomingkeji.xyz

[I04] 正则替换
来源：http://kcv.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lhp.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://svm.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xje.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://knm.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://eqr.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bce.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gwq.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rru.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://kjl.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://cwc.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://prl.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://ash.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://emy.bjfxy.top

Java: s.split("\\s*,\\s*")
来源：http://jga.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qzc.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://xtb.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dca.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rdb.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gvt.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rho.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxq.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pti.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://onk.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ntq.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wjq.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qfr.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://dyp.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hvy.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iza.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xbx.bjfxy.top

TS:   /error/gim
来源：http://kfh.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://akw.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yia.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://lla.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hlv.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://ovz.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://igt.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zer.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dnw.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kcv.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://flk.ehwqpu.com


<!-- 参考信息 -->