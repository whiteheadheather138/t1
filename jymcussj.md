代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pqp.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uik.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kwt.svipenyu.cn

[F12] CSV 读写
来源：http://ioe.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gia.haohaochexian.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://syx.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ufo.shzxlz.cn

TS:   // 同上
来源：http://pil.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://koo.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jwg.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://phg.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bua.cashguo.top

================================================================================
来源：http://pbq.daxiang520.top

G. 面向对象
来源：http://jfx.zhengqikj.top

================================================================================
来源：http://ogv.uphjek.com

[G01] 定义类
来源：http://zrw.gaohongyu789.top

Py:   class User: pass
来源：http://gjs.yuxming.cn

PHP:  class User {}
来源：http://lvv.tarul.cn

JS:   class User {}
来源：http://riw.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://bwm.jinghuilouyu.cn

Java: class User {}
来源：http://jnb.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://ihg.feifeiyinyue.top

Ruby: class User; end
来源：http://tlz.zhengqikj.top

C#:   class User {}
来源：http://xdw.cqqwz.cn

[G02] 构造函数
来源：http://nmq.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://fnt.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://vvg.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://uue.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://gkz.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://lhq.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://phi.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://hym.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://bjz.hongshengwenyu.top

[G03] 实例属性
来源：http://sob.ppjwa.cn

Py:   self.name = "x"
来源：http://inz.jyoumei.cn

PHP:  public string $name = "x";
来源：http://eea.cucudq.cn

JS:   this.name = "x";
来源：http://hpw.jlsjyb.cn

TS:   name: string = "x";
来源：http://oni.fehbvm.com

Java: private String name;
来源：http://hwu.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xwf.hcnkem.com

Ruby: @name = "x"
来源：http://abp.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://fli.sweek.top

[G04] 定义方法
来源：http://fli.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://rso.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rxs.fktsv.cn

JS:   greet() { return this.name; }
来源：http://flo.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://gbh.bbcook.cn

Java: String greet() { return name; }
来源：http://iry.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yic.havefunace.top

Ruby: def greet; @name; end
来源：http://kub.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://tjb.shangyingyoupin.top

[G05] 继承
来源：http://sko.xuanzx.com

Py:   class Admin(User): pass
来源：http://amc.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://kek.hammf.cn

JS:   class Admin extends User {}
来源：http://gja.havefunace.top

TS:   class Admin extends User {}
来源：http://bhh.ppjwa.cn

Java: class Admin extends User {}
来源：http://rav.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dkk.ehwqpu.com

Ruby: class Admin < User; end
来源：http://fhs.iojbl.cn

C#:   class Admin : User {}
来源：http://rgl.0kj1m.cn

[G06] 重写方法
来源：http://pdb.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://xmx.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eop.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://sjz.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://gyg.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://llo.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fsd.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://kue.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://acz.9152youxi.cn

[G07] 调用父类方法
来源：http://kay.jinghuilouyu.cn

Py:   super().greet()
来源：http://lyd.zhoulong.xyz

PHP:  parent::greet();
来源：http://dao.aizwys.cn

JS:   super.greet();
来源：http://wvr.epnwcf.com

TS:   super.greet();
来源：http://aoo.smart0.xyz

Java: super.greet();
来源：http://ekx.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://umx.cdnleiting.top

Ruby: super
来源：http://oqz.hongshengwenyu.top

C#:   base.Greet();
来源：http://fax.cheryme.top

[G08] 静态方法与属性
来源：http://dgv.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://piz.daxiang520.top

PHP:  public static function f() {}
来源：http://jzb.dianchejie.cn

JS:   static f() {}
来源：http://hij.xuanzx.com

TS:   static f(): void {}
来源：http://uep.zhaomingkeji.xyz

Java: static void f() {}
来源：http://nzp.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ujs.xuanzx.com

Ruby: def self.f; end
来源：http://hiv.hammf.cn

C#:   public static void F() {}
来源：http://edi.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://rht.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://irn.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hhj.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zkk.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://rmh.xuanzx.com

Java: interface Shape { double area(); }
来源：http://yuq.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://iho.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pcx.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://mhy.jinghuilouyu.cn

[G10] 访问控制
来源：http://xum.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://bjs.sjlbkw.cn

PHP:  public / protected / private
来源：http://zdt.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://dok.gotoacloud.top

TS:   public / protected / private
来源：http://bri.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://lqf.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bim.sysykeji.top

Ruby: public / protected / private
来源：http://hbu.jianghu66.top

C#:   public / protected / private / internal
来源：http://jbq.tianlin.xyz

[G11] getter / setter
来源：http://kjc.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://sug.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pfq.pycfn.com

JS:   get name() { return this._name; }
来源：http://xbb.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://edc.smart0.xyz

Java: public String getName() { return name; }
来源：http://yff.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ktv.yj202588.top

Ruby: attr_accessor :name
来源：http://uvv.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://oah.bbcook.cn

[G12] 对象转字符串
来源：http://ehn.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://ywq.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qpj.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://sqz.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://hpc.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://ocp.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://wrh.hesvh.cn

Ruby: def to_s; @name; end
来源：http://ggb.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://vbs.feifeiyinyue.top

[G13] 判断对象类型
来源：http://ksj.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://nsr.andypj.xyz

PHP:  $u instanceof User
来源：http://fof.tianlin.xyz

JS:   u instanceof User
来源：http://wpo.jinqigufen.top

TS:   u instanceof User
来源：http://nwg.xinyue.icu

Java: u instanceof User
来源：http://inn.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://dmw.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://cky.zhengqikj.top

C#:   u is User
来源：http://hom.epnwcf.com

[G14] 数据类 / record
来源：http://cyj.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kff.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ukn.zhijiandao.cn

JS:   // 无内置：普通类或对象字面量
来源：http://htm.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://ytt.hnqzz.top

Java: record User(String name, int age) {}
来源：http://pud.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://bpl.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://doy.yj20258.top

C#:   record User(string Name, int Age);
来源：http://xgy.hesvh.cn

[G15] 枚举
来源：http://dkh.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dev.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://khd.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fkw.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qdu.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://lgh.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbc.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://osx.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fmn.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://hta.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sfx.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://ofo.nanxinkj.top

JS:   Object.entries(obj)
来源：http://sth.svipenyu.cn

TS:   Object.entries(obj)
来源：http://lvm.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fdk.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ypk.hysaishi.cn

Ruby: obj.instance_variables
来源：http://gds.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://zoe.zdqjudy.top

================================================================================
来源：http://yki.c1oappe.top

H. 异常与错误处理
来源：http://saw.shzxlz.cn

================================================================================
来源：http://kxy.jinqigfzy.top

[H01] try / catch 基础
来源：http://lkl.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rkv.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://krw.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xur.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kfd.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tjg.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nvr.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://crj.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://har.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://ngl.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://lhd.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://yly.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://huw.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fad.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uus.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://txd.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zjs.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ywy.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://cjk.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://dyb.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eeq.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://klb.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://cxb.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cun.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lss.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hde.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://nzs.ydjk.org.cn

[H04] 自定义异常类型
来源：http://jlt.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://thu.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://efq.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://qpb.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://mwp.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://nzz.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mrz.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://phz.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://spq.xinyue.icu

[H05] 捕获特定类型
来源：http://epx.xylfe.cn

Py:   except ValueError as e:
来源：http://vge.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dpy.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://rlf.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://sep.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://rgk.hesvh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://upf.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://lzh.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ffu.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://tsu.redwolf501.top

Py:   value = d.get("k") or default
来源：http://cyx.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://amh.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://irp.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://ihp.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vvu.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://obr.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://buq.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://cfp.ivvv.top

[H07] 断言
来源：http://mqn.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://smd.dianchejie.cn

PHP:  assert($x > 0);
来源：http://lrt.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://pdg.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://wal.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://egm.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jvi.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ltk.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://sle.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://ldi.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://rya.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yiq.xylfe.cn

JS:   e.message;  e.stack
来源：http://ipt.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ket.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sdl.andypj.xyz

Go:   err.Error()
来源：http://leb.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://ica.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://pzk.yuanzhike.top

[H09] 带错误码的异常
来源：http://xxg.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wwv.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://zub.zhaomingkeji.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xub.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lpg.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ngt.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ofh.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://oon.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ydr.pengpengdd.cyou

[H10] 资源自动释放
来源：http://tcj.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vok.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oth.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gqq.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://scg.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nfx.guowangkeji.top

Go:   defer f.Close()
来源：http://iff.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vfp.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://flp.andypj.xyz

================================================================================
来源：http://jrv.mhx1999.top

I. 正则表达式
来源：http://cws.shanyushiyangtech.top

================================================================================
来源：http://ghz.yanxiufei.cn

[I01] 判断是否匹配
来源：http://egn.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://odj.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://xqr.epnwcf.com

JS:   /\d+/.test(s)
来源：http://ykj.xylfe.cn

TS:   /\d+/.test(s)
来源：http://ptf.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rjk.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qni.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://fzt.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ngv.zhoulong.xyz

[I02] 提取所有匹配
来源：http://tlp.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://alh.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://muo.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zbm.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://hbd.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ren.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rgs.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://wfo.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hmz.316326.xyz

[I03] 提取捕获分组
来源：http://hrt.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://epk.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fwr.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nxa.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qvl.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://srl.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpi.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ciz.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eio.gaohongyu789.top

[I04] 正则替换
来源：http://vdl.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rch.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bbp.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xbf.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wel.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://aph.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yeo.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oxd.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jwb.hammf.cn

[I05] 按正则拆分
来源：http://pnu.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lbp.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ppu.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://vru.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://efm.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://ofv.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pac.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://xlw.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mpa.yongpay.top


<!-- 参考信息 -->