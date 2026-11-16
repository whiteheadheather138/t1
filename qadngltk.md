代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wiq.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://bwi.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ecm.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xdf.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://ktf.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dqj.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jmd.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vhm.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ozo.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qoc.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cpg.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://rcq.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mwt.feifeiyinyue.top

================================================================================
来源：http://elf.yj20258888.top

F. 文件与目录
来源：http://kmh.shzxlz.cn

================================================================================
来源：http://cjx.zycfv.cn

[F01] 读取整个文件
来源：http://prh.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gcl.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://ffw.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ano.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://beu.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hja.xingfuxueyuan.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dxd.birdmap.top

Ruby: File.read("a.txt")
来源：http://knf.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://maw.cheryme.top

[F02] 逐行读取文件
来源：http://udx.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ryv.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xdj.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihb.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vke.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dti.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xxl.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vni.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xmm.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://kdz.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tvw.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://exy.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fhl.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://len.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ytr.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mav.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://wwz.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hln.fehbvm.com

[F04] 追加写入文件
来源：http://tml.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zfl.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xgs.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://quj.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://syx.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zdq.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kcf.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://trx.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://etg.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://qqg.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://avh.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://sng.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://sjw.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://chy.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ays.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vmr.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://rmi.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://ebb.0kj1m.cn

[F06] 删除文件
来源：http://pep.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://ggx.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://rog.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uvb.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://rvj.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cne.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://xva.yongpay.top

Ruby: File.delete("a.txt")
来源：http://kvw.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://aym.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://gbc.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fiq.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://shw.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kfk.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lqi.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ajg.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://olo.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lhz.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jwp.hcnkem.com

[F08] 遍历目录
来源：http://lom.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xeu.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mhf.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://maa.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://wtk.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gph.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kgy.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://axb.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://tsc.shuidangran.top

[F09] 获取文件大小
来源：http://wky.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://xby.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://xwb.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://qqb.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://wvm.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ozk.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bwa.cheryme.top

Ruby: File.size("a.txt")
来源：http://mia.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://ehc.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://khv.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bjz.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://agg.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wxu.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://vtv.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iba.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ztr.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eog.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cmz.shuidangran.top

[F11] 复制与移动文件
来源：http://aot.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hje.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hag.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tyf.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzk.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pqq.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ddo.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bdp.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bfr.yanxiufei.cn

[F12] CSV 读写
来源：http://luj.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ltn.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gac.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jth.sweek.top

TS:   // 同上
来源：http://uqf.ppjwa.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zws.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://trc.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bxn.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lsw.jlsjyb.cn

================================================================================
来源：http://gje.jinqigfzy.top

G. 面向对象
来源：http://tpq.iojbl.cn

================================================================================
来源：http://qhr.yfazqb.com

[G01] 定义类
来源：http://yva.ppjwa.cn

Py:   class User: pass
来源：http://qfk.52xcode.cn

PHP:  class User {}
来源：http://pvn.yanxiufei.cn

JS:   class User {}
来源：http://jgs.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://hsh.xingfuxueyuan.xyz

Java: class User {}
来源：http://jwh.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://pdn.havefunace.top

Ruby: class User; end
来源：http://urp.birdmap.top

C#:   class User {}
来源：http://kqg.hnqzz.top

[G02] 构造函数
来源：http://rwf.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://ulk.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://ugr.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://skq.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://fvr.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://dtf.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wuy.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://poi.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://zat.xylfe.cn

[G03] 实例属性
来源：http://myr.yuanzhike.top

Py:   self.name = "x"
来源：http://rqx.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://wba.zdqjudy.top

JS:   this.name = "x";
来源：http://gox.shzxlz.cn

TS:   name: string = "x";
来源：http://uie.tanke756.top

Java: private String name;
来源：http://ojr.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uld.gaohongyu789.top

Ruby: @name = "x"
来源：http://laz.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://mfm.jyoumei.cn

[G04] 定义方法
来源：http://kxd.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://uhg.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dvu.iojbl.cn

JS:   greet() { return this.name; }
来源：http://pmg.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://ifl.nanxinkj.top

Java: String greet() { return name; }
来源：http://epv.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://xuu.yueranfly.top

Ruby: def greet; @name; end
来源：http://wxl.52xcode.cn

C#:   public string Greet() => Name;
来源：http://afl.ywan-chungtsiang.top

[G05] 继承
来源：http://dju.shuidangran.top

Py:   class Admin(User): pass
来源：http://vzb.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://vdq.shuidangran.top

JS:   class Admin extends User {}
来源：http://qrt.yangfankeji.com

TS:   class Admin extends User {}
来源：http://yxi.tarul.cn

Java: class Admin extends User {}
来源：http://krl.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zqt.birdmap.top

Ruby: class Admin < User; end
来源：http://pzs.jqgufenzy.top

C#:   class Admin : User {}
来源：http://kga.zhengqikj.top

[G06] 重写方法
来源：http://wga.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://siz.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://urz.yj20258.top

JS:   greet() { return "admin"; }
来源：http://gfb.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://kaw.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://wrs.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kav.pycfn.com

Ruby: def greet; "admin"; end
来源：http://rvl.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://sti.yj202588.top

[G07] 调用父类方法
来源：http://tcf.jqgufenzy.top

Py:   super().greet()
来源：http://wba.yuanzhike.top

PHP:  parent::greet();
来源：http://myi.daria6918.cn

JS:   super.greet();
来源：http://frz.jianghu66.top

TS:   super.greet();
来源：http://qub.chenjidiqi.icu

Java: super.greet();
来源：http://teh.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nxn.dashuyun.cn

Ruby: super
来源：http://szq.haohaochexian.top

C#:   base.Greet();
来源：http://mpc.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://yjv.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fma.bbcook.cn

PHP:  public static function f() {}
来源：http://hnq.cucudq.cn

JS:   static f() {}
来源：http://foh.0kj1m.cn

TS:   static f(): void {}
来源：http://xnt.nanxuanxn.top

Java: static void f() {}
来源：http://wcg.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://evo.hnqzz.top

Ruby: def self.f; end
来源：http://wba.yongpay.top

C#:   public static void F() {}
来源：http://tkq.hammf.cn

[G09] 接口 / 抽象类
来源：http://wdi.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://qfw.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://spt.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mjr.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://uxd.yj202588.top

Java: interface Shape { double area(); }
来源：http://ugo.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://dtf.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nyh.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://iya.ctjpmb.com

[G10] 访问控制
来源：http://nqo.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://gyw.mhx1999.top

PHP:  public / protected / private
来源：http://zyl.yuxming.cn

JS:   #private 字段；其余公开
来源：http://jek.tianlin.xyz

TS:   public / protected / private
来源：http://big.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://upy.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://xej.fktsv.cn

Ruby: public / protected / private
来源：http://vdn.hnqzz.top

C#:   public / protected / private / internal
来源：http://rvs.sysykeji.top

[G11] getter / setter
来源：http://dbu.havefunace.top

Py:   @property 与 @x.setter
来源：http://tkz.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uze.tarul.cn

JS:   get name() { return this._name; }
来源：http://hpi.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://kce.gogol.net.cn

Java: public String getName() { return name; }
来源：http://jva.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://vkp.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://ofe.ydzc1.top

C#:   public string Name { get; set; }
来源：http://alu.hcnkem.com

[G12] 对象转字符串
来源：http://ywc.yj202588.top

Py:   def __str__(self): return self.name
来源：http://lpz.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vco.fktsv.cn

JS:   toString() { return this.name; }
来源：http://ois.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://rjg.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://gpw.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://rzg.iojbl.cn

Ruby: def to_s; @name; end
来源：http://kzj.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://lnb.fzhhl.top

[G13] 判断对象类型
来源：http://bxv.nwbrower.top

Py:   isinstance(u, User)
来源：http://wdx.yonumen.top

PHP:  $u instanceof User
来源：http://tuy.ybcxt.top

JS:   u instanceof User
来源：http://thy.shanyushiyangtech.top

TS:   u instanceof User
来源：http://qto.jyoumei.cn

Java: u instanceof User
来源：http://pbt.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oqr.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://ses.iojbl.cn

C#:   u is User
来源：http://tnm.shzxlz.cn

[G14] 数据类 / record
来源：http://mtj.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://avb.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://hwd.iojbl.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gtb.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://tui.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://vjk.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://vjn.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bml.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://avp.jlsjyb.cn

[G15] 枚举
来源：http://sqy.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fzh.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wbb.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hgc.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lal.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://syb.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ppq.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://xpn.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gxf.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://hhx.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://azk.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://jfz.aizwys.cn

JS:   Object.entries(obj)
来源：http://ohw.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://hut.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gml.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mll.yuxming.cn

Ruby: obj.instance_variables
来源：http://lvk.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://ati.zhoulong.xyz

================================================================================
来源：http://noe.shanyushiyangtech.top

H. 异常与错误处理
来源：http://tyh.9152youxi.cn

================================================================================
来源：http://ovg.havefunace.top

[H01] try / catch 基础
来源：http://ssg.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://upx.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fmc.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hdj.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://saf.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sge.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vlj.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pej.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vib.yj20258888.top

[H02] finally / ensure 收尾
来源：http://ngw.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dsv.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hmu.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fce.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kfj.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://rqk.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uql.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mup.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nhb.zhixingplan.top

[H03] 主动抛出异常
来源：http://aff.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://pth.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wup.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://uvv.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://aiw.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uxj.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ecc.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://cqg.chenlongwang.top


<!-- 参考信息 -->