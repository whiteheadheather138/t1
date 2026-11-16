代发 wailian999

[E22] 字节长度与字符长度
来源：http://pah.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jra.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://daa.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://thn.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uex.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bgw.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uzd.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://gwi.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bdb.gaohongyu789.top

================================================================================
来源：http://jda.tanke756.top

F. 文件与目录
来源：http://ffj.xuanzx.com

================================================================================
来源：http://sgz.sysykeji.top

[F01] 读取整个文件
来源：http://jby.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://feo.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://rwe.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jcw.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gsn.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eyi.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iwz.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://eda.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://tfm.hywenlv.cn

[F02] 逐行读取文件
来源：http://zmu.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ngd.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uxn.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://duw.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kbb.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eib.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hel.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cru.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iab.uphjek.com

[F03] 写入文件（覆盖）
来源：http://nju.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://stt.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hnj.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ytb.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://inb.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jbk.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xbs.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://poh.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jdq.snrcjt.cn

[F04] 追加写入文件
来源：http://amc.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gos.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jjh.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fcb.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qeh.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bsb.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nje.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://poo.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sfq.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://tff.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xma.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://nvu.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://cqj.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://esh.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lfw.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wpn.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://vie.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://djr.hesvh.cn

[F06] 删除文件
来源：http://sft.meibo888.top

Py:   os.remove("a.txt")
来源：http://tjd.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://pmq.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://lef.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://psd.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cye.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://znx.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://lvy.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://jtx.meibo888.top

[F07] 创建目录（含多级）
来源：http://mvh.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jtw.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cmh.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yfk.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqu.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vhp.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vum.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rdl.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jek.kuanghao11.cn

[F08] 遍历目录
来源：http://wnn.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zwq.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wzg.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://qlh.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://sub.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gwv.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jec.cashguo.top

Ruby: Dir.children("dir")
来源：http://cgj.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://wxs.c1oappe.top

[F09] 获取文件大小
来源：http://jdw.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://nks.vehdjk.com

PHP:  filesize("a.txt");
来源：http://ird.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://tnx.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://zvh.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://ekg.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zxd.uphjek.com

Ruby: File.size("a.txt")
来源：http://rfg.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://lai.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://ctm.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gjw.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uwv.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lfr.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://tyl.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbi.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cly.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ccm.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gwg.hesvh.cn

[F11] 复制与移动文件
来源：http://lft.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xtk.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tcd.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sjr.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tlj.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lqg.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zxc.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eoh.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bjt.pycfn.com

[F12] CSV 读写
来源：http://kub.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ybx.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dxz.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pvl.aizwys.cn

TS:   // 同上
来源：http://vav.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://doj.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mor.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rfl.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://riq.redwolf501.top

================================================================================
来源：http://uak.zhaomingkeji.xyz

G. 面向对象
来源：http://ele.fengsongda.top

================================================================================
来源：http://jzq.jianghu66.top

[G01] 定义类
来源：http://ufx.gotoacloud.top

Py:   class User: pass
来源：http://qzk.daxiang520.top

PHP:  class User {}
来源：http://iqu.ehwqpu.com

JS:   class User {}
来源：http://ayk.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://exy.andypj.xyz

Java: class User {}
来源：http://jit.zdqjudy.top

Go:   type User struct { Name string }
来源：http://nbg.ydzc1.top

Ruby: class User; end
来源：http://nit.xuetiantiany.cn

C#:   class User {}
来源：http://qwx.pengpengdd.cyou

[G02] 构造函数
来源：http://jzs.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ved.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://edc.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://joo.birdmap.top

TS:   constructor(public name: string) {}
来源：http://uhk.sweek.top

Java: User(String name) { this.name = name; }
来源：http://dtc.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://voq.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://jjh.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://syp.dashuyun.cn

[G03] 实例属性
来源：http://gbr.birdmap.top

Py:   self.name = "x"
来源：http://mwy.aibaodan.cn

PHP:  public string $name = "x";
来源：http://mwd.wangshuangyany.cn

JS:   this.name = "x";
来源：http://bfn.vqdsnc.cn

TS:   name: string = "x";
来源：http://pjc.fzhhl.top

Java: private String name;
来源：http://yda.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yqj.jqgufenzy.top

Ruby: @name = "x"
来源：http://lcz.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://nil.redwolf501.top

[G04] 定义方法
来源：http://uog.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://ltg.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qcw.yueranfly.top

JS:   greet() { return this.name; }
来源：http://cpo.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://wmj.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://frk.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vax.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://kdl.cucudq.cn

C#:   public string Greet() => Name;
来源：http://igb.gzhubu.top

[G05] 继承
来源：http://yaf.pycfn.com

Py:   class Admin(User): pass
来源：http://okz.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://vwy.dianchejie.cn

JS:   class Admin extends User {}
来源：http://zyi.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://xhp.sysykeji.top

Java: class Admin extends User {}
来源：http://mky.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://muv.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://jnq.gzhubu.top

C#:   class Admin : User {}
来源：http://qyy.hysaishi.cn

[G06] 重写方法
来源：http://peh.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://uil.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fgl.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://bag.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://wgj.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://lmq.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zvk.birdmap.top

Ruby: def greet; "admin"; end
来源：http://cml.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://njg.wangshuangyany.cn

[G07] 调用父类方法
来源：http://vzu.zhoulong.xyz

Py:   super().greet()
来源：http://ueb.hammf.cn

PHP:  parent::greet();
来源：http://idr.havefunace.top

JS:   super.greet();
来源：http://brf.tian-w.cn

TS:   super.greet();
来源：http://twp.chenlongwang.top

Java: super.greet();
来源：http://too.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ubs.tarul.cn

Ruby: super
来源：http://zsg.quarkkingdee.top

C#:   base.Greet();
来源：http://zgf.redwolf501.top

[G08] 静态方法与属性
来源：http://ynt.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ixt.yvedp.cn

PHP:  public static function f() {}
来源：http://bzd.shzxlz.cn

JS:   static f() {}
来源：http://yfs.jlsjyb.cn

TS:   static f(): void {}
来源：http://nbs.nanxinkj.top

Java: static void f() {}
来源：http://jkj.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://iko.jqgufenzy.top

Ruby: def self.f; end
来源：http://zzn.cqqwz.cn

C#:   public static void F() {}
来源：http://ghe.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://jov.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://qzt.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://txz.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ltg.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://meu.epnwcf.com

Java: interface Shape { double area(); }
来源：http://wtj.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://saz.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://thu.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://dbx.guannengcc.top

[G10] 访问控制
来源：http://nkc.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://idy.tian-w.cn

PHP:  public / protected / private
来源：http://ocf.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://lpv.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://ooo.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://hwz.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cys.shzxlz.cn

Ruby: public / protected / private
来源：http://kay.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://nql.cashguo.top

[G11] getter / setter
来源：http://srx.iojbl.cn

Py:   @property 与 @x.setter
来源：http://qnx.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ztt.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://vrc.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://lth.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://upl.jqgfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tuk.ehwqpu.com

Ruby: attr_accessor :name
来源：http://qyq.xylfe.cn

C#:   public string Name { get; set; }
来源：http://exp.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://jdi.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://jer.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://xhk.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://jky.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://vgu.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://teg.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://csi.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://jcb.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://vgf.gogol.net.cn

[G13] 判断对象类型
来源：http://sff.tian-w.cn

Py:   isinstance(u, User)
来源：http://ues.zhengqikj.top

PHP:  $u instanceof User
来源：http://daa.ydzc1.top

JS:   u instanceof User
来源：http://ghr.zdqjudy.top

TS:   u instanceof User
来源：http://osw.cdnleiting.top

Java: u instanceof User
来源：http://lmp.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hoj.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://lrd.haohaochexian.top

C#:   u is User
来源：http://cay.cucudq.cn

[G14] 数据类 / record
来源：http://zyj.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ehb.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://usg.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://pyw.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://sjl.ivvv.top

Java: record User(String name, int age) {}
来源：http://cuq.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://plt.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sul.birdmap.top

C#:   record User(string Name, int Age);
来源：http://xvf.sweek.top

[G15] 枚举
来源：http://eux.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vqr.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cam.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ynm.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jgu.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://ghs.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://abe.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://eyz.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://csi.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://fep.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bsc.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://jyf.ivvv.top

JS:   Object.entries(obj)
来源：http://zjr.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://vni.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nmd.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://cii.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://ncl.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://dox.yuanzhike.top

================================================================================
来源：http://ajk.quarkkingdee.top

H. 异常与错误处理
来源：http://uvt.yangfankeji.com

================================================================================
来源：http://pge.sjlbkw.cn

[H01] try / catch 基础
来源：http://fib.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dga.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ecl.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bqv.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hjs.jinqigufen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cgb.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jqx.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://glq.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jkr.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://uvy.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://sop.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ozb.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eue.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ioi.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://oeb.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pnk.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gaf.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nrh.wangdashe.top

[H03] 主动抛出异常
来源：http://yno.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://oja.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bnk.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://qey.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://bmu.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fax.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ykf.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tsm.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://opw.9152youxi.cn

[H04] 自定义异常类型
来源：http://jme.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://jdd.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sxx.fehbvm.com


<!-- 参考信息 -->