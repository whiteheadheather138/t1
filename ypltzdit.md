代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xbw.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ona.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vvo.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bii.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lap.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://plp.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://kyv.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nkp.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oxs.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vly.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mil.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ezh.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qvy.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://gvf.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://elo.uphjek.com

[F04] 追加写入文件
来源：http://bqn.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wzz.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://quf.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kho.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qke.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ymq.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pla.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ldl.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rxj.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://uab.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ehz.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://mwr.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://pil.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://asb.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nnx.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bkp.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://jul.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://qvy.sxryk.cn

[F06] 删除文件
来源：http://zzw.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://nmo.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://awp.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://luc.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://nys.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://frc.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://wln.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://mku.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://amr.shuidangran.top

[F07] 创建目录（含多级）
来源：http://qhm.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://drx.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qev.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xez.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxl.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kxm.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kwg.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://owo.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nrq.iojbl.cn

[F08] 遍历目录
来源：http://zpz.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ubd.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rua.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://gaw.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://gvj.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kou.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aau.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://iav.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://lvc.gzhubu.top

[F09] 获取文件大小
来源：http://iru.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://pcr.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://syh.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://vpp.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://ojx.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://yrj.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oxe.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://zhn.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://jew.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://psv.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zzy.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zwi.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xan.iojbl.cn

TS:   path.extname("a.txt")
来源：http://ove.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://stz.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uic.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vef.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ccj.daxiang520.top

[F11] 复制与移动文件
来源：http://pkq.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hro.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tqf.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jjg.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nia.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://swo.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eav.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://geg.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hir.haohaochexian.top

[F12] CSV 读写
来源：http://qzq.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fkl.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vqd.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ojg.yanxiufei.cn

TS:   // 同上
来源：http://lid.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nsl.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jry.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eqy.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dpt.sysykeji.top

================================================================================
来源：http://wwa.xuetiantiany.cn

G. 面向对象
来源：http://vrk.gzhubu.top

================================================================================
来源：http://mmr.chenlongwang.top

[G01] 定义类
来源：http://iap.shzxlz.cn

Py:   class User: pass
来源：http://dtd.fzhhl.top

PHP:  class User {}
来源：http://gnj.316326.xyz

JS:   class User {}
来源：http://jxu.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://kkb.epnwcf.com

Java: class User {}
来源：http://isz.ybcxt.top

Go:   type User struct { Name string }
来源：http://okv.shuidangran.top

Ruby: class User; end
来源：http://hvk.yangfankeji.com

C#:   class User {}
来源：http://cqz.yanxiufei.cn

[G02] 构造函数
来源：http://fad.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://itm.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://kqd.chenjidiqi.icu

JS:   constructor(name) { this.name = name; }
来源：http://hkv.ivvv.top

TS:   constructor(public name: string) {}
来源：http://cxn.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://bdu.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://coo.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://kod.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://bgn.nanxuanxn.top

[G03] 实例属性
来源：http://ywl.yuxming.cn

Py:   self.name = "x"
来源：http://oir.ctjpmb.com

PHP:  public string $name = "x";
来源：http://pgt.shangyingyoupin.top

JS:   this.name = "x";
来源：http://squ.xinyue.icu

TS:   name: string = "x";
来源：http://olb.chenzaomai.com

Java: private String name;
来源：http://rbf.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kxx.cheryme.top

Ruby: @name = "x"
来源：http://rjy.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://wsl.tian-w.cn

[G04] 定义方法
来源：http://moc.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://dun.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kyd.xinyue.icu

JS:   greet() { return this.name; }
来源：http://rhv.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://jfy.yuanzhike.top

Java: String greet() { return name; }
来源：http://jbh.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rxe.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://wov.birdmap.top

C#:   public string Greet() => Name;
来源：http://rhw.yfazqb.com

[G05] 继承
来源：http://xsi.c1oappe.top

Py:   class Admin(User): pass
来源：http://msh.epnwcf.com

PHP:  class Admin extends User {}
来源：http://hth.dashuyun.cn

JS:   class Admin extends User {}
来源：http://zun.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://xci.chenlongwang.top

Java: class Admin extends User {}
来源：http://dur.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ycf.fengsongda.top

Ruby: class Admin < User; end
来源：http://goo.ppjwa.cn

C#:   class Admin : User {}
来源：http://eog.zhixingplan.top

[G06] 重写方法
来源：http://top.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://now.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dhd.vqdsnc.cn

JS:   greet() { return "admin"; }
来源：http://owm.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://dvy.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://uiw.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pbv.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://dcu.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://azk.chenjidiqi.icu

[G07] 调用父类方法
来源：http://dop.wangshuangyany.cn

Py:   super().greet()
来源：http://rit.feifeiyinyue.top

PHP:  parent::greet();
来源：http://uut.jinqigfzy.top

JS:   super.greet();
来源：http://faf.xziqi.cn

TS:   super.greet();
来源：http://kqt.xinyue.icu

Java: super.greet();
来源：http://krb.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ipo.gzhubu.top

Ruby: super
来源：http://qlg.zhoulong.xyz

C#:   base.Greet();
来源：http://ejt.yonumen.top

[G08] 静态方法与属性
来源：http://kxm.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vnn.jqgfzy.top

PHP:  public static function f() {}
来源：http://niw.gzhubu.top

JS:   static f() {}
来源：http://qcv.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://bgd.guowangkeji.top

Java: static void f() {}
来源：http://sbq.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zki.vehdjk.com

Ruby: def self.f; end
来源：http://lxz.shuidangran.top

C#:   public static void F() {}
来源：http://luj.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://lqf.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://nvg.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://drz.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xqs.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://zrw.andypj.xyz

Java: interface Shape { double area(); }
来源：http://gcg.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://udv.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypw.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://gdf.tarul.cn

[G10] 访问控制
来源：http://nkb.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://ivd.hnqzz.top

PHP:  public / protected / private
来源：http://ofm.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://xnt.dianchejie.cn

TS:   public / protected / private
来源：http://siz.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://dsk.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gpu.iojbl.cn

Ruby: public / protected / private
来源：http://ylq.fengsongda.top

C#:   public / protected / private / internal
来源：http://glg.zhengqikj.top

[G11] getter / setter
来源：http://rxp.hnqzz.top

Py:   @property 与 @x.setter
来源：http://wwc.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ubq.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://csu.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://ecy.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://vgm.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pzv.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://qif.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://etp.nwbrower.top

[G12] 对象转字符串
来源：http://eco.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://gmf.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bao.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://iql.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://wgx.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://aqo.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://rsx.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://qvr.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://vys.jiagoushi.top

[G13] 判断对象类型
来源：http://evn.tian-w.cn

Py:   isinstance(u, User)
来源：http://skd.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://amc.chenzaomai.com

JS:   u instanceof User
来源：http://epj.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://zdq.gaohongyu789.top

Java: u instanceof User
来源：http://pmz.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://icq.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://dkg.ybcxt.top

C#:   u is User
来源：http://how.quarkkingdee.top

[G14] 数据类 / record
来源：http://dsx.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rdh.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://lso.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://nrk.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://ypk.xinyue.icu

Java: record User(String name, int age) {}
来源：http://cal.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://vhk.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://twy.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://aop.haohaochexian.top

[G15] 枚举
来源：http://oqu.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tjd.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zey.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wsd.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rsg.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://rkq.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rfr.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://qyd.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ljm.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://emw.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xpg.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://sdv.yfazqb.com

JS:   Object.entries(obj)
来源：http://tnw.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://imb.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dqu.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://ddf.sxryk.cn

Ruby: obj.instance_variables
来源：http://vka.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://vuc.haohaochexian.top

================================================================================
来源：http://jhq.sysykeji.top

H. 异常与错误处理
来源：http://rji.cashguo.top

================================================================================
来源：http://rev.pycfn.com

[H01] try / catch 基础
来源：http://nrr.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lml.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uor.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mkw.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ehw.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wqz.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://syb.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hmy.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hgm.yueranfly.top

[H02] finally / ensure 收尾
来源：http://gbe.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iqz.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://cil.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ihj.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yhl.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jdp.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ele.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tcu.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iwf.havefunace.top

[H03] 主动抛出异常
来源：http://xkr.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://kiw.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jkj.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://qib.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://jzu.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://mya.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pgl.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zjp.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://ljx.ybcxt.top

[H04] 自定义异常类型
来源：http://gwh.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://sim.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mbn.meibo888.top

JS:   class MyError extends Error {}
来源：http://vwj.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://lrt.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://nfc.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tta.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://svl.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://hpx.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://cdv.xziqi.cn

Py:   except ValueError as e:
来源：http://nzp.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umv.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://mnq.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://fle.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://pex.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://quo.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://rya.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ghi.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://tho.52xcode.cn

Py:   value = d.get("k") or default
来源：http://lmn.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://iyy.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://nhh.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ndm.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://siy.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://saf.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://iyh.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://sum.zhiwuduotai.top


<!-- 参考信息 -->