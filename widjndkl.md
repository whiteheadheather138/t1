代发 wailian999

[F01] 读取整个文件
来源：http://lke.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bdp.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://snx.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dni.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qyr.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tvs.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.cheryme.top

Ruby: File.read("a.txt")
来源：http://rwx.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://pmt.haohaochexian.top

[F02] 逐行读取文件
来源：http://piz.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hse.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xqc.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://laj.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zvl.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mqi.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://scl.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kxi.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oxj.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://wiz.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rxm.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fag.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://okj.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lvh.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fdi.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rnp.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://idh.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://arz.chenjidiqi.icu

[F04] 追加写入文件
来源：http://slt.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cqs.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://end.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifw.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wfd.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cjx.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oxt.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nsw.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qkt.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://rye.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lsd.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://foj.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://xcq.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://nfy.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ump.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nrq.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://pms.cashguo.top

C#:   File.Exists("a.txt")
来源：http://dqu.ydzc1.top

[F06] 删除文件
来源：http://igr.xinyue.icu

Py:   os.remove("a.txt")
来源：http://ryp.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://mwj.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wvd.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tws.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ueb.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://ohg.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://fdj.yongpay.top

C#:   File.Delete("a.txt");
来源：http://boy.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://mbj.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zui.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dgq.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ddk.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gts.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ess.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jil.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yfw.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dlz.jinqigfzy.top

[F08] 遍历目录
来源：http://rho.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mjw.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pia.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://gtw.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://rry.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hoe.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://did.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://udf.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://dbb.cheryme.top

[F09] 获取文件大小
来源：http://kxm.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://xhs.vehdjk.com

PHP:  filesize("a.txt");
来源：http://eab.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://ldi.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://tro.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://rnc.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nye.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://xyt.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://tji.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://fhm.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ado.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lhl.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ggl.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://wtg.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rph.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gww.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tfj.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aof.svipenyu.cn

[F11] 复制与移动文件
来源：http://kqm.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wwt.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uub.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkk.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sor.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://chd.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://obe.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wjr.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kzr.yanxiufei.cn

[F12] CSV 读写
来源：http://iza.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ifn.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mjh.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://egu.iojbl.cn

TS:   // 同上
来源：http://sbb.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bxr.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kuw.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fpi.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ntt.jianghu66.top

================================================================================
来源：http://jgh.fzhhl.top

G. 面向对象
来源：http://eqk.zhoulong.xyz

================================================================================
来源：http://sdq.yangfankeji.com

[G01] 定义类
来源：http://oac.xylfe.cn

Py:   class User: pass
来源：http://jto.shanyushiyangkeji.top

PHP:  class User {}
来源：http://ejz.hnxiangtu.top

JS:   class User {}
来源：http://kfg.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://wyg.ctjpmb.com

Java: class User {}
来源：http://moc.daxiang520.top

Go:   type User struct { Name string }
来源：http://kla.fehbvm.com

Ruby: class User; end
来源：http://iyc.iojbl.cn

C#:   class User {}
来源：http://pjo.meibo888.top

[G02] 构造函数
来源：http://ude.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://qsi.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://fbj.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://oxk.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://jqs.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://qpz.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oce.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://sqm.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://lph.sxryk.cn

[G03] 实例属性
来源：http://alr.birdmap.top

Py:   self.name = "x"
来源：http://uyi.dianchejie.cn

PHP:  public string $name = "x";
来源：http://rny.jqgfzy.top

JS:   this.name = "x";
来源：http://umb.zdbjq.cn

TS:   name: string = "x";
来源：http://pxl.zhijiandao.cn

Java: private String name;
来源：http://jlv.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xyi.iojbl.cn

Ruby: @name = "x"
来源：http://fdt.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://baf.daria6918.cn

[G04] 定义方法
来源：http://bcj.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://toa.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fbi.smart0.xyz

JS:   greet() { return this.name; }
来源：http://hbc.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://nyn.guannengcc.top

Java: String greet() { return name; }
来源：http://ald.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iik.yj20258888.top

Ruby: def greet; @name; end
来源：http://enu.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://uie.gotoacloud.top

[G05] 继承
来源：http://tex.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://mar.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://riv.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://ezf.haohaochexian.top

TS:   class Admin extends User {}
来源：http://cri.kuanghao11.cn

Java: class Admin extends User {}
来源：http://vpf.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fcq.zycfv.cn

Ruby: class Admin < User; end
来源：http://hlk.xylfe.cn

C#:   class Admin : User {}
来源：http://aln.fengsongda.top

[G06] 重写方法
来源：http://rlr.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://haj.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hdl.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://qhb.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://udt.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://rmq.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hyz.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://cxc.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://pba.zhongyouzk.top

[G07] 调用父类方法
来源：http://usc.feifeiyinyue.top

Py:   super().greet()
来源：http://dcm.yongpay.top

PHP:  parent::greet();
来源：http://fee.daria6918.cn

JS:   super.greet();
来源：http://awj.shangyingyoupin.top

TS:   super.greet();
来源：http://mhw.yj20258888.top

Java: super.greet();
来源：http://bnl.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mww.zdqjudy.top

Ruby: super
来源：http://alp.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://xor.zhongyouzk.top

[G08] 静态方法与属性
来源：http://sqd.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://azz.xylfe.cn

PHP:  public static function f() {}
来源：http://ukk.bbcook.cn

JS:   static f() {}
来源：http://upv.zycfv.cn

TS:   static f(): void {}
来源：http://okg.epnwcf.com

Java: static void f() {}
来源：http://mjo.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://vbl.hesvh.cn

Ruby: def self.f; end
来源：http://qba.hywenlv.cn

C#:   public static void F() {}
来源：http://ibg.xinyue.icu

[G09] 接口 / 抽象类
来源：http://otg.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://fji.jianghu66.top

PHP:  interface Shape { public function area(): float; }
来源：http://yvn.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oal.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://oyu.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://nxs.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://qhk.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ptk.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://ype.fengsongda.top

[G10] 访问控制
来源：http://xng.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://dhe.nanxinkj.top

PHP:  public / protected / private
来源：http://sxq.birdmap.top

JS:   #private 字段；其余公开
来源：http://omy.yfazqb.com

TS:   public / protected / private
来源：http://lfl.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://mka.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://scd.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://lfo.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://cll.birdmap.top

[G11] getter / setter
来源：http://fod.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://hpn.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ndj.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://jul.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://rsp.daria6918.cn

Java: public String getName() { return name; }
来源：http://inm.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://mka.gotoacloud.top

Ruby: attr_accessor :name
来源：http://ivk.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://muz.pycfn.com

[G12] 对象转字符串
来源：http://tsh.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://emp.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://uix.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://bhv.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://isn.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://har.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tgu.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://igd.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://aql.guannengcc.top

[G13] 判断对象类型
来源：http://ced.hysaishi.cn

Py:   isinstance(u, User)
来源：http://ags.xziqi.cn

PHP:  $u instanceof User
来源：http://lvt.xziqi.cn

JS:   u instanceof User
来源：http://ywe.fzhhl.top

TS:   u instanceof User
来源：http://mvu.ydzc1.top

Java: u instanceof User
来源：http://hnx.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hgq.yj20258888.top

Ruby: u.is_a?(User)
来源：http://lmc.0kj1m.cn

C#:   u is User
来源：http://pfm.cdnleiting.top

[G14] 数据类 / record
来源：http://svk.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sfl.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://qqp.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://bns.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://yqa.bjfxy.top

Java: record User(String name, int age) {}
来源：http://hvb.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://ppg.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tcq.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://ztm.shzxlz.cn

[G15] 枚举
来源：http://evc.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tau.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pmw.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zzv.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qty.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://kdf.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kpk.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://hsw.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suu.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://grr.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gjb.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://knn.bbcook.cn

JS:   Object.entries(obj)
来源：http://pcs.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://owo.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qcw.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://avg.mhx1999.top

Ruby: obj.instance_variables
来源：http://pqs.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://jnf.fktsv.cn

================================================================================
来源：http://akx.kuanghao11.cn

H. 异常与错误处理
来源：http://znu.jqgfzy.top

================================================================================
来源：http://wyj.yj20258888.top

[H01] try / catch 基础
来源：http://kux.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gkw.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yai.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nii.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jnm.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://olo.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uzm.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://brj.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nhu.fktsv.cn

[H02] finally / ensure 收尾
来源：http://ycj.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://omr.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jbo.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ich.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://euf.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://wrs.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ucv.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nic.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://hlb.dashuyun.cn

[H03] 主动抛出异常
来源：http://rjw.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://uiv.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://anm.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://fjx.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://szr.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zwo.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iyy.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lae.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://yem.cucudq.cn

[H04] 自定义异常类型
来源：http://pvd.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://wib.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://huo.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://czu.tarul.cn

TS:   class MyError extends Error {}
来源：http://ptt.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://fsc.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jxp.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://cfr.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://vgm.zhijiandao.cn

[H05] 捕获特定类型
来源：http://azf.sxryk.cn

Py:   except ValueError as e:
来源：http://znn.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://owu.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://aap.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://jfp.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://ttm.yuanzhike.top


<!-- 参考信息 -->