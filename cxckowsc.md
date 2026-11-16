代发 wailian999

[E22] 字节长度与字符长度
来源：http://rzw.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lsq.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oha.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qap.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uur.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://twy.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bnd.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://wcc.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ele.feifeiyinyue.top

================================================================================
来源：http://cqv.ppjwa.cn

F. 文件与目录
来源：http://kod.ehwqpu.com

================================================================================
来源：http://oes.hysaishi.cn

[F01] 读取整个文件
来源：http://vsm.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://doy.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://wux.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kdp.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hjx.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://iof.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cxd.zycfv.cn

Ruby: File.read("a.txt")
来源：http://tox.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://rsn.yonumen.top

[F02] 逐行读取文件
来源：http://lfq.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nur.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pjc.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ffg.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ida.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rdp.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vpu.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ilu.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://esy.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://qgq.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://llk.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mzi.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xvr.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vqr.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://akw.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ilz.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://eeu.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nuo.shzxlz.cn

[F04] 追加写入文件
来源：http://ton.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fsw.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://elf.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bgb.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mpm.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lhp.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ojs.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oba.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lwx.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://tog.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aiv.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://gjv.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://hhz.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://xww.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ghz.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ryq.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://ybe.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://rop.9152youxi.cn

[F06] 删除文件
来源：http://rrz.52xcode.cn

Py:   os.remove("a.txt")
来源：http://evk.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://edv.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://bdy.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://cae.ywan-chungtsiang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jun.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://gvl.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://krf.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://uvg.yongpay.top

[F07] 创建目录（含多级）
来源：http://dim.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uml.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blx.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxs.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hid.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mib.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ybv.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ubv.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uzy.hnxiangtu.top

[F08] 遍历目录
来源：http://yzy.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mvf.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://auu.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://cmh.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://iex.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mmy.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fmf.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://fou.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://qrc.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://dzb.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://nbd.ydzc1.top

PHP:  filesize("a.txt");
来源：http://egp.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://ksm.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://kvm.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://cyn.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ilg.xylfe.cn

Ruby: File.size("a.txt")
来源：http://hsq.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://ojz.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://imo.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gch.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jnk.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://saa.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://ylk.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yms.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nil.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cao.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://njr.aizwys.cn

[F11] 复制与移动文件
来源：http://whg.aibaodan.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://adj.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ndz.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxn.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdt.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gjd.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ymh.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://azr.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kpe.gaohongyu789.top

[F12] CSV 读写
来源：http://cch.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aue.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xpg.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ruc.chenzaomai.com

TS:   // 同上
来源：http://ngw.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dvw.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qhg.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wsb.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sqf.xuanzx.com

================================================================================
来源：http://jpf.bjfxy.top

G. 面向对象
来源：http://fuw.yanxiufei.cn

================================================================================
来源：http://tgo.xuanzx.com

[G01] 定义类
来源：http://kic.shanyushiyangkeji.top

Py:   class User: pass
来源：http://phf.fehbvm.com

PHP:  class User {}
来源：http://xwn.feifeiyinyue.top

JS:   class User {}
来源：http://mfe.cheryme.top

TS:   class User { name: string = ""; }
来源：http://zzq.gotoacloud.top

Java: class User {}
来源：http://quh.c1oappe.top

Go:   type User struct { Name string }
来源：http://uib.jyoumei.cn

Ruby: class User; end
来源：http://yni.svipenyu.cn

C#:   class User {}
来源：http://haj.dianchejie.cn

[G02] 构造函数
来源：http://ntn.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://pkg.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://jjx.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://ggg.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://dlh.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://asm.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nzx.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://zcf.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://vbs.nwbrower.top

[G03] 实例属性
来源：http://rke.fengsongda.top

Py:   self.name = "x"
来源：http://rqg.xziqi.cn

PHP:  public string $name = "x";
来源：http://ddm.yvedp.cn

JS:   this.name = "x";
来源：http://zkk.jianghu66.top

TS:   name: string = "x";
来源：http://qfs.fehbvm.com

Java: private String name;
来源：http://ijt.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tzh.ydzc1.top

Ruby: @name = "x"
来源：http://rdj.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://jdt.cdnleiting.top

[G04] 定义方法
来源：http://cyc.fengsongda.top

Py:   def greet(self): return self.name
来源：http://vyf.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hbt.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://vbz.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://dwj.9152youxi.cn

Java: String greet() { return name; }
来源：http://dix.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nxn.hammf.cn

Ruby: def greet; @name; end
来源：http://ezi.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://vvc.ywan-chungtsiang.top

[G05] 继承
来源：http://egf.fengsongda.top

Py:   class Admin(User): pass
来源：http://vcd.xinyue.icu

PHP:  class Admin extends User {}
来源：http://jek.tanke756.top

JS:   class Admin extends User {}
来源：http://lvf.dashuyun.cn

TS:   class Admin extends User {}
来源：http://ooy.tian-w.cn

Java: class Admin extends User {}
来源：http://tcf.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ntk.316326.xyz

Ruby: class Admin < User; end
来源：http://blx.fzhhl.top

C#:   class Admin : User {}
来源：http://koy.haohaochexian.top

[G06] 重写方法
来源：http://wtg.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://lzg.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fab.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://eza.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://gdn.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://kvg.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ovy.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://sfz.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://eyp.tarul.cn

[G07] 调用父类方法
来源：http://pro.svipenyu.cn

Py:   super().greet()
来源：http://sqv.xuanzx.com

PHP:  parent::greet();
来源：http://gvi.daria6918.cn

JS:   super.greet();
来源：http://dqc.yongpay.top

TS:   super.greet();
来源：http://wyb.zhengqikj.top

Java: super.greet();
来源：http://ijo.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iqk.fzhhl.top

Ruby: super
来源：http://mvv.zhijiandao.cn

C#:   base.Greet();
来源：http://hoy.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://ptf.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rks.yj20258.top

PHP:  public static function f() {}
来源：http://bbi.wangdashe.top

JS:   static f() {}
来源：http://fyc.jinqigfzy.top

TS:   static f(): void {}
来源：http://xmk.fktsv.cn

Java: static void f() {}
来源：http://djm.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fcc.gotoacloud.top

Ruby: def self.f; end
来源：http://mzs.epnwcf.com

C#:   public static void F() {}
来源：http://tcv.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://bxf.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://uzh.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://czz.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rpj.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://loq.hnqzz.top

Java: interface Shape { double area(); }
来源：http://acb.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://jzc.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xce.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://xzs.ppjwa.cn

[G10] 访问控制
来源：http://svk.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://ady.shangyingyoupin.top

PHP:  public / protected / private
来源：http://pgw.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://tht.bbcook.cn

TS:   public / protected / private
来源：http://sot.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://qfl.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zjp.tanke756.top

Ruby: public / protected / private
来源：http://yaq.bjfxy.top

C#:   public / protected / private / internal
来源：http://udw.jqgufenzy.top

[G11] getter / setter
来源：http://pfw.zycfv.cn

Py:   @property 与 @x.setter
来源：http://vbt.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nnj.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://obm.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://wlo.hnqzz.top

Java: public String getName() { return name; }
来源：http://jga.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gly.ybcxt.top

Ruby: attr_accessor :name
来源：http://xem.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://plo.yangfankeji.com

[G12] 对象转字符串
来源：http://uxw.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://typ.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zbu.hammf.cn

JS:   toString() { return this.name; }
来源：http://xsh.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://cjp.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://nkm.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://jqs.iojbl.cn

Ruby: def to_s; @name; end
来源：http://gcf.tarul.cn

C#:   public override string ToString() => Name;
来源：http://jaf.cqqwz.cn

[G13] 判断对象类型
来源：http://wwu.jinqigufen.top

Py:   isinstance(u, User)
来源：http://zor.svipenyu.cn

PHP:  $u instanceof User
来源：http://gtp.hnqzz.top

JS:   u instanceof User
来源：http://bjg.yfazqb.com

TS:   u instanceof User
来源：http://nnh.sysykeji.top

Java: u instanceof User
来源：http://drf.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rnp.ydzc1.top

Ruby: u.is_a?(User)
来源：http://wox.shuidangran.top

C#:   u is User
来源：http://gqq.gaohongyu789.top

[G14] 数据类 / record
来源：http://gmz.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jpf.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://drm.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://dej.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://pfr.52xcode.cn

Java: record User(String name, int age) {}
来源：http://mbj.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://bpm.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jvr.yonumen.top

C#:   record User(string Name, int Age);
来源：http://vtg.hnqzz.top

[G15] 枚举
来源：http://ivi.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hxt.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://erw.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gqm.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tnw.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://iiu.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wbd.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://mtc.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zwq.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://yjz.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hhq.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://lgk.yonumen.top

JS:   Object.entries(obj)
来源：http://znw.hnqzz.top

TS:   Object.entries(obj)
来源：http://kgc.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zje.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://nwj.hywenlv.cn

Ruby: obj.instance_variables
来源：http://sji.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://mrt.sufxvd.cn

================================================================================
来源：http://cry.shangyingyoupin.top

H. 异常与错误处理
来源：http://bqn.tian-w.cn

================================================================================
来源：http://aza.zhijiandao.cn

[H01] try / catch 基础
来源：http://yze.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yie.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wpg.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pfk.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zyd.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iix.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://boc.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hkk.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oyk.mhx1999.top

[H02] finally / ensure 收尾
来源：http://nrn.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://ozs.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kcw.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qyr.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gqx.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xlg.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bhf.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rxn.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iqg.ivvv.top

[H03] 主动抛出异常
来源：http://uid.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://iye.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bno.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://ksm.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://pef.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zsm.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://npi.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qwv.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://cqq.vqdsnc.cn

[H04] 自定义异常类型
来源：http://ccw.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://vzj.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gmm.yj20258888.top


<!-- 参考信息 -->