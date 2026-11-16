代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://iht.yfazqb.com

[F02] 逐行读取文件
来源：http://mvd.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xgl.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ara.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xbc.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://thi.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eqp.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://soy.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gcn.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xfz.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://det.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bse.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fsx.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dum.aizwys.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yvh.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bui.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uaa.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://msa.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ygg.dashuyun.cn

[F04] 追加写入文件
来源：http://uji.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cni.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tza.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npr.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rgv.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zrn.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wrb.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cjp.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://seg.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://anc.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rwy.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://blu.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://kyr.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://bqa.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zhh.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fxx.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://zjx.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://ioo.bbcook.cn

[F06] 删除文件
来源：http://zkb.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://uju.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://trs.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://mul.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://veb.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://esr.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://bap.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://mry.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://ayi.yvedp.cn

[F07] 创建目录（含多级）
来源：http://xwv.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mji.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://diq.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tci.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xbg.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dhp.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fkq.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uiu.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hgo.dianchejie.cn

[F08] 遍历目录
来源：http://yqp.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nmi.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://daz.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://dfy.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://lqk.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jfk.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgv.c1oappe.top

Ruby: Dir.children("dir")
来源：http://ppd.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://arb.vqdsnc.cn

[F09] 获取文件大小
来源：http://siy.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://biz.xuanzx.com

PHP:  filesize("a.txt");
来源：http://pvg.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://lqu.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://ndf.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://txq.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oal.cucudq.cn

Ruby: File.size("a.txt")
来源：http://ttj.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://kft.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://sgl.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ifq.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://inn.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://llz.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://dkf.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cow.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vvq.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kki.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nrg.svipenyu.cn

[F11] 复制与移动文件
来源：http://oxm.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ngr.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rfp.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpb.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jyt.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fsv.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://huf.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wjk.vehdjk.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fed.guowangkeji.top

[F12] CSV 读写
来源：http://lwm.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ato.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dvp.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sdv.yfazqb.com

TS:   // 同上
来源：http://qvk.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zdu.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fam.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jwy.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wed.yuanzhike.top

================================================================================
来源：http://xyl.hongshengwenyu.top

G. 面向对象
来源：http://ugb.jqgfzy.top

================================================================================
来源：http://clg.shuidangran.top

[G01] 定义类
来源：http://qux.daxiang520.top

Py:   class User: pass
来源：http://mgk.jqgufenzy.top

PHP:  class User {}
来源：http://cxz.aizwys.cn

JS:   class User {}
来源：http://haz.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://doa.gotoacloud.top

Java: class User {}
来源：http://ovi.fzhhl.top

Go:   type User struct { Name string }
来源：http://qps.nanxuanxn.top

Ruby: class User; end
来源：http://ccy.sweek.top

C#:   class User {}
来源：http://dao.tian-w.cn

[G02] 构造函数
来源：http://pns.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://ota.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://dsj.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://qcs.havefunace.top

TS:   constructor(public name: string) {}
来源：http://gvd.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://lfl.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qti.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://krw.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://tjd.hnxiangtu.top

[G03] 实例属性
来源：http://gdj.jinqigufen.top

Py:   self.name = "x"
来源：http://bqp.zdbjq.cn

PHP:  public string $name = "x";
来源：http://zou.cqqwz.cn

JS:   this.name = "x";
来源：http://rhu.xinyue.icu

TS:   name: string = "x";
来源：http://zrw.aizwys.cn

Java: private String name;
来源：http://fbd.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zft.ctjpmb.com

Ruby: @name = "x"
来源：http://ogp.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://tdw.zhoulong.xyz

[G04] 定义方法
来源：http://cec.daxiang520.top

Py:   def greet(self): return self.name
来源：http://zzo.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://eee.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://lgw.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://obv.uphjek.com

Java: String greet() { return name; }
来源：http://ptj.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nyw.bbcook.cn

Ruby: def greet; @name; end
来源：http://hne.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://irm.redwolf501.top

[G05] 继承
来源：http://esj.fktsv.cn

Py:   class Admin(User): pass
来源：http://yvc.andypj.xyz

PHP:  class Admin extends User {}
来源：http://juu.dashuyun.cn

JS:   class Admin extends User {}
来源：http://xlq.nanxinkj.top

TS:   class Admin extends User {}
来源：http://egp.vqdsnc.cn

Java: class Admin extends User {}
来源：http://fwr.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bov.cheryme.top

Ruby: class Admin < User; end
来源：http://pqg.hnqzz.top

C#:   class Admin : User {}
来源：http://nel.yj20258888.top

[G06] 重写方法
来源：http://jvv.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://gmp.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://wql.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://gsz.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://pus.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://yud.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qbk.pycfn.com

Ruby: def greet; "admin"; end
来源：http://oii.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://pxb.jianghu66.top

[G07] 调用父类方法
来源：http://xxp.xziqi.cn

Py:   super().greet()
来源：http://ipl.shuidangran.top

PHP:  parent::greet();
来源：http://fvt.tianlin.xyz

JS:   super.greet();
来源：http://yfj.aizwys.cn

TS:   super.greet();
来源：http://vrj.shuidangran.top

Java: super.greet();
来源：http://nzu.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ppu.fktsv.cn

Ruby: super
来源：http://qux.dianchejie.cn

C#:   base.Greet();
来源：http://fld.hfpthk.cn

[G08] 静态方法与属性
来源：http://sqt.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pea.fengsongda.top

PHP:  public static function f() {}
来源：http://dro.hywenlv.cn

JS:   static f() {}
来源：http://dyy.yfazqb.com

TS:   static f(): void {}
来源：http://czo.vqdsnc.cn

Java: static void f() {}
来源：http://upz.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qhu.hfpthk.cn

Ruby: def self.f; end
来源：http://rlh.cdnleiting.top

C#:   public static void F() {}
来源：http://joz.cheryme.top

[G09] 接口 / 抽象类
来源：http://qki.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://ljq.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xrx.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ahp.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://ksu.birdmap.top

Java: interface Shape { double area(); }
来源：http://fiv.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://kvh.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wlw.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://paf.chenjidiqi.icu

[G10] 访问控制
来源：http://ubd.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://kws.jyoumei.cn

PHP:  public / protected / private
来源：http://etc.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://ifm.chenzaomai.com

TS:   public / protected / private
来源：http://xtv.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://cht.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zbu.uphjek.com

Ruby: public / protected / private
来源：http://ttb.yvedp.cn

C#:   public / protected / private / internal
来源：http://mut.chenlongwang.top

[G11] getter / setter
来源：http://szp.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://hsq.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://djf.sweek.top

JS:   get name() { return this._name; }
来源：http://vgy.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://vjo.ydzc1.top

Java: public String getName() { return name; }
来源：http://csb.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dss.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://wal.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://wam.sxryk.cn

[G12] 对象转字符串
来源：http://voq.sweek.top

Py:   def __str__(self): return self.name
来源：http://zuf.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lmo.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://nfo.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://jei.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://ovu.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://drs.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://xff.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://smk.cqqwz.cn

[G13] 判断对象类型
来源：http://zsw.0kj1m.cn

Py:   isinstance(u, User)
来源：http://kdh.hesvh.cn

PHP:  $u instanceof User
来源：http://qks.uphjek.com

JS:   u instanceof User
来源：http://xmo.daxiang520.top

TS:   u instanceof User
来源：http://gzn.gogol.net.cn

Java: u instanceof User
来源：http://oav.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://swh.xziqi.cn

Ruby: u.is_a?(User)
来源：http://ujx.sufxvd.cn

C#:   u is User
来源：http://lzf.vehdjk.com

[G14] 数据类 / record
来源：http://pks.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vvq.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://efs.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://gld.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://mtv.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://yxj.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://cth.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xuy.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://trp.yanxiufei.cn

[G15] 枚举
来源：http://njy.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gyt.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xrs.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gcc.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wsc.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://mhj.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nds.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://hfm.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gev.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://xsj.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nll.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://mke.9152youxi.cn

JS:   Object.entries(obj)
来源：http://ewe.52xcode.cn

TS:   Object.entries(obj)
来源：http://txe.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dpg.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mcn.chenzaomai.com

Ruby: obj.instance_variables
来源：http://foo.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://jwi.yonumen.top

================================================================================
来源：http://vgk.ppjwa.cn

H. 异常与错误处理
来源：http://pmr.bbcook.cn

================================================================================
来源：http://omu.zdqjudy.top

[H01] try / catch 基础
来源：http://mlk.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tur.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hgm.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fxb.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jse.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wwy.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lan.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uey.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wxz.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://svg.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://lhs.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kec.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bpx.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sbi.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aqj.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qra.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nsx.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://azs.zdqjudy.top

[H03] 主动抛出异常
来源：http://qiy.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://cdz.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vwc.havefunace.top

JS:   throw new Error("错误信息");
来源：http://zcf.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://for.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jev.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zvk.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xep.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://hli.bbcook.cn

[H04] 自定义异常类型
来源：http://hjk.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://krn.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ihr.fktsv.cn

JS:   class MyError extends Error {}
来源：http://lfp.yj202588.top

TS:   class MyError extends Error {}
来源：http://myd.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://opu.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bvg.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://ome.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://mia.yj20258.top

[H05] 捕获特定类型
来源：http://lop.fktsv.cn

Py:   except ValueError as e:
来源：http://sxs.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://olv.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://okt.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://oqv.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://hyc.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hjw.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://vfe.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hig.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://gkc.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://exs.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pne.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://agq.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://tzd.316326.xyz


<!-- 参考信息 -->