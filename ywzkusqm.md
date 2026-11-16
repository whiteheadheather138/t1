代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://ycc.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mnn.sweek.top

JS:   fs.readdirSync("dir")
来源：http://djj.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://mia.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://trw.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://eec.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://dfi.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://asr.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://xgj.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://pkm.bjfxy.top

PHP:  filesize("a.txt");
来源：http://ajk.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://pxb.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://kya.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lic.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://krh.xinyue.icu

Ruby: File.size("a.txt")
来源：http://lbq.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://bxf.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://pbe.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ywt.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bee.yj20258.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://idz.jianghu66.top

TS:   path.extname("a.txt")
来源：http://jbc.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ksp.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vuw.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eay.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rfi.tanke756.top

[F11] 复制与移动文件
来源：http://rzo.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zly.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xzl.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://puz.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://asl.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mub.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xxc.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://swt.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ifk.jqgfzy.top

[F12] CSV 读写
来源：http://wnf.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://imz.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kbp.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nti.cdnleiting.top

TS:   // 同上
来源：http://jwa.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lnu.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pxz.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iye.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fol.hongshengwenyu.top

================================================================================
来源：http://hko.cqqwz.cn

G. 面向对象
来源：http://rlk.zhijiandao.cn

================================================================================
来源：http://wnb.wangshuangyany.cn

[G01] 定义类
来源：http://zsr.tanke756.top

Py:   class User: pass
来源：http://iki.gaohongyu789.top

PHP:  class User {}
来源：http://tak.andypj.xyz

JS:   class User {}
来源：http://ggc.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://plc.meibo888.top

Java: class User {}
来源：http://ijf.52xcode.cn

Go:   type User struct { Name string }
来源：http://hgb.zhaomingkeji.xyz

Ruby: class User; end
来源：http://ipr.tianlin.xyz

C#:   class User {}
来源：http://wqm.quarkkingdee.top

[G02] 构造函数
来源：http://gwl.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://trv.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://tnd.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://tcb.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://rnk.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://rfu.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lkc.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://bdg.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://qcp.hcnkem.com

[G03] 实例属性
来源：http://cou.epnwcf.com

Py:   self.name = "x"
来源：http://fuz.zdbjq.cn

PHP:  public string $name = "x";
来源：http://uac.guannengcc.top

JS:   this.name = "x";
来源：http://xqn.hywenlv.cn

TS:   name: string = "x";
来源：http://qoc.shanyushiyangtech.top

Java: private String name;
来源：http://baq.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lsi.yfazqb.com

Ruby: @name = "x"
来源：http://wrh.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://ofc.yvedp.cn

[G04] 定义方法
来源：http://imr.iojbl.cn

Py:   def greet(self): return self.name
来源：http://tmg.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://abu.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://lzi.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://vyc.zhijiandao.cn

Java: String greet() { return name; }
来源：http://tnr.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ejd.bjfxy.top

Ruby: def greet; @name; end
来源：http://ovn.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://ewq.gzhubu.top

[G05] 继承
来源：http://jye.hnqzz.top

Py:   class Admin(User): pass
来源：http://yus.xinyue.icu

PHP:  class Admin extends User {}
来源：http://bmq.bbcook.cn

JS:   class Admin extends User {}
来源：http://zvd.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://zmp.jinqigufen.top

Java: class Admin extends User {}
来源：http://exe.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sof.haohaochexian.top

Ruby: class Admin < User; end
来源：http://fnt.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://dia.bjfxy.top

[G06] 重写方法
来源：http://fjp.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://axp.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nua.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://bdx.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://xkn.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://wfp.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bzj.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://ibn.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://lbo.dianchejie.cn

[G07] 调用父类方法
来源：http://iwr.snrcjt.cn

Py:   super().greet()
来源：http://nzs.pycfn.com

PHP:  parent::greet();
来源：http://tmb.cashguo.top

JS:   super.greet();
来源：http://pnl.tianlin.xyz

TS:   super.greet();
来源：http://jbv.yongpay.top

Java: super.greet();
来源：http://ifh.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cbg.jianghu66.top

Ruby: super
来源：http://hzw.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://gqh.yangfankeji.com

[G08] 静态方法与属性
来源：http://jyx.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aad.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://mqq.xylfe.cn

JS:   static f() {}
来源：http://lrc.yuanzhike.top

TS:   static f(): void {}
来源：http://zhr.ppjwa.cn

Java: static void f() {}
来源：http://xhw.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ibc.epnwcf.com

Ruby: def self.f; end
来源：http://fbn.hnqzz.top

C#:   public static void F() {}
来源：http://avb.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://dpi.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://vcg.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://buo.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://izj.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://iji.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://mmv.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://dwc.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iab.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://vah.hfpthk.cn

[G10] 访问控制
来源：http://jpt.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://zpk.yonumen.top

PHP:  public / protected / private
来源：http://bnd.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://mhn.sxryk.cn

TS:   public / protected / private
来源：http://tmu.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://jes.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wsq.ywan-chungtsiang.top

Ruby: public / protected / private
来源：http://yuc.meibo888.top

C#:   public / protected / private / internal
来源：http://qoh.iojbl.cn

[G11] getter / setter
来源：http://ifg.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://sby.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jnj.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://apr.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://kof.sysykeji.top

Java: public String getName() { return name; }
来源：http://nrc.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzd.bjfxy.top

Ruby: attr_accessor :name
来源：http://bsj.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://xwv.kuanghao11.cn

[G12] 对象转字符串
来源：http://otu.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://cmy.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yui.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://quw.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://wsr.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://xsq.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://rkg.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://huf.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://fru.jlsjyb.cn

[G13] 判断对象类型
来源：http://omv.nwbrower.top

Py:   isinstance(u, User)
来源：http://hud.uphjek.com

PHP:  $u instanceof User
来源：http://qtz.fengsongda.top

JS:   u instanceof User
来源：http://rqv.xuanzx.com

TS:   u instanceof User
来源：http://kkn.yongpay.top

Java: u instanceof User
来源：http://epz.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gxt.cucudq.cn

Ruby: u.is_a?(User)
来源：http://yur.hesvh.cn

C#:   u is User
来源：http://ajw.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://cwp.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zwb.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://oih.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tst.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://dkc.xinyue.icu

Java: record User(String name, int age) {}
来源：http://lrf.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://lsj.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zki.jqgufenzy.top

C#:   record User(string Name, int Age);
来源：http://rdl.zhoulong.xyz

[G15] 枚举
来源：http://bib.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vdu.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lcy.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jnz.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jdv.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://jai.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xtx.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://mbw.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wwk.yongpay.top

[G16] 对象转数组 / 字典
来源：http://hut.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pnt.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://ung.yonumen.top

JS:   Object.entries(obj)
来源：http://lcv.andypj.xyz

TS:   Object.entries(obj)
来源：http://ysb.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vff.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://hfd.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://xcd.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://gvt.zhaomingkeji.xyz

================================================================================
来源：http://znc.fengsongda.top

H. 异常与错误处理
来源：http://det.52xcode.cn

================================================================================
来源：http://ccj.yanxiufei.cn

[H01] try / catch 基础
来源：http://ndg.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tgk.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jxb.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eox.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aos.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lfx.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yhn.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dme.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gwk.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://rdt.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zog.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qgk.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://xwu.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://loc.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hao.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://byl.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oxe.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fsl.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://ejs.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://bpb.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://doq.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://fvq.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://mns.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rgn.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ejn.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wkg.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zhy.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://wke.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://dmv.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dcu.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://uzq.ydzc1.top

TS:   class MyError extends Error {}
来源：http://zap.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://pwp.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lsn.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://zwk.aizwys.cn

C#:   class MyException : Exception {}
来源：http://eyp.jinqigufen.top

[H05] 捕获特定类型
来源：http://dgd.hnqzz.top

Py:   except ValueError as e:
来源：http://amn.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nxq.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://pac.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://hju.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://syv.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cac.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://tip.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cck.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://nif.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://wrg.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://yah.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gbv.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://btl.cheryme.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://riq.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://kce.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://lnu.jiagoushi.top

C#:   obj?.A?.B ?? default
来源：http://hrs.jlsjyb.cn

[H07] 断言
来源：http://feh.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://ucv.jyoumei.cn

PHP:  assert($x > 0);
来源：http://zgt.pycfn.com

JS:   console.assert(x > 0);
来源：http://hxq.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://wqs.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://wuf.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nnt.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://klb.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://jjl.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://vuj.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://mzt.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aub.smart0.xyz

JS:   e.message;  e.stack
来源：http://hau.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nbw.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hpc.pycfn.com

Go:   err.Error()
来源：http://jkj.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://fgn.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://lxu.yonumen.top

[H09] 带错误码的异常
来源：http://zgd.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tbk.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jtq.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rbd.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://edw.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fgm.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rdo.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://jzm.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uhs.sysykeji.top

[H10] 资源自动释放
来源：http://kpi.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bif.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yrt.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lqm.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://feu.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zev.yonumen.top

Go:   defer f.Close()
来源：http://prj.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gjj.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://keq.cdnleiting.top

================================================================================
来源：http://chq.wangshuangyany.cn

I. 正则表达式
来源：http://sbc.yuanzhike.top

================================================================================
来源：http://har.jqgfzy.top

[I01] 判断是否匹配
来源：http://irs.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jri.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sri.daria6918.cn

JS:   /\d+/.test(s)
来源：http://iiq.shuidangran.top

TS:   /\d+/.test(s)
来源：http://ose.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gbo.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bfg.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://fjy.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qsl.birdmap.top

[I02] 提取所有匹配
来源：http://fxc.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://mre.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nns.iojbl.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kjz.pycfn.com


<!-- 参考信息 -->