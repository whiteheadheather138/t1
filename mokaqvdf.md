代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hun.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zbx.uphjek.com

PHP:  file_exists("a.txt");
来源：http://qne.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://nnl.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://xfk.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kxl.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ctu.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://mub.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://wxq.yuxming.cn

[F06] 删除文件
来源：http://ysf.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://swu.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://bdg.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://cag.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://uqq.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uec.tarul.cn

Go:   os.Remove("a.txt")
来源：http://zjp.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://yta.sweek.top

C#:   File.Delete("a.txt");
来源：http://zze.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://zrx.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kwy.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nlg.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfh.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qzk.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://skb.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kpd.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fni.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ogc.fengsongda.top

[F08] 遍历目录
来源：http://ury.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vtw.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tkp.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://ffm.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://kwp.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dcu.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vol.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://czs.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://qey.mhx1999.top

[F09] 获取文件大小
来源：http://uxf.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://fhu.xinyue.icu

PHP:  filesize("a.txt");
来源：http://bph.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://aqi.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://gfq.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jcz.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ztk.hammf.cn

Ruby: File.size("a.txt")
来源：http://isk.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://rtl.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://eci.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dxw.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gqu.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mbs.xylfe.cn

TS:   path.extname("a.txt")
来源：http://yas.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ycq.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zpc.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xfs.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nsl.yfazqb.com

[F11] 复制与移动文件
来源：http://rcf.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://utf.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sjf.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ewq.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lra.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kls.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tcn.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://okd.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybi.zdbjq.cn

[F12] CSV 读写
来源：http://gts.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gcb.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://let.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vpp.ppjwa.cn

TS:   // 同上
来源：http://rrg.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cqw.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bbk.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gxl.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qcy.svipenyu.cn

================================================================================
来源：http://zaj.xuetiantiany.cn

G. 面向对象
来源：http://dtz.yonumen.top

================================================================================
来源：http://pcx.quarkkingdee.top

[G01] 定义类
来源：http://ihk.dianchejie.cn

Py:   class User: pass
来源：http://vby.yonumen.top

PHP:  class User {}
来源：http://bva.xingfuxueyuan.xyz

JS:   class User {}
来源：http://ujk.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://fbh.cucudq.cn

Java: class User {}
来源：http://lkb.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://edk.chenjidiqi.icu

Ruby: class User; end
来源：http://ixy.sufxvd.cn

C#:   class User {}
来源：http://txz.316326.xyz

[G02] 构造函数
来源：http://czu.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://kkv.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://ajt.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://bbs.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://rcs.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://hfp.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wyw.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://zkb.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://bmm.ybcxt.top

[G03] 实例属性
来源：http://oeo.jqgfzy.top

Py:   self.name = "x"
来源：http://ulz.ydzc1.top

PHP:  public string $name = "x";
来源：http://iah.cucudq.cn

JS:   this.name = "x";
来源：http://rzp.nanxinkj.top

TS:   name: string = "x";
来源：http://xth.jlsjyb.cn

Java: private String name;
来源：http://fgq.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rtt.yanxiufei.cn

Ruby: @name = "x"
来源：http://ugc.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://mfp.epnwcf.com

[G04] 定义方法
来源：http://pvs.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://zit.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fvl.yuxming.cn

JS:   greet() { return this.name; }
来源：http://kqj.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://xry.bjfxy.top

Java: String greet() { return name; }
来源：http://sfv.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qve.smart0.xyz

Ruby: def greet; @name; end
来源：http://wwd.316326.xyz

C#:   public string Greet() => Name;
来源：http://ykg.uphjek.com

[G05] 继承
来源：http://sfd.sxryk.cn

Py:   class Admin(User): pass
来源：http://yey.ivvv.top

PHP:  class Admin extends User {}
来源：http://qmm.svipenyu.cn

JS:   class Admin extends User {}
来源：http://ekr.fehbvm.com

TS:   class Admin extends User {}
来源：http://kju.ydzc1.top

Java: class Admin extends User {}
来源：http://ixv.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rln.andypj.xyz

Ruby: class Admin < User; end
来源：http://rhb.hnqzz.top

C#:   class Admin : User {}
来源：http://psn.zhengqikj.top

[G06] 重写方法
来源：http://yrj.yj20258.top

Py:   def greet(self): return "admin"
来源：http://zda.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dtl.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://nvf.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://ugg.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://vri.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xje.gzhubu.top

Ruby: def greet; "admin"; end
来源：http://kqs.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://ocl.haohaochexian.top

[G07] 调用父类方法
来源：http://gdx.birdmap.top

Py:   super().greet()
来源：http://nii.uphjek.com

PHP:  parent::greet();
来源：http://blt.sysykeji.top

JS:   super.greet();
来源：http://wuu.chenjidiqi.icu

TS:   super.greet();
来源：http://kos.kuanghao11.cn

Java: super.greet();
来源：http://peo.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://onj.uphjek.com

Ruby: super
来源：http://xhp.hesvh.cn

C#:   base.Greet();
来源：http://gvg.sweek.top

[G08] 静态方法与属性
来源：http://pbc.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zaf.jqgufenzy.top

PHP:  public static function f() {}
来源：http://kid.pengpengdd.cyou

JS:   static f() {}
来源：http://zpx.daria6918.cn

TS:   static f(): void {}
来源：http://xwk.yfazqb.com

Java: static void f() {}
来源：http://ftq.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://tyo.jinqigfzy.top

Ruby: def self.f; end
来源：http://edk.gotoacloud.top

C#:   public static void F() {}
来源：http://xox.havefunace.top

[G09] 接口 / 抽象类
来源：http://ucd.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://deu.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://twl.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kkb.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://ncv.wangdashe.top

Java: interface Shape { double area(); }
来源：http://pwb.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://cly.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vac.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://dym.meibo888.top

[G10] 访问控制
来源：http://vxt.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://qtw.jyoumei.cn

PHP:  public / protected / private
来源：http://puo.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://xoi.pycfn.com

TS:   public / protected / private
来源：http://vxy.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://oaw.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gfz.aibaodan.cn

Ruby: public / protected / private
来源：http://uxi.sxryk.cn

C#:   public / protected / private / internal
来源：http://gko.shanyushiyangkeji.top

[G11] getter / setter
来源：http://jeb.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://zej.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jgj.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://dfh.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://lxs.pycfn.com

Java: public String getName() { return name; }
来源：http://slq.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://upp.yangfankeji.com

Ruby: attr_accessor :name
来源：http://unj.zycfv.cn

C#:   public string Name { get; set; }
来源：http://brw.sysykeji.top

[G12] 对象转字符串
来源：http://pzv.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://ynm.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zvv.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://etm.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://pos.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://swl.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xlz.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://lit.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://yby.shuidangran.top

[G13] 判断对象类型
来源：http://ikj.yueranfly.top

Py:   isinstance(u, User)
来源：http://ezs.gzhubu.top

PHP:  $u instanceof User
来源：http://ivb.pengpengdd.cyou

JS:   u instanceof User
来源：http://yoe.yj20258.top

TS:   u instanceof User
来源：http://ndq.yongpay.top

Java: u instanceof User
来源：http://bzk.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hyj.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://kak.yanxiufei.cn

C#:   u is User
来源：http://zzb.hesvh.cn

[G14] 数据类 / record
来源：http://ucv.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pdh.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://wqj.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://sqs.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://dzx.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://nuv.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://chr.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zch.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://smf.hnxiangtu.top

[G15] 枚举
来源：http://ucc.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ack.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fol.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tyi.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rgm.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://pwu.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mgd.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://bsz.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tlo.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://irr.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://btm.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://lmj.redwolf501.top

JS:   Object.entries(obj)
来源：http://qsg.fzhhl.top

TS:   Object.entries(obj)
来源：http://wcx.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ttx.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tlh.hammf.cn

Ruby: obj.instance_variables
来源：http://ffm.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://gsr.jinqigfzy.top

================================================================================
来源：http://rht.aizwys.cn

H. 异常与错误处理
来源：http://vqa.vehdjk.com

================================================================================
来源：http://ycm.meibo888.top

[H01] try / catch 基础
来源：http://oae.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lso.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uam.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cyy.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lsa.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iji.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oaw.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vqx.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jah.fktsv.cn

[H02] finally / ensure 收尾
来源：http://fmq.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://csd.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iny.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://pko.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vgi.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://hek.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://psf.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jmt.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://arf.iojbl.cn

[H03] 主动抛出异常
来源：http://ezv.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://kcm.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dyr.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://pbg.yonumen.top

TS:   throw new Error("错误信息");
来源：http://ixr.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://awu.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hbq.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ytc.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://lvs.xinyue.icu

[H04] 自定义异常类型
来源：http://yaf.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://jae.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://uyl.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://fhs.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://dez.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://xqs.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jqe.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://uzu.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://krg.cdnleiting.top

[H05] 捕获特定类型
来源：http://bjn.ivvv.top

Py:   except ValueError as e:
来源：http://per.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pdb.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://hgz.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://dya.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://sgm.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://slh.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://ymw.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tdl.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://vqu.52xcode.cn

Py:   value = d.get("k") or default
来源：http://vvz.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dwz.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://hrc.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://qdc.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wdd.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://njt.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://isu.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://jva.haohaochexian.top

[H07] 断言
来源：http://zky.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://ala.sufxvd.cn

PHP:  assert($x > 0);
来源：http://und.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://tdi.fzhhl.top

TS:   console.assert(x > 0);
来源：http://zyc.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://qol.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aad.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ztt.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://nta.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://lfq.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://sos.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kmk.gzhubu.top

JS:   e.message;  e.stack
来源：http://kbs.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hoh.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://whf.shangyingyoupin.top

Go:   err.Error()
来源：http://saz.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://pyd.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://cyz.nanxinkj.top

[H09] 带错误码的异常
来源：http://lrb.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ftm.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kab.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fym.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://adt.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nsy.vehdjk.com


<!-- 参考信息 -->