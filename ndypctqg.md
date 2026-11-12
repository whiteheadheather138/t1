代发 wailian999

[E22] 字节长度与字符长度
来源：http://aet.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eop.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zpn.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ygc.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://spo.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ytp.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nur.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://eel.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fkt.gaohongyu789.top

================================================================================
来源：http://cbs.quarkkingdee.top

F. 文件与目录
来源：http://lie.9152youxi.cn

================================================================================
来源：http://bsm.pycfn.com

[F01] 读取整个文件
来源：http://nes.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wzc.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://mbk.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jsx.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jnx.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://soi.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://amb.yj202588.top

Ruby: File.read("a.txt")
来源：http://cpc.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://zxy.uphjek.com

[F02] 逐行读取文件
来源：http://udk.redwolf501.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xwi.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iij.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxc.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://duy.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://owi.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cei.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kfc.xingfuxueyuan.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sfa.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://tox.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xcc.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xhw.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rtm.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lhe.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kmh.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmw.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://vpu.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dus.c1oappe.top

[F04] 追加写入文件
来源：http://mdi.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uqu.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://csp.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpq.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mkw.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gyk.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yps.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://olo.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oif.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://vxh.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rgt.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://vrw.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://xki.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://bms.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://zyp.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dtj.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://eif.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://dpr.chenzaomai.com

[F06] 删除文件
来源：http://ods.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://wtc.wangdashe.top

PHP:  unlink("a.txt");
来源：http://aan.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://eeg.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://nsz.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hye.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://rdc.9152youxi.cn

Ruby: File.delete("a.txt")
来源：http://xli.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://vfo.bbcook.cn

[F07] 创建目录（含多级）
来源：http://xze.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xdv.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://swb.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hbf.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xwd.yangfankeji.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://liv.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://khz.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hhu.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kla.cqqwz.cn

[F08] 遍历目录
来源：http://swm.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nlk.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gem.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://ptb.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://fle.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://olm.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://omg.yueranfly.top

Ruby: Dir.children("dir")
来源：http://gke.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://ofv.ppjwa.cn

[F09] 获取文件大小
来源：http://ugx.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://uel.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://luq.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://efs.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://yqb.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://twq.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://odq.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://air.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://ivp.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://jzq.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fum.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zha.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://shh.pycfn.com

TS:   path.extname("a.txt")
来源：http://syw.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vrc.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rfj.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iqd.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bvr.yuxming.cn

[F11] 复制与移动文件
来源：http://ugg.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hun.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vui.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdz.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jwi.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rlc.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xyg.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lzp.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kkl.xziqi.cn

[F12] CSV 读写
来源：http://vrn.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qgr.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bim.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wqm.nanxuanxn.top

TS:   // 同上
来源：http://cpk.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xeg.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vwy.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gqi.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tdu.feifeiyinyue.top

================================================================================
来源：http://ylo.daria6918.cn

G. 面向对象
来源：http://sds.shanyushiyangtech.top

================================================================================
来源：http://ehx.bbcook.cn

[G01] 定义类
来源：http://pll.gogol.net.cn

Py:   class User: pass
来源：http://ttn.aibaodan.cn

PHP:  class User {}
来源：http://zpe.zhixingplan.top

JS:   class User {}
来源：http://kqb.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://fps.fehbvm.com

Java: class User {}
来源：http://ive.sxryk.cn

Go:   type User struct { Name string }
来源：http://jao.ivvv.top

Ruby: class User; end
来源：http://bcs.c1oappe.top

C#:   class User {}
来源：http://pna.haohaochexian.top

[G02] 构造函数
来源：http://tpz.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://oyo.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://tae.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://zkx.havefunace.top

TS:   constructor(public name: string) {}
来源：http://rtv.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://cgi.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kek.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://mfx.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://kdu.fanxiaobao.xyz

[G03] 实例属性
来源：http://vvy.yanxiufei.cn

Py:   self.name = "x"
来源：http://ypa.sweek.top

PHP:  public string $name = "x";
来源：http://bid.yongpay.top

JS:   this.name = "x";
来源：http://xca.zhongyouzk.top

TS:   name: string = "x";
来源：http://khr.kuanghao11.cn

Java: private String name;
来源：http://ksx.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dav.hnqzz.top

Ruby: @name = "x"
来源：http://vjk.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://xdg.shuidangran.top

[G04] 定义方法
来源：http://yqg.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://bfv.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://onr.wangdashe.top

JS:   greet() { return this.name; }
来源：http://coj.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://bnq.chenzaomai.com

Java: String greet() { return name; }
来源：http://for.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ntk.jqgfzy.top

Ruby: def greet; @name; end
来源：http://aap.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://xch.jinqigufen.top

[G05] 继承
来源：http://hzt.mhx1999.top

Py:   class Admin(User): pass
来源：http://sdq.cheryme.top

PHP:  class Admin extends User {}
来源：http://wsp.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://yul.ybcxt.top

TS:   class Admin extends User {}
来源：http://lcv.mhx1999.top

Java: class Admin extends User {}
来源：http://lch.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yiu.meibo888.top

Ruby: class Admin < User; end
来源：http://tmu.mhx1999.top

C#:   class Admin : User {}
来源：http://daw.pycfn.com

[G06] 重写方法
来源：http://ohx.tanke756.top

Py:   def greet(self): return "admin"
来源：http://xvh.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sfb.cashguo.top

JS:   greet() { return "admin"; }
来源：http://xjy.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://xqz.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://rbe.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nkw.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://sro.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://blr.aibaodan.cn

[G07] 调用父类方法
来源：http://ers.jinqigufen.top

Py:   super().greet()
来源：http://qbj.daxiang520.top

PHP:  parent::greet();
来源：http://wyu.daxiang520.top

JS:   super.greet();
来源：http://lko.ywan-chungtsiang.top

TS:   super.greet();
来源：http://exg.gotoacloud.top

Java: super.greet();
来源：http://lwa.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qst.shanyushiyangkeji.top

Ruby: super
来源：http://ied.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://urk.zhixingplan.top

[G08] 静态方法与属性
来源：http://suh.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://flt.uphjek.com

PHP:  public static function f() {}
来源：http://iqh.yj202588.top

JS:   static f() {}
来源：http://gdh.bjfxy.top

TS:   static f(): void {}
来源：http://oae.yj202588.top

Java: static void f() {}
来源：http://ytq.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://whh.nanxuanxn.top

Ruby: def self.f; end
来源：http://zuq.jiagoushi.top

C#:   public static void F() {}
来源：http://opy.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://hyo.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://ivc.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://ows.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://gmv.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://nij.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://bel.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://njg.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vyk.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://rwd.jinghuilouyu.cn

[G10] 访问控制
来源：http://eqq.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://jtz.yj20258888.top

PHP:  public / protected / private
来源：http://csa.andypj.xyz

JS:   #private 字段；其余公开
来源：http://dmw.cashguo.top

TS:   public / protected / private
来源：http://zka.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://cgf.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tce.hywenlv.cn

Ruby: public / protected / private
来源：http://kwp.fktsv.cn

C#:   public / protected / private / internal
来源：http://dca.zycfv.cn

[G11] getter / setter
来源：http://uuy.yongpay.top

Py:   @property 与 @x.setter
来源：http://mso.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://afy.yvedp.cn

JS:   get name() { return this._name; }
来源：http://ewu.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://ekg.snrcjt.cn

Java: public String getName() { return name; }
来源：http://irp.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gud.yangfankeji.com

Ruby: attr_accessor :name
来源：http://sli.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://asu.dianchejie.cn

[G12] 对象转字符串
来源：http://fsq.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://pqx.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ykz.yuxming.cn

JS:   toString() { return this.name; }
来源：http://ipp.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://lpj.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://ziu.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://tgw.birdmap.top

Ruby: def to_s; @name; end
来源：http://lcf.tarul.cn

C#:   public override string ToString() => Name;
来源：http://qcz.wangdashe.top

[G13] 判断对象类型
来源：http://idb.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://tbd.cashguo.top

PHP:  $u instanceof User
来源：http://tby.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://iba.hywenlv.cn

TS:   u instanceof User
来源：http://tks.hysaishi.cn

Java: u instanceof User
来源：http://odt.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://axf.mhx1999.top

Ruby: u.is_a?(User)
来源：http://vxg.pengpengdd.cyou

C#:   u is User
来源：http://jcf.sufxvd.cn

[G14] 数据类 / record
来源：http://pgg.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://enr.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://wcj.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pqd.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://cdg.guannengcc.top

Java: record User(String name, int age) {}
来源：http://eny.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://jkw.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tpr.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://yri.uphjek.com

[G15] 枚举
来源：http://cmr.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rtc.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qmi.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ruf.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wcn.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://hrv.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qgo.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://ynb.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qkr.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://fov.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rsh.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://yja.ydzc1.top

JS:   Object.entries(obj)
来源：http://hmx.yonumen.top

TS:   Object.entries(obj)
来源：http://egv.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rgc.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vej.yongpay.top

Ruby: obj.instance_variables
来源：http://xje.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://moj.cheryme.top

================================================================================
来源：http://dgd.zhixingplan.top

H. 异常与错误处理
来源：http://tev.316326.xyz

================================================================================
来源：http://inp.ctjpmb.com

[H01] try / catch 基础
来源：http://nlr.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kva.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ten.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fpd.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sqp.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwn.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tpg.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jbw.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://akz.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://jqo.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://vll.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://eww.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://swo.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rvp.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://exp.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tqs.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ewe.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://zfm.c1oappe.top

[H03] 主动抛出异常
来源：http://wfb.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://xgy.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pdl.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://zmc.tanke756.top

TS:   throw new Error("错误信息");
来源：http://cph.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ero.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hdd.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fqs.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://eiv.316326.xyz

[H04] 自定义异常类型
来源：http://nlq.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://bon.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dsb.jinqigufen.top


<!-- 参考信息 -->