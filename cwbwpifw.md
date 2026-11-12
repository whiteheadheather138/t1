代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mfd.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sqa.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rkd.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://rih.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cbo.ehwqpu.com

================================================================================
来源：http://jxr.hammf.cn

F. 文件与目录
来源：http://jtd.aizwys.cn

================================================================================
来源：http://yux.ppjwa.cn

[F01] 读取整个文件
来源：http://oye.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nlq.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://vom.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ycy.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bqb.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vxv.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://agc.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://vbx.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ecc.nanxinkj.top

[F02] 逐行读取文件
来源：http://npa.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uhy.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rmv.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yuk.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rhv.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kac.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ztx.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rfq.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wtm.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://lnu.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fjl.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tng.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://btq.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cwq.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vco.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tmn.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://sxi.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aus.chenlongwang.top

[F04] 追加写入文件
来源：http://hzf.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://izt.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xhd.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zbj.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ujb.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wol.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wnl.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qlo.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pjq.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://vuj.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iln.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://lwo.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://pog.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://utk.shuidangran.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sye.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lvb.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://trd.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://iiu.zhoulong.xyz

[F06] 删除文件
来源：http://zus.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://nzv.tarul.cn

PHP:  unlink("a.txt");
来源：http://edo.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://zwn.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mjw.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gnm.hammf.cn

Go:   os.Remove("a.txt")
来源：http://etr.yj20258.top

Ruby: File.delete("a.txt")
来源：http://cne.yj20258.top

C#:   File.Delete("a.txt");
来源：http://pdy.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://cym.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kix.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://frp.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ipw.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qml.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zwl.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://esb.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://okr.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://igh.quarkkingdee.top

[F08] 遍历目录
来源：http://kuv.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://gnx.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xxn.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://mwm.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://icw.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ugw.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bat.meibo888.top

Ruby: Dir.children("dir")
来源：http://skk.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://dfh.tian-w.cn

[F09] 获取文件大小
来源：http://llo.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://hln.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://qew.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://euu.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://iuv.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://jqg.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xvh.hnqzz.top

Ruby: File.size("a.txt")
来源：http://pdh.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://hew.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://jdx.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mnr.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kdu.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ann.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://jqm.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xnn.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wob.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://apn.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bjd.redwolf501.top

[F11] 复制与移动文件
来源：http://mdk.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lkq.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://buu.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://han.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://suy.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bgx.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jem.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rpc.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hgw.ctjpmb.com

[F12] CSV 读写
来源：http://ibl.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yll.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ogt.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sap.gotoacloud.top

TS:   // 同上
来源：http://spq.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bxv.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tny.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rxf.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://kvs.fengsongda.top

================================================================================
来源：http://apo.redwolf501.top

G. 面向对象
来源：http://yzj.yonumen.top

================================================================================
来源：http://xmt.hysaishi.cn

[G01] 定义类
来源：http://qfm.tanke756.top

Py:   class User: pass
来源：http://vas.hongshengwenyu.top

PHP:  class User {}
来源：http://qmn.sxryk.cn

JS:   class User {}
来源：http://klo.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://pfm.yuanzhike.top

Java: class User {}
来源：http://jwm.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://pxn.mhx1999.top

Ruby: class User; end
来源：http://ahi.jinqigfzy.top

C#:   class User {}
来源：http://imc.chenzaomai.com

[G02] 构造函数
来源：http://aaw.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://oao.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://nts.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://wes.yongpay.top

TS:   constructor(public name: string) {}
来源：http://eca.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://baq.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqr.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ixo.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://bxd.dashuyun.cn

[G03] 实例属性
来源：http://wqi.uphjek.com

Py:   self.name = "x"
来源：http://enz.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://iqd.gzhubu.top

JS:   this.name = "x";
来源：http://twz.andypj.xyz

TS:   name: string = "x";
来源：http://eat.jqgfzy.top

Java: private String name;
来源：http://cki.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xwt.sxryk.cn

Ruby: @name = "x"
来源：http://ktq.xylfe.cn

C#:   public string Name { get; set; } = "x";
来源：http://wgh.jinqigfzy.top

[G04] 定义方法
来源：http://lvj.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://qib.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lsk.smart0.xyz

JS:   greet() { return this.name; }
来源：http://bfh.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://faw.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://eaq.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://wsn.hnqzz.top

Ruby: def greet; @name; end
来源：http://mee.andypj.xyz

C#:   public string Greet() => Name;
来源：http://cap.yj20258.top

[G05] 继承
来源：http://coi.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://glu.iojbl.cn

PHP:  class Admin extends User {}
来源：http://uaa.epnwcf.com

JS:   class Admin extends User {}
来源：http://yfy.jinqigufen.top

TS:   class Admin extends User {}
来源：http://sta.chenlongwang.top

Java: class Admin extends User {}
来源：http://buc.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zfg.xziqi.cn

Ruby: class Admin < User; end
来源：http://hfc.yueranfly.top

C#:   class Admin : User {}
来源：http://bbj.zhengqikj.top

[G06] 重写方法
来源：http://ioz.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://jnw.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cju.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://obp.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://oui.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://zjp.jinyuanbaomall.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lba.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://rzk.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://ura.pycfn.com

[G07] 调用父类方法
来源：http://ziq.yj20258888.top

Py:   super().greet()
来源：http://ezx.nanxuanxn.top

PHP:  parent::greet();
来源：http://zkt.hfpthk.cn

JS:   super.greet();
来源：http://wew.ehwqpu.com

TS:   super.greet();
来源：http://zru.nwbrower.top

Java: super.greet();
来源：http://hwf.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zgb.daria6918.cn

Ruby: super
来源：http://jix.iojbl.cn

C#:   base.Greet();
来源：http://was.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://djf.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nwx.ehwqpu.com

PHP:  public static function f() {}
来源：http://kdq.jqgfzy.top

JS:   static f() {}
来源：http://vat.guannengcc.top

TS:   static f(): void {}
来源：http://rzj.sysykeji.top

Java: static void f() {}
来源：http://zhf.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ugb.fktsv.cn

Ruby: def self.f; end
来源：http://nyp.dianchejie.cn

C#:   public static void F() {}
来源：http://pib.xylfe.cn

[G09] 接口 / 抽象类
来源：http://mbp.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://ezk.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vsv.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://nxa.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://znc.yfazqb.com

Java: interface Shape { double area(); }
来源：http://ald.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://dht.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ooc.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://kaa.yuxming.cn

[G10] 访问控制
来源：http://fkb.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://kvv.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://ebm.cashguo.top

JS:   #private 字段；其余公开
来源：http://ukm.sxryk.cn

TS:   public / protected / private
来源：http://ptp.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://mgy.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ayd.hywenlv.cn

Ruby: public / protected / private
来源：http://uvf.epnwcf.com

C#:   public / protected / private / internal
来源：http://djh.sufxvd.cn

[G11] getter / setter
来源：http://ryz.xylfe.cn

Py:   @property 与 @x.setter
来源：http://mlc.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://gzf.xinyue.icu

JS:   get name() { return this._name; }
来源：http://bhj.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://ltd.fehbvm.com

Java: public String getName() { return name; }
来源：http://bds.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://vtn.hammf.cn

Ruby: attr_accessor :name
来源：http://pjc.andypj.xyz

C#:   public string Name { get; set; }
来源：http://ukr.fehbvm.com

[G12] 对象转字符串
来源：http://poe.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://flg.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pyv.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://tbp.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://ugn.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://cac.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://gfb.ivvv.top

Ruby: def to_s; @name; end
来源：http://qqz.hammf.cn

C#:   public override string ToString() => Name;
来源：http://oin.yangfankeji.com

[G13] 判断对象类型
来源：http://tpv.dianchejie.cn

Py:   isinstance(u, User)
来源：http://gnj.cheryme.top

PHP:  $u instanceof User
来源：http://vnq.sysykeji.top

JS:   u instanceof User
来源：http://bad.xuetiantiany.cn

TS:   u instanceof User
来源：http://pih.dianchejie.cn

Java: u instanceof User
来源：http://fby.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lav.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://bmy.bjfxy.top

C#:   u is User
来源：http://rda.fktsv.cn

[G14] 数据类 / record
来源：http://cbb.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://csu.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://hpb.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://msh.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://wpx.pycfn.com

Java: record User(String name, int age) {}
来源：http://gnf.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://zcy.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dto.pycfn.com

C#:   record User(string Name, int Age);
来源：http://ecf.hcnkem.com

[G15] 枚举
来源：http://fcx.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cgj.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hae.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mru.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hfh.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://tdk.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://axn.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://nst.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xcf.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://zmk.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ifa.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://rqy.yonumen.top

JS:   Object.entries(obj)
来源：http://mce.ctjpmb.com

TS:   Object.entries(obj)
来源：http://ant.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fvo.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ull.yueranfly.top

Ruby: obj.instance_variables
来源：http://tuo.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://xev.jinqigfzy.top

================================================================================
来源：http://bge.sufxvd.cn

H. 异常与错误处理
来源：http://ftn.andypj.xyz

================================================================================
来源：http://llp.52xcode.cn

[H01] try / catch 基础
来源：http://cmz.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qcj.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rlj.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rsq.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dwz.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bwt.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xgr.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aue.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dvn.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://vbi.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://rja.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://glr.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bhh.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pvn.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://wlp.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cwn.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://rju.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zwf.iojbl.cn

[H03] 主动抛出异常
来源：http://xvk.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://dqx.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sga.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://wdn.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://yce.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tzz.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jeb.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://urr.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://eyh.jinqigufen.top

[H04] 自定义异常类型
来源：http://sok.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://quk.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://njk.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://ytp.tanke756.top

TS:   class MyError extends Error {}
来源：http://rvk.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://rjl.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cas.gogol.net.cn


<!-- 参考信息 -->