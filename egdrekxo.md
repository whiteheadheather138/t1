代发 wailian999

[F01] 读取整个文件
来源：http://rcy.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cuw.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://rsw.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hbr.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ief.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://efj.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kmi.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://vxp.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://dte.cucudq.cn

[F02] 逐行读取文件
来源：http://pea.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tbz.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bpy.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xcq.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ykx.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gcf.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://soi.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kok.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gvs.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://ptb.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oly.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://szl.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xow.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cly.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pwm.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fxa.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://xdp.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yiv.sufxvd.cn

[F04] 追加写入文件
来源：http://hnu.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xdd.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oxz.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gqx.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zkk.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ekc.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ihz.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lqc.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mzr.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://ind.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://adw.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://hhr.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://krq.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://omm.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kvd.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bav.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://fzl.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://axm.yuxming.cn

[F06] 删除文件
来源：http://abn.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://btn.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://uav.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://sux.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://voz.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qlc.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://pug.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://eyn.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://app.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://wob.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ppz.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yao.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vxi.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nfn.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://imf.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ubv.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nfz.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ivu.yj20258888.top

[F08] 遍历目录
来源：http://lpd.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://emc.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dby.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://hqt.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://ped.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zkh.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vwr.yfazqb.com

Ruby: Dir.children("dir")
来源：http://flm.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://txs.yongpay.top

[F09] 获取文件大小
来源：http://xrp.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://gkq.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://lsb.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://qai.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://ybz.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qnf.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bsy.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://isa.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://dfx.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://zpv.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kid.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ucw.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lan.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://xki.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ark.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dyj.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://htl.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zuy.52xcode.cn

[F11] 复制与移动文件
来源：http://wnv.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://whe.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://llv.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rep.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgi.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xsz.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hxf.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mml.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nlv.ctjpmb.com

[F12] CSV 读写
来源：http://zbr.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zea.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iat.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lxp.tian-w.cn

TS:   // 同上
来源：http://anc.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cvc.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nun.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qsa.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://msh.hesvh.cn

================================================================================
来源：http://acc.yj20258888.top

G. 面向对象
来源：http://gbr.hesvh.cn

================================================================================
来源：http://pss.gotoacloud.top

[G01] 定义类
来源：http://ogx.dashuyun.cn

Py:   class User: pass
来源：http://jwa.vehdjk.com

PHP:  class User {}
来源：http://yew.9152youxi.cn

JS:   class User {}
来源：http://glz.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://uqw.ivvv.top

Java: class User {}
来源：http://sqp.jqgfzy.top

Go:   type User struct { Name string }
来源：http://lbf.jianghu66.top

Ruby: class User; end
来源：http://xzp.hesvh.cn

C#:   class User {}
来源：http://vtn.jlsjyb.cn

[G02] 构造函数
来源：http://yiv.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://lhc.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://giy.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://zsj.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://fzk.fanxiaobao.xyz

Java: User(String name) { this.name = name; }
来源：http://nre.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gpq.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://xrf.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://ocx.yonumen.top

[G03] 实例属性
来源：http://fip.yuxming.cn

Py:   self.name = "x"
来源：http://xzo.aizwys.cn

PHP:  public string $name = "x";
来源：http://gty.mhx1999.top

JS:   this.name = "x";
来源：http://acz.zhengqikj.top

TS:   name: string = "x";
来源：http://kdf.ppjwa.cn

Java: private String name;
来源：http://umo.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tfm.jinqigufen.top

Ruby: @name = "x"
来源：http://zjh.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://ybt.yj20258888.top

[G04] 定义方法
来源：http://jru.shuidangran.top

Py:   def greet(self): return self.name
来源：http://igf.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://osj.cucudq.cn

JS:   greet() { return this.name; }
来源：http://ujx.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://voi.dianchejie.cn

Java: String greet() { return name; }
来源：http://lqw.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pqu.zdbjq.cn

Ruby: def greet; @name; end
来源：http://pev.ybcxt.top

C#:   public string Greet() => Name;
来源：http://olx.tian-w.cn

[G05] 继承
来源：http://klb.guannengcc.top

Py:   class Admin(User): pass
来源：http://mda.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://qyt.jyoumei.cn

JS:   class Admin extends User {}
来源：http://mpk.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://okm.svipenyu.cn

Java: class Admin extends User {}
来源：http://fqm.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gqi.hfpthk.cn

Ruby: class Admin < User; end
来源：http://xbs.tianlin.xyz

C#:   class Admin : User {}
来源：http://zvy.tian-w.cn

[G06] 重写方法
来源：http://cmm.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://nzj.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nyc.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://wax.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://zcr.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://rzo.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yds.yonumen.top

Ruby: def greet; "admin"; end
来源：http://tvn.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://hre.9152youxi.cn

[G07] 调用父类方法
来源：http://dzp.yongpay.top

Py:   super().greet()
来源：http://khl.yangfankeji.com

PHP:  parent::greet();
来源：http://mnf.sufxvd.cn

JS:   super.greet();
来源：http://hoz.jlsjyb.cn

TS:   super.greet();
来源：http://upu.hfpthk.cn

Java: super.greet();
来源：http://efc.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vmd.daria6918.cn

Ruby: super
来源：http://twz.jlsjyb.cn

C#:   base.Greet();
来源：http://skh.daxiang520.top

[G08] 静态方法与属性
来源：http://mmg.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eqc.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://jmo.fengsongda.top

JS:   static f() {}
来源：http://kds.zdqjudy.top

TS:   static f(): void {}
来源：http://dmv.tarul.cn

Java: static void f() {}
来源：http://emq.bbcook.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ior.chenzaomai.com

Ruby: def self.f; end
来源：http://qht.gaohongyu789.top

C#:   public static void F() {}
来源：http://fbl.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://zsi.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://mqs.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://wzy.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fvu.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://amh.iojbl.cn

Java: interface Shape { double area(); }
来源：http://uow.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://are.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lvp.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://cxu.fanxiaobao.xyz

[G10] 访问控制
来源：http://zzf.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://kud.xylfe.cn

PHP:  public / protected / private
来源：http://fzq.birdmap.top

JS:   #private 字段；其余公开
来源：http://qbx.ppjwa.cn

TS:   public / protected / private
来源：http://fww.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://anq.iojbl.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nxp.redwolf501.top

Ruby: public / protected / private
来源：http://kbu.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://pee.smart0.xyz

[G11] getter / setter
来源：http://jom.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://pvr.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zqn.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://kcb.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://ops.yvedp.cn

Java: public String getName() { return name; }
来源：http://dwg.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nmr.chenlongwang.top

Ruby: attr_accessor :name
来源：http://xrg.c1oappe.top

C#:   public string Name { get; set; }
来源：http://vxs.shuidangran.top

[G12] 对象转字符串
来源：http://ogp.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://qpn.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zpa.uphjek.com

JS:   toString() { return this.name; }
来源：http://sdm.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://cty.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://cnx.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://mpt.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://isg.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://qrt.cdnleiting.top

[G13] 判断对象类型
来源：http://igw.ctjpmb.com

Py:   isinstance(u, User)
来源：http://xty.xuanzx.com

PHP:  $u instanceof User
来源：http://osp.quarkkingdee.top

JS:   u instanceof User
来源：http://hxv.guowangkeji.top

TS:   u instanceof User
来源：http://rul.jqgufenzy.top

Java: u instanceof User
来源：http://dju.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://igv.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://wnd.jqgufenzy.top

C#:   u is User
来源：http://mzw.feifeiyinyue.top

[G14] 数据类 / record
来源：http://pmq.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aqf.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://rca.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://exk.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://reb.meibo888.top

Java: record User(String name, int age) {}
来源：http://upu.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://ozp.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vay.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://rwz.ppjwa.cn

[G15] 枚举
来源：http://pgx.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mit.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lxd.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://onk.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uzj.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://orp.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qfh.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://mhh.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://izq.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://evb.sxryk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cee.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://xaf.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://idg.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://val.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zbg.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://sat.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://ddg.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://xbm.ydzc1.top

================================================================================
来源：http://blw.cqqwz.cn

H. 异常与错误处理
来源：http://zuo.hcnkem.com

================================================================================
来源：http://vrh.yangfankeji.com

[H01] try / catch 基础
来源：http://wfv.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eqg.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mcq.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gdj.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nne.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gih.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rss.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iaa.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eys.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://jdi.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://zyk.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ndh.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ikx.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bem.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://fev.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zkz.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pts.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://bvr.hywenlv.cn

[H03] 主动抛出异常
来源：http://ijf.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://jmq.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hbp.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://msg.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://mxa.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://koe.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gle.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ffv.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://exx.dashuyun.cn

[H04] 自定义异常类型
来源：http://yij.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://qfl.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://tdr.iojbl.cn

JS:   class MyError extends Error {}
来源：http://gtg.xinyue.icu

TS:   class MyError extends Error {}
来源：http://hnb.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://igy.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nhu.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://zkj.andypj.xyz

C#:   class MyException : Exception {}
来源：http://xmj.meibo888.top

[H05] 捕获特定类型
来源：http://ppo.quarkkingdee.top

Py:   except ValueError as e:
来源：http://tmc.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qdx.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://bje.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://joy.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://qkv.fanxiaobao.xyz


<!-- 参考信息 -->