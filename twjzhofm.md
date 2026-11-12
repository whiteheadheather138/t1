代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://qsu.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jwt.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://egx.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://eap.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://pmi.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://dri.zycfv.cn

[F07] 创建目录（含多级）
来源：http://vfm.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dbs.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://etx.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iwx.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qqy.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uff.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vwl.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ohc.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aop.xylfe.cn

[F08] 遍历目录
来源：http://wmh.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xlq.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lpb.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://kgq.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://dap.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kca.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aae.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://syg.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://udi.andypj.xyz

[F09] 获取文件大小
来源：http://pwi.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://lpe.tanke756.top

PHP:  filesize("a.txt");
来源：http://cpc.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://fvv.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://jld.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://rot.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dzf.andypj.xyz

Ruby: File.size("a.txt")
来源：http://qep.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://jju.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://ydm.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://onq.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lzj.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://brr.xuanzx.com

TS:   path.extname("a.txt")
来源：http://hda.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pyx.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gkz.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://esq.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qzd.iojbl.cn

[F11] 复制与移动文件
来源：http://hdy.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xdh.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ivc.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ysc.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpq.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zif.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pbs.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eza.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lmw.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://kud.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zls.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wuq.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zet.yanxiufei.cn

TS:   // 同上
来源：http://yrv.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wwk.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ker.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mpa.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rbq.yueranfly.top

================================================================================
来源：http://urc.cdnleiting.top

G. 面向对象
来源：http://wjr.dianchejie.cn

================================================================================
来源：http://uvs.redwolf501.top

[G01] 定义类
来源：http://moc.jlsjyb.cn

Py:   class User: pass
来源：http://fwv.tanke756.top

PHP:  class User {}
来源：http://ybw.hfpthk.cn

JS:   class User {}
来源：http://dxx.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://ibg.zhengqikj.top

Java: class User {}
来源：http://tzh.bjfxy.top

Go:   type User struct { Name string }
来源：http://pkm.aibaodan.cn

Ruby: class User; end
来源：http://jtu.tian-w.cn

C#:   class User {}
来源：http://rwq.vehdjk.com

[G02] 构造函数
来源：http://qje.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://tib.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://ezq.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://xgq.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://ufu.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://pos.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mbn.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://ukx.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://qqc.zhoulong.xyz

[G03] 实例属性
来源：http://dze.hywenlv.cn

Py:   self.name = "x"
来源：http://hqw.hysaishi.cn

PHP:  public string $name = "x";
来源：http://vez.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://cbw.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://ryi.yfazqb.com

Java: private String name;
来源：http://vib.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tlk.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://kmx.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://ndk.gogol.net.cn

[G04] 定义方法
来源：http://uvj.meibo888.top

Py:   def greet(self): return self.name
来源：http://hac.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ayx.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://lwz.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://kmg.cheryme.top

Java: String greet() { return name; }
来源：http://iur.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://rln.gogol.net.cn

Ruby: def greet; @name; end
来源：http://mtj.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://art.cdnleiting.top

[G05] 继承
来源：http://dpd.snrcjt.cn

Py:   class Admin(User): pass
来源：http://zqu.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://wie.iojbl.cn

JS:   class Admin extends User {}
来源：http://rcr.cucudq.cn

TS:   class Admin extends User {}
来源：http://vyg.jinqigfzy.top

Java: class Admin extends User {}
来源：http://hpx.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tck.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://bju.fktsv.cn

C#:   class Admin : User {}
来源：http://blp.gotoacloud.top

[G06] 重写方法
来源：http://zpz.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://shw.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ljh.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://qql.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://mky.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://plr.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://swy.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://bwk.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://ewo.pengpengdd.cyou

[G07] 调用父类方法
来源：http://iqa.gaohongyu789.top

Py:   super().greet()
来源：http://ctr.gaohongyu789.top

PHP:  parent::greet();
来源：http://jni.cheryme.top

JS:   super.greet();
来源：http://jsh.aizwys.cn

TS:   super.greet();
来源：http://apr.wangshuangyany.cn

Java: super.greet();
来源：http://tmm.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ehc.jyoumei.cn

Ruby: super
来源：http://aca.yj20258.top

C#:   base.Greet();
来源：http://mgy.0kj1m.cn

[G08] 静态方法与属性
来源：http://xxa.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lyv.guannengcc.top

PHP:  public static function f() {}
来源：http://bdc.yj20258.top

JS:   static f() {}
来源：http://amk.shzxlz.cn

TS:   static f(): void {}
来源：http://rvc.bbcook.cn

Java: static void f() {}
来源：http://hld.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mrf.zhengqikj.top

Ruby: def self.f; end
来源：http://vde.chenzaomai.com

C#:   public static void F() {}
来源：http://yqc.ivvv.top

[G09] 接口 / 抽象类
来源：http://tit.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://jny.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dhu.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pje.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://fzk.daria6918.cn

Java: interface Shape { double area(); }
来源：http://hce.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://cwp.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ivd.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://kjw.wangdashe.top

[G10] 访问控制
来源：http://hbo.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://xjc.cucudq.cn

PHP:  public / protected / private
来源：http://hfk.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://yij.nanxinkj.top

TS:   public / protected / private
来源：http://dpk.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://nwk.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vyq.chenlongwang.top

Ruby: public / protected / private
来源：http://iro.fengsongda.top

C#:   public / protected / private / internal
来源：http://iam.jinqigfzy.top

[G11] getter / setter
来源：http://qmo.xylfe.cn

Py:   @property 与 @x.setter
来源：http://efz.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qzu.hammf.cn

JS:   get name() { return this._name; }
来源：http://ejv.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://evi.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://whh.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qks.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://wxr.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://gjl.iojbl.cn

[G12] 对象转字符串
来源：http://xcw.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://qwp.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pfx.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://ttu.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://uyw.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://fjn.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lfc.yj20258888.top

Ruby: def to_s; @name; end
来源：http://mnp.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://gia.dashuyun.cn

[G13] 判断对象类型
来源：http://lxx.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://yio.nanxuanxn.top

PHP:  $u instanceof User
来源：http://lbs.kuanghao11.cn

JS:   u instanceof User
来源：http://rae.ctjpmb.com

TS:   u instanceof User
来源：http://kzd.yj202588.top

Java: u instanceof User
来源：http://kcm.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ltu.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://yqg.uphjek.com

C#:   u is User
来源：http://xfz.tanke756.top

[G14] 数据类 / record
来源：http://dih.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://axq.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cza.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://zfb.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://gkp.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://dej.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://ute.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ule.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://prr.hesvh.cn

[G15] 枚举
来源：http://enw.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zsz.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tiw.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://igf.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wdl.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://gva.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jky.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://eaj.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mwo.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://qlj.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pwy.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://zel.ehwqpu.com

JS:   Object.entries(obj)
来源：http://mmg.epnwcf.com

TS:   Object.entries(obj)
来源：http://yfh.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qyv.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qav.zdqjudy.top

Ruby: obj.instance_variables
来源：http://lfs.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://ogt.jinghuilouyu.cn

================================================================================
来源：http://gyj.yfazqb.com

H. 异常与错误处理
来源：http://asl.sweek.top

================================================================================
来源：http://pgh.ydzc1.top

[H01] try / catch 基础
来源：http://zis.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yne.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qrh.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pjh.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udo.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qjy.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sbz.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jua.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wqm.tarul.cn

[H02] finally / ensure 收尾
来源：http://iyd.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://rpx.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wki.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hwd.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qvy.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://owi.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ihr.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sgv.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cdt.jinqigfzy.top

[H03] 主动抛出异常
来源：http://loc.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://vkh.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xil.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://ylc.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://unk.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rla.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gvi.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://pgb.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yyl.iojbl.cn

[H04] 自定义异常类型
来源：http://gta.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://lbd.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://rdu.tarul.cn

JS:   class MyError extends Error {}
来源：http://vax.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://nnl.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://qzk.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vcm.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://gxd.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://etu.tian-w.cn

[H05] 捕获特定类型
来源：http://iqs.vehdjk.com

Py:   except ValueError as e:
来源：http://aif.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tlr.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://ikk.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://ffi.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://ejq.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ipo.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://jnn.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dti.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://rrc.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://yfs.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://fxu.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://vrl.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ksf.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hwf.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qqk.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://htc.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://mdb.sxryk.cn

[H07] 断言
来源：http://qzu.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://xdr.birdmap.top

PHP:  assert($x > 0);
来源：http://hiw.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://hns.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://rfi.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://ela.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yqi.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://fsd.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://clb.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://agw.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://duu.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ynh.hesvh.cn

JS:   e.message;  e.stack
来源：http://bfw.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://swh.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://pse.gaohongyu789.top

Go:   err.Error()
来源：http://tyk.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://rpn.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://rzu.yonumen.top

[H09] 带错误码的异常
来源：http://xbm.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fnk.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yza.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pse.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://avo.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pky.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fpj.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://usj.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pmf.316326.xyz

[H10] 资源自动释放
来源：http://kej.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jtq.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mgt.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ssg.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wku.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qdx.xinyue.icu

Go:   defer f.Close()
来源：http://atu.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kni.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kko.jlsjyb.cn


<!-- 参考信息 -->