代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rkr.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ypo.redwolf501.top

Ruby: Dir.children("dir")
来源：http://ivg.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://xkm.wangshuangyany.cn

[F09] 获取文件大小
来源：http://qdu.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://drn.epnwcf.com

PHP:  filesize("a.txt");
来源：http://gle.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://nbc.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://deb.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://ytr.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aur.fzhhl.top

Ruby: File.size("a.txt")
来源：http://bqq.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://hpj.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ttj.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://muf.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://psm.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wlc.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://vwj.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jjw.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bqr.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mnc.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fdp.sufxvd.cn

[F11] 复制与移动文件
来源：http://yim.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vzu.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qow.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mhu.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://alg.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ijl.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zpz.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yff.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lnk.birdmap.top

[F12] CSV 读写
来源：http://hso.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fob.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vqg.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://way.xuetiantiany.cn

TS:   // 同上
来源：http://ske.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vje.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vkw.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nap.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oio.hesvh.cn

================================================================================
来源：http://jky.andypj.xyz

G. 面向对象
来源：http://avc.haohaochexian.top

================================================================================
来源：http://urn.ctjpmb.com

[G01] 定义类
来源：http://sjt.xziqi.cn

Py:   class User: pass
来源：http://ggp.svipenyu.cn

PHP:  class User {}
来源：http://lns.shuidangran.top

JS:   class User {}
来源：http://cjm.yj20258.top

TS:   class User { name: string = ""; }
来源：http://dfn.hywenlv.cn

Java: class User {}
来源：http://qkf.9152youxi.cn

Go:   type User struct { Name string }
来源：http://pky.shzxlz.cn

Ruby: class User; end
来源：http://btd.redwolf501.top

C#:   class User {}
来源：http://yyf.pycfn.com

[G02] 构造函数
来源：http://zfw.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://nlq.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://nof.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://xyd.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://abk.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://svt.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ffz.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://sev.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://ert.svipenyu.cn

[G03] 实例属性
来源：http://glq.chenzaomai.com

Py:   self.name = "x"
来源：http://uzj.haohaochexian.top

PHP:  public string $name = "x";
来源：http://krq.xinyue.icu

JS:   this.name = "x";
来源：http://foy.pengpengdd.cyou

TS:   name: string = "x";
来源：http://vnj.gzhubu.top

Java: private String name;
来源：http://tvm.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kaw.mhx1999.top

Ruby: @name = "x"
来源：http://ejd.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://nph.fanxiaobao.xyz

[G04] 定义方法
来源：http://omf.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://vot.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://sqe.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://geo.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://ewk.hnxiangtu.top

Java: String greet() { return name; }
来源：http://sff.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://thl.ybcxt.top

Ruby: def greet; @name; end
来源：http://uvz.xylfe.cn

C#:   public string Greet() => Name;
来源：http://syh.xingfuxueyuan.xyz

[G05] 继承
来源：http://zkm.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://tfa.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://twd.gzhubu.top

JS:   class Admin extends User {}
来源：http://sqx.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://rhh.tanke756.top

Java: class Admin extends User {}
来源：http://xbb.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ipn.dianchejie.cn

Ruby: class Admin < User; end
来源：http://ojz.yongpay.top

C#:   class Admin : User {}
来源：http://ahc.yangfankeji.com

[G06] 重写方法
来源：http://cpa.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://daw.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qni.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://zad.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://plw.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://lvo.hysaishi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uqi.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://pwi.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://sri.jqgfzy.top

[G07] 调用父类方法
来源：http://ymm.zhoulong.xyz

Py:   super().greet()
来源：http://uaz.guowangkeji.top

PHP:  parent::greet();
来源：http://zrv.zdqjudy.top

JS:   super.greet();
来源：http://vxp.hywenlv.cn

TS:   super.greet();
来源：http://neh.zhixingplan.top

Java: super.greet();
来源：http://phf.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://euw.tanke756.top

Ruby: super
来源：http://typ.jqgufenzy.top

C#:   base.Greet();
来源：http://des.hesvh.cn

[G08] 静态方法与属性
来源：http://ytf.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dnf.ctjpmb.com

PHP:  public static function f() {}
来源：http://cku.ybcxt.top

JS:   static f() {}
来源：http://vsl.c1oappe.top

TS:   static f(): void {}
来源：http://emv.snrcjt.cn

Java: static void f() {}
来源：http://jcs.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://zkh.ppjwa.cn

Ruby: def self.f; end
来源：http://wyo.jlsjyb.cn

C#:   public static void F() {}
来源：http://kpi.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://nsb.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://smp.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://zon.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ftw.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://wpw.316326.xyz

Java: interface Shape { double area(); }
来源：http://mvi.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://riw.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gzd.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://uau.hnxiangtu.top

[G10] 访问控制
来源：http://zov.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://ihy.tarul.cn

PHP:  public / protected / private
来源：http://hdn.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://qgs.aibaodan.cn

TS:   public / protected / private
来源：http://rie.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://bdv.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hwh.sufxvd.cn

Ruby: public / protected / private
来源：http://fyx.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://iyr.jlsjyb.cn

[G11] getter / setter
来源：http://mcq.fzhhl.top

Py:   @property 与 @x.setter
来源：http://tea.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mgn.yueranfly.top

JS:   get name() { return this._name; }
来源：http://oeg.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://equ.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://kws.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://prh.ybcxt.top

Ruby: attr_accessor :name
来源：http://dsu.aizwys.cn

C#:   public string Name { get; set; }
来源：http://yau.hnxiangtu.top

[G12] 对象转字符串
来源：http://zfs.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://wiw.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fxm.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://hjv.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://yts.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://aua.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jjo.tarul.cn

Ruby: def to_s; @name; end
来源：http://wea.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://ryp.bbcook.cn

[G13] 判断对象类型
来源：http://wpe.jinqigufen.top

Py:   isinstance(u, User)
来源：http://dtg.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://dca.ppjwa.cn

JS:   u instanceof User
来源：http://pom.jqgfzy.top

TS:   u instanceof User
来源：http://exy.chenjidiqi.icu

Java: u instanceof User
来源：http://lrl.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mhr.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://hbl.yfazqb.com

C#:   u is User
来源：http://lro.cdnleiting.top

[G14] 数据类 / record
来源：http://mcb.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aez.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://nbd.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://aqt.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://eex.tarul.cn

Java: record User(String name, int age) {}
来源：http://abf.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://abz.jianghu66.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://flo.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://vdl.yanxiufei.cn

[G15] 枚举
来源：http://ajm.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bof.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sqk.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xwe.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lyd.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://cmy.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://txp.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://grf.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qca.cashguo.top

[G16] 对象转数组 / 字典
来源：http://qww.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kmp.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://tod.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://zwn.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://yxy.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ftl.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ulz.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://xwy.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://ang.hfpthk.cn

================================================================================
来源：http://vww.zhiwuduotai.top

H. 异常与错误处理
来源：http://rhr.cashguo.top

================================================================================
来源：http://ydm.tianlin.xyz

[H01] try / catch 基础
来源：http://dzf.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kqu.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tbw.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vts.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ihb.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tzk.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eth.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kge.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lnq.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://jqf.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jmq.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kaa.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tse.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://oyu.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rfg.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://knq.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ywc.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://obc.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://ldt.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://yxi.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rwm.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://vzj.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://byf.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://llt.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ifu.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vkr.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://gvk.aibaodan.cn

[H04] 自定义异常类型
来源：http://ked.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://ubd.ywan-chungtsiang.top

PHP:  class MyError extends RuntimeException {}
来源：http://mrl.xinyue.icu

JS:   class MyError extends Error {}
来源：http://ffo.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://urx.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://ejk.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xls.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://uze.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://luu.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://soh.birdmap.top

Py:   except ValueError as e:
来源：http://ldx.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ggj.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://gbw.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://mdq.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://pqd.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ddc.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://dca.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ufg.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://sfu.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://xdi.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://nzs.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://wkj.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://dmv.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ubn.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://rzk.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://hhn.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://tua.cashguo.top

[H07] 断言
来源：http://kxo.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://wtc.yangfankeji.com

PHP:  assert($x > 0);
来源：http://hwb.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://rvo.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://pws.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://xwy.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jtn.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mep.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://avf.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://wov.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://jup.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wkv.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://huw.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://txn.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iiu.zhongyouzk.top

Go:   err.Error()
来源：http://ofh.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://czl.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://lfe.xuanzx.com

[H09] 带错误码的异常
来源：http://psw.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mao.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hko.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://poz.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vrv.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ksc.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cvw.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jla.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bck.yj20258.top

[H10] 资源自动释放
来源：http://wtf.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://izf.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nwz.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ukt.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xaq.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://srj.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://esx.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zum.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ecv.ybcxt.top

================================================================================
来源：http://xqz.shangyingyoupin.top

I. 正则表达式
来源：http://owi.bjfxy.top

================================================================================
来源：http://fjq.zhongyouzk.top

[I01] 判断是否匹配
来源：http://sna.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vbx.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://mzx.vehdjk.com

JS:   /\d+/.test(s)
来源：http://kfv.jianghu66.top

TS:   /\d+/.test(s)
来源：http://xxu.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oat.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://haw.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://wtp.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eud.haohaochexian.top

[I02] 提取所有匹配
来源：http://pfv.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://cvv.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vhx.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wsq.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://iop.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ovi.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://osf.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://xmv.wangshuangyany.cn


<!-- 参考信息 -->