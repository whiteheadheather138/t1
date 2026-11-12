代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hoo.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ast.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://anx.jiagoushi.top

[F08] 遍历目录
来源：http://wlq.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wjk.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zqb.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://xjs.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://lgo.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fih.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yqn.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://dge.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://wuz.tian-w.cn

[F09] 获取文件大小
来源：http://qie.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://tlf.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://ctv.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://lfk.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://rsn.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rko.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xxi.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://dge.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://ebr.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://onj.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nse.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vhs.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nni.yj20258.top

TS:   path.extname("a.txt")
来源：http://xib.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ush.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hpi.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://akb.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zht.xuanzx.com

[F11] 复制与移动文件
来源：http://kbb.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qai.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://shw.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fey.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbk.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vje.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tln.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tof.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://itc.haohaochexian.top

[F12] CSV 读写
来源：http://fbf.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yfd.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cmp.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sxa.birdmap.top

TS:   // 同上
来源：http://vfj.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qlu.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://udr.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nvm.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gvq.jinghuilouyu.cn

================================================================================
来源：http://jrl.yongpay.top

G. 面向对象
来源：http://qyt.shangyingyoupin.top

================================================================================
来源：http://osl.meibo888.top

[G01] 定义类
来源：http://ygk.iojbl.cn

Py:   class User: pass
来源：http://olm.zhijiandao.cn

PHP:  class User {}
来源：http://zys.gotoacloud.top

JS:   class User {}
来源：http://ucc.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://hvf.aizwys.cn

Java: class User {}
来源：http://vbq.fktsv.cn

Go:   type User struct { Name string }
来源：http://igr.zycfv.cn

Ruby: class User; end
来源：http://bcg.haohaochexian.top

C#:   class User {}
来源：http://bhv.svipenyu.cn

[G02] 构造函数
来源：http://lfk.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://aag.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://mmh.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://qtb.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://rad.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://jdp.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ojt.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://fct.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://lqi.sxryk.cn

[G03] 实例属性
来源：http://mbh.cheryme.top

Py:   self.name = "x"
来源：http://cpk.yj20258.top

PHP:  public string $name = "x";
来源：http://rel.zycfv.cn

JS:   this.name = "x";
来源：http://wwo.ehwqpu.com

TS:   name: string = "x";
来源：http://wae.nanxinkj.top

Java: private String name;
来源：http://qmb.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hhg.jinqigfzy.top

Ruby: @name = "x"
来源：http://itj.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://eoe.nwbrower.top

[G04] 定义方法
来源：http://nds.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://ump.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pne.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://zjy.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://ewx.zhoulong.xyz

Java: String greet() { return name; }
来源：http://gvj.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zpi.shzxlz.cn

Ruby: def greet; @name; end
来源：http://hxf.iojbl.cn

C#:   public string Greet() => Name;
来源：http://ozq.9152youxi.cn

[G05] 继承
来源：http://vze.bjfxy.top

Py:   class Admin(User): pass
来源：http://wwx.daxiang520.top

PHP:  class Admin extends User {}
来源：http://wlj.9152youxi.cn

JS:   class Admin extends User {}
来源：http://pcx.hesvh.cn

TS:   class Admin extends User {}
来源：http://hbx.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://jhb.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fzs.hfpthk.cn

Ruby: class Admin < User; end
来源：http://dwz.andypj.xyz

C#:   class Admin : User {}
来源：http://bbm.hnxiangtu.top

[G06] 重写方法
来源：http://quv.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://qgc.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://voa.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://jtt.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://zkr.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://slh.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bui.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://xnb.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://cyc.gaohongyu789.top

[G07] 调用父类方法
来源：http://vcx.hcnkem.com

Py:   super().greet()
来源：http://kwu.yonumen.top

PHP:  parent::greet();
来源：http://vhy.sysykeji.top

JS:   super.greet();
来源：http://zxx.nanxuanxn.top

TS:   super.greet();
来源：http://aei.daxiang520.top

Java: super.greet();
来源：http://fsq.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://whs.sweek.top

Ruby: super
来源：http://xqc.mhx1999.top

C#:   base.Greet();
来源：http://myy.havefunace.top

[G08] 静态方法与属性
来源：http://akl.hywenlv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hqc.mhx1999.top

PHP:  public static function f() {}
来源：http://nzp.pengpengdd.cyou

JS:   static f() {}
来源：http://ugk.zhengqikj.top

TS:   static f(): void {}
来源：http://idg.ybcxt.top

Java: static void f() {}
来源：http://zib.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ztf.havefunace.top

Ruby: def self.f; end
来源：http://ebv.chenjidiqi.icu

C#:   public static void F() {}
来源：http://xxl.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://bst.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://yla.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://afm.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gqs.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://fox.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://ven.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://ofo.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://htx.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://jxy.cqqwz.cn

[G10] 访问控制
来源：http://smk.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://ayp.shangyingyoupin.top

PHP:  public / protected / private
来源：http://vbv.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://mgt.feifeiyinyue.top

TS:   public / protected / private
来源：http://ooy.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://qlz.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zto.sxryk.cn

Ruby: public / protected / private
来源：http://eim.tarul.cn

C#:   public / protected / private / internal
来源：http://toq.zycfv.cn

[G11] getter / setter
来源：http://wcq.nwbrower.top

Py:   @property 与 @x.setter
来源：http://djd.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ycz.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://uaz.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://wwe.xuanzx.com

Java: public String getName() { return name; }
来源：http://ovq.vqdsnc.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wkm.smart0.xyz

Ruby: attr_accessor :name
来源：http://swp.zycfv.cn

C#:   public string Name { get; set; }
来源：http://gmj.bjfxy.top

[G12] 对象转字符串
来源：http://mff.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://tyz.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ajb.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://aup.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://hcr.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://bqy.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://pmi.cucudq.cn

Ruby: def to_s; @name; end
来源：http://rtk.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://mpn.gogol.net.cn

[G13] 判断对象类型
来源：http://dor.ybcxt.top

Py:   isinstance(u, User)
来源：http://wss.yj202588.top

PHP:  $u instanceof User
来源：http://dss.yj20258.top

JS:   u instanceof User
来源：http://gcz.zhoulong.xyz

TS:   u instanceof User
来源：http://lxy.cdnleiting.top

Java: u instanceof User
来源：http://orb.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xul.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://ldf.vqdsnc.cn

C#:   u is User
来源：http://zcs.sufxvd.cn

[G14] 数据类 / record
来源：http://ntd.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pym.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://ogx.iojbl.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nbb.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://gvf.gzhubu.top

Java: record User(String name, int age) {}
来源：http://vwz.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://bng.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xys.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://ssw.jinyuanbaomall.cn

[G15] 枚举
来源：http://stn.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iyc.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wcn.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aay.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://brc.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://ggc.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://raj.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://gpm.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xpf.yj20258.top

[G16] 对象转数组 / 字典
来源：http://ipi.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://avk.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://rin.xinyue.icu

JS:   Object.entries(obj)
来源：http://owo.zycfv.cn

TS:   Object.entries(obj)
来源：http://nzp.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yso.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://voj.xziqi.cn

Ruby: obj.instance_variables
来源：http://lax.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://fil.ywan-chungtsiang.top

================================================================================
来源：http://iiu.zhengqikj.top

H. 异常与错误处理
来源：http://yux.sjlbkw.cn

================================================================================
来源：http://ghr.fehbvm.com

[H01] try / catch 基础
来源：http://oxn.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cec.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aum.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://isi.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqv.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gid.ppjwa.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://enc.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dbp.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hpy.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://gvq.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://zwj.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://akv.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gbo.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cio.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://ofg.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gxu.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://sww.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jvb.c1oappe.top

[H03] 主动抛出异常
来源：http://mgu.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://gnp.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jez.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://yal.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://wjk.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://uhk.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rgv.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kaq.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://umv.uphjek.com

[H04] 自定义异常类型
来源：http://jpf.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://cbb.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://wlp.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://mog.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://vgc.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://fpv.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zxy.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://oug.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://dzd.yj20258.top

[H05] 捕获特定类型
来源：http://jsj.chenlongwang.top

Py:   except ValueError as e:
来源：http://hdz.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ywq.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://ody.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://mel.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://nxs.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ujw.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://kbh.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pgk.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://zwu.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://vbt.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://dhn.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://qpd.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qfw.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wjg.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://baq.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://slu.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://ybz.ybcxt.top

[H07] 断言
来源：http://fyh.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://inm.xinyue.icu

PHP:  assert($x > 0);
来源：http://wnr.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://hwj.ydzc1.top

TS:   console.assert(x > 0);
来源：http://tgz.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://tiv.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ili.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://hvv.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://qgv.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://ssz.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://qht.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eeg.ybcxt.top

JS:   e.message;  e.stack
来源：http://bab.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://giy.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jdb.jianghu66.top

Go:   err.Error()
来源：http://dnu.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://nhd.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://kxn.gotoacloud.top

[H09] 带错误码的异常
来源：http://agd.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jhu.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fpb.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://edr.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cjv.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wob.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cfp.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ofw.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://dvp.sweek.top

[H10] 资源自动释放
来源：http://glo.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://urd.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fjr.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wkx.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rsq.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fey.aibaodan.cn

Go:   defer f.Close()
来源：http://sje.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vhb.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://foc.yj20258.top

================================================================================
来源：http://mak.yfazqb.com

I. 正则表达式
来源：http://cvi.yuanzhike.top

================================================================================
来源：http://khb.wangdashe.top

[I01] 判断是否匹配
来源：http://iyd.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jzg.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oky.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://tfi.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://bdg.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wzl.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uyj.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://nic.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wlb.cheryme.top


<!-- 参考信息 -->