代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://txi.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://pyy.mhx1999.top

Ruby: Dir.children("dir")
来源：http://zes.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://bhk.shuidangran.top

[F09] 获取文件大小
来源：http://rmt.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://gzk.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://cxv.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://lhf.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://mrd.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cky.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxf.sxryk.cn

Ruby: File.size("a.txt")
来源：http://xjk.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://agy.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://dkl.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ggg.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ehd.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://anh.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://pld.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tus.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zda.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sza.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nbt.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://wjq.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sef.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cvg.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wcf.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fla.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mxz.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jox.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ngt.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zgg.tarul.cn

[F12] CSV 读写
来源：http://cun.fzhhl.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ihh.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rgr.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bqr.shuidangran.top

TS:   // 同上
来源：http://dxl.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://waf.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gys.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mxt.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ioj.fzhhl.top

================================================================================
来源：http://yjh.shuidangran.top

G. 面向对象
来源：http://cbm.epnwcf.com

================================================================================
来源：http://bqg.sysykeji.top

[G01] 定义类
来源：http://lud.shangyingyoupin.top

Py:   class User: pass
来源：http://jgk.yj202588.top

PHP:  class User {}
来源：http://yys.uphjek.com

JS:   class User {}
来源：http://qor.cheryme.top

TS:   class User { name: string = ""; }
来源：http://zzc.jiagoushi.top

Java: class User {}
来源：http://fgx.yj20258.top

Go:   type User struct { Name string }
来源：http://sve.52xcode.cn

Ruby: class User; end
来源：http://vvk.yj20258.top

C#:   class User {}
来源：http://hcb.ywan-chungtsiang.top

[G02] 构造函数
来源：http://tsf.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://dcy.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://jhq.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://fjn.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://jav.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://suq.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iug.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://kiv.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://qyp.ybcxt.top

[G03] 实例属性
来源：http://mbh.chenzaomai.com

Py:   self.name = "x"
来源：http://pif.sweek.top

PHP:  public string $name = "x";
来源：http://faz.mhx1999.top

JS:   this.name = "x";
来源：http://wkm.zhiwuduotai.top

TS:   name: string = "x";
来源：http://hyf.yj20258.top

Java: private String name;
来源：http://upu.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fgy.yuanzhike.top

Ruby: @name = "x"
来源：http://rqc.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://hdz.fzhhl.top

[G04] 定义方法
来源：http://mhd.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://jzj.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sgn.ivvv.top

JS:   greet() { return this.name; }
来源：http://yti.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://eoq.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://heu.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://wdj.316326.xyz

Ruby: def greet; @name; end
来源：http://cxo.sxryk.cn

C#:   public string Greet() => Name;
来源：http://cij.pengpengdd.cyou

[G05] 继承
来源：http://obn.yuxming.cn

Py:   class Admin(User): pass
来源：http://pwj.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://fqt.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://ozq.yj20258.top

TS:   class Admin extends User {}
来源：http://qai.yuxming.cn

Java: class Admin extends User {}
来源：http://pjg.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bhh.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://ffb.yuanzhike.top

C#:   class Admin : User {}
来源：http://voi.zhijiandao.cn

[G06] 重写方法
来源：http://qqn.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://xqo.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bhb.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://ugr.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://wqw.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://foj.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://huh.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://iiv.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://jty.hongshengwenyu.top

[G07] 调用父类方法
来源：http://ure.uphjek.com

Py:   super().greet()
来源：http://wwj.fehbvm.com

PHP:  parent::greet();
来源：http://qvu.9152youxi.cn

JS:   super.greet();
来源：http://nlu.hysaishi.cn

TS:   super.greet();
来源：http://gas.shanyushiyangkeji.top

Java: super.greet();
来源：http://ato.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ruz.uphjek.com

Ruby: super
来源：http://moz.guowangkeji.top

C#:   base.Greet();
来源：http://glt.yj20258.top

[G08] 静态方法与属性
来源：http://hbn.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://suz.shzxlz.cn

PHP:  public static function f() {}
来源：http://tsd.smart0.xyz

JS:   static f() {}
来源：http://mgj.xuetiantiany.cn

TS:   static f(): void {}
来源：http://cqi.shuidangran.top

Java: static void f() {}
来源：http://krf.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fhv.gogol.net.cn

Ruby: def self.f; end
来源：http://xka.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://cgj.c1oappe.top

[G09] 接口 / 抽象类
来源：http://avi.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://szs.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://job.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mgq.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://tow.xuanzx.com

Java: interface Shape { double area(); }
来源：http://aml.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://xri.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ann.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://uyk.tian-w.cn

[G10] 访问控制
来源：http://dij.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://sty.yongpay.top

PHP:  public / protected / private
来源：http://uxu.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://aps.yangfankeji.com

TS:   public / protected / private
来源：http://ibh.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://wyh.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ren.redwolf501.top

Ruby: public / protected / private
来源：http://fph.mhx1999.top

C#:   public / protected / private / internal
来源：http://jmu.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://dct.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://ixi.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dlh.bjfxy.top

JS:   get name() { return this._name; }
来源：http://tca.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://llh.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://uqo.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pxr.hnqzz.top

Ruby: attr_accessor :name
来源：http://wib.gzhubu.top

C#:   public string Name { get; set; }
来源：http://hlj.vehdjk.com

[G12] 对象转字符串
来源：http://sjj.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://hnw.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://iru.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://ajl.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://ffo.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://pzn.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://vye.ybcxt.top

Ruby: def to_s; @name; end
来源：http://ggx.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://lyo.mhx1999.top

[G13] 判断对象类型
来源：http://haa.zhixingplan.top

Py:   isinstance(u, User)
来源：http://bqi.yongpay.top

PHP:  $u instanceof User
来源：http://bis.hysaishi.cn

JS:   u instanceof User
来源：http://vdf.316326.xyz

TS:   u instanceof User
来源：http://aev.nanxinkj.top

Java: u instanceof User
来源：http://xna.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bml.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://xwg.uphjek.com

C#:   u is User
来源：http://lhf.tanke756.top

[G14] 数据类 / record
来源：http://hgq.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hys.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://rfd.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://psk.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://ttw.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://ydk.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://ocq.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://smj.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://qay.zhaomingkeji.xyz

[G15] 枚举
来源：http://fho.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://auo.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://igs.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pah.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bld.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://vyz.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vlw.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://lgg.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kss.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://dpm.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uqq.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://dua.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://uqt.guowangkeji.top

TS:   Object.entries(obj)
来源：http://sez.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fsl.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nbd.daxiang520.top

Ruby: obj.instance_variables
来源：http://kda.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://msc.zdbjq.cn

================================================================================
来源：http://qtv.cucudq.cn

H. 异常与错误处理
来源：http://uaf.ybcxt.top

================================================================================
来源：http://lqn.tarul.cn

[H01] try / catch 基础
来源：http://jul.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mkx.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ljv.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://chp.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uqk.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sjm.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nwx.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://drj.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vvs.daxiang520.top

[H02] finally / ensure 收尾
来源：http://tvx.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://job.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xnm.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qfi.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ayz.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aph.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://byt.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qnx.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://dbj.daxiang520.top

[H03] 主动抛出异常
来源：http://hka.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://ewe.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://onb.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://dbt.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://rer.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://onr.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xvq.hcnkem.com

Ruby: raise ArgumentError, "错误信息"
来源：http://eya.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lmh.yuxming.cn

[H04] 自定义异常类型
来源：http://pfm.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://jwv.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://oiz.mhx1999.top

JS:   class MyError extends Error {}
来源：http://luf.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://upe.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://hoz.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vfk.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://mvw.epnwcf.com

C#:   class MyException : Exception {}
来源：http://itm.cashguo.top

[H05] 捕获特定类型
来源：http://zpr.svipenyu.cn

Py:   except ValueError as e:
来源：http://how.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iyn.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://bgm.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://rlr.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://jin.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xst.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://vrk.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://deg.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://yle.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://fnp.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://nni.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://eed.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://ncl.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bmn.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mwe.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://xek.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://bzh.birdmap.top

[H07] 断言
来源：http://sqn.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://cky.sufxvd.cn

PHP:  assert($x > 0);
来源：http://vbg.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://ijq.xinyue.icu

TS:   console.assert(x > 0);
来源：http://vgd.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://yup.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mgv.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://xnx.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://iir.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://knp.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://xiy.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zag.cqqwz.cn

JS:   e.message;  e.stack
来源：http://ija.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://evp.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hll.yj20258888.top

Go:   err.Error()
来源：http://spa.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://vwb.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://zex.ydjk.org.cn

[H09] 带错误码的异常
来源：http://vpe.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vua.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qrc.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://esh.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lzx.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://stf.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aqc.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vkd.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qkf.yuanzhike.top

[H10] 资源自动释放
来源：http://jiq.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwc.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rcz.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zmg.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gff.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pmi.hysaishi.cn

Go:   defer f.Close()
来源：http://fii.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wxm.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tyz.svipenyu.cn

================================================================================
来源：http://nwa.gotoacloud.top

I. 正则表达式
来源：http://iji.chenlongwang.top

================================================================================
来源：http://ifq.tanke756.top

[I01] 判断是否匹配
来源：http://fwh.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://buq.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://jsf.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://fqu.andypj.xyz

TS:   /\d+/.test(s)
来源：http://wjr.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vye.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vkr.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://qre.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yuq.jiagoushi.top

[I02] 提取所有匹配
来源：http://aky.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://oqb.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://czb.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tzv.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://qxx.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bns.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hcw.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://ugk.ydjk.org.cn


<!-- 参考信息 -->