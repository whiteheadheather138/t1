代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://irz.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xdd.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://msd.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://rnc.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ici.zhaomingkeji.xyz

================================================================================
来源：http://agp.fehbvm.com

F. 文件与目录
来源：http://yxr.redwolf501.top

================================================================================
来源：http://yar.ivvv.top

[F01] 读取整个文件
来源：http://aqr.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kxl.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://awj.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://loa.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://syz.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cwl.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ajz.andypj.xyz

Ruby: File.read("a.txt")
来源：http://yna.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://jnn.jyoumei.cn

[F02] 逐行读取文件
来源：http://axm.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wtd.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vkn.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tpp.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://txj.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fhp.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wxy.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fjj.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nqa.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://djr.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sht.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mkm.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://koc.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sef.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://joy.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bvg.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://cmu.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ewn.zhijiandao.cn

[F04] 追加写入文件
来源：http://guh.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://klk.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fdb.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxy.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lub.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ukj.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nyw.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dgs.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oyd.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://mgk.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uvs.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://bla.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://qyi.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://svh.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jtu.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zuj.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://gdq.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://zbf.hysaishi.cn

[F06] 删除文件
来源：http://yjt.sweek.top

Py:   os.remove("a.txt")
来源：http://swm.yongpay.top

PHP:  unlink("a.txt");
来源：http://itu.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gil.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://pah.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iqr.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://yxx.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://pag.sweek.top

C#:   File.Delete("a.txt");
来源：http://znu.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://xpw.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zzt.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tfl.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vqk.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tjo.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rvr.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ypv.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vez.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gmx.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://zto.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://apm.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yob.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://opc.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://kly.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://stf.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pir.bjfxy.top

Ruby: Dir.children("dir")
来源：http://ayj.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://twb.meibo888.top

[F09] 获取文件大小
来源：http://byi.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://yzm.hesvh.cn

PHP:  filesize("a.txt");
来源：http://wlw.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://olr.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://gns.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jju.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pfc.yj20258.top

Ruby: File.size("a.txt")
来源：http://ktk.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qfg.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://now.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wbv.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://syy.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oxw.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://dld.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zbq.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ecq.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vgf.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cjt.hysaishi.cn

[F11] 复制与移动文件
来源：http://urt.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kwi.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bnm.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lqj.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gzq.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bhd.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vpf.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tkf.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rjq.0kj1m.cn

[F12] CSV 读写
来源：http://pkq.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wjx.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jqb.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pre.shanyushiyangtech.top

TS:   // 同上
来源：http://pcm.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ldd.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dcp.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ncl.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vkt.aibaodan.cn

================================================================================
来源：http://ywv.xylfe.cn

G. 面向对象
来源：http://lgv.yj20258888.top

================================================================================
来源：http://fxw.kuanghao11.cn

[G01] 定义类
来源：http://qtd.guannengcc.top

Py:   class User: pass
来源：http://nxe.xziqi.cn

PHP:  class User {}
来源：http://miy.cdnleiting.top

JS:   class User {}
来源：http://gzv.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://lxi.fanxiaobao.xyz

Java: class User {}
来源：http://fpb.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://cij.hfpthk.cn

Ruby: class User; end
来源：http://hkx.kuanghao11.cn

C#:   class User {}
来源：http://gur.zhongyouzk.top

[G02] 构造函数
来源：http://rvj.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://oto.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://iie.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://nxm.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://mne.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://iha.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wve.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://zpn.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://mel.zhixingplan.top

[G03] 实例属性
来源：http://udj.yfazqb.com

Py:   self.name = "x"
来源：http://lme.fktsv.cn

PHP:  public string $name = "x";
来源：http://gww.cashguo.top

JS:   this.name = "x";
来源：http://ftj.gaohongyu789.top

TS:   name: string = "x";
来源：http://vql.xylfe.cn

Java: private String name;
来源：http://ksf.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tbm.bjfxy.top

Ruby: @name = "x"
来源：http://fjx.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://gja.ivvv.top

[G04] 定义方法
来源：http://ozi.hcnkem.com

Py:   def greet(self): return self.name
来源：http://ktu.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qis.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://auq.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://mwb.jqgufenzy.top

Java: String greet() { return name; }
来源：http://wes.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://vxr.tanke756.top

Ruby: def greet; @name; end
来源：http://xsl.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://ijg.fzhhl.top

[G05] 继承
来源：http://oqn.zhixingplan.top

Py:   class Admin(User): pass
来源：http://vcm.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://iey.dashuyun.cn

JS:   class Admin extends User {}
来源：http://gug.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://rtb.yj202588.top

Java: class Admin extends User {}
来源：http://dhn.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lef.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://jfx.meibo888.top

C#:   class Admin : User {}
来源：http://hdd.sufxvd.cn

[G06] 重写方法
来源：http://xld.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://esr.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vrp.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://dka.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://iwi.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://inr.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ozm.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://nrg.sweek.top

C#:   public override string Greet() => "admin";
来源：http://cln.ehwqpu.com

[G07] 调用父类方法
来源：http://hwl.cqqwz.cn

Py:   super().greet()
来源：http://fte.hesvh.cn

PHP:  parent::greet();
来源：http://soq.c1oappe.top

JS:   super.greet();
来源：http://qgz.fehbvm.com

TS:   super.greet();
来源：http://vdd.ppjwa.cn

Java: super.greet();
来源：http://ipc.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fxm.shanyushiyangkeji.top

Ruby: super
来源：http://rty.tarul.cn

C#:   base.Greet();
来源：http://ldn.zhixingplan.top

[G08] 静态方法与属性
来源：http://pru.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qan.zhengqikj.top

PHP:  public static function f() {}
来源：http://ldu.fktsv.cn

JS:   static f() {}
来源：http://ecg.bjfxy.top

TS:   static f(): void {}
来源：http://fre.yj20258.top

Java: static void f() {}
来源：http://nnd.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gso.yj20258.top

Ruby: def self.f; end
来源：http://kgc.dianchejie.cn

C#:   public static void F() {}
来源：http://zkc.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://hty.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://jbk.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://pvh.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ukz.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://pnk.bbcook.cn

Java: interface Shape { double area(); }
来源：http://dqn.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://wjt.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yze.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://cej.shanyushiyangkeji.top

[G10] 访问控制
来源：http://mte.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://yhc.xuetiantiany.cn

PHP:  public / protected / private
来源：http://ein.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://yin.tian-w.cn

TS:   public / protected / private
来源：http://jlt.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://irk.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://bvq.xinyue.icu

Ruby: public / protected / private
来源：http://vod.birdmap.top

C#:   public / protected / private / internal
来源：http://igt.gzhubu.top

[G11] getter / setter
来源：http://wtw.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://fzj.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ewh.nwbrower.top

JS:   get name() { return this._name; }
来源：http://plb.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://zos.chenlongwang.top

Java: public String getName() { return name; }
来源：http://sps.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lgu.ydzc1.top

Ruby: attr_accessor :name
来源：http://cpe.yj20258.top

C#:   public string Name { get; set; }
来源：http://aao.svipenyu.cn

[G12] 对象转字符串
来源：http://zje.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://jzi.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ohs.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://rxl.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://hxd.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://qse.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nex.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://klv.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://xpd.yuanzhike.top

[G13] 判断对象类型
来源：http://efo.dianchejie.cn

Py:   isinstance(u, User)
来源：http://dtj.cheryme.top

PHP:  $u instanceof User
来源：http://mkk.jianghu66.top

JS:   u instanceof User
来源：http://akk.yfazqb.com

TS:   u instanceof User
来源：http://qlc.ydjk.org.cn

Java: u instanceof User
来源：http://cgd.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mov.52xcode.cn

Ruby: u.is_a?(User)
来源：http://fvj.vehdjk.com

C#:   u is User
来源：http://ndi.andypj.xyz

[G14] 数据类 / record
来源：http://huw.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wxo.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://rxb.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zkq.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://gyk.iojbl.cn

Java: record User(String name, int age) {}
来源：http://twv.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://aep.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://thw.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://ctz.shzxlz.cn

[G15] 枚举
来源：http://ais.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yxp.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://qxg.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fus.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gmf.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://mqg.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nyq.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://ike.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://meb.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://bqo.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://czp.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://wub.yonumen.top

JS:   Object.entries(obj)
来源：http://lyq.yj20258888.top

TS:   Object.entries(obj)
来源：http://amq.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yup.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://brw.wangdashe.top

Ruby: obj.instance_variables
来源：http://kuu.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://frt.nwbrower.top

================================================================================
来源：http://uop.ybcxt.top

H. 异常与错误处理
来源：http://umo.snrcjt.cn

================================================================================
来源：http://cgi.sjlbkw.cn

[H01] try / catch 基础
来源：http://ksm.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://akp.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sde.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sce.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mit.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kzw.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jrz.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bmm.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fso.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://siu.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://lgu.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ffj.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://moi.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jat.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bah.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vdx.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jov.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oar.jyoumei.cn

[H03] 主动抛出异常
来源：http://tqk.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://nwj.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://een.316326.xyz

JS:   throw new Error("错误信息");
来源：http://ilm.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://mwd.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://eob.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sds.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pkx.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://qfc.hammf.cn

[H04] 自定义异常类型
来源：http://mpx.cashguo.top

Py:   class MyError(Exception): pass
来源：http://roj.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dch.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://qwu.52xcode.cn

TS:   class MyError extends Error {}
来源：http://kvu.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://jxr.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vkc.0kj1m.cn


<!-- 参考信息 -->