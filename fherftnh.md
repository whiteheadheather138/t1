代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hji.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://bjo.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://tcg.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qwz.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://glk.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nnz.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://syq.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tbb.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gwk.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gvo.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pxx.jinqigfzy.top

[F08] 遍历目录
来源：http://vyk.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://qnm.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://khs.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://ddm.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://ool.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rrp.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qey.jianghu66.top

Ruby: Dir.children("dir")
来源：http://hry.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://gpg.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://ezf.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://xkz.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://fbd.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://cud.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://zmh.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gvu.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zho.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://xmz.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://ird.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://vae.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vrx.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ilz.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://plh.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://jkl.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://atn.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lkm.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mso.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sks.sjlbkw.cn

[F11] 复制与移动文件
来源：http://qem.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://psg.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bgo.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tvt.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lfz.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vld.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ecn.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zdd.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nzh.pycfn.com

[F12] CSV 读写
来源：http://ams.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lyo.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bih.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ker.wangdashe.top

TS:   // 同上
来源：http://avi.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xby.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pkj.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blu.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jgn.ydjk.org.cn

================================================================================
来源：http://fjg.wangshuangyany.cn

G. 面向对象
来源：http://eda.xylfe.cn

================================================================================
来源：http://ahn.birdmap.top

[G01] 定义类
来源：http://cwu.jyoumei.cn

Py:   class User: pass
来源：http://cok.shzxlz.cn

PHP:  class User {}
来源：http://ckx.yueranfly.top

JS:   class User {}
来源：http://yam.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://oux.gogol.net.cn

Java: class User {}
来源：http://kbc.yuxming.cn

Go:   type User struct { Name string }
来源：http://jiy.yj20258888.top

Ruby: class User; end
来源：http://zes.jinyuanbaomall.cn

C#:   class User {}
来源：http://vaz.nanxuanxn.top

[G02] 构造函数
来源：http://dsp.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://jqu.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://jzl.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://uqm.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://lhi.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://uiy.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wvr.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://vnt.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://kjo.uphjek.com

[G03] 实例属性
来源：http://sub.hfpthk.cn

Py:   self.name = "x"
来源：http://nlq.zhengqikj.top

PHP:  public string $name = "x";
来源：http://hbn.hcnkem.com

JS:   this.name = "x";
来源：http://jna.guannengcc.top

TS:   name: string = "x";
来源：http://gii.yvedp.cn

Java: private String name;
来源：http://dom.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fbt.ivvv.top

Ruby: @name = "x"
来源：http://dbu.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://jhw.daxiang520.top

[G04] 定义方法
来源：http://sgl.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://hbo.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sbn.tanke756.top

JS:   greet() { return this.name; }
来源：http://gre.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://vls.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://hzu.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://iyb.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://doe.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://jhc.zdbjq.cn

[G05] 继承
来源：http://wjq.yueranfly.top

Py:   class Admin(User): pass
来源：http://bva.zycfv.cn

PHP:  class Admin extends User {}
来源：http://cqi.yj20258.top

JS:   class Admin extends User {}
来源：http://wla.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://kzj.xziqi.cn

Java: class Admin extends User {}
来源：http://jco.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://shh.cqqwz.cn

Ruby: class Admin < User; end
来源：http://ahk.hnqzz.top

C#:   class Admin : User {}
来源：http://hck.xziqi.cn

[G06] 重写方法
来源：http://sac.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://alk.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cut.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://ope.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://ihd.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://kjp.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nwu.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://cxj.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://pyk.dianchejie.cn

[G07] 调用父类方法
来源：http://lns.tianlin.xyz

Py:   super().greet()
来源：http://yqi.yangfankeji.com

PHP:  parent::greet();
来源：http://qoy.xuetiantiany.cn

JS:   super.greet();
来源：http://czr.cheryme.top

TS:   super.greet();
来源：http://zyn.bbcook.cn

Java: super.greet();
来源：http://aap.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iix.snrcjt.cn

Ruby: super
来源：http://wcc.xuetiantiany.cn

C#:   base.Greet();
来源：http://wvq.quarkkingdee.top

[G08] 静态方法与属性
来源：http://dli.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://etg.jiagoushi.top

PHP:  public static function f() {}
来源：http://ipg.havefunace.top

JS:   static f() {}
来源：http://vgs.yueranfly.top

TS:   static f(): void {}
来源：http://yyq.jinghuilouyu.cn

Java: static void f() {}
来源：http://tst.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://muo.bjfxy.top

Ruby: def self.f; end
来源：http://qqe.daxiang520.top

C#:   public static void F() {}
来源：http://lod.cheryme.top

[G09] 接口 / 抽象类
来源：http://rgs.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://krj.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://fzq.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://opn.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://zsm.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://bpx.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://mir.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xgp.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://zbw.cdnleiting.top

[G10] 访问控制
来源：http://jkb.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://eet.xuanzx.com

PHP:  public / protected / private
来源：http://yah.smart0.xyz

JS:   #private 字段；其余公开
来源：http://dvi.uphjek.com

TS:   public / protected / private
来源：http://qdu.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://xgt.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zon.cdnleiting.top

Ruby: public / protected / private
来源：http://img.tian-w.cn

C#:   public / protected / private / internal
来源：http://meg.xuanzx.com

[G11] getter / setter
来源：http://adg.yongpay.top

Py:   @property 与 @x.setter
来源：http://rso.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://myg.gotoacloud.top

JS:   get name() { return this._name; }
来源：http://cto.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://ckh.yj20258.top

Java: public String getName() { return name; }
来源：http://gjg.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jxp.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://djn.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://ffe.guannengcc.top

[G12] 对象转字符串
来源：http://qrd.tarul.cn

Py:   def __str__(self): return self.name
来源：http://dih.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ktt.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://uif.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://sub.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://rut.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://jpy.birdmap.top

Ruby: def to_s; @name; end
来源：http://jar.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://kml.snrcjt.cn

[G13] 判断对象类型
来源：http://bjt.gzhubu.top

Py:   isinstance(u, User)
来源：http://one.316326.xyz

PHP:  $u instanceof User
来源：http://rye.ydzc1.top

JS:   u instanceof User
来源：http://uod.tanke756.top

TS:   u instanceof User
来源：http://upn.yj202588.top

Java: u instanceof User
来源：http://zdn.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://khm.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://gtq.xylfe.cn

C#:   u is User
来源：http://thm.feifeiyinyue.top

[G14] 数据类 / record
来源：http://kex.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uxw.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://zxu.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://xsi.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://imd.tanke756.top

Java: record User(String name, int age) {}
来源：http://rwm.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://and.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fij.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://zor.ehwqpu.com

[G15] 枚举
来源：http://uhl.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://apt.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ara.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ebk.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ceb.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://bie.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vqj.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://diq.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qyu.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://nur.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fhf.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://syl.uphjek.com

JS:   Object.entries(obj)
来源：http://yzm.zdqjudy.top

TS:   Object.entries(obj)
来源：http://nhm.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ogu.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xgu.redwolf501.top

Ruby: obj.instance_variables
来源：http://hks.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://wvu.tian-w.cn

================================================================================
来源：http://hvv.52xcode.cn

H. 异常与错误处理
来源：http://xel.zhengqikj.top

================================================================================
来源：http://ync.pengpengdd.cyou

[H01] try / catch 基础
来源：http://wef.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kaf.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qqo.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pnb.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lma.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mkc.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tmx.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ped.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://noa.yj202588.top

[H02] finally / ensure 收尾
来源：http://jgd.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://spk.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://hlf.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yzs.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cna.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://drs.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://lbj.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://eyi.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pno.zhoulong.xyz

[H03] 主动抛出异常
来源：http://qbc.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://uya.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xxx.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://oha.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://mpl.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://feb.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hpn.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nur.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tnt.fehbvm.com

[H04] 自定义异常类型
来源：http://swg.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://gmv.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aml.wangdashe.top

JS:   class MyError extends Error {}
来源：http://mkv.yfazqb.com

TS:   class MyError extends Error {}
来源：http://ydj.ctjpmb.com

Java: class MyException extends RuntimeException {}
来源：http://upt.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://obu.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://pcb.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://jtp.ppjwa.cn

[H05] 捕获特定类型
来源：http://pzi.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://qcj.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ipx.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://khk.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://crb.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://eix.hesvh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cmc.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://htq.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yzc.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://wcd.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://vtf.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://mmr.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://afn.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vmd.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mmc.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qoo.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://ofp.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://hjy.zdbjq.cn

[H07] 断言
来源：http://bot.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://xge.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://pqr.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://cqe.xuanzx.com

TS:   console.assert(x > 0);
来源：http://med.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://cdf.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wwx.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://yci.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://whf.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://wpr.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://hla.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wws.hywenlv.cn

JS:   e.message;  e.stack
来源：http://mun.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zos.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://gii.smart0.xyz

Go:   err.Error()
来源：http://xsq.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://bon.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://hsl.ydjk.org.cn

[H09] 带错误码的异常
来源：http://yxp.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://izl.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kpk.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bbj.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pjj.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mbd.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jpf.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://hjs.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://zoz.snrcjt.cn

[H10] 资源自动释放
来源：http://cgu.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mot.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://epd.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lmc.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xlc.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ksq.yangfankeji.com

Go:   defer f.Close()
来源：http://mwl.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gas.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://znp.zhijiandao.cn

================================================================================
来源：http://rjo.hammf.cn

I. 正则表达式
来源：http://taq.zhengqikj.top

================================================================================
来源：http://jib.wangdashe.top

[I01] 判断是否匹配
来源：http://epu.meibo888.top


<!-- 参考信息 -->