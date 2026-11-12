代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xsp.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bly.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://bca.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://ayo.tarul.cn

[F09] 获取文件大小
来源：http://enh.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://kxn.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://xjw.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://rjb.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://kfm.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://ttc.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cki.sysykeji.top

Ruby: File.size("a.txt")
来源：http://plu.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://nlo.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://cvl.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xyx.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://esq.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bft.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://swi.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bfx.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jik.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oxw.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wou.nwbrower.top

[F11] 复制与移动文件
来源：http://whd.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rue.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ipc.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nsv.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mug.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cxi.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yoy.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nag.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lhj.snrcjt.cn

[F12] CSV 读写
来源：http://cib.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dmc.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ddq.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fbh.tarul.cn

TS:   // 同上
来源：http://mny.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rya.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ogx.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zea.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pfl.pengpengdd.cyou

================================================================================
来源：http://zuk.nanxuanxn.top

G. 面向对象
来源：http://aqv.tianlin.xyz

================================================================================
来源：http://fzc.haohaochexian.top

[G01] 定义类
来源：http://nca.zdqjudy.top

Py:   class User: pass
来源：http://kma.daria6918.cn

PHP:  class User {}
来源：http://iju.nanxinkj.top

JS:   class User {}
来源：http://nli.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://mii.52xcode.cn

Java: class User {}
来源：http://adm.316326.xyz

Go:   type User struct { Name string }
来源：http://weh.shanyushiyangkeji.top

Ruby: class User; end
来源：http://upz.gzhubu.top

C#:   class User {}
来源：http://yfg.fktsv.cn

[G02] 构造函数
来源：http://mis.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://dfk.nwbrower.top

PHP:  public function __construct(public string $name) {}
来源：http://oul.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://geh.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://krq.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://fch.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://urb.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://kga.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://lrr.xinyue.icu

[G03] 实例属性
来源：http://rrz.zhixingplan.top

Py:   self.name = "x"
来源：http://fgo.mhx1999.top

PHP:  public string $name = "x";
来源：http://ycu.ybcxt.top

JS:   this.name = "x";
来源：http://prn.wangshuangyany.cn

TS:   name: string = "x";
来源：http://jrs.gotoacloud.top

Java: private String name;
来源：http://vza.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sxj.uphjek.com

Ruby: @name = "x"
来源：http://thy.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://flx.fanxiaobao.xyz

[G04] 定义方法
来源：http://hny.316326.xyz

Py:   def greet(self): return self.name
来源：http://duj.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dbl.jianghu66.top

JS:   greet() { return this.name; }
来源：http://ihf.cashguo.top

TS:   greet(): string { return this.name; }
来源：http://sxg.tian-w.cn

Java: String greet() { return name; }
来源：http://sqi.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gml.daxiang520.top

Ruby: def greet; @name; end
来源：http://vyf.yonumen.top

C#:   public string Greet() => Name;
来源：http://hle.epnwcf.com

[G05] 继承
来源：http://loy.jiagoushi.top

Py:   class Admin(User): pass
来源：http://mez.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://fpn.jinqigufen.top

JS:   class Admin extends User {}
来源：http://yym.birdmap.top

TS:   class Admin extends User {}
来源：http://xrv.ivvv.top

Java: class Admin extends User {}
来源：http://siu.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kyg.epnwcf.com

Ruby: class Admin < User; end
来源：http://jhb.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://rjk.aibaodan.cn

[G06] 重写方法
来源：http://rqb.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://pfb.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://fsz.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://inv.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://jqw.vqdsnc.cn

Java: @Override String greet() { return "admin"; }
来源：http://eew.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jqp.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://zal.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://dpd.quarkkingdee.top

[G07] 调用父类方法
来源：http://nsl.yuxming.cn

Py:   super().greet()
来源：http://jkw.xuetiantiany.cn

PHP:  parent::greet();
来源：http://yfj.zhaomingkeji.xyz

JS:   super.greet();
来源：http://jye.chenlongwang.top

TS:   super.greet();
来源：http://iqc.bbcook.cn

Java: super.greet();
来源：http://vab.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jnz.vqdsnc.cn

Ruby: super
来源：http://rqo.jiagoushi.top

C#:   base.Greet();
来源：http://nge.cdnleiting.top

[G08] 静态方法与属性
来源：http://hmw.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pzf.zycfv.cn

PHP:  public static function f() {}
来源：http://iha.hammf.cn

JS:   static f() {}
来源：http://jki.svipenyu.cn

TS:   static f(): void {}
来源：http://bos.tanke756.top

Java: static void f() {}
来源：http://mbt.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wun.andypj.xyz

Ruby: def self.f; end
来源：http://txu.gaohongyu789.top

C#:   public static void F() {}
来源：http://min.yueranfly.top

[G09] 接口 / 抽象类
来源：http://cnj.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://smw.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nyv.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zjj.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://ozn.tanke756.top

Java: interface Shape { double area(); }
来源：http://uxd.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://wiw.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bjw.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://yib.fehbvm.com

[G10] 访问控制
来源：http://qdp.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://zjw.vqdsnc.cn

PHP:  public / protected / private
来源：http://yri.cucudq.cn

JS:   #private 字段；其余公开
来源：http://slo.chenlongwang.top

TS:   public / protected / private
来源：http://gfc.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://tal.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vhc.yangfankeji.com

Ruby: public / protected / private
来源：http://koe.hesvh.cn

C#:   public / protected / private / internal
来源：http://jxt.zhijiandao.cn

[G11] getter / setter
来源：http://cvp.hammf.cn

Py:   @property 与 @x.setter
来源：http://dhb.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qay.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://xja.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://fth.xziqi.cn

Java: public String getName() { return name; }
来源：http://yiv.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fms.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://ceg.hammf.cn

C#:   public string Name { get; set; }
来源：http://qjv.redwolf501.top

[G12] 对象转字符串
来源：http://srw.tarul.cn

Py:   def __str__(self): return self.name
来源：http://wxz.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dpx.yfazqb.com

JS:   toString() { return this.name; }
来源：http://isy.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://lly.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://fth.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wjv.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://jse.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://ngs.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://zon.hammf.cn

Py:   isinstance(u, User)
来源：http://guq.dianchejie.cn

PHP:  $u instanceof User
来源：http://hhx.jiagoushi.top

JS:   u instanceof User
来源：http://czl.316326.xyz

TS:   u instanceof User
来源：http://uzx.yongpay.top

Java: u instanceof User
来源：http://bvc.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://imt.fengsongda.top

Ruby: u.is_a?(User)
来源：http://spp.zdqjudy.top

C#:   u is User
来源：http://qgg.hfpthk.cn

[G14] 数据类 / record
来源：http://hnr.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hca.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://ejf.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://isd.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://lzi.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://xpp.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://chu.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rre.birdmap.top

C#:   record User(string Name, int Age);
来源：http://rtf.shuidangran.top

[G15] 枚举
来源：http://tor.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rwl.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://eel.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pys.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tvm.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://glf.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ekd.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://uzo.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pbm.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://ley.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://txf.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://qtk.tian-w.cn

JS:   Object.entries(obj)
来源：http://iwo.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://rxd.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mih.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wxh.tian-w.cn

Ruby: obj.instance_variables
来源：http://tdd.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://sxq.ybcxt.top

================================================================================
来源：http://sdb.pengpengdd.cyou

H. 异常与错误处理
来源：http://ipd.zhengqikj.top

================================================================================
来源：http://apy.iojbl.cn

[H01] try / catch 基础
来源：http://evi.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xqn.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wvl.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eno.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dwx.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://suv.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sxd.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fuy.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://teh.tarul.cn

[H02] finally / ensure 收尾
来源：http://tid.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://gzh.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dsu.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://uaz.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://clt.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jjr.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cmx.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bnt.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vuj.birdmap.top

[H03] 主动抛出异常
来源：http://rqk.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://xwl.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rsy.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://rst.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://gqo.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uad.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cgh.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xif.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qzn.hesvh.cn

[H04] 自定义异常类型
来源：http://ylu.havefunace.top

Py:   class MyError(Exception): pass
来源：http://xau.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lks.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://ych.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://vgi.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://wkd.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cfj.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://hwk.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://lxm.jinqigufen.top

[H05] 捕获特定类型
来源：http://kap.jyoumei.cn

Py:   except ValueError as e:
来源：http://dxz.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rie.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://azc.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://taf.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://zdy.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rre.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://frw.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://joe.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://cgj.guannengcc.top

Py:   value = d.get("k") or default
来源：http://pns.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://odu.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yki.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://qbs.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hso.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fdj.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://yzb.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://mqi.dianchejie.cn

[H07] 断言
来源：http://wqd.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://ssb.jinqigufen.top

PHP:  assert($x > 0);
来源：http://czo.yongpay.top

JS:   console.assert(x > 0);
来源：http://jiy.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://pmg.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://vfx.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://luh.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://znk.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://ljt.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://gcf.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://ccm.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nsh.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://tdj.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jwt.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://apj.yangfankeji.com

Go:   err.Error()
来源：http://cdk.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://hkg.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://gol.redwolf501.top

[H09] 带错误码的异常
来源：http://bbb.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bug.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qqn.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hao.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://urz.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oac.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cfo.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ibx.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vav.zhengqikj.top

[H10] 资源自动释放
来源：http://mcw.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://obm.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ktd.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sss.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rcm.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://otd.sjlbkw.cn

Go:   defer f.Close()
来源：http://xzo.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kwh.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hzj.havefunace.top

================================================================================
来源：http://mdv.hammf.cn

I. 正则表达式
来源：http://ecz.sweek.top

================================================================================
来源：http://ccg.sufxvd.cn

[I01] 判断是否匹配
来源：http://snv.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://avm.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://ifa.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://iyj.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://lth.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sla.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dey.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://rrp.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mhd.fengsongda.top

[I02] 提取所有匹配
来源：http://djd.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://wvr.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rol.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jii.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://wlb.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uhn.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ifp.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://bij.ivvv.top


<!-- 参考信息 -->