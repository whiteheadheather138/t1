代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://kin.quarkkingdee.top

[F02] 逐行读取文件
来源：http://apj.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kop.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sua.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vst.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jks.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gbv.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lkj.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ffe.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oyu.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://rhv.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hdv.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sif.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ihc.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npn.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tqm.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mbc.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://umh.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vkd.daria6918.cn

[F04] 追加写入文件
来源：http://hre.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eoy.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mui.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://euv.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jne.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ajs.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zgh.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://icw.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bnl.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://lkt.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aos.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://cwn.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://lek.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://tyd.chenjidiqi.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://qvr.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hyt.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://oet.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://rvh.svipenyu.cn

[F06] 删除文件
来源：http://tgo.tarul.cn

Py:   os.remove("a.txt")
来源：http://izn.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://mmq.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://qmr.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kti.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lcz.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://qzv.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://xui.cheryme.top

C#:   File.Delete("a.txt");
来源：http://vbr.tian-w.cn

[F07] 创建目录（含多级）
来源：http://efl.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zco.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qll.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zql.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://avf.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gia.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fde.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pky.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ras.feifeiyinyue.top

[F08] 遍历目录
来源：http://qmr.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hks.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lgw.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://aib.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://jbw.epnwcf.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tcp.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bqn.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://erx.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://vua.zhiwuduotai.top

[F09] 获取文件大小
来源：http://yeh.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://efb.sysykeji.top

PHP:  filesize("a.txt");
来源：http://emu.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://svf.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://uqw.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://cpw.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://znr.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://ury.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://fog.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ikn.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zvk.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kld.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nke.iojbl.cn

TS:   path.extname("a.txt")
来源：http://xqm.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rie.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xnr.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iia.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://itu.hfpthk.cn

[F11] 复制与移动文件
来源：http://jwf.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fsb.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fmb.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dav.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xjm.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://woh.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xfh.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xth.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://urx.iojbl.cn

[F12] CSV 读写
来源：http://qrh.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sna.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ekp.jianghu66.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hhp.cheryme.top

TS:   // 同上
来源：http://npg.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://unj.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ixi.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://avh.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rfj.yanxiufei.cn

================================================================================
来源：http://gyb.smart0.xyz

G. 面向对象
来源：http://tuw.smart0.xyz

================================================================================
来源：http://oux.ybcxt.top

[G01] 定义类
来源：http://fua.xuetiantiany.cn

Py:   class User: pass
来源：http://ett.hesvh.cn

PHP:  class User {}
来源：http://stq.yangfankeji.com

JS:   class User {}
来源：http://acf.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://ess.yfazqb.com

Java: class User {}
来源：http://hag.sxryk.cn

Go:   type User struct { Name string }
来源：http://cmr.fengsongda.top

Ruby: class User; end
来源：http://orw.zhiwuduotai.top

C#:   class User {}
来源：http://kac.daxiang520.top

[G02] 构造函数
来源：http://rxt.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://onu.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://dvw.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://fyw.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://msh.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://cex.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://znt.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://oiq.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://aub.zhiwuduotai.top

[G03] 实例属性
来源：http://obm.sweek.top

Py:   self.name = "x"
来源：http://rej.yuanzhike.top

PHP:  public string $name = "x";
来源：http://gqp.sufxvd.cn

JS:   this.name = "x";
来源：http://vdb.zhoulong.xyz

TS:   name: string = "x";
来源：http://oqz.iojbl.cn

Java: private String name;
来源：http://mts.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tsg.zhengqikj.top

Ruby: @name = "x"
来源：http://qrh.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://cij.gogol.net.cn

[G04] 定义方法
来源：http://yoq.tarul.cn

Py:   def greet(self): return self.name
来源：http://wbw.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tsd.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://ixl.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://seu.bbcook.cn

Java: String greet() { return name; }
来源：http://baz.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ozx.guannengcc.top

Ruby: def greet; @name; end
来源：http://upt.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://fve.snrcjt.cn

[G05] 继承
来源：http://plx.gotoacloud.top

Py:   class Admin(User): pass
来源：http://aas.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://dgk.yj20258888.top

JS:   class Admin extends User {}
来源：http://lfv.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://nxd.shzxlz.cn

Java: class Admin extends User {}
来源：http://qoz.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fdo.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://hea.gotoacloud.top

C#:   class Admin : User {}
来源：http://kge.jyoumei.cn

[G06] 重写方法
来源：http://mjo.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://kce.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ucj.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://hkc.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://zgj.andypj.xyz

Java: @Override String greet() { return "admin"; }
来源：http://qdx.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ghy.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://ktt.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://uqj.hesvh.cn

[G07] 调用父类方法
来源：http://rlo.yanxiufei.cn

Py:   super().greet()
来源：http://ntk.dianchejie.cn

PHP:  parent::greet();
来源：http://qeh.hammf.cn

JS:   super.greet();
来源：http://xrt.zhiwuduotai.top

TS:   super.greet();
来源：http://qci.chenjidiqi.icu

Java: super.greet();
来源：http://pmi.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bmu.chenzaomai.com

Ruby: super
来源：http://psq.jinghuilouyu.cn

C#:   base.Greet();
来源：http://hhr.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://pbr.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sag.jyoumei.cn

PHP:  public static function f() {}
来源：http://kby.svipenyu.cn

JS:   static f() {}
来源：http://lup.hysaishi.cn

TS:   static f(): void {}
来源：http://ebt.yj20258.top

Java: static void f() {}
来源：http://qxn.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jhm.epnwcf.com

Ruby: def self.f; end
来源：http://rpz.cucudq.cn

C#:   public static void F() {}
来源：http://etp.iojbl.cn

[G09] 接口 / 抽象类
来源：http://dgc.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://dzo.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uub.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://eyb.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://zae.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://tnt.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://lbb.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gjo.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://bjr.xuanzx.com

[G10] 访问控制
来源：http://ssx.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://wbf.hysaishi.cn

PHP:  public / protected / private
来源：http://dah.yj20258.top

JS:   #private 字段；其余公开
来源：http://btc.52xcode.cn

TS:   public / protected / private
来源：http://xmy.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://nlp.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ybg.nanxinkj.top

Ruby: public / protected / private
来源：http://cod.yj202588.top

C#:   public / protected / private / internal
来源：http://orf.uphjek.com

[G11] getter / setter
来源：http://mgn.sweek.top

Py:   @property 与 @x.setter
来源：http://ndh.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qma.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://xzz.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://nnm.fengsongda.top

Java: public String getName() { return name; }
来源：http://qja.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rsb.hammf.cn

Ruby: attr_accessor :name
来源：http://edi.vehdjk.com

C#:   public string Name { get; set; }
来源：http://oov.wangdashe.top

[G12] 对象转字符串
来源：http://sxm.hammf.cn

Py:   def __str__(self): return self.name
来源：http://ntg.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ihh.meibo888.top

JS:   toString() { return this.name; }
来源：http://bmv.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://dqh.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://vkw.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gar.yonumen.top

Ruby: def to_s; @name; end
来源：http://wql.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://msb.jiagoushi.top

[G13] 判断对象类型
来源：http://ylm.shzxlz.cn

Py:   isinstance(u, User)
来源：http://zen.vqdsnc.cn

PHP:  $u instanceof User
来源：http://wyl.jianghu66.top

JS:   u instanceof User
来源：http://cad.chenlongwang.top

TS:   u instanceof User
来源：http://nug.tanke756.top

Java: u instanceof User
来源：http://rjj.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uxk.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://xbc.vqdsnc.cn

C#:   u is User
来源：http://idi.ydzc1.top

[G14] 数据类 / record
来源：http://vmu.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hkx.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://zvv.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://xfa.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://rut.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://xbb.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://mdj.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qin.jqgufenzy.top

C#:   record User(string Name, int Age);
来源：http://cpn.yueranfly.top

[G15] 枚举
来源：http://knl.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jct.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://izf.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ncd.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://svo.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://fgk.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tjz.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://yav.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gou.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://szn.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://shq.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://clf.sxryk.cn

JS:   Object.entries(obj)
来源：http://irt.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://jiv.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mqc.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xhn.yongpay.top

Ruby: obj.instance_variables
来源：http://jks.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://vfm.yj202588.top

================================================================================
来源：http://dsf.hcnkem.com

H. 异常与错误处理
来源：http://gcu.cheryme.top

================================================================================
来源：http://frq.yangfankeji.com

[H01] try / catch 基础
来源：http://ued.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ckk.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://spl.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tzw.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xtl.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aoo.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qhz.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lie.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nux.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://qit.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://kdo.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ohu.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://euw.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jht.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://ymi.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yxs.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://squ.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://gnf.cashguo.top

[H03] 主动抛出异常
来源：http://ims.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://udj.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yvr.uphjek.com

JS:   throw new Error("错误信息");
来源：http://qhn.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://zkl.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gqv.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qlj.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bil.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://idx.nanxinkj.top

[H04] 自定义异常类型
来源：http://iej.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://ule.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://zue.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://epl.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://dqr.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://lpr.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gad.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://ntk.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://mrf.meibo888.top

[H05] 捕获特定类型
来源：http://ixv.ppjwa.cn

Py:   except ValueError as e:
来源：http://dro.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rtp.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://sum.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://akq.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://wym.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rrk.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://flt.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cgk.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://one.xylfe.cn

Py:   value = d.get("k") or default
来源：http://ntl.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://vbz.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xtn.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://hfn.fzhhl.top


<!-- 参考信息 -->