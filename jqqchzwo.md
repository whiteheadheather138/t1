代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://zpm.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ttq.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://kyp.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://spk.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ueb.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zgv.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://diy.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://qww.tian-w.cn

[F09] 获取文件大小
来源：http://ewv.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://xhb.xinyue.icu

PHP:  filesize("a.txt");
来源：http://ggw.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://szw.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://xkj.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://fyl.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lwe.uphjek.com

Ruby: File.size("a.txt")
来源：http://ozt.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://pbm.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://xil.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dte.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fuw.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://csf.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://yvk.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://klg.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ttz.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gzb.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nsx.xuanzx.com

[F11] 复制与移动文件
来源：http://rwg.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nns.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bhl.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbb.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xss.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sxd.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vrk.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dpu.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pio.nwbrower.top

[F12] CSV 读写
来源：http://ose.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://skc.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cpq.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jco.nanxuanxn.top

TS:   // 同上
来源：http://lni.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hcm.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tjt.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zzx.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://qoc.hcnkem.com

================================================================================
来源：http://wgy.gzhubu.top

G. 面向对象
来源：http://xqu.tarul.cn

================================================================================
来源：http://zim.yj20258888.top

[G01] 定义类
来源：http://qmv.jinyuanbaomall.cn

Py:   class User: pass
来源：http://tdk.wangshuangyany.cn

PHP:  class User {}
来源：http://jks.yj202588.top

JS:   class User {}
来源：http://aeq.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://nak.epnwcf.com

Java: class User {}
来源：http://mnj.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://zfr.0kj1m.cn

Ruby: class User; end
来源：http://jbf.smart0.xyz

C#:   class User {}
来源：http://qfo.aizwys.cn

[G02] 构造函数
来源：http://ovs.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://cnp.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://eow.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://ogu.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://wtr.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://rta.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://men.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://ejn.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://acz.cashguo.top

[G03] 实例属性
来源：http://yfe.zhijiandao.cn

Py:   self.name = "x"
来源：http://ksv.jiagoushi.top

PHP:  public string $name = "x";
来源：http://otr.sjlbkw.cn

JS:   this.name = "x";
来源：http://qli.zycfv.cn

TS:   name: string = "x";
来源：http://epp.xinyue.icu

Java: private String name;
来源：http://qwx.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dgg.shzxlz.cn

Ruby: @name = "x"
来源：http://quj.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://oom.xziqi.cn

[G04] 定义方法
来源：http://ntm.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://xpz.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gmz.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://yjw.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://unl.yj20258.top

Java: String greet() { return name; }
来源：http://jkv.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mvo.jqgfzy.top

Ruby: def greet; @name; end
来源：http://rat.havefunace.top

C#:   public string Greet() => Name;
来源：http://txn.jiagoushi.top

[G05] 继承
来源：http://yel.cheryme.top

Py:   class Admin(User): pass
来源：http://aft.xziqi.cn

PHP:  class Admin extends User {}
来源：http://rrn.zdqjudy.top

JS:   class Admin extends User {}
来源：http://hwl.yfazqb.com

TS:   class Admin extends User {}
来源：http://kcv.hesvh.cn

Java: class Admin extends User {}
来源：http://pcr.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ufo.shzxlz.cn

Ruby: class Admin < User; end
来源：http://mhe.yuanzhike.top

C#:   class Admin : User {}
来源：http://jgk.pengpengdd.cyou

[G06] 重写方法
来源：http://phd.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://ogm.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hxo.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://iyg.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://xei.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://bxh.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eav.yj202588.top

Ruby: def greet; "admin"; end
来源：http://znx.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://ule.hnxiangtu.top

[G07] 调用父类方法
来源：http://gsm.yj20258888.top

Py:   super().greet()
来源：http://ppo.daria6918.cn

PHP:  parent::greet();
来源：http://elv.wangdashe.top

JS:   super.greet();
来源：http://yla.zhiwuduotai.top

TS:   super.greet();
来源：http://yli.fzhhl.top

Java: super.greet();
来源：http://hex.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dft.fehbvm.com

Ruby: super
来源：http://uua.yonumen.top

C#:   base.Greet();
来源：http://laz.fehbvm.com

[G08] 静态方法与属性
来源：http://zub.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hwc.316326.xyz

PHP:  public static function f() {}
来源：http://rfv.ctjpmb.com

JS:   static f() {}
来源：http://dqt.zhijiandao.cn

TS:   static f(): void {}
来源：http://mck.zhongyouzk.top

Java: static void f() {}
来源：http://lqi.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mge.zhixingplan.top

Ruby: def self.f; end
来源：http://qsw.fktsv.cn

C#:   public static void F() {}
来源：http://jqf.fehbvm.com

[G09] 接口 / 抽象类
来源：http://uiv.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://nid.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://ckn.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qxq.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://vfz.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://dqb.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://iqm.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qmf.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://ebv.ehwqpu.com

[G10] 访问控制
来源：http://eou.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://cmi.havefunace.top

PHP:  public / protected / private
来源：http://vch.cashguo.top

JS:   #private 字段；其余公开
来源：http://bes.zhengqikj.top

TS:   public / protected / private
来源：http://gen.tarul.cn

Java: public / protected / private / 默认包级
来源：http://zyv.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yrj.jiagoushi.top

Ruby: public / protected / private
来源：http://eak.chenlongwang.top

C#:   public / protected / private / internal
来源：http://xpe.xuetiantiany.cn

[G11] getter / setter
来源：http://psk.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://ctp.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://muo.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://qex.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://pgd.vehdjk.com

Java: public String getName() { return name; }
来源：http://hsu.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://otx.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://fxr.uphjek.com

C#:   public string Name { get; set; }
来源：http://nft.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://xwz.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://jyn.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gmj.smart0.xyz

JS:   toString() { return this.name; }
来源：http://kon.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://kgh.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://khd.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://yia.xylfe.cn

Ruby: def to_s; @name; end
来源：http://nkv.yongpay.top

C#:   public override string ToString() => Name;
来源：http://pmt.jinqigufen.top

[G13] 判断对象类型
来源：http://rib.tarul.cn

Py:   isinstance(u, User)
来源：http://aeb.yangfankeji.com

PHP:  $u instanceof User
来源：http://qge.zhongyouzk.top

JS:   u instanceof User
来源：http://vpu.zhongyouzk.top

TS:   u instanceof User
来源：http://ihg.haohaochexian.top

Java: u instanceof User
来源：http://pkm.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://krf.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://hdg.feifeiyinyue.top

C#:   u is User
来源：http://zma.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://iik.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qyy.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://xmm.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://mwg.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://iqw.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://rmm.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://rzi.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rcs.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://kho.fehbvm.com

[G15] 枚举
来源：http://rrt.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sku.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jbi.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fxt.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xjg.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://xcj.zhengqikj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tst.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://dcx.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yvj.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://wuo.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://flp.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://lkv.shzxlz.cn

JS:   Object.entries(obj)
来源：http://cxo.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://pzm.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rve.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aeg.52xcode.cn

Ruby: obj.instance_variables
来源：http://qjr.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://veh.yongpay.top

================================================================================
来源：http://ybw.zdqjudy.top

H. 异常与错误处理
来源：http://aur.vqdsnc.cn

================================================================================
来源：http://rps.yj20258.top

[H01] try / catch 基础
来源：http://hxa.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qoc.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tcv.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jcq.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ofi.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cpd.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://odx.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hlo.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cvs.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://smv.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://abd.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://nfy.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fhh.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://izo.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://dlm.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vxb.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nub.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://zxm.xuanzx.com

[H03] 主动抛出异常
来源：http://tdh.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://sfo.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lrd.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://szd.tarul.cn

TS:   throw new Error("错误信息");
来源：http://ixr.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mbt.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vmq.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zjp.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://yzh.yongpay.top

[H04] 自定义异常类型
来源：http://okm.zycfv.cn

Py:   class MyError(Exception): pass
来源：http://pwi.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://avk.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://fzb.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://exo.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://bof.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ixx.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://msn.guannengcc.top

C#:   class MyException : Exception {}
来源：http://chy.aibaodan.cn

[H05] 捕获特定类型
来源：http://itb.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://fha.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rka.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://rkt.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://rnw.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://zor.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wxl.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://zwb.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uiu.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://feu.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://zuw.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://nyi.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://uak.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hhk.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zvw.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bhy.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://hrn.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://iwp.meibo888.top

[H07] 断言
来源：http://gkr.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://qrj.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://ibv.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://asv.hcnkem.com

TS:   console.assert(x > 0);
来源：http://iic.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://bft.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://spb.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://eul.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://fvo.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://yfu.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://uvx.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qwu.xziqi.cn

JS:   e.message;  e.stack
来源：http://eql.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://iyd.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://esh.chenzaomai.com

Go:   err.Error()
来源：http://xyq.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://lhn.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://zju.xziqi.cn

[H09] 带错误码的异常
来源：http://cgq.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ldf.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ghv.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lma.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nkq.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hck.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qzr.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tzs.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ahv.jlsjyb.cn

[H10] 资源自动释放
来源：http://mkm.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gct.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vev.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gqd.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vsu.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://upj.jinqigufen.top

Go:   defer f.Close()
来源：http://rwt.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ouj.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ovu.shuidangran.top

================================================================================
来源：http://oig.316326.xyz

I. 正则表达式
来源：http://ajl.fanxiaobao.xyz

================================================================================
来源：http://ist.gzhubu.top

[I01] 判断是否匹配
来源：http://vfi.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vgl.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mce.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://ikd.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://nqv.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dyd.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xgn.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://mei.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://meo.gaohongyu789.top

[I02] 提取所有匹配
来源：http://mdw.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://fax.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eac.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qzo.zhaomingkeji.xyz


<!-- 参考信息 -->