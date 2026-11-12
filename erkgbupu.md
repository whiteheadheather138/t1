代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gah.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mdi.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://crn.yfazqb.com

Ruby: File.read("a.txt")
来源：http://qnh.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lrb.yuanzhike.top

[F02] 逐行读取文件
来源：http://huh.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fef.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ofz.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vsm.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxq.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qrx.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://unh.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oyg.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cdh.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://qdk.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gxb.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hgk.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrg.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mcq.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jun.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yzr.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://dxp.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://znh.nwbrower.top

[F04] 追加写入文件
来源：http://rje.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nbc.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ihk.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xjz.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jul.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oxx.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ter.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qsg.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ond.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://mvd.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vwa.pycfn.com

PHP:  file_exists("a.txt");
来源：http://qsy.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://zwg.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://kvp.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gqb.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ebm.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://moo.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://uyb.cheryme.top

[F06] 删除文件
来源：http://puz.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://iek.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://nyg.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://dyx.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://lhn.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bkk.cashguo.top

Go:   os.Remove("a.txt")
来源：http://kac.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://afi.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://rqb.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://qtm.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://opv.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dwd.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dua.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nro.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vih.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jgb.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wlv.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hgv.zhixingplan.top

[F08] 遍历目录
来源：http://lxb.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ocz.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tyt.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://oso.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://lug.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qmu.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://odt.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://kjl.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://lvv.yfazqb.com

[F09] 获取文件大小
来源：http://eod.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://geu.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://ldu.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://jqw.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://blx.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rpw.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ojl.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://dni.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://xhk.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://hfg.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kni.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jvc.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wvk.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://sjq.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yrv.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cpt.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ljb.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pjm.jqgfzy.top

[F11] 复制与移动文件
来源：http://ibk.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yrl.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jkf.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sze.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lce.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qrq.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iux.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://frf.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vyo.cqqwz.cn

[F12] CSV 读写
来源：http://jvj.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ayz.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zmq.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://csn.zhixingplan.top

TS:   // 同上
来源：http://fif.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qpt.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fee.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hih.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tzg.nanxinkj.top

================================================================================
来源：http://fcj.hysaishi.cn

G. 面向对象
来源：http://wbv.jinqigfzy.top

================================================================================
来源：http://ujl.guowangkeji.top

[G01] 定义类
来源：http://bae.cqqwz.cn

Py:   class User: pass
来源：http://xou.gotoacloud.top

PHP:  class User {}
来源：http://pgx.guowangkeji.top

JS:   class User {}
来源：http://sxx.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://gqi.cashguo.top

Java: class User {}
来源：http://iaz.yongpay.top

Go:   type User struct { Name string }
来源：http://lcx.snrcjt.cn

Ruby: class User; end
来源：http://edr.52xcode.cn

C#:   class User {}
来源：http://opo.yj202588.top

[G02] 构造函数
来源：http://hvs.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://vsp.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://smp.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://tce.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://ykz.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://dnq.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hav.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://jfm.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://fcv.hongshengwenyu.top

[G03] 实例属性
来源：http://bnd.ppjwa.cn

Py:   self.name = "x"
来源：http://plb.cashguo.top

PHP:  public string $name = "x";
来源：http://gxp.kuanghao11.cn

JS:   this.name = "x";
来源：http://aot.yfazqb.com

TS:   name: string = "x";
来源：http://lak.sysykeji.top

Java: private String name;
来源：http://aja.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ymi.birdmap.top

Ruby: @name = "x"
来源：http://zum.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://zmr.ivvv.top

[G04] 定义方法
来源：http://rsr.xziqi.cn

Py:   def greet(self): return self.name
来源：http://orm.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kky.daria6918.cn

JS:   greet() { return this.name; }
来源：http://ryh.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://rml.hammf.cn

Java: String greet() { return name; }
来源：http://myu.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://afn.yj20258.top

Ruby: def greet; @name; end
来源：http://geu.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://tud.yuxming.cn

[G05] 继承
来源：http://gji.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://fxi.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://pzm.hywenlv.cn

JS:   class Admin extends User {}
来源：http://vcq.aibaodan.cn

TS:   class Admin extends User {}
来源：http://vhi.jinqigufen.top

Java: class Admin extends User {}
来源：http://ofr.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hzm.snrcjt.cn

Ruby: class Admin < User; end
来源：http://mgj.jqgufenzy.top

C#:   class Admin : User {}
来源：http://jkh.yuxming.cn

[G06] 重写方法
来源：http://npd.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://syl.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kxt.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://ays.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://sor.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://dya.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ttr.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://mkk.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://nzu.sjlbkw.cn

[G07] 调用父类方法
来源：http://dlq.quarkkingdee.top

Py:   super().greet()
来源：http://xdw.ydjk.org.cn

PHP:  parent::greet();
来源：http://gcr.hongshengwenyu.top

JS:   super.greet();
来源：http://ckw.gogol.net.cn

TS:   super.greet();
来源：http://hym.xingfuxueyuan.xyz

Java: super.greet();
来源：http://jui.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://efn.9152youxi.cn

Ruby: super
来源：http://lpj.iojbl.cn

C#:   base.Greet();
来源：http://kax.xinyue.icu

[G08] 静态方法与属性
来源：http://enz.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xgc.9152youxi.cn

PHP:  public static function f() {}
来源：http://uhe.chenlongwang.top

JS:   static f() {}
来源：http://gcy.andypj.xyz

TS:   static f(): void {}
来源：http://jxi.ybcxt.top

Java: static void f() {}
来源：http://ruz.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bda.gotoacloud.top

Ruby: def self.f; end
来源：http://ini.guowangkeji.top

C#:   public static void F() {}
来源：http://yqq.hnqzz.top

[G09] 接口 / 抽象类
来源：http://ccd.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://fak.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gfj.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gvu.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://gfl.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://leu.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://cwb.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gfa.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://dnx.yj202588.top

[G10] 访问控制
来源：http://waz.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://jhz.yongpay.top

PHP:  public / protected / private
来源：http://zwl.yfazqb.com

JS:   #private 字段；其余公开
来源：http://mxb.tarul.cn

TS:   public / protected / private
来源：http://ehv.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://rlu.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xbs.shzxlz.cn

Ruby: public / protected / private
来源：http://zjo.epnwcf.com

C#:   public / protected / private / internal
来源：http://zjw.ctjpmb.com

[G11] getter / setter
来源：http://uhw.cashguo.top

Py:   @property 与 @x.setter
来源：http://lfv.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uae.sysykeji.top

JS:   get name() { return this._name; }
来源：http://rbg.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://kaz.fengsongda.top

Java: public String getName() { return name; }
来源：http://sdg.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dod.ctjpmb.com

Ruby: attr_accessor :name
来源：http://vfg.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://lvv.tian-w.cn

[G12] 对象转字符串
来源：http://gqa.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://ayn.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hdn.hesvh.cn

JS:   toString() { return this.name; }
来源：http://zrh.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://fez.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://iyb.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://zaf.fehbvm.com

Ruby: def to_s; @name; end
来源：http://kbw.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://ahz.shuidangran.top

[G13] 判断对象类型
来源：http://pli.yj202588.top

Py:   isinstance(u, User)
来源：http://fia.mhx1999.top

PHP:  $u instanceof User
来源：http://wsp.ydzc1.top

JS:   u instanceof User
来源：http://jgd.yj202588.top

TS:   u instanceof User
来源：http://qtl.fanxiaobao.xyz

Java: u instanceof User
来源：http://ulx.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zqr.fzhhl.top

Ruby: u.is_a?(User)
来源：http://htd.hammf.cn

C#:   u is User
来源：http://ndl.yanxiufei.cn

[G14] 数据类 / record
来源：http://ejr.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hyt.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://krr.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://uhh.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://etm.uphjek.com

Java: record User(String name, int age) {}
来源：http://szk.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://fui.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fut.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://fcq.gotoacloud.top

[G15] 枚举
来源：http://ire.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tkw.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://gov.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://syy.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zdg.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://kgf.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uwi.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://frz.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lgu.meibo888.top

[G16] 对象转数组 / 字典
来源：http://gvg.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://apc.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://jtd.snrcjt.cn

JS:   Object.entries(obj)
来源：http://rrs.ydzc1.top

TS:   Object.entries(obj)
来源：http://ubz.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://les.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hcy.epnwcf.com

Ruby: obj.instance_variables
来源：http://pio.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://sbe.jinyuanbaomall.cn

================================================================================
来源：http://byc.jinghuilouyu.cn

H. 异常与错误处理
来源：http://xrc.zhoulong.xyz

================================================================================
来源：http://xls.yongpay.top

[H01] try / catch 基础
来源：http://rjy.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ohp.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yeq.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ptr.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fzx.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aer.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uig.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://shz.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lkb.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://nfm.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fbp.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://inc.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sij.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ytx.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ytu.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vpq.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://jsm.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://wjp.yj20258888.top

[H03] 主动抛出异常
来源：http://fhx.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://fqj.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://enf.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://iib.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://xmw.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mfv.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rqf.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://egp.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://rkf.zhijiandao.cn

[H04] 自定义异常类型
来源：http://tej.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://ims.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tdv.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://ztx.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://dso.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://baw.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dah.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://hvc.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://lgb.svipenyu.cn

[H05] 捕获特定类型
来源：http://awh.uphjek.com

Py:   except ValueError as e:
来源：http://muc.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ezl.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://lxw.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://qzx.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://abd.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://orh.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://jru.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yhm.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://zsx.pengpengdd.cyou


<!-- 参考信息 -->