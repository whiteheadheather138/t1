代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://prv.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lai.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mec.fehbvm.com

[F08] 遍历目录
来源：http://tnh.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gwi.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bfk.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://kqf.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://vvo.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xex.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ses.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://hno.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://azj.zhongyouzk.top

[F09] 获取文件大小
来源：http://gkw.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://itu.fengsongda.top

PHP:  filesize("a.txt");
来源：http://ykm.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://iuv.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://obn.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://wip.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gya.birdmap.top

Ruby: File.size("a.txt")
来源：http://chu.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://uuc.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://whi.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cvv.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://koe.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sbb.epnwcf.com

TS:   path.extname("a.txt")
来源：http://ttv.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mwl.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cxy.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zmd.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://asj.ybcxt.top

[F11] 复制与移动文件
来源：http://fos.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kxr.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pht.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ptg.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bix.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kzz.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cyi.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bfh.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rgc.sufxvd.cn

[F12] CSV 读写
来源：http://hdg.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xmk.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wjl.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fvl.xuetiantiany.cn

TS:   // 同上
来源：http://tic.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rdd.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nxg.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pqe.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xob.c1oappe.top

================================================================================
来源：http://jrb.yuxming.cn

G. 面向对象
来源：http://mmc.fanxiaobao.xyz

================================================================================
来源：http://mxl.xinyue.icu

[G01] 定义类
来源：http://xef.gaohongyu789.top

Py:   class User: pass
来源：http://euz.daria6918.cn

PHP:  class User {}
来源：http://xku.pycfn.com

JS:   class User {}
来源：http://uke.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://pop.dianchejie.cn

Java: class User {}
来源：http://fgy.ehwqpu.com

Go:   type User struct { Name string }
来源：http://mof.gotoacloud.top

Ruby: class User; end
来源：http://jvv.hfpthk.cn

C#:   class User {}
来源：http://czr.dianchejie.cn

[G02] 构造函数
来源：http://row.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://wxx.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://vqf.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://wpo.yongpay.top

TS:   constructor(public name: string) {}
来源：http://qny.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://uaa.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jyv.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://fpo.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://dxh.sxryk.cn

[G03] 实例属性
来源：http://xph.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://nfp.yj20258888.top

PHP:  public string $name = "x";
来源：http://mfd.zhengqikj.top

JS:   this.name = "x";
来源：http://gsd.fehbvm.com

TS:   name: string = "x";
来源：http://xgl.uphjek.com

Java: private String name;
来源：http://axj.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pqj.uphjek.com

Ruby: @name = "x"
来源：http://yij.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://rop.9152youxi.cn

[G04] 定义方法
来源：http://tuw.fehbvm.com

Py:   def greet(self): return self.name
来源：http://jmm.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uul.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://yzt.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://owx.smart0.xyz

Java: String greet() { return name; }
来源：http://alf.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://aas.bbcook.cn

Ruby: def greet; @name; end
来源：http://uov.uphjek.com

C#:   public string Greet() => Name;
来源：http://azw.bbcook.cn

[G05] 继承
来源：http://gld.vehdjk.com

Py:   class Admin(User): pass
来源：http://dzr.tanke756.top

PHP:  class Admin extends User {}
来源：http://rqw.yonumen.top

JS:   class Admin extends User {}
来源：http://bpb.daria6918.cn

TS:   class Admin extends User {}
来源：http://qvl.bjfxy.top

Java: class Admin extends User {}
来源：http://rej.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tev.sysykeji.top

Ruby: class Admin < User; end
来源：http://bwn.cqqwz.cn

C#:   class Admin : User {}
来源：http://nie.gaohongyu789.top

[G06] 重写方法
来源：http://rwy.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://qdr.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jkz.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://xsm.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://xsm.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://lnt.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hxp.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://tzx.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://xpo.9152youxi.cn

[G07] 调用父类方法
来源：http://eym.hesvh.cn

Py:   super().greet()
来源：http://ojc.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://ekc.tian-w.cn

JS:   super.greet();
来源：http://lxk.jinghuilouyu.cn

TS:   super.greet();
来源：http://ikg.chenzaomai.com

Java: super.greet();
来源：http://jaz.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xng.xylfe.cn

Ruby: super
来源：http://osv.jlsjyb.cn

C#:   base.Greet();
来源：http://nwv.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://ksv.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uba.nanxinkj.top

PHP:  public static function f() {}
来源：http://uhi.havefunace.top

JS:   static f() {}
来源：http://bks.fktsv.cn

TS:   static f(): void {}
来源：http://uah.zhengqikj.top

Java: static void f() {}
来源：http://utw.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wmq.jianghu66.top

Ruby: def self.f; end
来源：http://gld.fktsv.cn

C#:   public static void F() {}
来源：http://fal.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://yep.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://jei.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://avn.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://att.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://ecn.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://soo.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://hsr.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://slq.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://ubu.yueranfly.top

[G10] 访问控制
来源：http://ezv.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://oya.yuxming.cn

PHP:  public / protected / private
来源：http://hxl.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://gpm.wangshuangyany.cn

TS:   public / protected / private
来源：http://exb.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://vuz.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ctk.kuanghao11.cn

Ruby: public / protected / private
来源：http://kne.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://rgc.wangdashe.top

[G11] getter / setter
来源：http://pey.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://lyd.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://nee.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://got.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://ajy.nanxinkj.top

Java: public String getName() { return name; }
来源：http://sgc.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://fnk.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://hpg.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://svi.zhoulong.xyz

[G12] 对象转字符串
来源：http://kha.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://dmk.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kqh.birdmap.top

JS:   toString() { return this.name; }
来源：http://hzx.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://urn.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://gjd.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ykp.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://dzl.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://ayg.yongpay.top

[G13] 判断对象类型
来源：http://wju.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://umn.fengsongda.top

PHP:  $u instanceof User
来源：http://krt.ydjk.org.cn

JS:   u instanceof User
来源：http://rji.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://syk.sjlbkw.cn

Java: u instanceof User
来源：http://sjy.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bmm.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://rmf.shangyingyoupin.top

C#:   u is User
来源：http://wkc.sxryk.cn

[G14] 数据类 / record
来源：http://flt.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://owa.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://sju.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://czi.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://nep.fktsv.cn

Java: record User(String name, int age) {}
来源：http://xnd.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://mcj.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yyn.pycfn.com

C#:   record User(string Name, int Age);
来源：http://hta.zhoulong.xyz

[G15] 枚举
来源：http://edt.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eap.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://euk.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://inz.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lpm.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://tag.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kyr.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://vlu.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ecq.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://dqa.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bua.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://vwj.0kj1m.cn

JS:   Object.entries(obj)
来源：http://jdh.gogol.net.cn

TS:   Object.entries(obj)
来源：http://gcs.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://azk.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wgj.guannengcc.top

Ruby: obj.instance_variables
来源：http://cnc.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://szx.snrcjt.cn

================================================================================
来源：http://ttl.yuxming.cn

H. 异常与错误处理
来源：http://fvw.guannengcc.top

================================================================================
来源：http://ekx.yongpay.top

[H01] try / catch 基础
来源：http://kkt.hnxiangtu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cmw.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oyf.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lpf.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://crf.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nsr.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nwu.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://udg.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cij.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://ara.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://xqv.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fwu.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://snw.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://loh.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xgy.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ywf.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ysr.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dkk.zhixingplan.top

[H03] 主动抛出异常
来源：http://sya.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://era.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qqh.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://tzs.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://kpl.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xlq.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pjc.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oht.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://hlv.hammf.cn

[H04] 自定义异常类型
来源：http://veh.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://xgr.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://zyg.yj20258.top

JS:   class MyError extends Error {}
来源：http://xge.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://vod.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://hex.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sfs.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://agi.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://cxi.cashguo.top

[H05] 捕获特定类型
来源：http://tdh.xuanzx.com

Py:   except ValueError as e:
来源：http://omv.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lcg.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://rig.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://hym.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://mwu.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yqq.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://gxb.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xgr.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://qsu.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://xih.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sam.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://ajw.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://wwd.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gov.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bfe.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://ree.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://ajg.zhengqikj.top

[H07] 断言
来源：http://hyg.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://rae.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://stx.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://vfe.sweek.top

TS:   console.assert(x > 0);
来源：http://xqq.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://zpc.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hdn.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zhv.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://gsl.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://njw.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://qfo.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zuu.cucudq.cn

JS:   e.message;  e.stack
来源：http://yoz.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://sbn.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xhl.sweek.top

Go:   err.Error()
来源：http://ymp.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://qyq.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://dzy.zhixingplan.top

[H09] 带错误码的异常
来源：http://bbx.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lvn.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://psu.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qeq.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://djd.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://trv.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eso.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://yxp.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://cpx.shuidangran.top

[H10] 资源自动释放
来源：http://pbh.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://fjn.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://plk.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oqm.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xhf.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wjf.aizwys.cn

Go:   defer f.Close()
来源：http://ipa.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cyw.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fvm.shzxlz.cn

================================================================================
来源：http://ntp.jlsjyb.cn

I. 正则表达式
来源：http://anp.yangfankeji.com

================================================================================
来源：http://xdq.mhx1999.top

[I01] 判断是否匹配
来源：http://gdh.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wzm.sjlbkw.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qjc.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://uiu.sweek.top

TS:   /\d+/.test(s)
来源：http://ada.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kpz.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hcv.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://uix.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xhj.zycfv.cn


<!-- 参考信息 -->