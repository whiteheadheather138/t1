代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mfa.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ytk.cashguo.top

[F03] 写入文件（覆盖）
来源：http://ugw.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://znh.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bdi.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xdw.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aan.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vrk.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wfu.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://ejj.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mcy.aizwys.cn

[F04] 追加写入文件
来源：http://zxe.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xwa.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bnl.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swz.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyk.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bdb.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uzy.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ejf.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cej.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://xro.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zge.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://mpp.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://ejd.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://qos.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sfl.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wrt.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://rbo.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://iqw.quarkkingdee.top

[F06] 删除文件
来源：http://izy.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://spl.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://gyf.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dvm.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://tyv.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qmd.yj202588.top

Go:   os.Remove("a.txt")
来源：http://uai.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://eao.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://xpf.bbcook.cn

[F07] 创建目录（含多级）
来源：http://zak.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jys.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eui.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ddn.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ilw.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dru.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://huo.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bic.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dcf.daxiang520.top

[F08] 遍历目录
来源：http://uyb.9152youxi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://giw.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://prp.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://ost.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://zbr.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qad.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zos.ydzc1.top

Ruby: Dir.children("dir")
来源：http://hzn.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://qxv.tarul.cn

[F09] 获取文件大小
来源：http://nre.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://jsx.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://mhn.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://nce.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://mef.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://hwr.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qlq.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://gwj.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://upg.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://jto.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qyy.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cug.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dpj.yj202588.top

TS:   path.extname("a.txt")
来源：http://pgo.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ttm.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pfi.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bod.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jkk.ydzc1.top

[F11] 复制与移动文件
来源：http://wsd.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://emv.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vzx.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fkl.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yyx.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eix.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xiz.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://siv.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lsk.cashguo.top

[F12] CSV 读写
来源：http://kec.fzhhl.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kdv.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oyg.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rbf.pengpengdd.cyou

TS:   // 同上
来源：http://ths.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nab.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tcw.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kew.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://saf.vqdsnc.cn

================================================================================
来源：http://dmx.xingfuxueyuan.xyz

G. 面向对象
来源：http://syu.xingfuxueyuan.xyz

================================================================================
来源：http://imm.smart0.xyz

[G01] 定义类
来源：http://knq.yj202588.top

Py:   class User: pass
来源：http://thp.9152youxi.cn

PHP:  class User {}
来源：http://fmg.yuxming.cn

JS:   class User {}
来源：http://jrl.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://djd.tian-w.cn

Java: class User {}
来源：http://nya.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://lim.zycfv.cn

Ruby: class User; end
来源：http://qyc.feifeiyinyue.top

C#:   class User {}
来源：http://iwb.xinyue.icu

[G02] 构造函数
来源：http://rsc.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://xgx.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://gdo.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://twh.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://xhu.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://pgg.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aml.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://dtt.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://zjf.c1oappe.top

[G03] 实例属性
来源：http://hgy.zhengqikj.top

Py:   self.name = "x"
来源：http://aml.zdbjq.cn

PHP:  public string $name = "x";
来源：http://kcv.zdbjq.cn

JS:   this.name = "x";
来源：http://lbv.316326.xyz

TS:   name: string = "x";
来源：http://dda.xylfe.cn

Java: private String name;
来源：http://ydq.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qux.jlsjyb.cn

Ruby: @name = "x"
来源：http://wrz.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://pea.zhijiandao.cn

[G04] 定义方法
来源：http://cnu.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://ali.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://diz.hammf.cn

JS:   greet() { return this.name; }
来源：http://wtd.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://dnr.xinyue.icu

Java: String greet() { return name; }
来源：http://coj.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yzp.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://eky.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://dnf.hesvh.cn

[G05] 继承
来源：http://bsq.zycfv.cn

Py:   class Admin(User): pass
来源：http://rpv.hcnkem.com

PHP:  class Admin extends User {}
来源：http://glb.cheryme.top

JS:   class Admin extends User {}
来源：http://vzi.ivvv.top

TS:   class Admin extends User {}
来源：http://yfj.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://ano.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qgd.shuidangran.top

Ruby: class Admin < User; end
来源：http://tlp.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://wfh.shzxlz.cn

[G06] 重写方法
来源：http://rgs.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://fzu.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://seo.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://vln.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://bie.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://zwj.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ger.yj20258.top

Ruby: def greet; "admin"; end
来源：http://njg.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://dyy.fengsongda.top

[G07] 调用父类方法
来源：http://bfz.shanyushiyangkeji.top

Py:   super().greet()
来源：http://idz.c1oappe.top

PHP:  parent::greet();
来源：http://fob.cqqwz.cn

JS:   super.greet();
来源：http://mmo.nanxinkj.top

TS:   super.greet();
来源：http://ufl.meibo888.top

Java: super.greet();
来源：http://yua.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hyu.ydjk.org.cn

Ruby: super
来源：http://neo.wangdashe.top

C#:   base.Greet();
来源：http://kug.cdnleiting.top

[G08] 静态方法与属性
来源：http://lnz.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rie.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://smp.xuanzx.com

JS:   static f() {}
来源：http://xoy.aizwys.cn

TS:   static f(): void {}
来源：http://bqg.redwolf501.top

Java: static void f() {}
来源：http://njy.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://lfp.hywenlv.cn

Ruby: def self.f; end
来源：http://vgz.iojbl.cn

C#:   public static void F() {}
来源：http://lrn.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://oan.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://frj.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xww.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://nfr.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://vzv.gzhubu.top

Java: interface Shape { double area(); }
来源：http://fyc.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://jxq.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lxr.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://uko.gogol.net.cn

[G10] 访问控制
来源：http://cvw.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://dvx.jlsjyb.cn

PHP:  public / protected / private
来源：http://emv.fzhhl.top

JS:   #private 字段；其余公开
来源：http://usv.0kj1m.cn

TS:   public / protected / private
来源：http://gby.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://nct.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nnu.jiagoushi.top

Ruby: public / protected / private
来源：http://nhn.wangdashe.top

C#:   public / protected / private / internal
来源：http://jnx.jinqigufen.top

[G11] getter / setter
来源：http://tcc.hammf.cn

Py:   @property 与 @x.setter
来源：http://url.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zne.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://dhb.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://pvp.zhengqikj.top

Java: public String getName() { return name; }
来源：http://yud.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cuf.gotoacloud.top

Ruby: attr_accessor :name
来源：http://yst.mhx1999.top

C#:   public string Name { get; set; }
来源：http://ajz.jinqigfzy.top

[G12] 对象转字符串
来源：http://qmy.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://kip.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lzv.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://cvx.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://hft.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://lxn.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://mwx.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://xcv.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://dam.dianchejie.cn

[G13] 判断对象类型
来源：http://igq.meibo888.top

Py:   isinstance(u, User)
来源：http://ktg.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://zya.yueranfly.top

JS:   u instanceof User
来源：http://sqp.quarkkingdee.top

TS:   u instanceof User
来源：http://sqc.gzhubu.top

Java: u instanceof User
来源：http://yvx.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://geh.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://rtl.haohaochexian.top

C#:   u is User
来源：http://mqd.jianghu66.top

[G14] 数据类 / record
来源：http://iej.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wrp.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://teo.zhijiandao.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rxu.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://noi.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://hmi.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://ttv.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uaw.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://zeq.ydzc1.top

[G15] 枚举
来源：http://omu.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://omo.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ots.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://amf.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://saw.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://iix.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dud.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://ecq.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bfw.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://ast.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zms.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://qjq.hcnkem.com

JS:   Object.entries(obj)
来源：http://wvw.iojbl.cn

TS:   Object.entries(obj)
来源：http://iwx.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vrz.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bqo.shuidangran.top

Ruby: obj.instance_variables
来源：http://fzr.haohaochexian.top

C#:   // 用反射或 System.Text.Json
来源：http://mxq.xuetiantiany.cn

================================================================================
来源：http://pac.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://jhm.hammf.cn

================================================================================
来源：http://con.dashuyun.cn

[H01] try / catch 基础
来源：http://sab.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hes.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kkn.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fxn.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lym.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jtz.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gxc.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kyn.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ukj.havefunace.top

[H02] finally / ensure 收尾
来源：http://sxf.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://elo.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wpx.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zsw.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://naw.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lit.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nqn.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://goo.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://upn.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://jil.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://flj.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bmw.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://vxn.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://soa.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aya.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jxt.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yvl.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://yrb.shzxlz.cn

[H04] 自定义异常类型
来源：http://mjd.uphjek.com

Py:   class MyError(Exception): pass
来源：http://yei.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qqs.jianghu66.top

JS:   class MyError extends Error {}
来源：http://vrx.yonumen.top

TS:   class MyError extends Error {}
来源：http://apz.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://vog.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hod.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://tef.yvedp.cn

C#:   class MyException : Exception {}
来源：http://xdq.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://bip.dianchejie.cn

Py:   except ValueError as e:
来源：http://uau.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ylm.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://xwt.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://tth.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://nsq.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://keg.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://imd.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ums.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://hhr.yj202588.top

Py:   value = d.get("k") or default
来源：http://nec.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://gtw.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mkg.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://iwi.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sol.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://opx.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://vip.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://slt.ydjk.org.cn

[H07] 断言
来源：http://zno.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://ure.yfazqb.com

PHP:  assert($x > 0);
来源：http://ppy.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://amz.xingfuxueyuan.xyz


<!-- 参考信息 -->