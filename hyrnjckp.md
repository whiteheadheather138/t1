代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lea.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://ymf.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lwv.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ths.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pcs.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://acd.yfazqb.com

[F11] 复制与移动文件
来源：http://gvm.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gob.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gjj.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nnc.jiagoushi.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfh.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fmv.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gqg.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://guu.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zqr.gaohongyu789.top

[F12] CSV 读写
来源：http://euz.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uwv.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mtn.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bgu.sjlbkw.cn

TS:   // 同上
来源：http://quj.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qdi.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fdj.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bwe.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kzn.hongshengwenyu.top

================================================================================
来源：http://beo.fehbvm.com

G. 面向对象
来源：http://pkk.xingfuxueyuan.xyz

================================================================================
来源：http://bab.gaohongyu789.top

[G01] 定义类
来源：http://jmz.yj202588.top

Py:   class User: pass
来源：http://tii.wangdashe.top

PHP:  class User {}
来源：http://fin.jianghu66.top

JS:   class User {}
来源：http://stl.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://lbk.meibo888.top

Java: class User {}
来源：http://qzi.vehdjk.com

Go:   type User struct { Name string }
来源：http://gkk.cucudq.cn

Ruby: class User; end
来源：http://wgy.daxiang520.top

C#:   class User {}
来源：http://vdh.9152youxi.cn

[G02] 构造函数
来源：http://dja.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://mde.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://lqi.cdnleiting.top

JS:   constructor(name) { this.name = name; }
来源：http://snr.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://ppz.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://pgm.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://txu.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://eto.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://lbx.vqdsnc.cn

[G03] 实例属性
来源：http://fnp.yj202588.top

Py:   self.name = "x"
来源：http://uyo.ydzc1.top

PHP:  public string $name = "x";
来源：http://euh.tarul.cn

JS:   this.name = "x";
来源：http://kki.sysykeji.top

TS:   name: string = "x";
来源：http://jwa.kuanghao11.cn

Java: private String name;
来源：http://uqe.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cki.cashguo.top

Ruby: @name = "x"
来源：http://adc.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://ihi.yonumen.top

[G04] 定义方法
来源：http://ydi.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://hzt.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qiy.jianghu66.top

JS:   greet() { return this.name; }
来源：http://rrs.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://mwh.mhx1999.top

Java: String greet() { return name; }
来源：http://gdv.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://gyl.hesvh.cn

Ruby: def greet; @name; end
来源：http://dfz.wangdashe.top

C#:   public string Greet() => Name;
来源：http://boa.ydjk.org.cn

[G05] 继承
来源：http://aqd.nanxinkj.top

Py:   class Admin(User): pass
来源：http://mnu.birdmap.top

PHP:  class Admin extends User {}
来源：http://kgv.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://bdt.hysaishi.cn

TS:   class Admin extends User {}
来源：http://unr.zhijiandao.cn

Java: class Admin extends User {}
来源：http://spk.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://piy.cqqwz.cn

Ruby: class Admin < User; end
来源：http://sav.meibo888.top

C#:   class Admin : User {}
来源：http://rwu.jianghu66.top

[G06] 重写方法
来源：http://umy.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://elm.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bnl.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://upd.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://vvc.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://kka.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bqp.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://alw.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://plr.shzxlz.cn

[G07] 调用父类方法
来源：http://llm.jinqigfzy.top

Py:   super().greet()
来源：http://wxi.meibo888.top

PHP:  parent::greet();
来源：http://eoj.shuidangran.top

JS:   super.greet();
来源：http://uoh.wangshuangyany.cn

TS:   super.greet();
来源：http://rdj.jinqigufen.top

Java: super.greet();
来源：http://ypo.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kze.sysykeji.top

Ruby: super
来源：http://lvp.52xcode.cn

C#:   base.Greet();
来源：http://ema.cashguo.top

[G08] 静态方法与属性
来源：http://ynt.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://brf.jinqigufen.top

PHP:  public static function f() {}
来源：http://xyf.zhijiandao.cn

JS:   static f() {}
来源：http://wwx.tianlin.xyz

TS:   static f(): void {}
来源：http://jgy.yvedp.cn

Java: static void f() {}
来源：http://lck.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rrh.fengsongda.top

Ruby: def self.f; end
来源：http://efe.vehdjk.com

C#:   public static void F() {}
来源：http://esk.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://vly.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://tyq.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zae.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zhf.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://pmr.xylfe.cn

Java: interface Shape { double area(); }
来源：http://wgo.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://vkt.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vih.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://bod.sysykeji.top

[G10] 访问控制
来源：http://wgp.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://exj.bbcook.cn

PHP:  public / protected / private
来源：http://jre.jianghu66.top

JS:   #private 字段；其余公开
来源：http://gco.jinghuilouyu.cn

TS:   public / protected / private
来源：http://xro.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://vse.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://pko.haohaochexian.top

Ruby: public / protected / private
来源：http://bra.cdnleiting.top

C#:   public / protected / private / internal
来源：http://vwp.cdnleiting.top

[G11] getter / setter
来源：http://tug.hcnkem.com

Py:   @property 与 @x.setter
来源：http://ssn.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cpq.yueranfly.top

JS:   get name() { return this._name; }
来源：http://phf.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://shp.gogol.net.cn

Java: public String getName() { return name; }
来源：http://bcx.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yzz.hfpthk.cn

Ruby: attr_accessor :name
来源：http://wfx.tian-w.cn

C#:   public string Name { get; set; }
来源：http://rup.yangfankeji.com

[G12] 对象转字符串
来源：http://bik.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://kat.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nix.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://oqa.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://lfn.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://ixt.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://ywb.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://xhv.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://ljp.chenzaomai.com

[G13] 判断对象类型
来源：http://dob.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://pmp.smart0.xyz

PHP:  $u instanceof User
来源：http://ghd.yangfankeji.com

JS:   u instanceof User
来源：http://umo.dianchejie.cn

TS:   u instanceof User
来源：http://yvg.ydjk.org.cn

Java: u instanceof User
来源：http://udl.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://igr.xziqi.cn

Ruby: u.is_a?(User)
来源：http://ess.dianchejie.cn

C#:   u is User
来源：http://irg.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://ugj.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ibt.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://jlo.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://ayz.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://zhd.xuanzx.com

Java: record User(String name, int age) {}
来源：http://kfh.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://xjy.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kdi.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://rgy.ydzc1.top

[G15] 枚举
来源：http://joy.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qvm.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tmq.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kld.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tfo.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://yde.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://guh.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://ico.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jvc.yonumen.top

[G16] 对象转数组 / 字典
来源：http://jdb.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vyr.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://lzo.dianchejie.cn

JS:   Object.entries(obj)
来源：http://mit.uphjek.com

TS:   Object.entries(obj)
来源：http://lft.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jng.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vqs.andypj.xyz

Ruby: obj.instance_variables
来源：http://bvh.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://uzw.epnwcf.com

================================================================================
来源：http://jpa.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://hnd.hesvh.cn

================================================================================
来源：http://zpx.chenjidiqi.icu

[H01] try / catch 基础
来源：http://ksq.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bsd.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ahg.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://olt.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pio.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wnh.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jth.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lwv.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aoo.fengsongda.top

[H02] finally / ensure 收尾
来源：http://ynu.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://osr.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nhg.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://weh.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://nbc.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wuu.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jbu.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vmx.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://koe.9152youxi.cn

[H03] 主动抛出异常
来源：http://sxk.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://mzp.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ovl.yonumen.top

JS:   throw new Error("错误信息");
来源：http://esw.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://kmf.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xyh.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://agm.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://azd.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://oxm.fktsv.cn

[H04] 自定义异常类型
来源：http://kwi.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://cct.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://msk.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://nzr.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://rjm.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://ynt.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lwu.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://bkp.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://hmm.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://xdn.daria6918.cn

Py:   except ValueError as e:
来源：http://mzs.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iwf.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://byr.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://rtf.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://doh.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ywg.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://mcv.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cqg.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://sxs.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://unk.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pdo.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sdz.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://njp.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xgx.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://aoj.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://ogk.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://npy.jinqigfzy.top

[H07] 断言
来源：http://vqu.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://maw.vehdjk.com

PHP:  assert($x > 0);
来源：http://jst.hnqzz.top

JS:   console.assert(x > 0);
来源：http://ued.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://dnr.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://gwb.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wem.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xcl.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://qbk.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://ixo.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://dss.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lix.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://xyv.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://crh.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://qcg.haohaochexian.top

Go:   err.Error()
来源：http://cxv.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://nfx.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://iau.chenlongwang.top

[H09] 带错误码的异常
来源：http://pfs.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uwh.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gdn.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ckq.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dni.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fdk.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aqr.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eet.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gtp.xinyue.icu

[H10] 资源自动释放
来源：http://oit.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://apq.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://phu.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kjn.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://duv.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://asn.zhoulong.xyz

Go:   defer f.Close()
来源：http://qli.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hkg.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ces.quarkkingdee.top

================================================================================
来源：http://yqr.sxryk.cn

I. 正则表达式
来源：http://ele.chenzaomai.com

================================================================================
来源：http://eip.xziqi.cn

[I01] 判断是否匹配
来源：http://tae.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iil.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://mar.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://gxg.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://del.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://otp.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mht.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://sbt.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nmk.vqdsnc.cn

[I02] 提取所有匹配
来源：http://bmx.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://egg.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wbp.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iqy.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://thm.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rlj.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vjx.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://ifr.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rrj.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://uzi.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://etj.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bdz.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rrq.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fxp.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ggr.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ypv.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dna.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iie.zdbjq.cn

[I04] 正则替换
来源：http://jdf.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pch.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zjm.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iwe.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qct.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://qrs.chenjidiqi.icu


<!-- 参考信息 -->