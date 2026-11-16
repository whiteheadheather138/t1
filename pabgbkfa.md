代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pjs.yj20258888.top

TS:   path.extname("a.txt")
来源：http://pjt.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fmd.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vel.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://asc.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://udl.zhengqikj.top

[F11] 复制与移动文件
来源：http://qjq.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ulc.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tsu.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hqg.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ald.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ouj.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tyw.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pcv.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://adb.yvedp.cn

[F12] CSV 读写
来源：http://dap.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ndf.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gnv.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lwp.xziqi.cn

TS:   // 同上
来源：http://azb.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fjn.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cyh.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qgq.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://thn.gotoacloud.top

================================================================================
来源：http://brf.xuanzx.com

G. 面向对象
来源：http://spu.ivvv.top

================================================================================
来源：http://wqu.yonumen.top

[G01] 定义类
来源：http://tbd.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://oxd.yongpay.top

PHP:  class User {}
来源：http://twk.quarkkingdee.top

JS:   class User {}
来源：http://pdk.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://mux.52xcode.cn

Java: class User {}
来源：http://rxl.redwolf501.top

Go:   type User struct { Name string }
来源：http://tcz.fanxiaobao.xyz

Ruby: class User; end
来源：http://aty.zhiwuduotai.top

C#:   class User {}
来源：http://fsh.yj20258.top

[G02] 构造函数
来源：http://nng.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://ksp.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://drj.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://iov.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://ghn.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://ocw.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sql.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://uuu.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://ayg.jinqigufen.top

[G03] 实例属性
来源：http://nut.svipenyu.cn

Py:   self.name = "x"
来源：http://wuu.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://ius.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://cte.gzhubu.top

TS:   name: string = "x";
来源：http://kku.xziqi.cn

Java: private String name;
来源：http://rtk.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qos.hysaishi.cn

Ruby: @name = "x"
来源：http://usd.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://ppa.quarkkingdee.top

[G04] 定义方法
来源：http://dit.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://ewx.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://apg.yj20258.top

JS:   greet() { return this.name; }
来源：http://rny.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://oyp.c1oappe.top

Java: String greet() { return name; }
来源：http://vxs.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jww.jyoumei.cn

Ruby: def greet; @name; end
来源：http://ihm.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://xby.hesvh.cn

[G05] 继承
来源：http://ymo.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://uyo.vehdjk.com

PHP:  class Admin extends User {}
来源：http://aas.hfpthk.cn

JS:   class Admin extends User {}
来源：http://mls.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://jxe.gotoacloud.top

Java: class Admin extends User {}
来源：http://vlc.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uan.yueranfly.top

Ruby: class Admin < User; end
来源：http://ddv.yvedp.cn

C#:   class Admin : User {}
来源：http://utk.shanyushiyangkeji.top

[G06] 重写方法
来源：http://ajj.birdmap.top

Py:   def greet(self): return "admin"
来源：http://ath.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jrs.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://jez.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://ick.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://cij.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lrn.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://ets.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://syv.dashuyun.cn

[G07] 调用父类方法
来源：http://hzn.yfazqb.com

Py:   super().greet()
来源：http://myb.jinqigufen.top

PHP:  parent::greet();
来源：http://kbd.snrcjt.cn

JS:   super.greet();
来源：http://yei.cucudq.cn

TS:   super.greet();
来源：http://mfz.hfpthk.cn

Java: super.greet();
来源：http://ryl.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://svb.daxiang520.top

Ruby: super
来源：http://lpk.ydjk.org.cn

C#:   base.Greet();
来源：http://tgy.yj202588.top

[G08] 静态方法与属性
来源：http://obl.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bqx.ydzc1.top

PHP:  public static function f() {}
来源：http://tbb.shuidangran.top

JS:   static f() {}
来源：http://fqd.gogol.net.cn

TS:   static f(): void {}
来源：http://iky.hnqzz.top

Java: static void f() {}
来源：http://wjf.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nwp.yuanzhike.top

Ruby: def self.f; end
来源：http://tlx.zhongyouzk.top

C#:   public static void F() {}
来源：http://vzv.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://qms.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://opj.smart0.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ijf.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zxr.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://anx.ybcxt.top

Java: interface Shape { double area(); }
来源：http://ynp.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://wba.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xfo.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://vkn.tianlin.xyz

[G10] 访问控制
来源：http://css.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://imn.yuxming.cn

PHP:  public / protected / private
来源：http://kyv.pycfn.com

JS:   #private 字段；其余公开
来源：http://qcn.tanke756.top

TS:   public / protected / private
来源：http://bqz.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://xds.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wor.ppjwa.cn

Ruby: public / protected / private
来源：http://cfn.haohaochexian.top

C#:   public / protected / private / internal
来源：http://yil.chenlongwang.top

[G11] getter / setter
来源：http://uty.jqgfzy.top

Py:   @property 与 @x.setter
来源：http://uiu.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nyc.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://ziv.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://vil.shzxlz.cn

Java: public String getName() { return name; }
来源：http://ptt.redwolf501.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jpy.jyoumei.cn

Ruby: attr_accessor :name
来源：http://vrn.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://lfb.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://vsw.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://jvs.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bag.yuxming.cn

JS:   toString() { return this.name; }
来源：http://zai.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://onp.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://tii.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://shx.nwbrower.top

Ruby: def to_s; @name; end
来源：http://zsr.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://wyw.zhengqikj.top

[G13] 判断对象类型
来源：http://mri.guowangkeji.top

Py:   isinstance(u, User)
来源：http://iko.gogol.net.cn

PHP:  $u instanceof User
来源：http://nag.cdnleiting.top

JS:   u instanceof User
来源：http://lhs.yj20258888.top

TS:   u instanceof User
来源：http://jgd.ivvv.top

Java: u instanceof User
来源：http://uhb.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nlj.aizwys.cn

Ruby: u.is_a?(User)
来源：http://vjl.andypj.xyz

C#:   u is User
来源：http://hsp.sweek.top

[G14] 数据类 / record
来源：http://ool.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dix.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://pck.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://rzd.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://tqt.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://ghq.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://rxa.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tso.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://grj.redwolf501.top

[G15] 枚举
来源：http://hwe.gogol.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wyp.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rqd.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dvm.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gyf.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://wuv.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eql.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://ogp.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mun.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://nzd.sxryk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qjt.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://smq.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://ljp.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://uwo.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://plm.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xwz.jianghu66.top

Ruby: obj.instance_variables
来源：http://srl.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://fwa.mhx1999.top

================================================================================
来源：http://zvu.jqgfzy.top

H. 异常与错误处理
来源：http://ual.jinqigufen.top

================================================================================
来源：http://dyi.dashuyun.cn

[H01] try / catch 基础
来源：http://tsk.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xis.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kuf.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sqt.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hwa.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ypt.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://boy.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zfg.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vkg.jianghu66.top

[H02] finally / ensure 收尾
来源：http://iys.fehbvm.com

Py:   try: f()⏎finally: cleanup()
来源：http://fzc.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://osp.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ssm.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bvo.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://pld.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nxp.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ipz.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://qjb.chenlongwang.top

[H03] 主动抛出异常
来源：http://vrp.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://ehp.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hib.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://pwj.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://mfh.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ytx.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gsw.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dyp.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://pvg.birdmap.top

[H04] 自定义异常类型
来源：http://lzz.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://kyt.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sqp.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://sko.yj202588.top

TS:   class MyError extends Error {}
来源：http://vfr.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://jsf.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lzu.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://krh.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://xmf.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://cyl.hnxiangtu.top

Py:   except ValueError as e:
来源：http://vwr.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wtq.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://bkt.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://mqq.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://ekn.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hxy.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://vtb.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kwy.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://pim.mhx1999.top

Py:   value = d.get("k") or default
来源：http://uir.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yvu.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://ypp.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://hkb.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ael.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://atv.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://jrx.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://imk.iojbl.cn

[H07] 断言
来源：http://lbs.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://ugi.fktsv.cn

PHP:  assert($x > 0);
来源：http://rok.c1oappe.top

JS:   console.assert(x > 0);
来源：http://ssc.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://ali.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://xye.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bpi.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wje.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://eph.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://elu.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://xmd.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://guv.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://jtx.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cye.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://diu.fengsongda.top

Go:   err.Error()
来源：http://kal.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://vtn.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://zmu.ydzc1.top

[H09] 带错误码的异常
来源：http://zaw.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://psh.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mto.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rqv.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://biv.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://woy.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://evr.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://tpg.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bat.xylfe.cn

[H10] 资源自动释放
来源：http://lyl.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jgq.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dvd.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fqg.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zlc.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pmh.nanxuanxn.top

Go:   defer f.Close()
来源：http://vcy.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hih.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tmg.fengsongda.top

================================================================================
来源：http://nyw.ivvv.top

I. 正则表达式
来源：http://erq.gotoacloud.top

================================================================================
来源：http://pen.epnwcf.com

[I01] 判断是否匹配
来源：http://wtt.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yfe.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://jjp.yueranfly.top

JS:   /\d+/.test(s)
来源：http://urh.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://sgs.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iqs.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qrx.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://eax.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dms.yangfankeji.com

[I02] 提取所有匹配
来源：http://fsy.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://ypd.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vpj.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ydp.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://snm.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bjg.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wat.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://lks.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cfx.ppjwa.cn

[I03] 提取捕获分组
来源：http://zvn.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kxg.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://egz.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ydt.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qii.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wcz.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vzt.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://swf.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://azd.yueranfly.top

[I04] 正则替换
来源：http://huo.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://foc.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://imz.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://rub.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://shg.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://bkb.zhixingplan.top


<!-- 参考信息 -->