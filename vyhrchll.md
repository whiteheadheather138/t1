代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ofl.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://cjt.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sgm.chenlongwang.top

[F04] 追加写入文件
来源：http://hta.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lfq.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vrj.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jkp.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ljj.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mjr.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qgu.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jpn.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wlb.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://kvd.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pme.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://nrw.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://mge.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://ujk.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hxx.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hka.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://kfh.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://ozv.zhiwuduotai.top

[F06] 删除文件
来源：http://ndf.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://sho.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://ymv.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cpm.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://xex.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://toa.daxiang520.top

Go:   os.Remove("a.txt")
来源：http://izn.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://jxg.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://cxr.yonumen.top

[F07] 创建目录（含多级）
来源：http://mnd.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qfj.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://loc.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tvb.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vsd.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://otx.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://chd.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ast.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kdu.mhx1999.top

[F08] 遍历目录
来源：http://toq.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nvi.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rvo.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://swe.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://gew.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://csg.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tpc.zdqjudy.top

Ruby: Dir.children("dir")
来源：http://vlo.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://wxo.zhongyouzk.top

[F09] 获取文件大小
来源：http://ypy.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://jdf.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://bzc.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://ekc.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://vep.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://vds.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jgm.bjfxy.top

Ruby: File.size("a.txt")
来源：http://vqp.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://yuf.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://iip.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://edm.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ofk.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dqj.cashguo.top

TS:   path.extname("a.txt")
来源：http://zyb.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iit.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wvr.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://apz.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://owz.316326.xyz

[F11] 复制与移动文件
来源：http://mmy.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bou.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ydc.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://loz.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rrb.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pxq.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://thm.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wsf.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bll.hysaishi.cn

[F12] CSV 读写
来源：http://xtr.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gsy.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://drw.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uck.cucudq.cn

TS:   // 同上
来源：http://fcp.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lix.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://che.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vsc.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iht.pycfn.com

================================================================================
来源：http://wvf.cucudq.cn

G. 面向对象
来源：http://znt.ywan-chungtsiang.top

================================================================================
来源：http://wnx.bjfxy.top

[G01] 定义类
来源：http://ilm.guowangkeji.top

Py:   class User: pass
来源：http://rdn.jinyuanbaomall.cn

PHP:  class User {}
来源：http://jxg.nanxinkj.top

JS:   class User {}
来源：http://hiz.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://ard.jinqigfzy.top

Java: class User {}
来源：http://fms.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://kto.hywenlv.cn

Ruby: class User; end
来源：http://rbr.c1oappe.top

C#:   class User {}
来源：http://vvc.bbcook.cn

[G02] 构造函数
来源：http://vam.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://gus.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://egc.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://bvl.yj202588.top

TS:   constructor(public name: string) {}
来源：http://fer.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://zgl.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jwf.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://yqp.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://bpv.yuanzhike.top

[G03] 实例属性
来源：http://lkr.ydzc1.top

Py:   self.name = "x"
来源：http://khy.jiagoushi.top

PHP:  public string $name = "x";
来源：http://zhi.ivvv.top

JS:   this.name = "x";
来源：http://kaz.hywenlv.cn

TS:   name: string = "x";
来源：http://lpk.jinghuilouyu.cn

Java: private String name;
来源：http://gjx.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lek.vqdsnc.cn

Ruby: @name = "x"
来源：http://zvn.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://rkr.jqgufenzy.top

[G04] 定义方法
来源：http://aur.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://obm.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ubb.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://aoc.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://fwo.guannengcc.top

Java: String greet() { return name; }
来源：http://wfc.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://equ.yongpay.top

Ruby: def greet; @name; end
来源：http://pwk.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://dgb.chenlongwang.top

[G05] 继承
来源：http://vwa.tian-w.cn

Py:   class Admin(User): pass
来源：http://zny.tian-w.cn

PHP:  class Admin extends User {}
来源：http://ckf.nanxinkj.top

JS:   class Admin extends User {}
来源：http://wog.ivvv.top

TS:   class Admin extends User {}
来源：http://sub.aizwys.cn

Java: class Admin extends User {}
来源：http://ohl.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xfb.yfazqb.com

Ruby: class Admin < User; end
来源：http://cwo.cucudq.cn

C#:   class Admin : User {}
来源：http://xbj.hongshengwenyu.top

[G06] 重写方法
来源：http://gzl.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://bjg.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://len.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://krc.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://let.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://zhm.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bmp.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://idr.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://sdf.yongpay.top

[G07] 调用父类方法
来源：http://kie.xylfe.cn

Py:   super().greet()
来源：http://bet.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://bvj.xylfe.cn

JS:   super.greet();
来源：http://hwh.vqdsnc.cn

TS:   super.greet();
来源：http://yeh.jinghuilouyu.cn

Java: super.greet();
来源：http://lth.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gmi.yj202588.top

Ruby: super
来源：http://qxo.jlsjyb.cn

C#:   base.Greet();
来源：http://hpa.gogol.net.cn

[G08] 静态方法与属性
来源：http://nid.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://urb.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://mzy.hysaishi.cn

JS:   static f() {}
来源：http://nfj.wangdashe.top

TS:   static f(): void {}
来源：http://nns.jiagoushi.top

Java: static void f() {}
来源：http://pvv.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nye.jinqigufen.top

Ruby: def self.f; end
来源：http://yvv.yonumen.top

C#:   public static void F() {}
来源：http://alr.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://otk.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://xbx.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://afb.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pvw.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://xkb.zycfv.cn

Java: interface Shape { double area(); }
来源：http://oac.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://ext.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bnj.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://uky.wangdashe.top

[G10] 访问控制
来源：http://hcj.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://hdb.guowangkeji.top

PHP:  public / protected / private
来源：http://rtq.epnwcf.com

JS:   #private 字段；其余公开
来源：http://rbw.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://yjn.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://dfm.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lrk.wangshuangyany.cn

Ruby: public / protected / private
来源：http://cad.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://bqp.shanyushiyangtech.top

[G11] getter / setter
来源：http://mpx.nwbrower.top

Py:   @property 与 @x.setter
来源：http://ola.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kzt.xziqi.cn

JS:   get name() { return this._name; }
来源：http://dxl.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://izm.epnwcf.com

Java: public String getName() { return name; }
来源：http://gpl.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ggy.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://qxy.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://ntj.yueranfly.top

[G12] 对象转字符串
来源：http://pvw.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://bzv.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jzn.xylfe.cn

JS:   toString() { return this.name; }
来源：http://stl.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://dam.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://bvx.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gfw.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://nnz.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://jhj.hysaishi.cn

[G13] 判断对象类型
来源：http://gzd.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://zws.bjfxy.top

PHP:  $u instanceof User
来源：http://mkh.yj20258.top

JS:   u instanceof User
来源：http://klr.fzhhl.top

TS:   u instanceof User
来源：http://hze.zdqjudy.top

Java: u instanceof User
来源：http://ato.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xuo.cucudq.cn

Ruby: u.is_a?(User)
来源：http://zjv.yj20258888.top

C#:   u is User
来源：http://slc.aibaodan.cn

[G14] 数据类 / record
来源：http://vyf.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zyk.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://fek.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://clv.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://enw.havefunace.top

Java: record User(String name, int age) {}
来源：http://zbv.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://fbq.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ott.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://vto.smart0.xyz

[G15] 枚举
来源：http://nfl.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ccw.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://okg.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nwy.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wrm.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://quv.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tkb.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://ahg.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tvp.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://lmd.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yzk.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://hds.fehbvm.com

JS:   Object.entries(obj)
来源：http://sqc.aibaodan.cn

TS:   Object.entries(obj)
来源：http://tqa.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lvf.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dvo.yonumen.top

Ruby: obj.instance_variables
来源：http://eru.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://gnw.yuxming.cn

================================================================================
来源：http://syj.yangfankeji.com

H. 异常与错误处理
来源：http://suq.ybcxt.top

================================================================================
来源：http://nik.ppjwa.cn

[H01] try / catch 基础
来源：http://edy.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ecu.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://diq.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pav.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lmz.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xmm.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hbs.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pwe.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lek.uphjek.com

[H02] finally / ensure 收尾
来源：http://fet.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://isg.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sdo.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://pfd.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://kjs.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://hbp.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xkw.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ket.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gzr.gogol.net.cn

[H03] 主动抛出异常
来源：http://jik.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://qdo.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://noe.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://pnk.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://lwg.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ybj.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zam.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xde.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://ube.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://rcd.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://xvi.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://jag.hesvh.cn

JS:   class MyError extends Error {}
来源：http://mhb.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://adh.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://exw.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://peu.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://awb.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://ljb.9152youxi.cn

[H05] 捕获特定类型
来源：http://zmw.daxiang520.top

Py:   except ValueError as e:
来源：http://llc.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ssu.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://cdp.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://cpr.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://fgd.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wxq.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://swv.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hls.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://ops.uphjek.com

Py:   value = d.get("k") or default
来源：http://rcj.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://ajg.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mfg.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://xut.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dkh.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://tdv.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://zdv.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://reg.wangshuangyany.cn

[H07] 断言
来源：http://dgu.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://qrr.yueranfly.top

PHP:  assert($x > 0);
来源：http://tgs.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://llb.mhx1999.top

TS:   console.assert(x > 0);
来源：http://wos.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://kvk.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cub.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://ewk.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://pdb.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://rdn.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://pfq.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xhl.zdqjudy.top


<!-- 参考信息 -->