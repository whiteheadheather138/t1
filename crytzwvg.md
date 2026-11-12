代发 wailian999

[E22] 字节长度与字符长度
来源：http://unt.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wlr.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fzu.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://znw.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rdm.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ogb.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uhi.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://uvx.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lwi.bbcook.cn

================================================================================
来源：http://qiv.fzhhl.top

F. 文件与目录
来源：http://xzd.kuanghao11.cn

================================================================================
来源：http://hbh.hcnkem.com

[F01] 读取整个文件
来源：http://hmp.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xch.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://wzc.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wtl.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jrf.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yam.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://msk.hnqzz.top

Ruby: File.read("a.txt")
来源：http://drh.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://ytd.uphjek.com

[F02] 逐行读取文件
来源：http://vha.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uij.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://esf.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wft.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jkw.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ovt.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://shf.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ynx.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tna.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://vum.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tjp.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://zpy.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tqq.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kic.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ovs.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hgb.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://ttl.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sbu.ppjwa.cn

[F04] 追加写入文件
来源：http://awr.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sqa.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tyo.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qyx.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kws.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yso.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yfa.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iga.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fng.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://cle.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jfn.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://ziu.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://iia.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://rdq.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uky.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qme.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://xwr.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://vse.andypj.xyz

[F06] 删除文件
来源：http://hap.gzhubu.top

Py:   os.remove("a.txt")
来源：http://nnk.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://hvv.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://azl.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qwh.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yeb.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://anc.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://jfw.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://gpe.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://yix.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://thq.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ntf.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hxr.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xmw.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://alf.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ysf.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rrl.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pqy.yj20258888.top

[F08] 遍历目录
来源：http://qoa.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tdm.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qrx.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://dpj.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://pcm.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://znn.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eax.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://shf.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://hov.jiagoushi.top

[F09] 获取文件大小
来源：http://bam.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://yqk.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://lgv.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://uza.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://rtq.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://vdq.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ggb.redwolf501.top

Ruby: File.size("a.txt")
来源：http://qce.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ydx.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://vmr.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zso.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rsw.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pqp.52xcode.cn

TS:   path.extname("a.txt")
来源：http://xnc.yfazqb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://imq.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://teg.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cdv.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://puw.xziqi.cn

[F11] 复制与移动文件
来源：http://gzb.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://htw.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fzq.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tfi.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zes.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://htn.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rmt.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aga.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fdm.9152youxi.cn

[F12] CSV 读写
来源：http://daq.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://loh.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lam.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qgz.hywenlv.cn

TS:   // 同上
来源：http://noe.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ape.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vna.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rwm.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://qnx.quarkkingdee.top

================================================================================
来源：http://jtj.ehwqpu.com

G. 面向对象
来源：http://qaf.aibaodan.cn

================================================================================
来源：http://uin.sxryk.cn

[G01] 定义类
来源：http://qwn.yuxming.cn

Py:   class User: pass
来源：http://cun.yj202588.top

PHP:  class User {}
来源：http://blq.uphjek.com

JS:   class User {}
来源：http://lnp.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://cqz.zhoulong.xyz

Java: class User {}
来源：http://oov.ivvv.top

Go:   type User struct { Name string }
来源：http://cbx.xylfe.cn

Ruby: class User; end
来源：http://sgb.jlsjyb.cn

C#:   class User {}
来源：http://adi.316326.xyz

[G02] 构造函数
来源：http://bfy.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://ctx.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://vvr.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://nje.316326.xyz

TS:   constructor(public name: string) {}
来源：http://sfd.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://byk.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eqm.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://auw.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://igo.yangfankeji.com

[G03] 实例属性
来源：http://rph.nanxuanxn.top

Py:   self.name = "x"
来源：http://rpa.yvedp.cn

PHP:  public string $name = "x";
来源：http://wok.daria6918.cn

JS:   this.name = "x";
来源：http://jvk.hnqzz.top

TS:   name: string = "x";
来源：http://egv.shuidangran.top

Java: private String name;
来源：http://kxr.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vbl.nwbrower.top

Ruby: @name = "x"
来源：http://qxj.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://hnn.sweek.top

[G04] 定义方法
来源：http://vyi.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://vej.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lmt.sweek.top

JS:   greet() { return this.name; }
来源：http://snp.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://kgh.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://dfn.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nka.sxryk.cn

Ruby: def greet; @name; end
来源：http://ccs.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://pjj.9152youxi.cn

[G05] 继承
来源：http://nur.tianlin.xyz

Py:   class Admin(User): pass
来源：http://poa.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://hhy.fehbvm.com

JS:   class Admin extends User {}
来源：http://ahv.hammf.cn

TS:   class Admin extends User {}
来源：http://ake.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://iyz.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wup.epnwcf.com

Ruby: class Admin < User; end
来源：http://odk.ydzc1.top

C#:   class Admin : User {}
来源：http://npp.yueranfly.top

[G06] 重写方法
来源：http://xvq.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://lkt.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://drh.cashguo.top

JS:   greet() { return "admin"; }
来源：http://seh.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://wzt.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://cjs.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gkq.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://qdu.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://pex.kuanghao11.cn

[G07] 调用父类方法
来源：http://zip.gzhubu.top

Py:   super().greet()
来源：http://xom.daria6918.cn

PHP:  parent::greet();
来源：http://gga.jiagoushi.top

JS:   super.greet();
来源：http://kig.c1oappe.top

TS:   super.greet();
来源：http://ijb.smart0.xyz

Java: super.greet();
来源：http://ejn.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://glh.vehdjk.com

Ruby: super
来源：http://kav.yuanzhike.top

C#:   base.Greet();
来源：http://ocg.gotoacloud.top

[G08] 静态方法与属性
来源：http://fxm.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pwl.zhixingplan.top

PHP:  public static function f() {}
来源：http://lrt.chenzaomai.com

JS:   static f() {}
来源：http://ahu.smart0.xyz

TS:   static f(): void {}
来源：http://llw.gzhubu.top

Java: static void f() {}
来源：http://fcu.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hye.fehbvm.com

Ruby: def self.f; end
来源：http://ztx.zhongyouzk.top

C#:   public static void F() {}
来源：http://dly.yongpay.top

[G09] 接口 / 抽象类
来源：http://ptz.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://xbd.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hau.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dhb.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://puk.tarul.cn

Java: interface Shape { double area(); }
来源：http://cge.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://prx.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fkw.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://fmo.shuidangran.top

[G10] 访问控制
来源：http://yia.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://lqu.ivvv.top

PHP:  public / protected / private
来源：http://lyi.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://tic.yanxiufei.cn

TS:   public / protected / private
来源：http://veq.cheryme.top

Java: public / protected / private / 默认包级
来源：http://nbl.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kwe.nanxuanxn.top

Ruby: public / protected / private
来源：http://zpx.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://mgu.jinghuilouyu.cn

[G11] getter / setter
来源：http://huv.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://ccq.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ipp.aizwys.cn

JS:   get name() { return this._name; }
来源：http://eci.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://ocg.meibo888.top

Java: public String getName() { return name; }
来源：http://wjw.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hqr.epnwcf.com

Ruby: attr_accessor :name
来源：http://cos.fehbvm.com

C#:   public string Name { get; set; }
来源：http://ypk.aibaodan.cn

[G12] 对象转字符串
来源：http://yed.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://iko.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nxw.xziqi.cn

JS:   toString() { return this.name; }
来源：http://wlm.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://tfc.yangfankeji.com

Java: @Override public String toString() { return name; }
来源：http://rvj.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wqz.yj20258.top

Ruby: def to_s; @name; end
来源：http://vqm.tarul.cn

C#:   public override string ToString() => Name;
来源：http://slh.snrcjt.cn

[G13] 判断对象类型
来源：http://fhe.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://rzf.yongpay.top

PHP:  $u instanceof User
来源：http://wcs.xylfe.cn

JS:   u instanceof User
来源：http://hil.ctjpmb.com

TS:   u instanceof User
来源：http://ayn.dianchejie.cn

Java: u instanceof User
来源：http://mky.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bqr.guannengcc.top

Ruby: u.is_a?(User)
来源：http://zix.jqgfzy.top

C#:   u is User
来源：http://rgm.xuetiantiany.cn

[G14] 数据类 / record
来源：http://kgx.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xwz.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://dob.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://tir.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://vgu.sweek.top

Java: record User(String name, int age) {}
来源：http://rde.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://gre.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://deu.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://awz.hongshengwenyu.top

[G15] 枚举
来源：http://fbu.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kxl.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pzo.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wmt.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ubx.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://ppg.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lqq.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://ust.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gzg.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://thp.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jse.meibo888.top

PHP:  get_object_vars($obj);
来源：http://svz.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://dij.gzhubu.top

TS:   Object.entries(obj)
来源：http://idj.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jxp.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fxc.daria6918.cn

Ruby: obj.instance_variables
来源：http://hyx.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://cgq.xuanzx.com

================================================================================
来源：http://sox.aizwys.cn

H. 异常与错误处理
来源：http://xei.yongpay.top

================================================================================
来源：http://xpu.ydzc1.top

[H01] try / catch 基础
来源：http://nzl.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://npy.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ppz.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tnl.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aem.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jbl.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://onj.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ied.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mcr.cheryme.top

[H02] finally / ensure 收尾
来源：http://odh.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://lxv.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://twm.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hfn.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://evv.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://ild.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qva.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nkc.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ixd.fktsv.cn

[H03] 主动抛出异常
来源：http://pqj.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://tfx.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pow.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://cwd.cashguo.top

TS:   throw new Error("错误信息");
来源：http://lif.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dus.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rap.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cvx.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://rwj.hnxiangtu.top

[H04] 自定义异常类型
来源：http://smj.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://yna.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://xxy.havefunace.top


<!-- 参考信息 -->