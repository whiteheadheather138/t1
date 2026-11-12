代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yvf.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ato.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cuw.fengsongda.top

[F12] CSV 读写
来源：http://mql.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dpp.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://igm.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kvm.yanxiufei.cn

TS:   // 同上
来源：http://fne.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vri.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kyo.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zqa.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fjo.zhijiandao.cn

================================================================================
来源：http://fcz.shangyingyoupin.top

G. 面向对象
来源：http://hat.daxiang520.top

================================================================================
来源：http://yhu.zhoulong.xyz

[G01] 定义类
来源：http://whr.cheryme.top

Py:   class User: pass
来源：http://nyj.guannengcc.top

PHP:  class User {}
来源：http://vkb.daria6918.cn

JS:   class User {}
来源：http://fhz.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://eny.daxiang520.top

Java: class User {}
来源：http://sfj.nanxinkj.top

Go:   type User struct { Name string }
来源：http://ooz.tian-w.cn

Ruby: class User; end
来源：http://vld.aizwys.cn

C#:   class User {}
来源：http://idm.hnxiangtu.top

[G02] 构造函数
来源：http://ofo.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://exr.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://ofn.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://sgq.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://aid.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://atn.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rps.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://wja.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://ckb.redwolf501.top

[G03] 实例属性
来源：http://hng.jlsjyb.cn

Py:   self.name = "x"
来源：http://jjh.aizwys.cn

PHP:  public string $name = "x";
来源：http://ofp.zhiwuduotai.top

JS:   this.name = "x";
来源：http://ctk.gogol.net.cn

TS:   name: string = "x";
来源：http://rfh.ywan-chungtsiang.top

Java: private String name;
来源：http://owq.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vhn.pengpengdd.cyou

Ruby: @name = "x"
来源：http://whn.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://yad.kuanghao11.cn

[G04] 定义方法
来源：http://fti.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://cev.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tsp.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://idk.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://fpd.ehwqpu.com

Java: String greet() { return name; }
来源：http://ped.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kxr.iojbl.cn

Ruby: def greet; @name; end
来源：http://amf.redwolf501.top

C#:   public string Greet() => Name;
来源：http://wth.zdqjudy.top

[G05] 继承
来源：http://vyd.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://cyq.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://zlf.yangfankeji.com

JS:   class Admin extends User {}
来源：http://hmb.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://tqh.shzxlz.cn

Java: class Admin extends User {}
来源：http://sdg.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ekn.jianghu66.top

Ruby: class Admin < User; end
来源：http://ixs.fengsongda.top

C#:   class Admin : User {}
来源：http://jng.xylfe.cn

[G06] 重写方法
来源：http://duo.hammf.cn

Py:   def greet(self): return "admin"
来源：http://cza.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://aje.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://cyu.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://sks.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://wdg.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ezr.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://vir.ybcxt.top

C#:   public override string Greet() => "admin";
来源：http://llk.redwolf501.top

[G07] 调用父类方法
来源：http://mgc.dianchejie.cn

Py:   super().greet()
来源：http://eok.xuetiantiany.cn

PHP:  parent::greet();
来源：http://qyx.shanyushiyangtech.top

JS:   super.greet();
来源：http://qiz.xinyue.icu

TS:   super.greet();
来源：http://sqq.52xcode.cn

Java: super.greet();
来源：http://gif.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://flw.yangfankeji.com

Ruby: super
来源：http://htl.guannengcc.top

C#:   base.Greet();
来源：http://ubn.nanxuanxn.top

[G08] 静态方法与属性
来源：http://raa.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ayl.yuxming.cn

PHP:  public static function f() {}
来源：http://hfw.shuidangran.top

JS:   static f() {}
来源：http://csi.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://qhj.jqgufenzy.top

Java: static void f() {}
来源：http://ujl.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kkr.svipenyu.cn

Ruby: def self.f; end
来源：http://gce.uphjek.com

C#:   public static void F() {}
来源：http://uue.hcnkem.com

[G09] 接口 / 抽象类
来源：http://huo.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://zed.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://uoh.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ghl.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://hgs.fktsv.cn

Java: interface Shape { double area(); }
来源：http://gmz.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://ics.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://irt.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://sll.shanyushiyangkeji.top

[G10] 访问控制
来源：http://jym.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://yxo.hysaishi.cn

PHP:  public / protected / private
来源：http://tlx.yuxming.cn

JS:   #private 字段；其余公开
来源：http://lxt.ehwqpu.com

TS:   public / protected / private
来源：http://urd.yonumen.top

Java: public / protected / private / 默认包级
来源：http://jyl.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vsy.ehwqpu.com

Ruby: public / protected / private
来源：http://wve.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://rzj.quarkkingdee.top

[G11] getter / setter
来源：http://tov.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://lvn.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xio.ybcxt.top

JS:   get name() { return this._name; }
来源：http://hhj.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://hwl.andypj.xyz

Java: public String getName() { return name; }
来源：http://ffx.wangdashe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cmd.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://jtu.hesvh.cn

C#:   public string Name { get; set; }
来源：http://yvb.sufxvd.cn

[G12] 对象转字符串
来源：http://tgq.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://spu.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fni.ybcxt.top

JS:   toString() { return this.name; }
来源：http://hvu.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://ztf.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://jfz.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://uel.yj20258888.top

Ruby: def to_s; @name; end
来源：http://wyj.sweek.top

C#:   public override string ToString() => Name;
来源：http://pwi.sufxvd.cn

[G13] 判断对象类型
来源：http://dul.nanxinkj.top

Py:   isinstance(u, User)
来源：http://fjj.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://pku.ydjk.org.cn

JS:   u instanceof User
来源：http://rvq.shangyingyoupin.top

TS:   u instanceof User
来源：http://fus.nanxinkj.top

Java: u instanceof User
来源：http://qyk.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eqv.sysykeji.top

Ruby: u.is_a?(User)
来源：http://wbl.cashguo.top

C#:   u is User
来源：http://yjd.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://dtp.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://isq.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://ler.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://afn.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://mbo.redwolf501.top

Java: record User(String name, int age) {}
来源：http://ncc.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://hka.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zsl.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://bca.guowangkeji.top

[G15] 枚举
来源：http://kza.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uut.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ezv.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ldi.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jrv.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://rpl.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://spy.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://okl.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lya.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://zrt.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xcl.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://cvd.sufxvd.cn

JS:   Object.entries(obj)
来源：http://cjz.dianchejie.cn

TS:   Object.entries(obj)
来源：http://mlh.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://log.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://die.ydzc1.top

Ruby: obj.instance_variables
来源：http://vtn.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://fck.pengpengdd.cyou

================================================================================
来源：http://upa.fehbvm.com

H. 异常与错误处理
来源：http://pgl.fzhhl.top

================================================================================
来源：http://uuw.c1oappe.top

[H01] try / catch 基础
来源：http://clw.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eyp.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yci.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://usl.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ayi.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nac.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kwp.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dwq.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vqn.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://xwv.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://oeg.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jam.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qhm.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://cpc.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://lve.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://vzr.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hsh.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://xwq.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://lvz.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://bxw.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fty.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://awo.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://tif.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tnz.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rnv.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://amp.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://hku.hesvh.cn

[H04] 自定义异常类型
来源：http://hqc.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://dgk.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yfg.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://cit.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://ckx.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://mxe.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uhg.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://aia.bbcook.cn

C#:   class MyException : Exception {}
来源：http://jcp.tian-w.cn

[H05] 捕获特定类型
来源：http://vmq.haohaochexian.top

Py:   except ValueError as e:
来源：http://ocv.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bxk.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://gjc.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://jtr.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://wnd.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bec.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://bxf.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nie.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://knx.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://npw.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://inw.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://flr.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://jpo.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hwx.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fdm.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://flc.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://mzx.bbcook.cn

[H07] 断言
来源：http://iow.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://atn.tian-w.cn

PHP:  assert($x > 0);
来源：http://yfe.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://rcf.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://onp.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://ilj.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://juh.jiagoushi.top

Ruby: raise "必须为正" unless x > 0
来源：http://cjb.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://ubl.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://lar.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://kyp.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xeh.jiagoushi.top

JS:   e.message;  e.stack
来源：http://mpf.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://nva.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pvn.zhoulong.xyz

Go:   err.Error()
来源：http://nah.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://xox.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://gyu.yj202588.top

[H09] 带错误码的异常
来源：http://bhm.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wym.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://noc.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gsr.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ava.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://deg.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://onp.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bfv.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yzx.xuanzx.com

[H10] 资源自动释放
来源：http://ksh.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eun.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hdw.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eco.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jel.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ukl.jinqigfzy.top

Go:   defer f.Close()
来源：http://gbt.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zvu.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fnh.tian-w.cn

================================================================================
来源：http://ixw.ywan-chungtsiang.top

I. 正则表达式
来源：http://ijy.fanxiaobao.xyz

================================================================================
来源：http://oyj.jinqigfzy.top

[I01] 判断是否匹配
来源：http://xzf.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uzj.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kot.yj20258.top

JS:   /\d+/.test(s)
来源：http://sll.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://wke.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hxt.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bqk.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://ufn.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ajq.bjfxy.top

[I02] 提取所有匹配
来源：http://isx.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://dko.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xwi.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qlz.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://ruc.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hhl.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vsy.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://tjm.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nyq.zhijiandao.cn

[I03] 提取捕获分组
来源：http://lfl.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tuw.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://who.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ckx.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://anb.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hfv.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pne.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gpw.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://alo.jqgufenzy.top

[I04] 正则替换
来源：http://kam.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://sev.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://axi.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qmh.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kyz.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ezj.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lmm.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zgi.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mte.fzhhl.top

[I05] 按正则拆分
来源：http://dhx.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dig.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xzj.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://rmh.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://cqq.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://mpz.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dsz.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tkk.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iaz.0kj1m.cn


<!-- 参考信息 -->