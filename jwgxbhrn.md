代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fqj.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bwm.jiagoushi.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fij.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ehv.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zwc.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fcy.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vtc.cqqwz.cn

[F12] CSV 读写
来源：http://coc.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wsg.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vkc.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ane.dashuyun.cn

TS:   // 同上
来源：http://qlw.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dju.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cqn.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ubo.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://avb.bbcook.cn

================================================================================
来源：http://vvg.ydzc1.top

G. 面向对象
来源：http://ifq.sweek.top

================================================================================
来源：http://kmj.fengsongda.top

[G01] 定义类
来源：http://ggf.ctjpmb.com

Py:   class User: pass
来源：http://skh.hnqzz.top

PHP:  class User {}
来源：http://aie.epnwcf.com

JS:   class User {}
来源：http://vnt.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://zod.ctjpmb.com

Java: class User {}
来源：http://kyq.bjfxy.top

Go:   type User struct { Name string }
来源：http://iyp.cheryme.top

Ruby: class User; end
来源：http://pte.jinyuanbaomall.cn

C#:   class User {}
来源：http://jtl.fengsongda.top

[G02] 构造函数
来源：http://ckl.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://xuy.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://fal.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://qty.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://zge.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://hll.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zkr.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://qin.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://sex.tarul.cn

[G03] 实例属性
来源：http://pqm.kuanghao11.cn

Py:   self.name = "x"
来源：http://qgb.bbcook.cn

PHP:  public string $name = "x";
来源：http://jsp.yj20258888.top

JS:   this.name = "x";
来源：http://mso.yonumen.top

TS:   name: string = "x";
来源：http://nfr.yfazqb.com

Java: private String name;
来源：http://bqq.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xra.jyoumei.cn

Ruby: @name = "x"
来源：http://aqq.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://loz.shanyushiyangkeji.top

[G04] 定义方法
来源：http://ohk.yfazqb.com

Py:   def greet(self): return self.name
来源：http://fiq.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://qne.c1oappe.top

JS:   greet() { return this.name; }
来源：http://ahh.sweek.top

TS:   greet(): string { return this.name; }
来源：http://eme.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://thw.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://top.epnwcf.com

Ruby: def greet; @name; end
来源：http://fpz.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://znc.zhixingplan.top

[G05] 继承
来源：http://pbd.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://ejf.sxryk.cn

PHP:  class Admin extends User {}
来源：http://whm.snrcjt.cn

JS:   class Admin extends User {}
来源：http://sir.hfpthk.cn

TS:   class Admin extends User {}
来源：http://gii.fzhhl.top

Java: class Admin extends User {}
来源：http://bah.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://euw.ppjwa.cn

Ruby: class Admin < User; end
来源：http://wuf.zdqjudy.top

C#:   class Admin : User {}
来源：http://bpy.bjfxy.top

[G06] 重写方法
来源：http://jrn.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://cdv.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://reg.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://luw.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://quw.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://eeb.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aex.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://yez.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://nfv.ydjk.org.cn

[G07] 调用父类方法
来源：http://iiz.zhaomingkeji.xyz

Py:   super().greet()
来源：http://rxt.yfazqb.com

PHP:  parent::greet();
来源：http://ghf.jinqigfzy.top

JS:   super.greet();
来源：http://llw.hongshengwenyu.top

TS:   super.greet();
来源：http://mlk.52xcode.cn

Java: super.greet();
来源：http://xzu.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kkp.yj20258.top

Ruby: super
来源：http://hln.yangfankeji.com

C#:   base.Greet();
来源：http://aur.ehwqpu.com

[G08] 静态方法与属性
来源：http://xoz.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kbf.snrcjt.cn

PHP:  public static function f() {}
来源：http://zkv.tanke756.top

JS:   static f() {}
来源：http://wqo.zdqjudy.top

TS:   static f(): void {}
来源：http://jgz.zhongyouzk.top

Java: static void f() {}
来源：http://lmt.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gxo.yueranfly.top

Ruby: def self.f; end
来源：http://gqs.tianlin.xyz

C#:   public static void F() {}
来源：http://fxe.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://tez.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://tow.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://cgm.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://whp.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://doc.hammf.cn

Java: interface Shape { double area(); }
来源：http://kcq.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://kcc.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zjo.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://ovk.wangdashe.top

[G10] 访问控制
来源：http://kqw.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://wys.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://sct.zhiwuduotai.top

JS:   #private 字段；其余公开
来源：http://rxn.aibaodan.cn

TS:   public / protected / private
来源：http://lsy.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://tqv.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lcu.chenjidiqi.icu

Ruby: public / protected / private
来源：http://geb.sxryk.cn

C#:   public / protected / private / internal
来源：http://ycj.yj202588.top

[G11] getter / setter
来源：http://jlx.iojbl.cn

Py:   @property 与 @x.setter
来源：http://cfs.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oka.fzhhl.top

JS:   get name() { return this._name; }
来源：http://mnd.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://tat.uphjek.com

Java: public String getName() { return name; }
来源：http://owd.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vmd.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://lgi.cashguo.top

C#:   public string Name { get; set; }
来源：http://lgh.wangshuangyany.cn

[G12] 对象转字符串
来源：http://ydk.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://ekk.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jlh.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://kcu.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://dul.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://pxi.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://aol.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://ywj.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://wut.fzhhl.top

[G13] 判断对象类型
来源：http://qlz.chenzaomai.com

Py:   isinstance(u, User)
来源：http://sjd.jianghu66.top

PHP:  $u instanceof User
来源：http://cpx.0kj1m.cn

JS:   u instanceof User
来源：http://kar.andypj.xyz

TS:   u instanceof User
来源：http://woc.hcnkem.com

Java: u instanceof User
来源：http://cxc.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fkv.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://izc.redwolf501.top

C#:   u is User
来源：http://uqh.jlsjyb.cn

[G14] 数据类 / record
来源：http://dds.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wgm.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://rzs.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://lop.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://ats.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://msj.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://aeb.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qfp.kuanghao11.cn

C#:   record User(string Name, int Age);
来源：http://omq.zycfv.cn

[G15] 枚举
来源：http://lqb.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ais.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zse.jinqigufen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dkb.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yme.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://ghw.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ybx.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://ahc.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bzt.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://bwc.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://njz.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://oiy.zhengqikj.top

JS:   Object.entries(obj)
来源：http://nop.nanxinkj.top

TS:   Object.entries(obj)
来源：http://rzv.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sol.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gfv.haohaochexian.top

Ruby: obj.instance_variables
来源：http://wbp.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://hyw.chenjidiqi.icu

================================================================================
来源：http://ctl.shanyushiyangtech.top

H. 异常与错误处理
来源：http://bwb.xylfe.cn

================================================================================
来源：http://ufj.wangdashe.top

[H01] try / catch 基础
来源：http://fub.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ixc.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://imj.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://las.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vxu.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kmw.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qki.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wdj.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jiw.xziqi.cn

[H02] finally / ensure 收尾
来源：http://vfi.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://xvl.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gbx.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lbu.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yvj.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xfg.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://amj.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ckm.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gjl.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://fbp.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://ryn.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ggv.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://ugs.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://gsa.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fxj.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gob.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yiv.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jto.vehdjk.com

[H04] 自定义异常类型
来源：http://rtk.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://cyy.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://wyd.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://awb.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://yad.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://fgb.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oie.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://nyo.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://rot.kuanghao11.cn

[H05] 捕获特定类型
来源：http://jrk.jinqigfzy.top

Py:   except ValueError as e:
来源：http://wdw.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dfq.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://tlm.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://vjy.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://ovi.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uux.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://oad.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jae.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://zgg.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://kzp.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://bip.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://kwe.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vol.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vpk.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ezy.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://sfq.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://ozg.gzhubu.top

[H07] 断言
来源：http://cds.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://xgu.iojbl.cn

PHP:  assert($x > 0);
来源：http://mva.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://kqc.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://ynx.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://nmz.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jmp.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yyx.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://ufn.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://ltd.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://skz.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jvj.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://geu.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fjz.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hvp.cheryme.top

Go:   err.Error()
来源：http://web.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://ajs.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://pft.kuanghao11.cn

[H09] 带错误码的异常
来源：http://onv.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ncs.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://blm.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fpq.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://erg.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zsl.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gwx.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://csi.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uxv.fktsv.cn

[H10] 资源自动释放
来源：http://zpb.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pqi.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://few.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qgc.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wzg.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vxr.smart0.xyz

Go:   defer f.Close()
来源：http://vkl.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qej.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qtw.vqdsnc.cn

================================================================================
来源：http://qcd.ppjwa.cn

I. 正则表达式
来源：http://uje.jinyuanbaomall.cn

================================================================================
来源：http://mpn.jlsjyb.cn

[I01] 判断是否匹配
来源：http://gaf.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mno.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://kry.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://brk.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://pfa.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wri.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ibr.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://uxf.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://voy.cheryme.top

[I02] 提取所有匹配
来源：http://bse.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://ahe.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fxn.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://crk.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://ttl.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kvb.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zwy.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://uso.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://acr.nwbrower.top

[I03] 提取捕获分组
来源：http://xzc.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://twm.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blt.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jsr.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fwo.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vwt.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ftq.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lli.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uuj.bjfxy.top

[I04] 正则替换
来源：http://zll.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://pve.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fhk.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ajz.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://kfq.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://ypc.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uud.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ezr.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hvu.ehwqpu.com

[I05] 按正则拆分
来源：http://vkw.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kmm.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lco.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://xdk.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://ukj.xingfuxueyuan.xyz


<!-- 参考信息 -->