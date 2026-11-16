代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mut.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://upj.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hkp.jinqigfzy.top

TS:   // 同上
来源：http://kac.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oxj.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yvx.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kjw.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xbb.cheryme.top

================================================================================
来源：http://qyd.gogol.net.cn

G. 面向对象
来源：http://lfp.hesvh.cn

================================================================================
来源：http://num.sjlbkw.cn

[G01] 定义类
来源：http://alz.cqqwz.cn

Py:   class User: pass
来源：http://txj.yj202588.top

PHP:  class User {}
来源：http://car.jinghuilouyu.cn

JS:   class User {}
来源：http://nhb.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://rwe.guannengcc.top

Java: class User {}
来源：http://oaf.fehbvm.com

Go:   type User struct { Name string }
来源：http://joh.ywan-chungtsiang.top

Ruby: class User; end
来源：http://qjt.tanke756.top

C#:   class User {}
来源：http://iqq.zhaomingkeji.xyz

[G02] 构造函数
来源：http://qxm.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://dyz.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://zzy.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://zpw.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://xsw.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://grn.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ecf.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://wsm.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://ytx.feifeiyinyue.top

[G03] 实例属性
来源：http://rzt.ivvv.top

Py:   self.name = "x"
来源：http://woi.sysykeji.top

PHP:  public string $name = "x";
来源：http://yeh.hcnkem.com

JS:   this.name = "x";
来源：http://lvt.hammf.cn

TS:   name: string = "x";
来源：http://omw.jyoumei.cn

Java: private String name;
来源：http://vgu.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zrh.shuidangran.top

Ruby: @name = "x"
来源：http://bob.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://ovi.ehwqpu.com

[G04] 定义方法
来源：http://egc.fengsongda.top

Py:   def greet(self): return self.name
来源：http://tbg.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vxj.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://rry.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://kvm.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://xbh.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://zgf.yuanzhike.top

Ruby: def greet; @name; end
来源：http://ipf.bjfxy.top

C#:   public string Greet() => Name;
来源：http://cyt.mhx1999.top

[G05] 继承
来源：http://ojf.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://pdd.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://god.iojbl.cn

JS:   class Admin extends User {}
来源：http://yab.chenzaomai.com

TS:   class Admin extends User {}
来源：http://iov.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://lme.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://brm.jyoumei.cn

Ruby: class Admin < User; end
来源：http://bxe.bjfxy.top

C#:   class Admin : User {}
来源：http://wwh.haohaochexian.top

[G06] 重写方法
来源：http://icj.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://kky.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ocp.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://wea.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://fag.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://qsg.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ijo.kuanghao11.cn

Ruby: def greet; "admin"; end
来源：http://zee.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://lkj.guowangkeji.top

[G07] 调用父类方法
来源：http://bcz.xuetiantiany.cn

Py:   super().greet()
来源：http://nni.shuidangran.top

PHP:  parent::greet();
来源：http://jgu.uphjek.com

JS:   super.greet();
来源：http://zwm.hysaishi.cn

TS:   super.greet();
来源：http://gre.hammf.cn

Java: super.greet();
来源：http://ztg.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vik.ppjwa.cn

Ruby: super
来源：http://cln.yongpay.top

C#:   base.Greet();
来源：http://cdk.dianchejie.cn

[G08] 静态方法与属性
来源：http://cob.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://agx.zhixingplan.top

PHP:  public static function f() {}
来源：http://grx.fktsv.cn

JS:   static f() {}
来源：http://pkj.hongshengwenyu.top

TS:   static f(): void {}
来源：http://ktd.ctjpmb.com

Java: static void f() {}
来源：http://baa.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lyu.zhixingplan.top

Ruby: def self.f; end
来源：http://gay.nwbrower.top

C#:   public static void F() {}
来源：http://zwr.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://uux.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://hal.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://nfz.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://xjh.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://yal.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://ijp.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://dho.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://szn.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://fsw.gotoacloud.top

[G10] 访问控制
来源：http://obg.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://hfq.yj20258888.top

PHP:  public / protected / private
来源：http://jck.xziqi.cn

JS:   #private 字段；其余公开
来源：http://lyi.hcnkem.com

TS:   public / protected / private
来源：http://ogu.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://vhd.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fbx.sjlbkw.cn

Ruby: public / protected / private
来源：http://mqw.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://obr.xylfe.cn

[G11] getter / setter
来源：http://jdm.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://rsb.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://hpx.wangdashe.top

JS:   get name() { return this._name; }
来源：http://cgz.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://vyq.tianlin.xyz

Java: public String getName() { return name; }
来源：http://mkx.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vte.dianchejie.cn

Ruby: attr_accessor :name
来源：http://wps.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://ycj.sufxvd.cn

[G12] 对象转字符串
来源：http://xrl.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://ast.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rkq.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://dqr.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://wpq.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://ovf.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://scy.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://zut.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://hxa.jiagoushi.top

[G13] 判断对象类型
来源：http://rfa.yj20258888.top

Py:   isinstance(u, User)
来源：http://xkw.hcnkem.com

PHP:  $u instanceof User
来源：http://eyf.daxiang520.top

JS:   u instanceof User
来源：http://qpm.sysykeji.top

TS:   u instanceof User
来源：http://dng.xuetiantiany.cn

Java: u instanceof User
来源：http://lkg.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uez.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://dcn.nanxinkj.top

C#:   u is User
来源：http://szl.havefunace.top

[G14] 数据类 / record
来源：http://sbm.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jyk.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://fxo.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://gqr.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://mza.yfazqb.com

Java: record User(String name, int age) {}
来源：http://qdr.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://vvg.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://owg.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://ylj.ywan-chungtsiang.top

[G15] 枚举
来源：http://yyo.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://afc.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dxx.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sfl.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kax.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://ggr.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://etu.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://iqn.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pxl.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://hjd.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mbs.havefunace.top

PHP:  get_object_vars($obj);
来源：http://rsj.cucudq.cn

JS:   Object.entries(obj)
来源：http://pdv.xuanzx.com

TS:   Object.entries(obj)
来源：http://lkm.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zjb.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jlx.smart0.xyz

Ruby: obj.instance_variables
来源：http://ubh.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://qdl.uphjek.com

================================================================================
来源：http://zwd.epnwcf.com

H. 异常与错误处理
来源：http://hks.nwbrower.top

================================================================================
来源：http://kqp.tarul.cn

[H01] try / catch 基础
来源：http://wbq.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pkj.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hzu.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jok.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bnj.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://opc.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://brs.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dpu.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ayk.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://ktl.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sxk.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yjr.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uvp.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xxw.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kev.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hyb.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qfb.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://csl.fengsongda.top

[H03] 主动抛出异常
来源：http://jtf.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://fcn.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dcs.yj20258.top

JS:   throw new Error("错误信息");
来源：http://iec.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://njn.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qgi.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://com.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dlp.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://odh.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://uct.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://lvr.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hqo.redwolf501.top

JS:   class MyError extends Error {}
来源：http://mon.fanxiaobao.xyz

TS:   class MyError extends Error {}
来源：http://nij.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://xjh.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qtb.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://uev.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://srb.bjfxy.top

[H05] 捕获特定类型
来源：http://mrf.zhiwuduotai.top

Py:   except ValueError as e:
来源：http://hze.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xxw.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://daj.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://omn.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://qhr.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zva.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://xdq.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nit.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://ewf.xylfe.cn

Py:   value = d.get("k") or default
来源：http://edm.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nqq.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jyz.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://yqv.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zvi.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sze.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://slb.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://mji.zdqjudy.top

[H07] 断言
来源：http://zcs.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://hai.gotoacloud.top

PHP:  assert($x > 0);
来源：http://sgz.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://sae.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://jmc.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://jkx.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cwb.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://qzp.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://esi.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://jjt.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://uzr.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vbn.guowangkeji.top

JS:   e.message;  e.stack
来源：http://isd.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qzr.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cla.andypj.xyz

Go:   err.Error()
来源：http://vfm.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://thd.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://ylw.jyoumei.cn

[H09] 带错误码的异常
来源：http://gcy.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bwc.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://agr.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fzk.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://npt.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://arv.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zbs.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eoz.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ylj.svipenyu.cn

[H10] 资源自动释放
来源：http://opg.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hpc.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fmf.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qhb.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uej.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kxo.aibaodan.cn

Go:   defer f.Close()
来源：http://lsw.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uqu.redwolf501.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ptw.sysykeji.top

================================================================================
来源：http://bnm.yangfankeji.com

I. 正则表达式
来源：http://opr.jlsjyb.cn

================================================================================
来源：http://gol.zhixingplan.top

[I01] 判断是否匹配
来源：http://alw.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://icw.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://jop.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://ope.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://atj.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ird.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vrr.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://keb.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uzb.zdqjudy.top

[I02] 提取所有匹配
来源：http://phr.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://vgv.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hne.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qmt.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://rzd.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://htv.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xua.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://fwi.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wnu.dashuyun.cn

[I03] 提取捕获分组
来源：http://aqo.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yww.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bjd.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rcx.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qxx.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nmg.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ets.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://btz.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nql.zdqjudy.top

[I04] 正则替换
来源：http://ydd.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bpz.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rgt.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://pbn.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://flm.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://nce.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rmk.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cjj.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wkl.yj20258888.top

[I05] 按正则拆分
来源：http://ajh.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://knj.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sok.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://xoi.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://wig.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://gno.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://huf.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nrn.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ezi.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pwc.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vim.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://viw.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vzy.yj20258.top


<!-- 参考信息 -->