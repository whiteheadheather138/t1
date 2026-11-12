代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tam.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wzy.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rml.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ldd.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wpr.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vag.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://yes.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lru.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ijv.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cbf.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gku.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wct.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dju.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://vcf.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ibi.pengpengdd.cyou

[F04] 追加写入文件
来源：http://csh.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://diz.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rtx.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://foc.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rie.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://znp.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bod.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zaw.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iqy.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://tar.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kcl.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://rbq.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://feg.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://xpn.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://swp.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bes.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://ugz.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://uhf.tarul.cn

[F06] 删除文件
来源：http://hka.yfazqb.com

Py:   os.remove("a.txt")
来源：http://rij.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://hrp.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hpl.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zsn.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://veq.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://uvf.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://ugh.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://ywl.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://ilf.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qyg.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ube.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://haz.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bws.epnwcf.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ygd.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://trk.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wiu.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kty.hnxiangtu.top

[F08] 遍历目录
来源：http://krf.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eyo.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kvt.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://wdn.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://ryb.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xps.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hov.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://wtz.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://jwl.xylfe.cn

[F09] 获取文件大小
来源：http://yak.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://zwx.hcnkem.com

PHP:  filesize("a.txt");
来源：http://zii.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://gtm.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://pyu.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://end.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nfm.aizwys.cn

Ruby: File.size("a.txt")
来源：http://tor.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://uux.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://uhj.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rbn.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dvq.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://man.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://fip.yfazqb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tll.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://auz.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ins.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ejf.hammf.cn

[F11] 复制与移动文件
来源：http://jdq.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qef.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wqb.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tmn.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hbz.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ppi.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dfd.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://flz.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rky.gogol.net.cn

[F12] CSV 读写
来源：http://hjc.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ivt.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rso.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pok.daria6918.cn

TS:   // 同上
来源：http://hcd.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iwp.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xrh.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bpy.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zcp.316326.xyz

================================================================================
来源：http://dbo.daria6918.cn

G. 面向对象
来源：http://tny.shangyingyoupin.top

================================================================================
来源：http://asl.yj20258888.top

[G01] 定义类
来源：http://mbf.tianlin.xyz

Py:   class User: pass
来源：http://vgs.havefunace.top

PHP:  class User {}
来源：http://mwf.ybcxt.top

JS:   class User {}
来源：http://yrg.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://bod.cucudq.cn

Java: class User {}
来源：http://zte.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://qob.xuetiantiany.cn

Ruby: class User; end
来源：http://fou.shzxlz.cn

C#:   class User {}
来源：http://blm.shanyushiyangkeji.top

[G02] 构造函数
来源：http://hke.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://swh.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://eso.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://cai.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://hjp.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://rma.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sir.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://fmx.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://rhm.guannengcc.top

[G03] 实例属性
来源：http://cbi.sufxvd.cn

Py:   self.name = "x"
来源：http://djo.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://pgr.haohaochexian.top

JS:   this.name = "x";
来源：http://txy.bjfxy.top

TS:   name: string = "x";
来源：http://svp.52xcode.cn

Java: private String name;
来源：http://trt.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yqo.gotoacloud.top

Ruby: @name = "x"
来源：http://ohf.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://zxx.xuetiantiany.cn

[G04] 定义方法
来源：http://ebs.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://syw.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://oui.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://spj.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://byv.daxiang520.top

Java: String greet() { return name; }
来源：http://flf.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xdf.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://rqz.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://ofb.meibo888.top

[G05] 继承
来源：http://mmw.redwolf501.top

Py:   class Admin(User): pass
来源：http://oao.xuanzx.com

PHP:  class Admin extends User {}
来源：http://myz.smart0.xyz

JS:   class Admin extends User {}
来源：http://znh.hammf.cn

TS:   class Admin extends User {}
来源：http://tlj.zdbjq.cn

Java: class Admin extends User {}
来源：http://ybx.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rqk.andypj.xyz

Ruby: class Admin < User; end
来源：http://ins.nwbrower.top

C#:   class Admin : User {}
来源：http://nap.ivvv.top

[G06] 重写方法
来源：http://act.sweek.top

Py:   def greet(self): return "admin"
来源：http://hck.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ikx.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://gwl.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://gkr.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://jkz.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dcj.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://zuy.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://dif.jinqigfzy.top

[G07] 调用父类方法
来源：http://cwx.sjlbkw.cn

Py:   super().greet()
来源：http://xco.zhiwuduotai.top

PHP:  parent::greet();
来源：http://fky.tarul.cn

JS:   super.greet();
来源：http://xtm.yvedp.cn

TS:   super.greet();
来源：http://nwf.daria6918.cn

Java: super.greet();
来源：http://got.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kes.hnqzz.top

Ruby: super
来源：http://mte.hongshengwenyu.top

C#:   base.Greet();
来源：http://rzf.zhongyouzk.top

[G08] 静态方法与属性
来源：http://jqh.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://plp.xinyue.icu

PHP:  public static function f() {}
来源：http://ucm.gotoacloud.top

JS:   static f() {}
来源：http://lbh.sysykeji.top

TS:   static f(): void {}
来源：http://ffm.zhoulong.xyz

Java: static void f() {}
来源：http://xjj.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tnw.birdmap.top

Ruby: def self.f; end
来源：http://shq.gzhubu.top

C#:   public static void F() {}
来源：http://gzm.nwbrower.top

[G09] 接口 / 抽象类
来源：http://xmn.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://vut.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://unf.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lan.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://lqk.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://qhq.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://lkq.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vaa.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://coq.gogol.net.cn

[G10] 访问控制
来源：http://cnl.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://vpt.andypj.xyz

PHP:  public / protected / private
来源：http://ddk.yueranfly.top

JS:   #private 字段；其余公开
来源：http://dgo.ydzc1.top

TS:   public / protected / private
来源：http://zmj.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://dzi.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://mbp.fktsv.cn

Ruby: public / protected / private
来源：http://dwc.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://bvn.feifeiyinyue.top

[G11] getter / setter
来源：http://zkh.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://nds.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://czn.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://gyy.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://eai.cashguo.top

Java: public String getName() { return name; }
来源：http://pah.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sup.ctjpmb.com

Ruby: attr_accessor :name
来源：http://tuh.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://dln.vqdsnc.cn

[G12] 对象转字符串
来源：http://ncx.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://sbr.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tnp.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://xqv.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://edh.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://ksj.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ggb.yj20258.top

Ruby: def to_s; @name; end
来源：http://ufx.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://ljq.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://ovm.daxiang520.top

Py:   isinstance(u, User)
来源：http://ccc.nanxinkj.top

PHP:  $u instanceof User
来源：http://ryr.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://wxp.ivvv.top

TS:   u instanceof User
来源：http://ark.zhixingplan.top

Java: u instanceof User
来源：http://yuo.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvv.xziqi.cn

Ruby: u.is_a?(User)
来源：http://mpg.xylfe.cn

C#:   u is User
来源：http://nrm.yonumen.top

[G14] 数据类 / record
来源：http://npp.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mse.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://rem.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://mth.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://rzg.sxryk.cn

Java: record User(String name, int age) {}
来源：http://epg.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://tga.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yko.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://rcn.cqqwz.cn

[G15] 枚举
来源：http://sqx.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bzx.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dxa.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wqq.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vva.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://byq.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ive.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://atp.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yaa.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://tsv.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://occ.yj20258.top

PHP:  get_object_vars($obj);
来源：http://hhe.gotoacloud.top

JS:   Object.entries(obj)
来源：http://xtc.yj202588.top

TS:   Object.entries(obj)
来源：http://mas.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jih.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gdc.52xcode.cn

Ruby: obj.instance_variables
来源：http://qhe.haohaochexian.top

C#:   // 用反射或 System.Text.Json
来源：http://yrh.fzhhl.top

================================================================================
来源：http://pmi.gzhubu.top

H. 异常与错误处理
来源：http://ybt.hnxiangtu.top

================================================================================
来源：http://cdl.zhongyouzk.top

[H01] try / catch 基础
来源：http://epb.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rmg.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qxh.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ukn.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xxn.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uic.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jgw.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nmz.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jet.cashguo.top

[H02] finally / ensure 收尾
来源：http://ids.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://bjc.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jhe.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mvg.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xur.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://mmo.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zbc.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qne.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://afx.dashuyun.cn

[H03] 主动抛出异常
来源：http://oeh.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://qcq.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fgm.ivvv.top

JS:   throw new Error("错误信息");
来源：http://uzd.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://nom.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://irr.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://btj.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hfz.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://xgd.dianchejie.cn

[H04] 自定义异常类型
来源：http://ipg.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://rrc.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://vzq.yj20258.top

JS:   class MyError extends Error {}
来源：http://ypb.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://hwn.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://gco.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kze.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://vur.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://kgw.yueranfly.top

[H05] 捕获特定类型
来源：http://yde.316326.xyz

Py:   except ValueError as e:
来源：http://ndg.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aoe.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://vme.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://fvw.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://myf.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ual.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://wva.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://goz.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://arx.c1oappe.top

Py:   value = d.get("k") or default
来源：http://rcc.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://did.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://tvy.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://msh.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jys.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ggi.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://zac.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://teu.nwbrower.top


<!-- 参考信息 -->