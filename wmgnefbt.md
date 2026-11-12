代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://luo.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qzb.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fma.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://wqw.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://abw.guannengcc.top

================================================================================
来源：http://wdz.jqgfzy.top

F. 文件与目录
来源：http://afv.shzxlz.cn

================================================================================
来源：http://kjb.jinqigfzy.top

[F01] 读取整个文件
来源：http://pkm.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rok.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://brh.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rrl.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yyc.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cph.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hws.xylfe.cn

Ruby: File.read("a.txt")
来源：http://wlf.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://jtr.chenzaomai.com

[F02] 逐行读取文件
来源：http://tbh.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mxt.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eay.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://syb.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zyx.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qeb.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dak.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rgn.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wvc.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://cma.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dhj.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wnj.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hxn.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfb.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gnw.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fye.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://wfa.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jei.hnxiangtu.top

[F04] 追加写入文件
来源：http://aer.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dnj.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://max.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mky.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwo.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xst.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tqs.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://meo.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uvw.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://ajd.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zre.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://fta.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://xjf.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://ffh.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sad.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xop.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://hhp.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://dcw.0kj1m.cn

[F06] 删除文件
来源：http://yfc.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://njh.fehbvm.com

PHP:  unlink("a.txt");
来源：http://dah.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://cks.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fuz.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ggh.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://jos.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://frm.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://wla.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://mmz.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dih.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zhh.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kyg.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvq.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vcv.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wkh.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wkv.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tbo.fehbvm.com

[F08] 遍历目录
来源：http://vwd.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lpq.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jlv.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://bhq.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://wav.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fpg.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jmd.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://jyu.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://jao.aibaodan.cn

[F09] 获取文件大小
来源：http://jle.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://vtb.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://iqi.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://qiy.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://wpm.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://wnq.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sxq.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://yje.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://cps.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://pvf.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://apd.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nny.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kvi.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://ubb.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbg.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rjc.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzf.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ogm.uphjek.com

[F11] 复制与移动文件
来源：http://jbo.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dpy.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wft.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lzw.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ydz.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bnp.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://umt.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ove.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dqh.jqgfzy.top

[F12] CSV 读写
来源：http://asi.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sca.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vdy.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gus.feifeiyinyue.top

TS:   // 同上
来源：http://bde.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ojz.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://duj.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ygo.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wur.jinqigufen.top

================================================================================
来源：http://deg.zdbjq.cn

G. 面向对象
来源：http://cba.zhengqikj.top

================================================================================
来源：http://djr.cheryme.top

[G01] 定义类
来源：http://xur.0kj1m.cn

Py:   class User: pass
来源：http://xcf.tian-w.cn

PHP:  class User {}
来源：http://nfo.zdqjudy.top

JS:   class User {}
来源：http://lrg.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://byg.gogol.net.cn

Java: class User {}
来源：http://vhu.hnqzz.top

Go:   type User struct { Name string }
来源：http://swn.bbcook.cn

Ruby: class User; end
来源：http://txi.vqdsnc.cn

C#:   class User {}
来源：http://ale.epnwcf.com

[G02] 构造函数
来源：http://xcb.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://fmo.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://get.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://bzr.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://nwr.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://nvt.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vum.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://elb.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://ebd.fktsv.cn

[G03] 实例属性
来源：http://lsv.jianghu66.top

Py:   self.name = "x"
来源：http://zkv.9152youxi.cn

PHP:  public string $name = "x";
来源：http://txv.jlsjyb.cn

JS:   this.name = "x";
来源：http://ygh.tanke756.top

TS:   name: string = "x";
来源：http://cyz.nwbrower.top

Java: private String name;
来源：http://hza.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jbt.hammf.cn

Ruby: @name = "x"
来源：http://zcb.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://fpm.xuetiantiany.cn

[G04] 定义方法
来源：http://ota.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://idb.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pju.bjfxy.top

JS:   greet() { return this.name; }
来源：http://rpm.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://cfi.tarul.cn

Java: String greet() { return name; }
来源：http://hel.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sbj.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://amx.mhx1999.top

C#:   public string Greet() => Name;
来源：http://qdv.kuanghao11.cn

[G05] 继承
来源：http://ddw.hcnkem.com

Py:   class Admin(User): pass
来源：http://cbz.iojbl.cn

PHP:  class Admin extends User {}
来源：http://gxe.yueranfly.top

JS:   class Admin extends User {}
来源：http://nmc.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://gbj.yuanzhike.top

Java: class Admin extends User {}
来源：http://fmr.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://llh.fzhhl.top

Ruby: class Admin < User; end
来源：http://obu.fehbvm.com

C#:   class Admin : User {}
来源：http://jwy.yfazqb.com

[G06] 重写方法
来源：http://vuf.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://baw.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tfp.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://mqw.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://nli.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://rpf.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kjx.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://wdt.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://wcm.jianghu66.top

[G07] 调用父类方法
来源：http://izb.52xcode.cn

Py:   super().greet()
来源：http://mqj.yuanzhike.top

PHP:  parent::greet();
来源：http://qcn.shanyushiyangtech.top

JS:   super.greet();
来源：http://taj.bbcook.cn

TS:   super.greet();
来源：http://ocg.0kj1m.cn

Java: super.greet();
来源：http://ubu.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ksb.wangdashe.top

Ruby: super
来源：http://ujz.hesvh.cn

C#:   base.Greet();
来源：http://ukq.gaohongyu789.top

[G08] 静态方法与属性
来源：http://uee.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dhn.quarkkingdee.top

PHP:  public static function f() {}
来源：http://wfr.jinqigfzy.top

JS:   static f() {}
来源：http://okx.xuanzx.com

TS:   static f(): void {}
来源：http://ark.gogol.net.cn

Java: static void f() {}
来源：http://fbt.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uim.hesvh.cn

Ruby: def self.f; end
来源：http://hlz.zhoulong.xyz

C#:   public static void F() {}
来源：http://stq.andypj.xyz

[G09] 接口 / 抽象类
来源：http://pqy.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://ikb.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://bmi.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wux.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://tvi.ivvv.top

Java: interface Shape { double area(); }
来源：http://ymy.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://nvu.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qle.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://ysl.svipenyu.cn

[G10] 访问控制
来源：http://yjt.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://ntn.bbcook.cn

PHP:  public / protected / private
来源：http://rbn.sweek.top

JS:   #private 字段；其余公开
来源：http://xgn.jiagoushi.top

TS:   public / protected / private
来源：http://btf.316326.xyz

Java: public / protected / private / 默认包级
来源：http://atw.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qqj.jinqigufen.top

Ruby: public / protected / private
来源：http://nuv.wangdashe.top

C#:   public / protected / private / internal
来源：http://dzt.tian-w.cn

[G11] getter / setter
来源：http://thc.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://qrr.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://blg.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://mgz.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://byf.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://ajw.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bbm.havefunace.top

Ruby: attr_accessor :name
来源：http://xux.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://xzf.9152youxi.cn

[G12] 对象转字符串
来源：http://bxq.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://jqz.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nsf.ybcxt.top

JS:   toString() { return this.name; }
来源：http://zkj.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://xht.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://xzi.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://qkh.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://nrb.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://wvs.yfazqb.com

[G13] 判断对象类型
来源：http://pck.ydzc1.top

Py:   isinstance(u, User)
来源：http://yyo.ivvv.top

PHP:  $u instanceof User
来源：http://rut.ybcxt.top

JS:   u instanceof User
来源：http://okv.yonumen.top

TS:   u instanceof User
来源：http://pgx.ivvv.top

Java: u instanceof User
来源：http://haz.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://zoi.xuanzx.com

Ruby: u.is_a?(User)
来源：http://qey.zhongyouzk.top

C#:   u is User
来源：http://woa.gogol.net.cn

[G14] 数据类 / record
来源：http://cae.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ija.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://pox.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://mrq.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://uvp.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://bfk.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://uri.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pts.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://nxe.yj202588.top

[G15] 枚举
来源：http://bwh.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ukx.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wtq.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ueu.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qgz.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://vvd.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gdq.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://lie.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rzb.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://jrf.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ers.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://ogu.hnqzz.top

JS:   Object.entries(obj)
来源：http://odt.yongpay.top

TS:   Object.entries(obj)
来源：http://zdf.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wci.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vff.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://dqc.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://txv.jinyuanbaomall.cn

================================================================================
来源：http://xxa.jyoumei.cn

H. 异常与错误处理
来源：http://amw.316326.xyz

================================================================================
来源：http://jpy.hcnkem.com

[H01] try / catch 基础
来源：http://wkn.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pvo.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwh.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yyu.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mfq.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ktr.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ogn.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kkd.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blj.zycfv.cn

[H02] finally / ensure 收尾
来源：http://qeg.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://ctd.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mdh.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://esd.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://hlb.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tja.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zgu.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xqc.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wwb.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://sjd.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://jsr.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nsl.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://lck.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://zad.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bao.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qlk.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mat.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://xek.daxiang520.top

[H04] 自定义异常类型
来源：http://fco.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://erk.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fyo.tanke756.top

JS:   class MyError extends Error {}
来源：http://iem.sxryk.cn

TS:   class MyError extends Error {}
来源：http://bkv.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://luf.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ian.feifeiyinyue.top


<!-- 参考信息 -->