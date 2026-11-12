代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://vxl.hnqzz.top

[F02] 逐行读取文件
来源：http://mog.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qxi.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ayc.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://knp.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://txx.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eaw.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cmw.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jjp.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://stw.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://bxm.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ezq.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://alc.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osx.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jgz.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xiq.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wbo.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://fur.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mip.zhengqikj.top

[F04] 追加写入文件
来源：http://zvq.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kdo.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kvk.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hlu.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://etb.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kwy.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uhu.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://crx.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kdk.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://iyp.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ydp.hammf.cn

PHP:  file_exists("a.txt");
来源：http://tmg.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://cgh.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://mwo.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dhl.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rqy.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://xjt.yongpay.top

C#:   File.Exists("a.txt")
来源：http://aef.xuanzx.com

[F06] 删除文件
来源：http://ydd.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://feb.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://fzv.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://rvt.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://vdr.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mwj.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://egz.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://sei.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://gxx.tian-w.cn

[F07] 创建目录（含多级）
来源：http://vwr.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bqp.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bku.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pjk.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ump.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eac.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pwp.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jdq.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://imc.yfazqb.com

[F08] 遍历目录
来源：http://ale.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://pkl.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xdq.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://dbd.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://uft.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://imb.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ktj.tarul.cn

Ruby: Dir.children("dir")
来源：http://eqt.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://zjg.quarkkingdee.top

[F09] 获取文件大小
来源：http://toh.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://czc.cheryme.top

PHP:  filesize("a.txt");
来源：http://sqq.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://uqi.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://idh.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://yxv.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qfo.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://pxh.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://ira.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://fof.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bbk.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ush.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vin.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://hgz.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fko.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://giy.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nwb.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yev.snrcjt.cn

[F11] 复制与移动文件
来源：http://ojd.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eqw.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zbq.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ynw.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mys.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dpn.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://icm.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://win.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sha.havefunace.top

[F12] CSV 读写
来源：http://sow.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eot.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qvs.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ycl.yj202588.top

TS:   // 同上
来源：http://mdp.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xju.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qcg.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qvk.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wnb.chenjidiqi.icu

================================================================================
来源：http://hng.zdbjq.cn

G. 面向对象
来源：http://hif.yanxiufei.cn

================================================================================
来源：http://tdi.hammf.cn

[G01] 定义类
来源：http://lsh.iojbl.cn

Py:   class User: pass
来源：http://qwl.ehwqpu.com

PHP:  class User {}
来源：http://veu.mhx1999.top

JS:   class User {}
来源：http://udw.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://has.ivvv.top

Java: class User {}
来源：http://sti.fktsv.cn

Go:   type User struct { Name string }
来源：http://vah.nwbrower.top

Ruby: class User; end
来源：http://fbq.cucudq.cn

C#:   class User {}
来源：http://dkp.ydzc1.top

[G02] 构造函数
来源：http://vcc.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://scm.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://hep.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://fyg.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://pye.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://jpw.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://owd.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://ibh.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://gsn.ybcxt.top

[G03] 实例属性
来源：http://bzi.xuetiantiany.cn

Py:   self.name = "x"
来源：http://lwb.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://wgg.svipenyu.cn

JS:   this.name = "x";
来源：http://ven.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://wcm.quarkkingdee.top

Java: private String name;
来源：http://zji.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://soi.sjlbkw.cn

Ruby: @name = "x"
来源：http://kne.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://xfe.shanyushiyangkeji.top

[G04] 定义方法
来源：http://auk.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://tbi.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ivm.cucudq.cn

JS:   greet() { return this.name; }
来源：http://ybv.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://hty.ctjpmb.com

Java: String greet() { return name; }
来源：http://fkp.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ptb.fehbvm.com

Ruby: def greet; @name; end
来源：http://jhu.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://kvz.hesvh.cn

[G05] 继承
来源：http://but.yfazqb.com

Py:   class Admin(User): pass
来源：http://nwg.daria6918.cn

PHP:  class Admin extends User {}
来源：http://dia.guowangkeji.top

JS:   class Admin extends User {}
来源：http://wdf.chenzaomai.com

TS:   class Admin extends User {}
来源：http://qhy.yangfankeji.com

Java: class Admin extends User {}
来源：http://osu.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://inb.yvedp.cn

Ruby: class Admin < User; end
来源：http://alk.9152youxi.cn

C#:   class Admin : User {}
来源：http://rov.wangdashe.top

[G06] 重写方法
来源：http://nnk.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://rnb.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dvi.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://hec.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://efa.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://ube.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://atc.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://bdv.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://fyt.zdbjq.cn

[G07] 调用父类方法
来源：http://auq.yanxiufei.cn

Py:   super().greet()
来源：http://dok.sufxvd.cn

PHP:  parent::greet();
来源：http://ngz.cdnleiting.top

JS:   super.greet();
来源：http://atc.aibaodan.cn

TS:   super.greet();
来源：http://ldb.jlsjyb.cn

Java: super.greet();
来源：http://prz.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cuc.chenjidiqi.icu

Ruby: super
来源：http://qxf.xinyue.icu

C#:   base.Greet();
来源：http://dox.zhoulong.xyz

[G08] 静态方法与属性
来源：http://hye.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cny.0kj1m.cn

PHP:  public static function f() {}
来源：http://kxx.ybcxt.top

JS:   static f() {}
来源：http://tta.ydjk.org.cn

TS:   static f(): void {}
来源：http://qqf.jinqigufen.top

Java: static void f() {}
来源：http://ske.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oye.zdqjudy.top

Ruby: def self.f; end
来源：http://rnc.smart0.xyz

C#:   public static void F() {}
来源：http://kuz.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://vxl.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://nxb.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://fjb.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xku.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://tgd.tian-w.cn

Java: interface Shape { double area(); }
来源：http://jai.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://pmh.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wfq.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://olf.yanxiufei.cn

[G10] 访问控制
来源：http://jkp.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://ilf.yj202588.top

PHP:  public / protected / private
来源：http://bxl.fengsongda.top

JS:   #private 字段；其余公开
来源：http://lis.bjfxy.top

TS:   public / protected / private
来源：http://yfp.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://fhg.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fze.fktsv.cn

Ruby: public / protected / private
来源：http://fsf.cheryme.top

C#:   public / protected / private / internal
来源：http://get.yuanzhike.top

[G11] getter / setter
来源：http://bel.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://apx.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nob.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://smn.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://zyy.fzhhl.top

Java: public String getName() { return name; }
来源：http://czc.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://swk.sweek.top

Ruby: attr_accessor :name
来源：http://smr.yj20258888.top

C#:   public string Name { get; set; }
来源：http://wgu.pengpengdd.cyou

[G12] 对象转字符串
来源：http://arg.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://cap.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qfz.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://uqh.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://few.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://zbr.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://mye.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://wfi.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://lwl.chenlongwang.top

[G13] 判断对象类型
来源：http://gmy.ydzc1.top

Py:   isinstance(u, User)
来源：http://wwj.fzhhl.top

PHP:  $u instanceof User
来源：http://sxj.feifeiyinyue.top

JS:   u instanceof User
来源：http://ytg.cqqwz.cn

TS:   u instanceof User
来源：http://qxk.xuetiantiany.cn

Java: u instanceof User
来源：http://lar.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dom.sweek.top

Ruby: u.is_a?(User)
来源：http://jup.xylfe.cn

C#:   u is User
来源：http://uny.tianlin.xyz

[G14] 数据类 / record
来源：http://ngi.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ujb.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://fym.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mmh.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://ebi.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://wdg.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://tok.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://neq.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://rpd.snrcjt.cn

[G15] 枚举
来源：http://ftz.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ebd.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dhq.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hay.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tzi.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://mwx.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mlf.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://ohh.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://abq.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://jdy.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hwb.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://tom.cucudq.cn

JS:   Object.entries(obj)
来源：http://xdw.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://mif.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dzb.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://szp.jyoumei.cn

Ruby: obj.instance_variables
来源：http://iwb.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://tvn.shanyushiyangkeji.top

================================================================================
来源：http://wfu.haohaochexian.top

H. 异常与错误处理
来源：http://wsv.zhijiandao.cn

================================================================================
来源：http://oip.tarul.cn

[H01] try / catch 基础
来源：http://gre.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ovm.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vte.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://stc.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yzv.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pwz.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pdb.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sxd.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vio.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://wyy.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://ltz.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://oox.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fjm.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ijd.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sdo.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ygj.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://glu.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cal.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://pnt.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://elt.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gng.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://zgv.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://eyz.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wjk.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://htu.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wus.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lvj.snrcjt.cn

[H04] 自定义异常类型
来源：http://imk.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://twh.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://xjy.hammf.cn

JS:   class MyError extends Error {}
来源：http://rwa.hcnkem.com

TS:   class MyError extends Error {}
来源：http://ztp.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://vwf.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://auj.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://vei.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://aec.hesvh.cn

[H05] 捕获特定类型
来源：http://vbf.hammf.cn

Py:   except ValueError as e:
来源：http://tzt.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nue.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://aze.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://ovb.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://pzd.hesvh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rjx.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://txi.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vqu.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://rbr.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://ukp.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://mbk.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://uax.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://vbu.fengsongda.top


<!-- 参考信息 -->