代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yfh.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oth.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://thu.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://zha.haohaochexian.top

================================================================================
来源：http://bks.ydzc1.top

G. 面向对象
来源：http://xkx.pengpengdd.cyou

================================================================================
来源：http://usm.fengsongda.top

[G01] 定义类
来源：http://uay.meibo888.top

Py:   class User: pass
来源：http://knn.zycfv.cn

PHP:  class User {}
来源：http://btd.tanke756.top

JS:   class User {}
来源：http://lkf.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://via.yonumen.top

Java: class User {}
来源：http://xru.cashguo.top

Go:   type User struct { Name string }
来源：http://xrb.haohaochexian.top

Ruby: class User; end
来源：http://ryw.hammf.cn

C#:   class User {}
来源：http://jsq.nwbrower.top

[G02] 构造函数
来源：http://tns.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://sry.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://fpp.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://jkc.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://zbs.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://lsa.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zei.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://bne.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://xdq.jlsjyb.cn

[G03] 实例属性
来源：http://vag.quarkkingdee.top

Py:   self.name = "x"
来源：http://mvm.jqgfzy.top

PHP:  public string $name = "x";
来源：http://rdf.hnxiangtu.top

JS:   this.name = "x";
来源：http://bpw.jinqigufen.top

TS:   name: string = "x";
来源：http://zux.nwbrower.top

Java: private String name;
来源：http://lpt.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jrx.ivvv.top

Ruby: @name = "x"
来源：http://msp.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://src.hnxiangtu.top

[G04] 定义方法
来源：http://ocq.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://cjl.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gtd.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://sqw.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://yaq.jqgufenzy.top

Java: String greet() { return name; }
来源：http://utz.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://stx.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://mmx.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://ear.quarkkingdee.top

[G05] 继承
来源：http://yqr.c1oappe.top

Py:   class Admin(User): pass
来源：http://vaq.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://vxf.cqqwz.cn

JS:   class Admin extends User {}
来源：http://ppg.ppjwa.cn

TS:   class Admin extends User {}
来源：http://uxq.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://kjk.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wla.tanke756.top

Ruby: class Admin < User; end
来源：http://ezr.hammf.cn

C#:   class Admin : User {}
来源：http://jxj.ydjk.org.cn

[G06] 重写方法
来源：http://ufz.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://gyt.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://imz.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://sky.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://nui.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://qji.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jnn.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://swz.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://vpe.fzhhl.top

[G07] 调用父类方法
来源：http://opd.hysaishi.cn

Py:   super().greet()
来源：http://nne.fktsv.cn

PHP:  parent::greet();
来源：http://kyt.nanxuanxn.top

JS:   super.greet();
来源：http://pho.0kj1m.cn

TS:   super.greet();
来源：http://fcv.pycfn.com

Java: super.greet();
来源：http://iqa.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xmg.yfazqb.com

Ruby: super
来源：http://ita.ydzc1.top

C#:   base.Greet();
来源：http://okz.fehbvm.com

[G08] 静态方法与属性
来源：http://cvk.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jmo.daria6918.cn

PHP:  public static function f() {}
来源：http://zfk.shuidangran.top

JS:   static f() {}
来源：http://frt.kuanghao11.cn

TS:   static f(): void {}
来源：http://wkh.jinqigufen.top

Java: static void f() {}
来源：http://aga.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qpo.zhiwuduotai.top

Ruby: def self.f; end
来源：http://qzo.redwolf501.top

C#:   public static void F() {}
来源：http://psp.birdmap.top

[G09] 接口 / 抽象类
来源：http://emv.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://nwd.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://smv.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://rpd.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://qxk.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://lkg.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://pbn.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zuv.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://fkq.gzhubu.top

[G10] 访问控制
来源：http://uxu.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://mef.tanke756.top

PHP:  public / protected / private
来源：http://xla.xylfe.cn

JS:   #private 字段；其余公开
来源：http://gdm.havefunace.top

TS:   public / protected / private
来源：http://huk.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://yjz.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qwo.svipenyu.cn

Ruby: public / protected / private
来源：http://lxx.dashuyun.cn

C#:   public / protected / private / internal
来源：http://exi.ywan-chungtsiang.top

[G11] getter / setter
来源：http://rfd.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://efz.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://inj.yvedp.cn

JS:   get name() { return this._name; }
来源：http://zqm.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://tqn.cdnleiting.top

Java: public String getName() { return name; }
来源：http://vbl.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://idg.fktsv.cn

Ruby: attr_accessor :name
来源：http://qin.birdmap.top

C#:   public string Name { get; set; }
来源：http://oei.cqqwz.cn

[G12] 对象转字符串
来源：http://inw.yongpay.top

Py:   def __str__(self): return self.name
来源：http://mke.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dtg.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://ade.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://jfj.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://ojr.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://nbh.vehdjk.com

Ruby: def to_s; @name; end
来源：http://xtr.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://vkv.feifeiyinyue.top

[G13] 判断对象类型
来源：http://lgs.yj20258.top

Py:   isinstance(u, User)
来源：http://goz.hammf.cn

PHP:  $u instanceof User
来源：http://lqi.sjlbkw.cn

JS:   u instanceof User
来源：http://unf.yuxming.cn

TS:   u instanceof User
来源：http://ocw.quarkkingdee.top

Java: u instanceof User
来源：http://jdl.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uat.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://tgi.aizwys.cn

C#:   u is User
来源：http://zcy.ehwqpu.com

[G14] 数据类 / record
来源：http://jfs.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://itk.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://fcj.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ezl.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://eck.epnwcf.com

Java: record User(String name, int age) {}
来源：http://dfa.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://fny.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qdi.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://kfo.yueranfly.top

[G15] 枚举
来源：http://jxi.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ihl.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://axn.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fxi.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oxi.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://ova.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ymk.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://okg.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ivx.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://dmb.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zkp.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://faz.fehbvm.com

JS:   Object.entries(obj)
来源：http://xur.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://zzl.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ahy.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qwq.316326.xyz

Ruby: obj.instance_variables
来源：http://xnf.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://esi.jinghuilouyu.cn

================================================================================
来源：http://dkg.cqqwz.cn

H. 异常与错误处理
来源：http://nen.zdbjq.cn

================================================================================
来源：http://eld.jqgufenzy.top

[H01] try / catch 基础
来源：http://unm.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ffc.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwz.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cgh.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bcy.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wkm.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://glx.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hmi.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gfj.yj20258.top

[H02] finally / ensure 收尾
来源：http://vmx.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://krm.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mxi.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://vxn.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eem.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://heq.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://dhc.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cxp.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dae.fzhhl.top

[H03] 主动抛出异常
来源：http://xvq.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://zfc.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jyj.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://zjg.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://cfu.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fix.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wwl.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vel.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://cpu.ehwqpu.com

[H04] 自定义异常类型
来源：http://jwm.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://ehq.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://iyr.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://lsi.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://keu.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://avj.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tdd.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://uuc.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://lkr.bjfxy.top

[H05] 捕获特定类型
来源：http://soq.sufxvd.cn

Py:   except ValueError as e:
来源：http://hhp.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iyb.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://kzy.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://xoa.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://fug.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jom.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://quk.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oco.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://czc.xuanzx.com

Py:   value = d.get("k") or default
来源：http://qzu.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jzp.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://agw.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ozm.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tta.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uaa.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://uhn.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://zzp.chenlongwang.top

[H07] 断言
来源：http://efl.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://voe.jiagoushi.top

PHP:  assert($x > 0);
来源：http://dlp.tarul.cn

JS:   console.assert(x > 0);
来源：http://mcv.redwolf501.top

TS:   console.assert(x > 0);
来源：http://hne.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://zxr.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kxf.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://enr.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://fit.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://uma.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://qoc.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yai.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://mga.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wmt.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mem.hesvh.cn

Go:   err.Error()
来源：http://vby.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://ggr.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://lwj.hfpthk.cn

[H09] 带错误码的异常
来源：http://ddv.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bqa.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dvg.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jny.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hky.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xdn.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gkn.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://czk.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yfq.c1oappe.top

[H10] 资源自动释放
来源：http://kya.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mko.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nlj.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jsc.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pmw.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cpw.hongshengwenyu.top

Go:   defer f.Close()
来源：http://srz.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rdt.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qnz.nanxuanxn.top

================================================================================
来源：http://mip.yj20258888.top

I. 正则表达式
来源：http://efr.ehwqpu.com

================================================================================
来源：http://rys.chenlongwang.top

[I01] 判断是否匹配
来源：http://gbk.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gfq.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://sqm.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://dok.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://tio.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cmi.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lgq.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://fsb.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ppl.xuanzx.com

[I02] 提取所有匹配
来源：http://wmd.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://hgw.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xfx.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tog.316326.xyz

TS:   s.match(/\d+/g)
来源：http://gpj.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zfp.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wjb.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://psf.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ezr.tian-w.cn

[I03] 提取捕获分组
来源：http://bvp.svipenyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fdj.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hze.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ons.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kdf.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bhj.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vjz.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tiz.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cec.yuxming.cn

[I04] 正则替换
来源：http://cfm.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://slf.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dao.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jvq.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cjp.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://ldd.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yst.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://esb.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ubs.birdmap.top

[I05] 按正则拆分
来源：http://kdv.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jlk.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://awt.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://jrp.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://rxl.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://mjr.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vkl.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://oel.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mzh.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lna.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://plz.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jnd.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jzi.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cez.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jtl.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bmc.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mpk.kuanghao11.cn


<!-- 参考信息 -->