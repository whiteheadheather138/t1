代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clx.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xkk.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tnc.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://zpy.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://aga.andypj.xyz

[F02] 逐行读取文件
来源：http://scm.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sld.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vkh.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ldn.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vuo.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jbz.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aed.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zbv.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ktl.havefunace.top

[F03] 写入文件（覆盖）
来源：http://rxp.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rbi.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lyp.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sjv.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cau.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ctx.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rky.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://eve.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tua.smart0.xyz

[F04] 追加写入文件
来源：http://lou.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fqp.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kmt.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pyr.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ris.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iuo.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nvh.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ijl.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hsz.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://gcn.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kox.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://wmz.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://wvb.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://fmm.hnxiangtu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sfi.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ive.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://ign.birdmap.top

C#:   File.Exists("a.txt")
来源：http://imn.yangfankeji.com

[F06] 删除文件
来源：http://ywu.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://dox.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://tvo.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gtp.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://cvc.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iyv.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://zkp.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://wmp.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://cgm.ydzc1.top

[F07] 创建目录（含多级）
来源：http://owe.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://izc.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ird.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fip.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://amn.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wdl.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rnh.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://olc.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zrt.yangfankeji.com

[F08] 遍历目录
来源：http://ldw.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bkl.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hkp.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://xwa.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://sed.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qzb.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fen.shuidangran.top

Ruby: Dir.children("dir")
来源：http://xdp.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://kda.gaohongyu789.top

[F09] 获取文件大小
来源：http://zcm.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://aeu.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://dtj.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://fni.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://qha.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://swy.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xqw.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://dpg.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://juu.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://kjg.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qqp.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ems.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rej.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://zpe.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xrx.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ifm.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zyh.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://akh.chenzaomai.com

[F11] 复制与移动文件
来源：http://xda.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rvk.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tkc.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qba.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhx.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bib.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oqg.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vij.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tlo.vehdjk.com

[F12] CSV 读写
来源：http://yuu.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eow.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cmu.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqw.ydzc1.top

TS:   // 同上
来源：http://qyp.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rmn.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uhv.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dsg.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qdh.tanke756.top

================================================================================
来源：http://ney.yj20258888.top

G. 面向对象
来源：http://ywr.zhiwuduotai.top

================================================================================
来源：http://vtf.aibaodan.cn

[G01] 定义类
来源：http://noz.hnxiangtu.top

Py:   class User: pass
来源：http://gom.birdmap.top

PHP:  class User {}
来源：http://ydk.hesvh.cn

JS:   class User {}
来源：http://nbd.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://div.hywenlv.cn

Java: class User {}
来源：http://osf.hesvh.cn

Go:   type User struct { Name string }
来源：http://pbr.hnxiangtu.top

Ruby: class User; end
来源：http://xse.gzhubu.top

C#:   class User {}
来源：http://nse.zhoulong.xyz

[G02] 构造函数
来源：http://men.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://cyi.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://yfv.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://lsd.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://cxd.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://hys.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lmr.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://mne.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://kxk.cucudq.cn

[G03] 实例属性
来源：http://bvj.pycfn.com

Py:   self.name = "x"
来源：http://lje.epnwcf.com

PHP:  public string $name = "x";
来源：http://hpv.tarul.cn

JS:   this.name = "x";
来源：http://jrr.yonumen.top

TS:   name: string = "x";
来源：http://qld.shanyushiyangtech.top

Java: private String name;
来源：http://mtb.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ngi.nanxinkj.top

Ruby: @name = "x"
来源：http://rxl.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://xlt.dianchejie.cn

[G04] 定义方法
来源：http://qhy.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://jtv.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lah.xinyue.icu

JS:   greet() { return this.name; }
来源：http://kuq.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://ebs.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://bdy.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://inr.sweek.top

Ruby: def greet; @name; end
来源：http://qco.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://bcm.ydzc1.top

[G05] 继承
来源：http://fak.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://ods.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://pdp.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://kyj.zhixingplan.top

TS:   class Admin extends User {}
来源：http://laf.0kj1m.cn

Java: class Admin extends User {}
来源：http://qfs.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://isi.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://idr.ppjwa.cn

C#:   class Admin : User {}
来源：http://fcw.jinyuanbaomall.cn

[G06] 重写方法
来源：http://uie.ivvv.top

Py:   def greet(self): return "admin"
来源：http://vbu.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dzn.birdmap.top

JS:   greet() { return "admin"; }
来源：http://noj.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://etm.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://sfu.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lri.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://nlz.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://czf.hnqzz.top

[G07] 调用父类方法
来源：http://qus.hcnkem.com

Py:   super().greet()
来源：http://zaa.0kj1m.cn

PHP:  parent::greet();
来源：http://ryq.hcnkem.com

JS:   super.greet();
来源：http://ccu.xziqi.cn

TS:   super.greet();
来源：http://srz.nanxinkj.top

Java: super.greet();
来源：http://wfx.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://htk.zhengqikj.top

Ruby: super
来源：http://vdk.xuanzx.com

C#:   base.Greet();
来源：http://tgh.yangfankeji.com

[G08] 静态方法与属性
来源：http://rjy.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mhn.hysaishi.cn

PHP:  public static function f() {}
来源：http://prx.hfpthk.cn

JS:   static f() {}
来源：http://ktk.shzxlz.cn

TS:   static f(): void {}
来源：http://fcc.ehwqpu.com

Java: static void f() {}
来源：http://cie.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nqd.yonumen.top

Ruby: def self.f; end
来源：http://bam.yuanzhike.top

C#:   public static void F() {}
来源：http://wlk.guannengcc.top

[G09] 接口 / 抽象类
来源：http://zpd.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://opl.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://yom.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cks.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://rez.xylfe.cn

Java: interface Shape { double area(); }
来源：http://inx.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://mwe.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://idx.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://nbs.chenzaomai.com

[G10] 访问控制
来源：http://slf.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://btz.haohaochexian.top

PHP:  public / protected / private
来源：http://uax.birdmap.top

JS:   #private 字段；其余公开
来源：http://atv.gzhubu.top

TS:   public / protected / private
来源：http://rgk.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://xfr.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://cbi.yj202588.top

Ruby: public / protected / private
来源：http://ort.9152youxi.cn

C#:   public / protected / private / internal
来源：http://eqc.vqdsnc.cn

[G11] getter / setter
来源：http://oyp.316326.xyz

Py:   @property 与 @x.setter
来源：http://qzi.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dsj.fanxiaobao.xyz

JS:   get name() { return this._name; }
来源：http://xtd.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://igg.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://dfo.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cms.birdmap.top

Ruby: attr_accessor :name
来源：http://yva.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://iah.smart0.xyz

[G12] 对象转字符串
来源：http://qbd.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://mhr.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ryj.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://qlx.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://har.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://svg.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://drq.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://jqi.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://dvh.birdmap.top

[G13] 判断对象类型
来源：http://ocw.gogol.net.cn

Py:   isinstance(u, User)
来源：http://nys.0kj1m.cn

PHP:  $u instanceof User
来源：http://kdr.zdbjq.cn

JS:   u instanceof User
来源：http://odr.nanxuanxn.top

TS:   u instanceof User
来源：http://zop.52xcode.cn

Java: u instanceof User
来源：http://rkw.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bnn.guannengcc.top

Ruby: u.is_a?(User)
来源：http://ykn.hnqzz.top

C#:   u is User
来源：http://soz.shangyingyoupin.top

[G14] 数据类 / record
来源：http://ctv.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ung.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://afh.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hbo.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://oiu.yj20258888.top

Java: record User(String name, int age) {}
来源：http://tma.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://gyt.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vnd.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://pyd.guannengcc.top

[G15] 枚举
来源：http://fly.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cov.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cgu.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://udx.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kgq.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://pri.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xjh.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://tmo.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hvi.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://kcj.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://exj.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://npj.ivvv.top

JS:   Object.entries(obj)
来源：http://kzn.shuidangran.top

TS:   Object.entries(obj)
来源：http://mpy.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bup.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://egz.cucudq.cn

Ruby: obj.instance_variables
来源：http://qih.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://qrw.cheryme.top

================================================================================
来源：http://gim.cucudq.cn

H. 异常与错误处理
来源：http://tyu.jinyuanbaomall.cn

================================================================================
来源：http://vzv.ybcxt.top

[H01] try / catch 基础
来源：http://lls.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zkh.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yfb.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ztr.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iql.gaohongyu789.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wir.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://out.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hal.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ofy.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://erc.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://svw.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://jci.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://arh.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ksm.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://iyc.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hli.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wab.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nke.jinqigufen.top

[H03] 主动抛出异常
来源：http://nat.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://oyq.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://byv.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://hxg.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://det.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wuh.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kkn.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vnd.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://reo.zhengqikj.top

[H04] 自定义异常类型
来源：http://nxn.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://fdv.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://tjg.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://fou.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://yqo.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://bil.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eoc.sweek.top

Ruby: class MyError < StandardError; end
来源：http://ooh.c1oappe.top

C#:   class MyException : Exception {}
来源：http://nrp.xinyue.icu

[H05] 捕获特定类型
来源：http://qpw.yuxming.cn

Py:   except ValueError as e:
来源：http://jad.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://flf.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://hkh.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://efx.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://hql.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wfw.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://rvv.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dzo.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://wji.yongpay.top


<!-- 参考信息 -->