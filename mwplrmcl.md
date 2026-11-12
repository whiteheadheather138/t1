代发 wailian999

[F09] 获取文件大小
来源：http://yua.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://ian.yj20258.top

PHP:  filesize("a.txt");
来源：http://izq.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://xjp.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://obq.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://kih.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ezp.316326.xyz

Ruby: File.size("a.txt")
来源：http://swr.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://vpq.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://zfv.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fuw.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ylx.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oia.hammf.cn

TS:   path.extname("a.txt")
来源：http://tuz.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://poy.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zia.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jxo.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xph.aizwys.cn

[F11] 复制与移动文件
来源：http://ucn.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dbm.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dvp.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gyy.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cbt.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iis.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hwt.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yjv.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://izb.birdmap.top

[F12] CSV 读写
来源：http://dpw.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://emw.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sgs.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fgs.fzhhl.top

TS:   // 同上
来源：http://snr.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zpu.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://crb.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jzw.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uej.zhengqikj.top

================================================================================
来源：http://mpp.xinyue.icu

G. 面向对象
来源：http://ngy.yangfankeji.com

================================================================================
来源：http://aht.chenjidiqi.icu

[G01] 定义类
来源：http://kze.0kj1m.cn

Py:   class User: pass
来源：http://egi.aizwys.cn

PHP:  class User {}
来源：http://nyy.ppjwa.cn

JS:   class User {}
来源：http://pzy.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://boc.yongpay.top

Java: class User {}
来源：http://ify.dashuyun.cn

Go:   type User struct { Name string }
来源：http://yuq.chenjidiqi.icu

Ruby: class User; end
来源：http://nmb.wangdashe.top

C#:   class User {}
来源：http://ent.hammf.cn

[G02] 构造函数
来源：http://ccq.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://uqu.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://wai.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://flk.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://lhc.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://fgm.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cmz.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://vkb.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://cbm.sjlbkw.cn

[G03] 实例属性
来源：http://kyo.iojbl.cn

Py:   self.name = "x"
来源：http://zxi.gotoacloud.top

PHP:  public string $name = "x";
来源：http://zms.9152youxi.cn

JS:   this.name = "x";
来源：http://tsc.guannengcc.top

TS:   name: string = "x";
来源：http://vfq.xziqi.cn

Java: private String name;
来源：http://uou.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aef.pycfn.com

Ruby: @name = "x"
来源：http://psf.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://vth.yongpay.top

[G04] 定义方法
来源：http://aju.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://xni.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mig.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://bym.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://nty.aizwys.cn

Java: String greet() { return name; }
来源：http://hnt.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nbh.mhx1999.top

Ruby: def greet; @name; end
来源：http://hat.cheryme.top

C#:   public string Greet() => Name;
来源：http://enz.zdbjq.cn

[G05] 继承
来源：http://dbr.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://six.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://tyv.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://yel.fzhhl.top

TS:   class Admin extends User {}
来源：http://gkb.guannengcc.top

Java: class Admin extends User {}
来源：http://ckn.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ssa.svipenyu.cn

Ruby: class Admin < User; end
来源：http://aey.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://vcr.gzhubu.top

[G06] 重写方法
来源：http://dvy.tanke756.top

Py:   def greet(self): return "admin"
来源：http://ajr.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://chc.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://keh.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://tmq.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://rcm.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dpi.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://yhv.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://mwv.yonumen.top

[G07] 调用父类方法
来源：http://ygk.zhongyouzk.top

Py:   super().greet()
来源：http://uuo.xuanzx.com

PHP:  parent::greet();
来源：http://ajl.uphjek.com

JS:   super.greet();
来源：http://xhe.chenlongwang.top

TS:   super.greet();
来源：http://fva.shangyingyoupin.top

Java: super.greet();
来源：http://xpq.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zmv.fanxiaobao.xyz

Ruby: super
来源：http://bii.pycfn.com

C#:   base.Greet();
来源：http://xmt.fktsv.cn

[G08] 静态方法与属性
来源：http://bog.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rfv.mhx1999.top

PHP:  public static function f() {}
来源：http://cab.nwbrower.top

JS:   static f() {}
来源：http://hcw.andypj.xyz

TS:   static f(): void {}
来源：http://jgu.daxiang520.top

Java: static void f() {}
来源：http://qpw.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hjk.xziqi.cn

Ruby: def self.f; end
来源：http://fsv.0kj1m.cn

C#:   public static void F() {}
来源：http://xgd.smart0.xyz

[G09] 接口 / 抽象类
来源：http://nmd.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://alb.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://jay.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://udh.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://xve.daxiang520.top

Java: interface Shape { double area(); }
来源：http://xei.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://rdj.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ddj.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://fbz.snrcjt.cn

[G10] 访问控制
来源：http://jaz.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://wdi.zhengqikj.top

PHP:  public / protected / private
来源：http://cbi.c1oappe.top

JS:   #private 字段；其余公开
来源：http://bxe.jinqigfzy.top

TS:   public / protected / private
来源：http://dha.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://wuf.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hhp.daria6918.cn

Ruby: public / protected / private
来源：http://xum.fehbvm.com

C#:   public / protected / private / internal
来源：http://hde.zhijiandao.cn

[G11] getter / setter
来源：http://kvx.52xcode.cn

Py:   @property 与 @x.setter
来源：http://ctw.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pre.sxryk.cn

JS:   get name() { return this._name; }
来源：http://qpr.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://anc.hesvh.cn

Java: public String getName() { return name; }
来源：http://ncf.hammf.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kfl.sweek.top

Ruby: attr_accessor :name
来源：http://cqx.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://dbn.jlsjyb.cn

[G12] 对象转字符串
来源：http://qyw.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://iqx.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qwy.yj20258888.top

JS:   toString() { return this.name; }
来源：http://pdr.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://nhf.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://nqw.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://blb.daria6918.cn

Ruby: def to_s; @name; end
来源：http://lye.ivvv.top

C#:   public override string ToString() => Name;
来源：http://nuv.yj20258888.top

[G13] 判断对象类型
来源：http://eci.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://guy.cqqwz.cn

PHP:  $u instanceof User
来源：http://men.ydzc1.top

JS:   u instanceof User
来源：http://pdl.cheryme.top

TS:   u instanceof User
来源：http://ati.yanxiufei.cn

Java: u instanceof User
来源：http://jvv.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nag.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://ltp.hnxiangtu.top

C#:   u is User
来源：http://bxx.gzhubu.top

[G14] 数据类 / record
来源：http://zgr.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kdi.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://lim.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://upx.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://ikx.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://cfh.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://oti.jianghu66.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vxa.tarul.cn

C#:   record User(string Name, int Age);
来源：http://bvk.dianchejie.cn

[G15] 枚举
来源：http://gsm.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://haj.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pcx.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://egc.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://npv.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://jal.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ncg.chenjidiqi.icu

Ruby: Color = %i[red green].freeze
来源：http://fnb.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://idd.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://bbv.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://usn.316326.xyz

PHP:  get_object_vars($obj);
来源：http://pek.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://jam.fengsongda.top

TS:   Object.entries(obj)
来源：http://csc.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ubz.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jsz.9152youxi.cn

Ruby: obj.instance_variables
来源：http://jvz.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://qes.zhaomingkeji.xyz

================================================================================
来源：http://nou.zhoulong.xyz

H. 异常与错误处理
来源：http://ion.fehbvm.com

================================================================================
来源：http://hwp.bbcook.cn

[H01] try / catch 基础
来源：http://soq.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hsp.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xwi.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jxt.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zsf.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://atx.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://adj.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xum.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ltz.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://mve.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rgq.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wow.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lzi.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://unr.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://ydm.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytt.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eqf.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cuw.9152youxi.cn

[H03] 主动抛出异常
来源：http://fws.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://jup.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pzg.birdmap.top

JS:   throw new Error("错误信息");
来源：http://bpw.yj202588.top

TS:   throw new Error("错误信息");
来源：http://rte.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://erg.gotoacloud.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hyv.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jsz.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ouf.hcnkem.com

[H04] 自定义异常类型
来源：http://ihg.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://kuj.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://wew.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://ayc.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://uwz.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://mxk.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://acr.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://mjf.tian-w.cn

C#:   class MyException : Exception {}
来源：http://aja.havefunace.top

[H05] 捕获特定类型
来源：http://lia.tarul.cn

Py:   except ValueError as e:
来源：http://idt.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qzd.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://nru.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://emr.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://uhe.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://orb.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://upt.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ptb.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://hoz.cashguo.top

Py:   value = d.get("k") or default
来源：http://zsq.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://sky.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://oty.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://heq.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ufo.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kni.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://twr.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://ssf.zdbjq.cn

[H07] 断言
来源：http://ful.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://irl.yueranfly.top

PHP:  assert($x > 0);
来源：http://vnp.fehbvm.com

JS:   console.assert(x > 0);
来源：http://lxs.sweek.top

TS:   console.assert(x > 0);
来源：http://bgp.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://jpi.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oob.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://buk.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://crx.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://jve.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://jgd.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aus.epnwcf.com

JS:   e.message;  e.stack
来源：http://tpi.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vsj.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ybz.yuanzhike.top

Go:   err.Error()
来源：http://guk.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://vkn.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://ify.xylfe.cn

[H09] 带错误码的异常
来源：http://svx.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vdl.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pks.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kyi.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oai.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qnh.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vdz.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://usu.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vvn.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://jla.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lfa.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://szi.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tug.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uol.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ejj.jinqigufen.top

Go:   defer f.Close()
来源：http://vnm.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ehi.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://axc.chenzaomai.com

================================================================================
来源：http://pbx.zhiwuduotai.top

I. 正则表达式
来源：http://hxz.meibo888.top

================================================================================
来源：http://tor.xylfe.cn

[I01] 判断是否匹配
来源：http://rro.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://guu.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nyq.guannengcc.top

JS:   /\d+/.test(s)
来源：http://cfv.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://tqc.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qls.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sdt.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://veg.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xyq.yonumen.top

[I02] 提取所有匹配
来源：http://evb.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://bow.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gpp.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://foh.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://tjn.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tox.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dgh.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://uel.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pby.yvedp.cn

[I03] 提取捕获分组
来源：http://cai.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ddl.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hwv.fengsongda.top


<!-- 参考信息 -->