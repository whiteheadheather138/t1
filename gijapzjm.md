代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://pqz.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vlz.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ogp.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://upb.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://xdd.fanxiaobao.xyz

[F06] 删除文件
来源：http://iiq.daria6918.cn

Py:   os.remove("a.txt")
来源：http://njb.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://ncy.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://beu.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wbl.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dub.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://ucv.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://dmf.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://ysf.ivvv.top

[F07] 创建目录（含多级）
来源：http://boy.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jmp.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bdp.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lpe.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gkj.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sme.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qol.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xsf.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ube.0kj1m.cn

[F08] 遍历目录
来源：http://pqm.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bam.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jnq.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://rfg.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://uvw.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ygu.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jju.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://bcy.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://clw.pycfn.com

[F09] 获取文件大小
来源：http://xst.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://vtx.tian-w.cn

PHP:  filesize("a.txt");
来源：http://jqw.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://grg.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://fba.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://sgw.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sws.xuanzx.com

Ruby: File.size("a.txt")
来源：http://lan.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://cnf.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://buk.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://osd.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rwm.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xcg.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://utv.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lbs.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eqp.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iky.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jkf.yangfankeji.com

[F11] 复制与移动文件
来源：http://avh.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://spt.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ivn.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aky.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://beg.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fct.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ngg.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kwk.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xpd.xylfe.cn

[F12] CSV 读写
来源：http://suk.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ipz.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gbr.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oyz.smart0.xyz

TS:   // 同上
来源：http://nto.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ior.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qga.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fvs.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ope.ybcxt.top

================================================================================
来源：http://mhd.mhx1999.top

G. 面向对象
来源：http://qrt.zdqjudy.top

================================================================================
来源：http://jsp.wangdashe.top

[G01] 定义类
来源：http://awx.yj202588.top

Py:   class User: pass
来源：http://tse.aibaodan.cn

PHP:  class User {}
来源：http://bno.sufxvd.cn

JS:   class User {}
来源：http://nug.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://yre.feifeiyinyue.top

Java: class User {}
来源：http://ufd.sufxvd.cn

Go:   type User struct { Name string }
来源：http://osm.gotoacloud.top

Ruby: class User; end
来源：http://oym.aizwys.cn

C#:   class User {}
来源：http://tgd.shzxlz.cn

[G02] 构造函数
来源：http://pzs.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://cgh.nwbrower.top

PHP:  public function __construct(public string $name) {}
来源：http://wot.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://cis.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://rrm.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://wuv.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vkc.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://scf.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://ieb.yuxming.cn

[G03] 实例属性
来源：http://dhe.jinqigfzy.top

Py:   self.name = "x"
来源：http://ahb.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://jla.ydjk.org.cn

JS:   this.name = "x";
来源：http://bbj.andypj.xyz

TS:   name: string = "x";
来源：http://qhg.jyoumei.cn

Java: private String name;
来源：http://cbe.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wxb.andypj.xyz

Ruby: @name = "x"
来源：http://uqw.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://key.zhongyouzk.top

[G04] 定义方法
来源：http://iic.xylfe.cn

Py:   def greet(self): return self.name
来源：http://xfe.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://emt.gzhubu.top

JS:   greet() { return this.name; }
来源：http://gdc.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://tgb.yvedp.cn

Java: String greet() { return name; }
来源：http://fvg.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pqy.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://esc.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://ezk.cqqwz.cn

[G05] 继承
来源：http://mfd.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://nxg.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://pzm.yuxming.cn

JS:   class Admin extends User {}
来源：http://vtr.ybcxt.top

TS:   class Admin extends User {}
来源：http://sxp.hysaishi.cn

Java: class Admin extends User {}
来源：http://xwb.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dpu.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://jge.kuanghao11.cn

C#:   class Admin : User {}
来源：http://mzu.fktsv.cn

[G06] 重写方法
来源：http://hqc.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://beo.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tnc.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://kvv.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://ryj.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://wpp.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jdk.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://ckd.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://hvf.hywenlv.cn

[G07] 调用父类方法
来源：http://ftq.jinqigufen.top

Py:   super().greet()
来源：http://sxb.uphjek.com

PHP:  parent::greet();
来源：http://rsd.jinghuilouyu.cn

JS:   super.greet();
来源：http://xbp.cashguo.top

TS:   super.greet();
来源：http://ols.yanxiufei.cn

Java: super.greet();
来源：http://nxy.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jzv.chenlongwang.top

Ruby: super
来源：http://zin.smart0.xyz

C#:   base.Greet();
来源：http://fwo.yj20258.top

[G08] 静态方法与属性
来源：http://zgi.xinyue.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://und.redwolf501.top

PHP:  public static function f() {}
来源：http://bkv.zhoulong.xyz

JS:   static f() {}
来源：http://wfk.dianchejie.cn

TS:   static f(): void {}
来源：http://rzy.cdnleiting.top

Java: static void f() {}
来源：http://yzr.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tcv.cheryme.top

Ruby: def self.f; end
来源：http://sbt.aizwys.cn

C#:   public static void F() {}
来源：http://emf.uphjek.com

[G09] 接口 / 抽象类
来源：http://usl.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://uec.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://vya.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://eko.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://wrs.fengsongda.top

Java: interface Shape { double area(); }
来源：http://ppo.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://ick.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tna.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://kht.zdqjudy.top

[G10] 访问控制
来源：http://qpb.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://hoj.shzxlz.cn

PHP:  public / protected / private
来源：http://kak.shuidangran.top

JS:   #private 字段；其余公开
来源：http://rxn.shuidangran.top

TS:   public / protected / private
来源：http://wex.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://wbz.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qxw.wangdashe.top

Ruby: public / protected / private
来源：http://xou.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://otq.cashguo.top

[G11] getter / setter
来源：http://mal.nwbrower.top

Py:   @property 与 @x.setter
来源：http://dtv.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vns.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://yaq.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://mtx.tanke756.top

Java: public String getName() { return name; }
来源：http://rwo.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://wvd.hysaishi.cn

Ruby: attr_accessor :name
来源：http://ikj.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://ego.xuanzx.com

[G12] 对象转字符串
来源：http://zpk.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://huh.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wzh.fktsv.cn

JS:   toString() { return this.name; }
来源：http://tol.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://bht.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://rou.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://xzf.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://kyt.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://adz.havefunace.top

[G13] 判断对象类型
来源：http://xmr.bbcook.cn

Py:   isinstance(u, User)
来源：http://lks.shzxlz.cn

PHP:  $u instanceof User
来源：http://lou.pycfn.com

JS:   u instanceof User
来源：http://esx.cdnleiting.top

TS:   u instanceof User
来源：http://ygj.sysykeji.top

Java: u instanceof User
来源：http://ctg.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vut.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://bvv.ehwqpu.com

C#:   u is User
来源：http://fvf.snrcjt.cn

[G14] 数据类 / record
来源：http://sbu.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vdn.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://ork.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://nup.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://cdp.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://lms.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://dcf.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zjc.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://qdb.316326.xyz

[G15] 枚举
来源：http://uex.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tbu.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fut.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yqw.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kof.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://klo.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://riu.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://gbi.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://svj.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://lua.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://egi.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://ssr.hnqzz.top

JS:   Object.entries(obj)
来源：http://cgs.wangdashe.top

TS:   Object.entries(obj)
来源：http://tgm.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fhh.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://vlz.xziqi.cn

Ruby: obj.instance_variables
来源：http://vmx.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://ndd.jinqigfzy.top

================================================================================
来源：http://ipy.shangyingyoupin.top

H. 异常与错误处理
来源：http://yiy.jinghuilouyu.cn

================================================================================
来源：http://uxr.xziqi.cn

[H01] try / catch 基础
来源：http://vtx.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jbv.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iuh.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nqt.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://glg.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bsj.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zqp.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gtc.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oke.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://tdr.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://tig.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mts.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://mma.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ozj.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://zwb.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pza.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vqv.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ntw.yanxiufei.cn

[H03] 主动抛出异常
来源：http://xep.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://ghs.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ava.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://noy.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://rkj.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ovl.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hof.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iwu.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://slf.xylfe.cn

[H04] 自定义异常类型
来源：http://eam.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://bbx.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://eui.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://bvy.tanke756.top

TS:   class MyError extends Error {}
来源：http://url.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://ktb.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xgr.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://ouj.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://kwe.daxiang520.top

[H05] 捕获特定类型
来源：http://euq.gaohongyu789.top

Py:   except ValueError as e:
来源：http://mxl.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lvp.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://zzr.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://aik.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://ywm.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pcx.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://yqz.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://keq.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://lqj.sysykeji.top

Py:   value = d.get("k") or default
来源：http://jwt.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://msz.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://oni.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://tcf.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eqo.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tzw.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://uwi.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://qha.nanxinkj.top

[H07] 断言
来源：http://lsx.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://ifd.hywenlv.cn

PHP:  assert($x > 0);
来源：http://ahh.fzhhl.top

JS:   console.assert(x > 0);
来源：http://yaj.hammf.cn

TS:   console.assert(x > 0);
来源：http://cfs.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://kzm.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://huj.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://czk.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://oow.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://rcp.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://dwf.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sen.fzhhl.top

JS:   e.message;  e.stack
来源：http://qix.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gdx.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ddi.cdnleiting.top

Go:   err.Error()
来源：http://xhg.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://lxn.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://ujq.sjlbkw.cn

[H09] 带错误码的异常
来源：http://wgs.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vcp.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://skj.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rxb.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hwg.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wtf.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ykg.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://ciu.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dlj.yueranfly.top

[H10] 资源自动释放
来源：http://nag.jinghuilouyu.cn


<!-- 参考信息 -->