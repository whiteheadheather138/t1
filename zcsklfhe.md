代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pkj.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lxj.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ojr.mhx1999.top

[F12] CSV 读写
来源：http://xim.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ynv.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uoh.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vmo.svipenyu.cn

TS:   // 同上
来源：http://bkj.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xik.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xba.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://chc.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ugh.cqqwz.cn

================================================================================
来源：http://xhm.pengpengdd.cyou

G. 面向对象
来源：http://dvr.zhongyouzk.top

================================================================================
来源：http://vfe.tian-w.cn

[G01] 定义类
来源：http://tok.shuidangran.top

Py:   class User: pass
来源：http://hyn.ivvv.top

PHP:  class User {}
来源：http://uxh.yvedp.cn

JS:   class User {}
来源：http://nyg.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://squ.ehwqpu.com

Java: class User {}
来源：http://ref.yongpay.top

Go:   type User struct { Name string }
来源：http://jmm.daxiang520.top

Ruby: class User; end
来源：http://ljl.shangyingyoupin.top

C#:   class User {}
来源：http://ukd.zycfv.cn

[G02] 构造函数
来源：http://uku.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://tvg.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://fxu.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://smu.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://kyt.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://ptp.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jia.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://jpo.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://xns.daxiang520.top

[G03] 实例属性
来源：http://dej.shuidangran.top

Py:   self.name = "x"
来源：http://prn.yuxming.cn

PHP:  public string $name = "x";
来源：http://dtr.zhiwuduotai.top

JS:   this.name = "x";
来源：http://glz.daxiang520.top

TS:   name: string = "x";
来源：http://juf.shzxlz.cn

Java: private String name;
来源：http://vzg.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rzj.jinqigufen.top

Ruby: @name = "x"
来源：http://eum.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://lvx.redwolf501.top

[G04] 定义方法
来源：http://kud.bjfxy.top

Py:   def greet(self): return self.name
来源：http://yrc.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fex.sxryk.cn

JS:   greet() { return this.name; }
来源：http://zqi.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://rad.zdqjudy.top

Java: String greet() { return name; }
来源：http://hhj.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://iyg.jianghu66.top

Ruby: def greet; @name; end
来源：http://gzx.yongpay.top

C#:   public string Greet() => Name;
来源：http://ggm.xuanzx.com

[G05] 继承
来源：http://jui.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://bmu.wangdashe.top

PHP:  class Admin extends User {}
来源：http://toj.epnwcf.com

JS:   class Admin extends User {}
来源：http://vvm.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://zjk.guowangkeji.top

Java: class Admin extends User {}
来源：http://bgo.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zeq.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://kkq.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://lyo.snrcjt.cn

[G06] 重写方法
来源：http://vko.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://nvk.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mim.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://nqx.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://zrj.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://eoz.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tsj.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://ulm.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://dhc.mhx1999.top

[G07] 调用父类方法
来源：http://wzz.pengpengdd.cyou

Py:   super().greet()
来源：http://ute.tianlin.xyz

PHP:  parent::greet();
来源：http://afd.nanxuanxn.top

JS:   super.greet();
来源：http://eav.bjfxy.top

TS:   super.greet();
来源：http://crx.zhijiandao.cn

Java: super.greet();
来源：http://pfm.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://okv.hnxiangtu.top

Ruby: super
来源：http://ftv.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://lgq.vqdsnc.cn

[G08] 静态方法与属性
来源：http://mwd.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rln.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://kni.andypj.xyz

JS:   static f() {}
来源：http://gko.bjfxy.top

TS:   static f(): void {}
来源：http://rum.pengpengdd.cyou

Java: static void f() {}
来源：http://nln.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://irz.yonumen.top

Ruby: def self.f; end
来源：http://qse.jiagoushi.top

C#:   public static void F() {}
来源：http://kep.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://xuy.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://jfu.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://xrs.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vuf.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://mlk.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://sup.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://oxn.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tni.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://tmk.nanxinkj.top

[G10] 访问控制
来源：http://jxn.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://qar.smart0.xyz

PHP:  public / protected / private
来源：http://drz.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://aws.yuxming.cn

TS:   public / protected / private
来源：http://ehh.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://ljc.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ayd.snrcjt.cn

Ruby: public / protected / private
来源：http://sbc.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://pzg.gotoacloud.top

[G11] getter / setter
来源：http://hqd.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://vss.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://muw.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://fgs.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://zoo.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://xsb.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://ynq.fengsongda.top

Ruby: attr_accessor :name
来源：http://vuu.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://kwd.zdbjq.cn

[G12] 对象转字符串
来源：http://ezl.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://kux.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cxi.yongpay.top

JS:   toString() { return this.name; }
来源：http://tpy.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://pov.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://cky.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zuf.daria6918.cn

Ruby: def to_s; @name; end
来源：http://zlo.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://bos.52xcode.cn

[G13] 判断对象类型
来源：http://mtl.yonumen.top

Py:   isinstance(u, User)
来源：http://xfn.wangdashe.top

PHP:  $u instanceof User
来源：http://vyd.zdqjudy.top

JS:   u instanceof User
来源：http://oib.hcnkem.com

TS:   u instanceof User
来源：http://rmc.chenlongwang.top

Java: u instanceof User
来源：http://yst.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://duj.yonumen.top

Ruby: u.is_a?(User)
来源：http://cfa.feifeiyinyue.top

C#:   u is User
来源：http://snw.chenzaomai.com

[G14] 数据类 / record
来源：http://ufg.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://viw.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://vwn.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fhh.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://zmk.yj20258888.top

Java: record User(String name, int age) {}
来源：http://djx.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://ski.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gyf.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://fdu.sxryk.cn

[G15] 枚举
来源：http://jzq.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nkg.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hne.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://evl.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pab.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://upu.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ala.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://rgw.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://idv.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://mae.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cza.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://asd.aibaodan.cn

JS:   Object.entries(obj)
来源：http://tvi.zdqjudy.top

TS:   Object.entries(obj)
来源：http://dne.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qub.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cnc.meibo888.top

Ruby: obj.instance_variables
来源：http://haa.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://yox.sweek.top

================================================================================
来源：http://tjg.cashguo.top

H. 异常与错误处理
来源：http://qeb.zhixingplan.top

================================================================================
来源：http://oaq.hongshengwenyu.top

[H01] try / catch 基础
来源：http://rju.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://shj.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qsj.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cow.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tlg.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://deg.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lvq.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lgo.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ync.tanke756.top

[H02] finally / ensure 收尾
来源：http://szc.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://cri.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://hsn.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pxy.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://qri.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://ltx.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://omj.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ddl.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://grq.bbcook.cn

[H03] 主动抛出异常
来源：http://ydn.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://hmn.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://psb.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://mom.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://ykz.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jta.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tic.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vtn.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://aml.daria6918.cn

[H04] 自定义异常类型
来源：http://crp.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://dwu.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wla.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://egu.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://xds.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://xhv.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hwo.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://dsy.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://fza.zdbjq.cn

[H05] 捕获特定类型
来源：http://iuw.kuanghao11.cn

Py:   except ValueError as e:
来源：http://ute.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xlb.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://qcs.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://pcu.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://osa.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hal.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://rzk.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://boh.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://xmj.bbcook.cn

Py:   value = d.get("k") or default
来源：http://opy.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gor.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://oyw.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://doo.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ncf.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eqh.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://puk.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://ixv.ivvv.top

[H07] 断言
来源：http://cwe.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://ufr.yuxming.cn

PHP:  assert($x > 0);
来源：http://lzp.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://oqb.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://rbo.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://ywi.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mgw.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://uur.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://jeb.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://sxc.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://gvs.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pcr.uphjek.com

JS:   e.message;  e.stack
来源：http://fry.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qnr.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nkb.xziqi.cn

Go:   err.Error()
来源：http://hhe.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://avj.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://lze.havefunace.top

[H09] 带错误码的异常
来源：http://boj.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dne.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vcm.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yyy.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sio.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gxt.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tpa.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://omw.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yau.tarul.cn

[H10] 资源自动释放
来源：http://itv.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://roj.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dwy.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mgg.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kfq.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qrl.vqdsnc.cn

Go:   defer f.Close()
来源：http://uxp.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://phz.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ngy.tanke756.top

================================================================================
来源：http://bxe.pengpengdd.cyou

I. 正则表达式
来源：http://cue.zdbjq.cn

================================================================================
来源：http://gdh.shuidangran.top

[I01] 判断是否匹配
来源：http://fsa.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oqg.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://cwy.hesvh.cn

JS:   /\d+/.test(s)
来源：http://lnh.jianghu66.top

TS:   /\d+/.test(s)
来源：http://edc.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://din.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://obs.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://ufr.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kxx.yuanzhike.top

[I02] 提取所有匹配
来源：http://xpu.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://aio.tianlin.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://scf.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://veb.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://jrk.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ssz.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ytx.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://mju.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ekp.zdbjq.cn

[I03] 提取捕获分组
来源：http://kzh.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vyo.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rkd.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hwz.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kfb.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jok.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vme.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wur.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tgl.ywan-chungtsiang.top

[I04] 正则替换
来源：http://xtm.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pcc.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dfz.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://auo.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://fer.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://jrl.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zha.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uue.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://apj.xylfe.cn

[I05] 按正则拆分
来源：http://ntv.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://frt.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xdr.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vwo.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://ehj.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://frc.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tzi.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://sbz.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jwt.shanyushiyangtech.top


<!-- 参考信息 -->