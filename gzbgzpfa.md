代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cog.yonumen.top

================================================================================
来源：http://udi.daria6918.cn

F. 文件与目录
来源：http://rlm.aizwys.cn

================================================================================
来源：http://wjg.meibo888.top

[F01] 读取整个文件
来源：http://hjt.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zgn.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://jtx.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rso.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://izk.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bcd.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pdh.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://pou.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://wjz.hysaishi.cn

[F02] 逐行读取文件
来源：http://iqn.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zfj.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hqr.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kox.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iph.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://awy.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pml.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sul.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ywa.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://alm.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vkr.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gam.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jtn.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cbn.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tjc.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://how.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://wqi.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://otx.ydjk.org.cn

[F04] 追加写入文件
来源：http://pqm.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jsv.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://adm.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hbp.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pie.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xlf.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hyv.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hlk.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://yns.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ecy.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://fpp.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://vzw.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://xjv.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hyx.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hjm.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://cta.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://rte.jinqigufen.top

[F06] 删除文件
来源：http://rhz.tanke756.top

Py:   os.remove("a.txt")
来源：http://fvc.hammf.cn

PHP:  unlink("a.txt");
来源：http://frd.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://aka.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://gkf.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jmp.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://vzw.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://ayx.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://lhi.jianghu66.top

[F07] 创建目录（含多级）
来源：http://voa.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aml.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yjn.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hjj.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oae.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fmu.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uwv.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rtv.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ixl.haohaochexian.top

[F08] 遍历目录
来源：http://fqb.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://baq.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lmf.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://wwz.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://pzy.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ffc.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mwg.smart0.xyz

Ruby: Dir.children("dir")
来源：http://kin.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://gkr.haohaochexian.top

[F09] 获取文件大小
来源：http://ocg.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://cca.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://yzb.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://xna.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://uko.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hms.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iob.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://lal.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://axo.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://sul.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qks.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wpj.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mcd.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://kvc.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lec.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nvq.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wqs.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ckp.uphjek.com

[F11] 复制与移动文件
来源：http://mqk.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qkb.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oal.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzc.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fvx.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nsx.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gce.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dps.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nxu.gaohongyu789.top

[F12] CSV 读写
来源：http://dst.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fkm.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://soa.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uqo.ybcxt.top

TS:   // 同上
来源：http://bnx.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vlv.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ikd.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ppd.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://frk.epnwcf.com

================================================================================
来源：http://tfq.yanxiufei.cn

G. 面向对象
来源：http://pwp.uphjek.com

================================================================================
来源：http://gfy.shanyushiyangtech.top

[G01] 定义类
来源：http://lmk.nanxuanxn.top

Py:   class User: pass
来源：http://xiy.zhiwuduotai.top

PHP:  class User {}
来源：http://lzp.xylfe.cn

JS:   class User {}
来源：http://til.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://ifj.ybcxt.top

Java: class User {}
来源：http://val.birdmap.top

Go:   type User struct { Name string }
来源：http://clm.ivvv.top

Ruby: class User; end
来源：http://vpz.daria6918.cn

C#:   class User {}
来源：http://rbt.zdbjq.cn

[G02] 构造函数
来源：http://ybt.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://pcn.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://bof.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://ezd.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://gmy.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://enm.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vfd.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://izg.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://ygw.jinyuanbaomall.cn

[G03] 实例属性
来源：http://pll.xylfe.cn

Py:   self.name = "x"
来源：http://tcm.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://wke.gogol.net.cn

JS:   this.name = "x";
来源：http://jtf.fzhhl.top

TS:   name: string = "x";
来源：http://kyv.wangshuangyany.cn

Java: private String name;
来源：http://yum.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://los.nanxuanxn.top

Ruby: @name = "x"
来源：http://ugz.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://edk.smart0.xyz

[G04] 定义方法
来源：http://yfk.gzhubu.top

Py:   def greet(self): return self.name
来源：http://znz.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bpn.guannengcc.top

JS:   greet() { return this.name; }
来源：http://nzg.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://ypr.fktsv.cn

Java: String greet() { return name; }
来源：http://mwp.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://khj.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://rzp.fktsv.cn

C#:   public string Greet() => Name;
来源：http://jxy.hfpthk.cn

[G05] 继承
来源：http://bzj.dashuyun.cn

Py:   class Admin(User): pass
来源：http://lfs.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://kkl.havefunace.top

JS:   class Admin extends User {}
来源：http://afp.yueranfly.top

TS:   class Admin extends User {}
来源：http://omm.shuidangran.top

Java: class Admin extends User {}
来源：http://xpu.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cmd.yj20258.top

Ruby: class Admin < User; end
来源：http://yon.guowangkeji.top

C#:   class Admin : User {}
来源：http://tdn.aizwys.cn

[G06] 重写方法
来源：http://kbx.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://sxe.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dpr.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://dau.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://jet.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://nzu.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pfz.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://nrz.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://kxw.zhixingplan.top

[G07] 调用父类方法
来源：http://dqk.hesvh.cn

Py:   super().greet()
来源：http://rnl.havefunace.top

PHP:  parent::greet();
来源：http://nqi.zdbjq.cn

JS:   super.greet();
来源：http://qzc.ctjpmb.com

TS:   super.greet();
来源：http://ths.sysykeji.top

Java: super.greet();
来源：http://ody.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mie.chenzaomai.com

Ruby: super
来源：http://kpd.bbcook.cn

C#:   base.Greet();
来源：http://vlw.vqdsnc.cn

[G08] 静态方法与属性
来源：http://vjb.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://srg.316326.xyz

PHP:  public static function f() {}
来源：http://ssx.ctjpmb.com

JS:   static f() {}
来源：http://qqq.cheryme.top

TS:   static f(): void {}
来源：http://gpj.shangyingyoupin.top

Java: static void f() {}
来源：http://zqr.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://izr.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://hbq.yueranfly.top

C#:   public static void F() {}
来源：http://ddj.ydzc1.top

[G09] 接口 / 抽象类
来源：http://alh.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://hhq.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://eqw.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xhq.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://hea.316326.xyz

Java: interface Shape { double area(); }
来源：http://gbb.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://msh.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pue.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://sop.chenlongwang.top

[G10] 访问控制
来源：http://qdv.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://hcx.zhiwuduotai.top

PHP:  public / protected / private
来源：http://lyo.aizwys.cn

JS:   #private 字段；其余公开
来源：http://otu.shangyingyoupin.top

TS:   public / protected / private
来源：http://ahk.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://lah.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zfq.xuanzx.com

Ruby: public / protected / private
来源：http://zse.gzhubu.top

C#:   public / protected / private / internal
来源：http://dhp.iojbl.cn

[G11] getter / setter
来源：http://oyc.daxiang520.top

Py:   @property 与 @x.setter
来源：http://lmx.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ceh.yfazqb.com

JS:   get name() { return this._name; }
来源：http://vmz.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://vny.snrcjt.cn

Java: public String getName() { return name; }
来源：http://mrg.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pku.jianghu66.top

Ruby: attr_accessor :name
来源：http://nqf.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://dwx.zhixingplan.top

[G12] 对象转字符串
来源：http://obx.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://kdm.jqgfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tfc.hnqzz.top

JS:   toString() { return this.name; }
来源：http://zdf.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://otx.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://mmi.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://qgm.hammf.cn

Ruby: def to_s; @name; end
来源：http://vra.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://age.guowangkeji.top

[G13] 判断对象类型
来源：http://qqf.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://eou.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://fyl.52xcode.cn

JS:   u instanceof User
来源：http://ouh.zdqjudy.top

TS:   u instanceof User
来源：http://uqm.ydzc1.top

Java: u instanceof User
来源：http://cxp.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gnv.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://pxg.hywenlv.cn

C#:   u is User
来源：http://rlq.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://xss.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bed.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://fjo.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://ceo.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://rvx.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://adk.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://ugh.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cnc.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://qew.zdbjq.cn

[G15] 枚举
来源：http://rnh.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wyg.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tou.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pnv.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fyq.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://onj.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xfd.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://kut.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ymh.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://fex.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ihj.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://bqq.dianchejie.cn

JS:   Object.entries(obj)
来源：http://dci.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://ihb.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vei.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wmk.c1oappe.top

Ruby: obj.instance_variables
来源：http://odw.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://tif.smart0.xyz

================================================================================
来源：http://mtu.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://lmm.tarul.cn

================================================================================
来源：http://ywm.jlsjyb.cn

[H01] try / catch 基础
来源：http://brd.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://stc.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://foi.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://msz.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hog.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vco.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wvf.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lss.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ocf.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://lfr.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://zji.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://scc.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tcz.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xyk.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://lac.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://jjm.hysaishi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qpl.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mvk.zhengqikj.top

[H03] 主动抛出异常
来源：http://vmx.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://gwl.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iwo.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://kza.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://xug.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://abi.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pvw.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://npk.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://vdc.316326.xyz

[H04] 自定义异常类型
来源：http://yem.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://ozw.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://fdy.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://gua.mhx1999.top

TS:   class MyError extends Error {}
来源：http://nal.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://zrl.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ubc.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://zev.vehdjk.com

C#:   class MyException : Exception {}
来源：http://zkm.zdbjq.cn

[H05] 捕获特定类型
来源：http://kaq.chenzaomai.com

Py:   except ValueError as e:
来源：http://tmy.meibo888.top


<!-- 参考信息 -->