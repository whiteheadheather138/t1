代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://vzf.cqqwz.cn

[F02] 逐行读取文件
来源：http://zvr.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lvy.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rem.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ahf.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mcu.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vnm.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://idl.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lik.hywenlv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qen.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://ovo.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xky.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pen.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mye.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bre.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mel.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ikd.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://yms.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ohp.yangfankeji.com

[F04] 追加写入文件
来源：http://vho.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ont.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xqq.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ybq.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uwv.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wes.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iyl.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ejy.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ozr.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://oqk.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wjr.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://myl.shanyushiyangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://fdi.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://gbb.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ihc.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nse.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://axb.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://vjz.hnxiangtu.top

[F06] 删除文件
来源：http://sbi.xinyue.icu

Py:   os.remove("a.txt")
来源：http://nli.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://yhw.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://sdd.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://qmt.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mmd.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://qtv.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://bqd.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://jex.sweek.top

[F07] 创建目录（含多级）
来源：http://smw.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mxh.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cob.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivx.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zvu.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kus.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wbx.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fty.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zhu.zhongyouzk.top

[F08] 遍历目录
来源：http://spc.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://toy.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gaf.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://loa.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://hej.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xxt.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kww.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://jkc.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://xsv.fengsongda.top

[F09] 获取文件大小
来源：http://yaf.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://ofs.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://nzc.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://vbz.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://ugd.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://fri.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tqs.bjfxy.top

Ruby: File.size("a.txt")
来源：http://foy.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://uev.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://sev.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fvo.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://efj.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://olj.pycfn.com

TS:   path.extname("a.txt")
来源：http://nus.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://won.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eho.hcnkem.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dvt.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://imq.shuidangran.top

[F11] 复制与移动文件
来源：http://fhx.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ewv.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dbm.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lrf.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xkw.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tpv.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tbd.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tcj.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fku.shangyingyoupin.top

[F12] CSV 读写
来源：http://kco.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://odd.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hhs.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ors.jinqigufen.top

TS:   // 同上
来源：http://pyj.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bav.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lnu.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mvg.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zgw.zhiwuduotai.top

================================================================================
来源：http://sik.haohaochexian.top

G. 面向对象
来源：http://cnj.mhx1999.top

================================================================================
来源：http://iqa.wangdashe.top

[G01] 定义类
来源：http://jeu.yanxiufei.cn

Py:   class User: pass
来源：http://wku.shzxlz.cn

PHP:  class User {}
来源：http://dft.fanxiaobao.xyz

JS:   class User {}
来源：http://ydd.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://goy.zhijiandao.cn

Java: class User {}
来源：http://qtl.vqdsnc.cn

Go:   type User struct { Name string }
来源：http://hmu.aizwys.cn

Ruby: class User; end
来源：http://nhf.tianlin.xyz

C#:   class User {}
来源：http://rqc.guannengcc.top

[G02] 构造函数
来源：http://cli.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://dbq.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ilh.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://bgn.uphjek.com

TS:   constructor(public name: string) {}
来源：http://idy.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://vhu.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dit.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://hoj.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://dzx.hammf.cn

[G03] 实例属性
来源：http://mqf.fengsongda.top

Py:   self.name = "x"
来源：http://hoe.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://hss.sjlbkw.cn

JS:   this.name = "x";
来源：http://fsx.52xcode.cn

TS:   name: string = "x";
来源：http://qhv.fengsongda.top

Java: private String name;
来源：http://wqa.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://avd.bbcook.cn

Ruby: @name = "x"
来源：http://qkw.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://jiv.sjlbkw.cn

[G04] 定义方法
来源：http://bnv.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://vff.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gew.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://zvc.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://dle.jianghu66.top

Java: String greet() { return name; }
来源：http://bhm.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cjl.9152youxi.cn

Ruby: def greet; @name; end
来源：http://dsh.havefunace.top

C#:   public string Greet() => Name;
来源：http://inb.fzhhl.top

[G05] 继承
来源：http://xoi.daxiang520.top

Py:   class Admin(User): pass
来源：http://oll.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://avk.redwolf501.top

JS:   class Admin extends User {}
来源：http://tta.snrcjt.cn

TS:   class Admin extends User {}
来源：http://onn.zhengqikj.top

Java: class Admin extends User {}
来源：http://fcq.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rjr.xinyue.icu

Ruby: class Admin < User; end
来源：http://wvx.nwbrower.top

C#:   class Admin : User {}
来源：http://yii.zhaomingkeji.xyz

[G06] 重写方法
来源：http://hgy.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://rxv.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kzi.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://fba.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://cje.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://eak.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vak.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://klq.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://iat.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://wey.yueranfly.top

Py:   super().greet()
来源：http://iku.aizwys.cn

PHP:  parent::greet();
来源：http://cls.vqdsnc.cn

JS:   super.greet();
来源：http://fua.aibaodan.cn

TS:   super.greet();
来源：http://njn.mhx1999.top

Java: super.greet();
来源：http://jgd.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bve.hywenlv.cn

Ruby: super
来源：http://pip.nanxinkj.top

C#:   base.Greet();
来源：http://hdx.hfpthk.cn

[G08] 静态方法与属性
来源：http://xnx.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zrf.jianghu66.top

PHP:  public static function f() {}
来源：http://aru.zycfv.cn

JS:   static f() {}
来源：http://lnz.guannengcc.top

TS:   static f(): void {}
来源：http://cvq.cheryme.top

Java: static void f() {}
来源：http://efj.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://hbs.ivvv.top

Ruby: def self.f; end
来源：http://ajk.epnwcf.com

C#:   public static void F() {}
来源：http://pjm.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://awn.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://akq.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://pzo.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://pbc.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://mdq.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://rvj.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://nkx.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iyv.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://nvw.xylfe.cn

[G10] 访问控制
来源：http://avv.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://ava.hnqzz.top

PHP:  public / protected / private
来源：http://fyx.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://jty.iojbl.cn

TS:   public / protected / private
来源：http://hup.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://xey.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://yur.zhoulong.xyz

Ruby: public / protected / private
来源：http://xbz.sufxvd.cn

C#:   public / protected / private / internal
来源：http://mez.52xcode.cn

[G11] getter / setter
来源：http://uxl.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://may.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://htl.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://wyv.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://qys.dashuyun.cn

Java: public String getName() { return name; }
来源：http://qbk.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xuj.hnxiangtu.top

Ruby: attr_accessor :name
来源：http://eop.aizwys.cn

C#:   public string Name { get; set; }
来源：http://pnk.daxiang520.top

[G12] 对象转字符串
来源：http://sbb.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://ubq.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xjz.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://rte.meibo888.top

TS:   toString(): string { return this.name; }
来源：http://zdz.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://ksd.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://lff.mhx1999.top

Ruby: def to_s; @name; end
来源：http://sxk.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://spu.wangdashe.top

[G13] 判断对象类型
来源：http://jmv.ehwqpu.com

Py:   isinstance(u, User)
来源：http://lbs.nanxuanxn.top

PHP:  $u instanceof User
来源：http://gkr.nanxuanxn.top

JS:   u instanceof User
来源：http://dot.haohaochexian.top

TS:   u instanceof User
来源：http://yco.jinqigufen.top

Java: u instanceof User
来源：http://imv.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sgv.uphjek.com

Ruby: u.is_a?(User)
来源：http://fds.gaohongyu789.top

C#:   u is User
来源：http://hgr.chenlongwang.top

[G14] 数据类 / record
来源：http://fzy.hysaishi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jmx.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://tgi.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://kpr.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://ztt.sxryk.cn

Java: record User(String name, int age) {}
来源：http://eiz.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://xxm.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qys.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://wfu.jiagoushi.top

[G15] 枚举
来源：http://jyg.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ujd.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ngp.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sxv.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jcc.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://lsq.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cvm.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://dsw.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hri.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://ahc.xuetiantiany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://muj.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://ylb.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://dqh.tanke756.top

TS:   Object.entries(obj)
来源：http://ykk.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aqh.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://oyp.birdmap.top

Ruby: obj.instance_variables
来源：http://lka.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://mlt.xingfuxueyuan.xyz

================================================================================
来源：http://ita.hywenlv.cn

H. 异常与错误处理
来源：http://wrq.hcnkem.com

================================================================================
来源：http://kiq.shuidangran.top

[H01] try / catch 基础
来源：http://mgz.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xji.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wfa.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vcx.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cqf.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gwi.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://szn.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gub.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iib.yj20258888.top

[H02] finally / ensure 收尾
来源：http://nab.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://uac.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nyf.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iev.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kgr.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lqm.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://idp.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fbw.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ycd.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://qyy.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://hnk.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jcr.birdmap.top

JS:   throw new Error("错误信息");
来源：http://lfd.316326.xyz

TS:   throw new Error("错误信息");
来源：http://sda.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cap.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ugn.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://foq.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bfm.yueranfly.top

[H04] 自定义异常类型
来源：http://ojh.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://okk.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://lzp.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://usl.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://bqe.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://kng.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dpv.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://gud.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://fpn.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://bye.xziqi.cn

Py:   except ValueError as e:
来源：http://qzj.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uga.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://bzw.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://now.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://qro.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://php.sweek.top

Ruby: rescue ArgumentError => e
来源：http://vkq.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qfk.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://gns.ivvv.top

Py:   value = d.get("k") or default
来源：http://abp.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://jhm.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://phv.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://nqa.zhengqikj.top


<!-- 参考信息 -->