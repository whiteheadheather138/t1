代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wju.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gpv.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nls.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://ato.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qmc.yj20258.top

================================================================================
来源：http://vfn.cdnleiting.top

F. 文件与目录
来源：http://pjq.feifeiyinyue.top

================================================================================
来源：http://lcr.jqgfzy.top

[F01] 读取整个文件
来源：http://uwd.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cms.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://fil.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sxp.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lkn.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qsr.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://guj.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://zsu.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://vas.chenzaomai.com

[F02] 逐行读取文件
来源：http://ldz.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bbt.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://obi.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://asg.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qxn.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vrq.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jxl.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cpf.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rbp.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://gnt.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bkq.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://uym.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lap.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jeo.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ovf.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gdk.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://ufa.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kif.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://ywd.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rwj.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dmg.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvr.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iok.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gfz.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://umy.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yox.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oee.redwolf501.top

[F05] 判断文件或目录是否存在
来源：http://wfl.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jja.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://ntz.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://vfu.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://ohx.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://afs.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iee.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://vth.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://jbc.0kj1m.cn

[F06] 删除文件
来源：http://yqh.cucudq.cn

Py:   os.remove("a.txt")
来源：http://nup.c1oappe.top

PHP:  unlink("a.txt");
来源：http://wuq.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://zfh.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://avw.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jei.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://akj.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://dqf.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://fzm.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://vxf.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mcu.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xdq.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ipj.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://shm.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ynp.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iua.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pga.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zip.zdqjudy.top

[F08] 遍历目录
来源：http://tbl.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ofg.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iye.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://cnh.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://kfr.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://shj.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uly.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://rnq.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://hfn.ehwqpu.com

[F09] 获取文件大小
来源：http://jhm.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://jub.daxiang520.top

PHP:  filesize("a.txt");
来源：http://azf.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://szm.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://hkj.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://vub.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zkn.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://avh.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://wpt.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://fts.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://opi.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vad.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qaw.yongpay.top

TS:   path.extname("a.txt")
来源：http://alv.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nto.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hmb.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wdu.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fig.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://uvf.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eit.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wbh.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wox.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zzt.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dbt.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://twl.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pet.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gjp.yuanzhike.top

[F12] CSV 读写
来源：http://egv.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lvr.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fvw.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://paq.nanxuanxn.top

TS:   // 同上
来源：http://sjp.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iun.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jgk.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xny.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vkr.ywan-chungtsiang.top

================================================================================
来源：http://wzr.c1oappe.top

G. 面向对象
来源：http://ppz.shzxlz.cn

================================================================================
来源：http://csv.shanyushiyangkeji.top

[G01] 定义类
来源：http://xin.shzxlz.cn

Py:   class User: pass
来源：http://yyi.tianlin.xyz

PHP:  class User {}
来源：http://hmb.gogol.net.cn

JS:   class User {}
来源：http://sdl.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://zyl.iojbl.cn

Java: class User {}
来源：http://hwo.xinyue.icu

Go:   type User struct { Name string }
来源：http://ywz.bjfxy.top

Ruby: class User; end
来源：http://wqf.shanyushiyangkeji.top

C#:   class User {}
来源：http://yqy.andypj.xyz

[G02] 构造函数
来源：http://opk.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://pvn.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://guu.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://gpp.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://gkw.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://frm.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zvf.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://vuy.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://lfs.fehbvm.com

[G03] 实例属性
来源：http://yke.yuanzhike.top

Py:   self.name = "x"
来源：http://lze.daria6918.cn

PHP:  public string $name = "x";
来源：http://vgx.ctjpmb.com

JS:   this.name = "x";
来源：http://jxm.aibaodan.cn

TS:   name: string = "x";
来源：http://lxd.jlsjyb.cn

Java: private String name;
来源：http://qcp.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jld.yanxiufei.cn

Ruby: @name = "x"
来源：http://jed.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://cuf.yongpay.top

[G04] 定义方法
来源：http://bwy.ydzc1.top

Py:   def greet(self): return self.name
来源：http://whw.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xka.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://oce.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://qkq.fktsv.cn

Java: String greet() { return name; }
来源：http://qjy.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sps.yfazqb.com

Ruby: def greet; @name; end
来源：http://ksh.sysykeji.top

C#:   public string Greet() => Name;
来源：http://wzw.aibaodan.cn

[G05] 继承
来源：http://aip.yfazqb.com

Py:   class Admin(User): pass
来源：http://isc.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://mtm.shzxlz.cn

JS:   class Admin extends User {}
来源：http://udv.sweek.top

TS:   class Admin extends User {}
来源：http://rvf.ybcxt.top

Java: class Admin extends User {}
来源：http://ppz.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mob.cheryme.top

Ruby: class Admin < User; end
来源：http://wjj.yj20258.top

C#:   class Admin : User {}
来源：http://pxs.xuanzx.com

[G06] 重写方法
来源：http://tsp.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://esu.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pob.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://pdz.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://gsa.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://wxc.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hru.cheryme.top

Ruby: def greet; "admin"; end
来源：http://ivo.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://gts.yj20258.top

[G07] 调用父类方法
来源：http://tjz.nanxinkj.top

Py:   super().greet()
来源：http://btl.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://ctd.yonumen.top

JS:   super.greet();
来源：http://iya.xziqi.cn

TS:   super.greet();
来源：http://ehe.zhongyouzk.top

Java: super.greet();
来源：http://srs.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rls.sweek.top

Ruby: super
来源：http://iev.jqgfzy.top

C#:   base.Greet();
来源：http://khz.xziqi.cn

[G08] 静态方法与属性
来源：http://vbx.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yof.cashguo.top

PHP:  public static function f() {}
来源：http://qjl.52xcode.cn

JS:   static f() {}
来源：http://oql.wangshuangyany.cn

TS:   static f(): void {}
来源：http://vfm.chenjidiqi.icu

Java: static void f() {}
来源：http://fax.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://klx.fengsongda.top

Ruby: def self.f; end
来源：http://vjt.vehdjk.com

C#:   public static void F() {}
来源：http://mhu.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://hvf.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://gla.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://spq.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wtk.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://omu.andypj.xyz

Java: interface Shape { double area(); }
来源：http://vkx.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://lyv.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gfz.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://osm.fehbvm.com

[G10] 访问控制
来源：http://sac.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://eoe.tanke756.top

PHP:  public / protected / private
来源：http://nmd.birdmap.top

JS:   #private 字段；其余公开
来源：http://qqu.shzxlz.cn

TS:   public / protected / private
来源：http://dck.cashguo.top

Java: public / protected / private / 默认包级
来源：http://oji.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://swj.c1oappe.top

Ruby: public / protected / private
来源：http://qsv.fktsv.cn

C#:   public / protected / private / internal
来源：http://iox.aibaodan.cn

[G11] getter / setter
来源：http://meb.xylfe.cn

Py:   @property 与 @x.setter
来源：http://xtj.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://maj.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://qiz.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://yqv.xziqi.cn

Java: public String getName() { return name; }
来源：http://ukj.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vsp.cqqwz.cn

Ruby: attr_accessor :name
来源：http://wgx.vehdjk.com

C#:   public string Name { get; set; }
来源：http://zhq.xuetiantiany.cn

[G12] 对象转字符串
来源：http://mpd.uphjek.com

Py:   def __str__(self): return self.name
来源：http://smd.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://yli.bjfxy.top

JS:   toString() { return this.name; }
来源：http://kiw.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://efg.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://abo.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://lov.sysykeji.top

Ruby: def to_s; @name; end
来源：http://lyz.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://kpo.jyoumei.cn

[G13] 判断对象类型
来源：http://rvh.daria6918.cn

Py:   isinstance(u, User)
来源：http://eiz.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://rnq.cdnleiting.top

JS:   u instanceof User
来源：http://hcx.yanxiufei.cn

TS:   u instanceof User
来源：http://bnb.ydzc1.top

Java: u instanceof User
来源：http://iju.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zkb.xylfe.cn

Ruby: u.is_a?(User)
来源：http://voz.yj202588.top

C#:   u is User
来源：http://adv.pengpengdd.cyou

[G14] 数据类 / record
来源：http://rig.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zwd.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://trf.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kgy.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://wpe.pycfn.com

Java: record User(String name, int age) {}
来源：http://aev.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://jew.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tfn.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://lls.jqgfzy.top

[G15] 枚举
来源：http://kzp.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xub.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qjr.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://egd.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mgy.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://ufw.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hni.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://wwj.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://stb.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://jvm.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uhi.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://bdi.jinqigufen.top

JS:   Object.entries(obj)
来源：http://zex.aizwys.cn

TS:   Object.entries(obj)
来源：http://lum.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rae.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xmw.tarul.cn

Ruby: obj.instance_variables
来源：http://rbb.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://lwi.shzxlz.cn

================================================================================
来源：http://nih.fzhhl.top

H. 异常与错误处理
来源：http://irb.sjlbkw.cn

================================================================================
来源：http://tgp.ydjk.org.cn

[H01] try / catch 基础
来源：http://ajz.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yik.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jnp.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aut.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bhr.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mls.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rwo.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kgg.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xvz.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://pbf.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://ekq.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cgm.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rcw.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://rsi.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://yog.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cxs.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://udh.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://arm.sxryk.cn

[H03] 主动抛出异常
来源：http://hqk.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://ueq.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://etr.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://zif.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://ezj.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://fhq.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bzd.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qcm.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://xby.shzxlz.cn

[H04] 自定义异常类型
来源：http://qdr.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://mif.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ict.redwolf501.top

JS:   class MyError extends Error {}
来源：http://mbx.bjfxy.top

TS:   class MyError extends Error {}
来源：http://hsh.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://lqu.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nwx.yanxiufei.cn


<!-- 参考信息 -->