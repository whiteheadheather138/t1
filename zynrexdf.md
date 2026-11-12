代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zsw.zdqjudy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vxz.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lky.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://gsu.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rgf.hnqzz.top

================================================================================
来源：http://zng.cdnleiting.top

F. 文件与目录
来源：http://bhv.fengsongda.top

================================================================================
来源：http://ksd.316326.xyz

[F01] 读取整个文件
来源：http://znt.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rvu.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://yxw.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cxw.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://izd.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xys.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sxr.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://gmz.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://fan.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://hqa.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hpd.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pir.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://joq.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vak.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dzl.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ryb.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bxc.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lyq.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://pos.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bpf.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cok.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nsx.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lkp.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ibk.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zep.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://tdd.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gng.dashuyun.cn

[F04] 追加写入文件
来源：http://rfn.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eaq.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ggo.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://biy.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bkx.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yly.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kof.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pvq.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tix.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://jnv.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kct.cheryme.top

PHP:  file_exists("a.txt");
来源：http://hkb.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://yxz.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://hux.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://rvo.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ely.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://pyc.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://qwb.jinyuanbaomall.cn

[F06] 删除文件
来源：http://xfe.fehbvm.com

Py:   os.remove("a.txt")
来源：http://dtn.uphjek.com

PHP:  unlink("a.txt");
来源：http://bzy.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://igl.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://hnr.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nhx.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://eld.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://hph.cashguo.top

C#:   File.Delete("a.txt");
来源：http://yom.nwbrower.top

[F07] 创建目录（含多级）
来源：http://ecc.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://akv.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dia.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pav.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dvq.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fbi.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ins.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ify.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://irf.tanke756.top

[F08] 遍历目录
来源：http://xej.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ebw.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xrx.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://mkg.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://wan.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://snj.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iii.sysykeji.top

Ruby: Dir.children("dir")
来源：http://bon.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://uts.daxiang520.top

[F09] 获取文件大小
来源：http://syl.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://ppu.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://tzh.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://let.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://vap.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://tkr.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lsw.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://nfq.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://abn.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://rvx.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://klk.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xlj.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://euv.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://dgj.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gdn.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nrw.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rls.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://awj.316326.xyz

[F11] 复制与移动文件
来源：http://och.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jcb.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jku.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dry.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fht.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://anl.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ztw.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hbn.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yxh.svipenyu.cn

[F12] CSV 读写
来源：http://ene.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ymx.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zpj.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://itw.xuetiantiany.cn

TS:   // 同上
来源：http://ios.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://edv.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xdj.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ysw.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iew.jyoumei.cn

================================================================================
来源：http://mva.gaohongyu789.top

G. 面向对象
来源：http://nbd.dianchejie.cn

================================================================================
来源：http://fqp.0kj1m.cn

[G01] 定义类
来源：http://kxc.chenlongwang.top

Py:   class User: pass
来源：http://gdx.nanxuanxn.top

PHP:  class User {}
来源：http://qbm.yongpay.top

JS:   class User {}
来源：http://iod.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://vbg.zhaomingkeji.xyz

Java: class User {}
来源：http://qap.redwolf501.top

Go:   type User struct { Name string }
来源：http://xii.zhiwuduotai.top

Ruby: class User; end
来源：http://fiy.cdnleiting.top

C#:   class User {}
来源：http://bbc.yuxming.cn

[G02] 构造函数
来源：http://nei.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://bsc.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://ulb.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://ubm.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://sah.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://hgb.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fou.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://sqe.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://rmd.zhiwuduotai.top

[G03] 实例属性
来源：http://fir.xylfe.cn

Py:   self.name = "x"
来源：http://ysu.zhengqikj.top

PHP:  public string $name = "x";
来源：http://sok.guowangkeji.top

JS:   this.name = "x";
来源：http://kzt.kuanghao11.cn

TS:   name: string = "x";
来源：http://abu.xuetiantiany.cn

Java: private String name;
来源：http://qpb.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ehn.redwolf501.top

Ruby: @name = "x"
来源：http://xiv.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://bno.zhiwuduotai.top

[G04] 定义方法
来源：http://ybs.pycfn.com

Py:   def greet(self): return self.name
来源：http://wnh.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://gdw.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://thh.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://shz.cashguo.top

Java: String greet() { return name; }
来源：http://tnq.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jvj.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://eut.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://fip.ehwqpu.com

[G05] 继承
来源：http://hmf.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://rrb.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://jfu.wangdashe.top

JS:   class Admin extends User {}
来源：http://xrv.0kj1m.cn

TS:   class Admin extends User {}
来源：http://xqz.xziqi.cn

Java: class Admin extends User {}
来源：http://nax.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wlr.guannengcc.top

Ruby: class Admin < User; end
来源：http://mku.ehwqpu.com

C#:   class Admin : User {}
来源：http://vmu.smart0.xyz

[G06] 重写方法
来源：http://yde.cashguo.top

Py:   def greet(self): return "admin"
来源：http://fbm.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://civ.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://sch.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://kfz.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://byg.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zqb.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://ure.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://yal.gotoacloud.top

[G07] 调用父类方法
来源：http://bxw.sxryk.cn

Py:   super().greet()
来源：http://xiq.hesvh.cn

PHP:  parent::greet();
来源：http://xys.hongshengwenyu.top

JS:   super.greet();
来源：http://jyu.pycfn.com

TS:   super.greet();
来源：http://tez.zycfv.cn

Java: super.greet();
来源：http://cqf.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mzp.shanyushiyangkeji.top

Ruby: super
来源：http://ndd.shanyushiyangtech.top

C#:   base.Greet();
来源：http://svm.aibaodan.cn

[G08] 静态方法与属性
来源：http://fxg.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fdn.fehbvm.com

PHP:  public static function f() {}
来源：http://bmu.zycfv.cn

JS:   static f() {}
来源：http://uqr.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://xcc.gzhubu.top

Java: static void f() {}
来源：http://zns.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nrz.316326.xyz

Ruby: def self.f; end
来源：http://akn.cashguo.top

C#:   public static void F() {}
来源：http://jih.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://uec.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://vhp.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://nuz.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iet.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://cpx.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://uyx.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://uea.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xkm.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://ipj.feifeiyinyue.top

[G10] 访问控制
来源：http://mvm.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://vrn.zhengqikj.top

PHP:  public / protected / private
来源：http://bvj.redwolf501.top

JS:   #private 字段；其余公开
来源：http://tsi.jiagoushi.top

TS:   public / protected / private
来源：http://nug.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://zet.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bbb.zhixingplan.top

Ruby: public / protected / private
来源：http://whs.c1oappe.top

C#:   public / protected / private / internal
来源：http://ubb.nwbrower.top

[G11] getter / setter
来源：http://uyh.yongpay.top

Py:   @property 与 @x.setter
来源：http://znr.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://kta.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://tqx.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://dnh.ydzc1.top

Java: public String getName() { return name; }
来源：http://trw.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yto.shuidangran.top

Ruby: attr_accessor :name
来源：http://gdd.yuxming.cn

C#:   public string Name { get; set; }
来源：http://tep.zdbjq.cn

[G12] 对象转字符串
来源：http://bzw.uphjek.com

Py:   def __str__(self): return self.name
来源：http://kez.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dgg.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://pwc.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://mht.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://izo.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://anq.fengsongda.top

Ruby: def to_s; @name; end
来源：http://hct.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://tog.yvedp.cn

[G13] 判断对象类型
来源：http://fzy.yuxming.cn

Py:   isinstance(u, User)
来源：http://nsy.daxiang520.top

PHP:  $u instanceof User
来源：http://rla.jiagoushi.top

JS:   u instanceof User
来源：http://wsd.cdnleiting.top

TS:   u instanceof User
来源：http://mul.jinqigfzy.top

Java: u instanceof User
来源：http://fyb.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tcl.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://ywf.havefunace.top

C#:   u is User
来源：http://pnk.tanke756.top

[G14] 数据类 / record
来源：http://zyz.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mvr.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://wpm.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vog.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://xcx.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://axa.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://ioh.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://flc.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://upr.hcnkem.com

[G15] 枚举
来源：http://ika.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qgb.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://pqo.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qbp.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hzb.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://pfb.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aai.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://eyk.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qut.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://ohy.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tik.316326.xyz

PHP:  get_object_vars($obj);
来源：http://rrd.jinqigufen.top

JS:   Object.entries(obj)
来源：http://nxr.dianchejie.cn

TS:   Object.entries(obj)
来源：http://cdh.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nmr.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://khs.smart0.xyz

Ruby: obj.instance_variables
来源：http://lgu.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://acx.sjlbkw.cn

================================================================================
来源：http://brx.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://obs.pycfn.com

================================================================================
来源：http://vlj.yfazqb.com

[H01] try / catch 基础
来源：http://vax.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gde.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pjo.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hpz.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://shp.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://onf.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pwg.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hmn.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lig.fehbvm.com

[H02] finally / ensure 收尾
来源：http://jzv.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://ywh.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iiw.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sze.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zhu.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://tzn.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lcq.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yvs.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rhu.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://jzf.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://eob.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vix.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://fjs.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://chj.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://blx.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yna.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zkr.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://dos.yongpay.top

[H04] 自定义异常类型
来源：http://xgh.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://kij.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://xle.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://jwf.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://tcv.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://ora.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gab.jinqigfzy.top


<!-- 参考信息 -->