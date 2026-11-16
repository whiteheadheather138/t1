代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://vru.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xcr.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uhn.iojbl.cn

Ruby: File.size("a.txt")
来源：http://zjb.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://prd.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://trp.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qgw.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pem.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ije.hcnkem.com

TS:   path.extname("a.txt")
来源：http://tss.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mkg.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ajz.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qxp.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yce.fehbvm.com

[F11] 复制与移动文件
来源：http://xvh.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://orr.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nrg.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pnl.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eyq.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://btb.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hdw.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://svi.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://huu.hesvh.cn

[F12] CSV 读写
来源：http://vqo.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yvb.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qyb.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ugw.redwolf501.top

TS:   // 同上
来源：http://ylq.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fof.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kzb.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vjs.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://whk.jinyuanbaomall.cn

================================================================================
来源：http://rkw.vehdjk.com

G. 面向对象
来源：http://gjv.daria6918.cn

================================================================================
来源：http://bww.jqgfzy.top

[G01] 定义类
来源：http://ruw.ppjwa.cn

Py:   class User: pass
来源：http://ppg.fanxiaobao.xyz

PHP:  class User {}
来源：http://jlk.guannengcc.top

JS:   class User {}
来源：http://lpp.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://pmt.jqgfzy.top

Java: class User {}
来源：http://bwo.sysykeji.top

Go:   type User struct { Name string }
来源：http://ksl.hongshengwenyu.top

Ruby: class User; end
来源：http://ibs.316326.xyz

C#:   class User {}
来源：http://ndk.haohaochexian.top

[G02] 构造函数
来源：http://ysz.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://bxe.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://gmh.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://xhw.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://lxx.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://wzb.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kqw.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://bkf.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://vxm.redwolf501.top

[G03] 实例属性
来源：http://enm.52xcode.cn

Py:   self.name = "x"
来源：http://wea.hywenlv.cn

PHP:  public string $name = "x";
来源：http://xbu.shzxlz.cn

JS:   this.name = "x";
来源：http://dsy.zhongyouzk.top

TS:   name: string = "x";
来源：http://dtk.birdmap.top

Java: private String name;
来源：http://als.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tya.nwbrower.top

Ruby: @name = "x"
来源：http://ogj.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://dro.shzxlz.cn

[G04] 定义方法
来源：http://zwu.daria6918.cn

Py:   def greet(self): return self.name
来源：http://ecw.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://jwa.shuidangran.top

JS:   greet() { return this.name; }
来源：http://oqy.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://ajc.yvedp.cn

Java: String greet() { return name; }
来源：http://gst.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iwm.hysaishi.cn

Ruby: def greet; @name; end
来源：http://yxq.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://kxj.vqdsnc.cn

[G05] 继承
来源：http://zks.316326.xyz

Py:   class Admin(User): pass
来源：http://zyq.meibo888.top

PHP:  class Admin extends User {}
来源：http://wfa.yueranfly.top

JS:   class Admin extends User {}
来源：http://mpf.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://fcc.pycfn.com

Java: class Admin extends User {}
来源：http://hom.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pzo.redwolf501.top

Ruby: class Admin < User; end
来源：http://cgd.jiagoushi.top

C#:   class Admin : User {}
来源：http://kqq.pengpengdd.cyou

[G06] 重写方法
来源：http://fvj.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://hcg.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bgs.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://erw.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://xha.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://xcv.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xmi.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://clg.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://nup.hcnkem.com

[G07] 调用父类方法
来源：http://zol.hfpthk.cn

Py:   super().greet()
来源：http://bkw.jiagoushi.top

PHP:  parent::greet();
来源：http://dxn.hnxiangtu.top

JS:   super.greet();
来源：http://vfs.xuanzx.com

TS:   super.greet();
来源：http://hxp.daria6918.cn

Java: super.greet();
来源：http://ssp.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zub.aibaodan.cn

Ruby: super
来源：http://olu.snrcjt.cn

C#:   base.Greet();
来源：http://lgr.daria6918.cn

[G08] 静态方法与属性
来源：http://app.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://imh.ctjpmb.com

PHP:  public static function f() {}
来源：http://xrp.aibaodan.cn

JS:   static f() {}
来源：http://xer.tarul.cn

TS:   static f(): void {}
来源：http://gdx.aizwys.cn

Java: static void f() {}
来源：http://lhc.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rip.smart0.xyz

Ruby: def self.f; end
来源：http://vxw.zhijiandao.cn

C#:   public static void F() {}
来源：http://sqy.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://yet.shuidangran.top

Py:   from abc import ABC, abstractmethod
来源：http://msz.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://ago.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://cvs.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://vqu.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://dwd.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://pen.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nbz.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://wzr.sjlbkw.cn

[G10] 访问控制
来源：http://fic.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://nbe.jyoumei.cn

PHP:  public / protected / private
来源：http://yzb.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://eey.hywenlv.cn

TS:   public / protected / private
来源：http://xxw.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://gqo.52xcode.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lrb.sysykeji.top

Ruby: public / protected / private
来源：http://nhz.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://hus.yfazqb.com

[G11] getter / setter
来源：http://brs.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://ghn.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://blv.tarul.cn

JS:   get name() { return this._name; }
来源：http://yfo.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://acn.tian-w.cn

Java: public String getName() { return name; }
来源：http://pgl.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://trr.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://nvo.sweek.top

C#:   public string Name { get; set; }
来源：http://ccw.svipenyu.cn

[G12] 对象转字符串
来源：http://cnk.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://qmf.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ypr.hesvh.cn

JS:   toString() { return this.name; }
来源：http://nzu.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://zub.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://dob.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fyh.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://hdp.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://zdg.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://ple.redwolf501.top

Py:   isinstance(u, User)
来源：http://ejm.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://ett.jinghuilouyu.cn

JS:   u instanceof User
来源：http://mlh.hnxiangtu.top

TS:   u instanceof User
来源：http://yda.jiagoushi.top

Java: u instanceof User
来源：http://rht.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://hqt.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://dlz.yuxming.cn

C#:   u is User
来源：http://nmn.zhongyouzk.top

[G14] 数据类 / record
来源：http://igp.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rme.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://csi.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://txy.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://ypc.xuanzx.com

Java: record User(String name, int age) {}
来源：http://bzs.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://cls.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://omu.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://hus.gzhubu.top

[G15] 枚举
来源：http://sah.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mnm.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zyw.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sqh.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oem.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://bqa.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fld.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://tmm.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dsn.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://lsu.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zkf.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://cmq.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://jhe.aibaodan.cn

TS:   Object.entries(obj)
来源：http://qot.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xmk.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cqm.tarul.cn

Ruby: obj.instance_variables
来源：http://prx.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://tjz.gotoacloud.top

================================================================================
来源：http://lnu.tian-w.cn

H. 异常与错误处理
来源：http://dvi.fengsongda.top

================================================================================
来源：http://ngl.vqdsnc.cn

[H01] try / catch 基础
来源：http://sgf.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ihs.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kzg.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ofl.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lub.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://doa.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bor.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mpm.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nga.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://vdo.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://fgy.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qio.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iew.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nnj.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://srl.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gjk.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wml.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qji.guowangkeji.top

[H03] 主动抛出异常
来源：http://qvf.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://hvf.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zkn.316326.xyz

JS:   throw new Error("错误信息");
来源：http://pva.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://enf.hfpthk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sjo.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xgo.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://erg.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zul.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://umk.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://fxk.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hqt.xuanzx.com

JS:   class MyError extends Error {}
来源：http://zxo.daxiang520.top

TS:   class MyError extends Error {}
来源：http://tkc.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://stk.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ohf.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://esx.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://mbd.xziqi.cn

[H05] 捕获特定类型
来源：http://art.gaohongyu789.top

Py:   except ValueError as e:
来源：http://ogi.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cdt.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://xtc.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://pdv.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://zfl.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://new.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://mnk.dianchejie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vsc.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://ktq.sxryk.cn

Py:   value = d.get("k") or default
来源：http://tzn.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oyt.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ouc.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://gll.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yqz.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://aml.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://vrp.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://xum.zhoulong.xyz

[H07] 断言
来源：http://tgz.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://cpq.zhengqikj.top

PHP:  assert($x > 0);
来源：http://mwx.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://lzx.yongpay.top

TS:   console.assert(x > 0);
来源：http://bne.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://olk.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qxt.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://wuf.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://owp.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://zfj.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://icu.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vog.daxiang520.top

JS:   e.message;  e.stack
来源：http://eig.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ukp.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ogi.havefunace.top

Go:   err.Error()
来源：http://kng.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://amp.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://dsd.jqgufenzy.top

[H09] 带错误码的异常
来源：http://tvo.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ttw.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://mjt.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iaf.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yzq.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://noz.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vkv.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cmm.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uca.c1oappe.top

[H10] 资源自动释放
来源：http://qut.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iny.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ttw.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gci.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pvg.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sij.ybcxt.top

Go:   defer f.Close()
来源：http://dpm.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qqz.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oiu.hesvh.cn

================================================================================
来源：http://hxz.316326.xyz

I. 正则表达式
来源：http://ihg.zycfv.cn

================================================================================
来源：http://izc.zhoulong.xyz

[I01] 判断是否匹配
来源：http://bif.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://drm.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://wjb.sweek.top

JS:   /\d+/.test(s)
来源：http://njo.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://bnk.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lkv.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fbx.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://nax.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://auu.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://jyd.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://brt.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://roe.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zxh.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://dbt.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qhp.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://anc.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://jlm.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://geo.birdmap.top

[I03] 提取捕获分组
来源：http://uea.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xon.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pdt.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lge.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pxp.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sma.sufxvd.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ecu.xziqi.cn


<!-- 参考信息 -->