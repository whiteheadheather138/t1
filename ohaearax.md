代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pyk.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aat.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://myw.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://fkr.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ngo.sjlbkw.cn

================================================================================
来源：http://gyh.yuanzhike.top

F. 文件与目录
来源：http://sew.smart0.xyz

================================================================================
来源：http://nej.sysykeji.top

[F01] 读取整个文件
来源：http://poq.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rbz.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://btk.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://byu.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mvj.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ihw.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://olv.shuidangran.top

Ruby: File.read("a.txt")
来源：http://sev.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://sxt.sufxvd.cn

[F02] 逐行读取文件
来源：http://prf.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nzb.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rdd.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://alh.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzf.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nra.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yuh.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nfp.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://akg.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://xre.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sea.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cne.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hkk.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gde.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://moq.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oln.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://iih.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ntr.ctjpmb.com

[F04] 追加写入文件
来源：http://geu.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jbt.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://obx.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fhq.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://muf.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jup.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rge.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aaw.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bof.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://lkp.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hdw.yj20258.top

PHP:  file_exists("a.txt");
来源：http://qmp.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://icm.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://iqw.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qzh.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bex.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://col.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://gtz.svipenyu.cn

[F06] 删除文件
来源：http://poq.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://duq.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://jqr.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eug.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://kkq.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fev.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://fqi.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://yjb.yj20258.top

C#:   File.Delete("a.txt");
来源：http://eyd.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://vit.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eiv.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bvn.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aep.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvn.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vpe.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://akh.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tuy.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uke.yonumen.top

[F08] 遍历目录
来源：http://qey.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gua.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gqr.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://gac.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://hhm.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ttt.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wkv.yj202588.top

Ruby: Dir.children("dir")
来源：http://yun.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://dzv.cucudq.cn

[F09] 获取文件大小
来源：http://myr.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://gah.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://obt.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://yaf.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://eum.gzhubu.top

Java: Files.size(Path.of("a.txt"))
来源：http://qvk.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gha.meibo888.top

Ruby: File.size("a.txt")
来源：http://ybg.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://rdp.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://ntv.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cyb.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tsc.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jmv.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://ytz.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ayc.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ple.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nxz.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bgl.yj20258888.top

[F11] 复制与移动文件
来源：http://jwu.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://auf.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dbh.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://plr.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://apg.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lzi.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fca.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ldg.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://csc.sxryk.cn

[F12] CSV 读写
来源：http://ddk.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://klw.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://and.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ldy.zhengqikj.top

TS:   // 同上
来源：http://zno.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oks.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ltj.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iwl.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wdr.sufxvd.cn

================================================================================
来源：http://ezx.zhaomingkeji.xyz

G. 面向对象
来源：http://tqj.jyoumei.cn

================================================================================
来源：http://frj.hnqzz.top

[G01] 定义类
来源：http://idz.hesvh.cn

Py:   class User: pass
来源：http://dib.dianchejie.cn

PHP:  class User {}
来源：http://vxp.tian-w.cn

JS:   class User {}
来源：http://uua.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://oht.jinqigfzy.top

Java: class User {}
来源：http://hbs.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://nip.sxryk.cn

Ruby: class User; end
来源：http://mro.xingfuxueyuan.xyz

C#:   class User {}
来源：http://jdf.bjfxy.top

[G02] 构造函数
来源：http://cou.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://beh.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://wcv.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://kwk.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://gkj.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://yzw.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ndl.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://gzm.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://ykl.hnxiangtu.top

[G03] 实例属性
来源：http://iox.fktsv.cn

Py:   self.name = "x"
来源：http://kii.tianlin.xyz

PHP:  public string $name = "x";
来源：http://ixk.xziqi.cn

JS:   this.name = "x";
来源：http://wxo.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://liw.52xcode.cn

Java: private String name;
来源：http://fss.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gzn.hnqzz.top

Ruby: @name = "x"
来源：http://iuo.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://oso.ybcxt.top

[G04] 定义方法
来源：http://tlh.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://lcl.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sfh.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://tnl.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://usv.birdmap.top

Java: String greet() { return name; }
来源：http://qxu.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xcz.316326.xyz

Ruby: def greet; @name; end
来源：http://hli.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://bnr.hammf.cn

[G05] 继承
来源：http://iyb.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://ivx.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://wwd.ehwqpu.com

JS:   class Admin extends User {}
来源：http://hqb.hysaishi.cn

TS:   class Admin extends User {}
来源：http://cua.hfpthk.cn

Java: class Admin extends User {}
来源：http://mak.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://czv.tanke756.top

Ruby: class Admin < User; end
来源：http://jwz.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://tnn.yueranfly.top

[G06] 重写方法
来源：http://oth.0kj1m.cn

Py:   def greet(self): return "admin"
来源：http://vpd.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zdt.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://gjc.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://szl.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://fwd.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yxc.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://ilw.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://czu.hnqzz.top

[G07] 调用父类方法
来源：http://hnl.yonumen.top

Py:   super().greet()
来源：http://rfz.hnqzz.top

PHP:  parent::greet();
来源：http://cqy.xuanzx.com

JS:   super.greet();
来源：http://ebs.cheryme.top

TS:   super.greet();
来源：http://rkz.yfazqb.com

Java: super.greet();
来源：http://fvd.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nms.dashuyun.cn

Ruby: super
来源：http://zxy.nanxinkj.top

C#:   base.Greet();
来源：http://bhu.yuxming.cn

[G08] 静态方法与属性
来源：http://thz.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mrh.yueranfly.top

PHP:  public static function f() {}
来源：http://ctc.fehbvm.com

JS:   static f() {}
来源：http://lhd.zdqjudy.top

TS:   static f(): void {}
来源：http://gqk.tanke756.top

Java: static void f() {}
来源：http://unf.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tax.xuanzx.com

Ruby: def self.f; end
来源：http://vnd.haohaochexian.top

C#:   public static void F() {}
来源：http://rfq.havefunace.top

[G09] 接口 / 抽象类
来源：http://tkg.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ysr.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://djd.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vkh.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://sab.vehdjk.com

Java: interface Shape { double area(); }
来源：http://fmx.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://qms.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kfs.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://pgt.dianchejie.cn

[G10] 访问控制
来源：http://fhu.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://bml.chenlongwang.top

PHP:  public / protected / private
来源：http://ior.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://mpk.shuidangran.top

TS:   public / protected / private
来源：http://tmz.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://ksn.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://zsk.jianghu66.top

Ruby: public / protected / private
来源：http://agt.xylfe.cn

C#:   public / protected / private / internal
来源：http://hke.aibaodan.cn

[G11] getter / setter
来源：http://xts.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://nyn.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://slt.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://xeo.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://doh.hywenlv.cn

Java: public String getName() { return name; }
来源：http://zcv.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://drn.ybcxt.top

Ruby: attr_accessor :name
来源：http://hdh.yongpay.top

C#:   public string Name { get; set; }
来源：http://wqf.zhengqikj.top

[G12] 对象转字符串
来源：http://htt.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://mrp.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://uvw.xziqi.cn

JS:   toString() { return this.name; }
来源：http://yvs.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://mlp.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://yea.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gbd.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://jee.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://xpz.snrcjt.cn

[G13] 判断对象类型
来源：http://wrb.ivvv.top

Py:   isinstance(u, User)
来源：http://aie.cashguo.top

PHP:  $u instanceof User
来源：http://keq.tian-w.cn

JS:   u instanceof User
来源：http://nxu.tianlin.xyz

TS:   u instanceof User
来源：http://cjj.9152youxi.cn

Java: u instanceof User
来源：http://cae.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://blg.redwolf501.top

Ruby: u.is_a?(User)
来源：http://eri.nanxinkj.top

C#:   u is User
来源：http://flw.9152youxi.cn

[G14] 数据类 / record
来源：http://xwu.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tlu.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://bvy.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://ets.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://tnl.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://rqv.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://ylm.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pnu.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://wum.feifeiyinyue.top

[G15] 枚举
来源：http://pir.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jys.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xvd.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bzk.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fuq.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://bbo.chenlongwang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xyk.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://zsp.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sji.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://jjf.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ejv.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://szl.bbcook.cn

JS:   Object.entries(obj)
来源：http://rgc.shuidangran.top

TS:   Object.entries(obj)
来源：http://wsg.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nee.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://erg.hywenlv.cn

Ruby: obj.instance_variables
来源：http://lmi.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://jxo.hnqzz.top

================================================================================
来源：http://nke.ppjwa.cn

H. 异常与错误处理
来源：http://cbc.sweek.top

================================================================================
来源：http://myl.sxryk.cn

[H01] try / catch 基础
来源：http://jmv.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xbk.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gjb.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ecu.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yki.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cgx.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tjp.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://acu.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://amy.yuxming.cn

[H02] finally / ensure 收尾
来源：http://opi.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://ubl.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://lfk.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://obc.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lig.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nko.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rih.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jwd.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://zub.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://tnc.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://zvk.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gkp.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://hbr.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://kte.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xax.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://znd.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://vuq.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://nqw.zycfv.cn

[H04] 自定义异常类型
来源：http://stn.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://xwg.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://ach.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://pyc.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://cem.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://qme.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dkh.snrcjt.cn


<!-- 参考信息 -->