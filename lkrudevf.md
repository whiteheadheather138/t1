代发 wailian999

Go:   if s == "" {}
来源：http://str.hcnkem.com

Ruby: if s.empty?
来源：http://gds.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tbd.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://xar.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kem.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fer.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qll.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lke.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ouu.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://ugd.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sta.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zfv.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://vyp.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fxx.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oko.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://foq.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqd.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wbt.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gno.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://rem.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lze.xingfuxueyuan.xyz

================================================================================
来源：http://bvj.uphjek.com

F. 文件与目录
来源：http://dsv.zdbjq.cn

================================================================================
来源：http://tjp.tianlin.xyz

[F01] 读取整个文件
来源：http://fds.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fsk.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://mzt.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cle.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://imu.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://uyy.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xyb.bjfxy.top

Ruby: File.read("a.txt")
来源：http://yva.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://hbn.daxiang520.top

[F02] 逐行读取文件
来源：http://fsa.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zki.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nbb.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bjp.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ose.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vah.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mgm.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ity.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://frd.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://nes.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pyi.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lmd.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oti.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zlj.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fvi.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pzg.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://yfi.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ume.shuidangran.top

[F04] 追加写入文件
来源：http://ktw.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cah.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fsp.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rgr.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pdw.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ifo.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zsh.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://umr.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dxk.sweek.top

[F05] 判断文件或目录是否存在
来源：http://brq.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oke.meibo888.top

PHP:  file_exists("a.txt");
来源：http://ykj.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://oxu.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://zbw.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://scn.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iym.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://mbq.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://qit.jinqigufen.top

[F06] 删除文件
来源：http://qvb.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://ywr.hesvh.cn

PHP:  unlink("a.txt");
来源：http://omp.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://xqx.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://lpy.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cxu.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://zze.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://bma.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://izz.sysykeji.top

[F07] 创建目录（含多级）
来源：http://hsh.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://faw.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gxk.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ipt.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://odi.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wul.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kba.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ywr.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ddv.feifeiyinyue.top

[F08] 遍历目录
来源：http://jjr.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dyq.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lsv.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://noe.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://gqq.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qvn.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://tpr.epnwcf.com

Ruby: Dir.children("dir")
来源：http://vai.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://wld.zhiwuduotai.top

[F09] 获取文件大小
来源：http://uhp.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://rph.epnwcf.com

PHP:  filesize("a.txt");
来源：http://lzt.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://uel.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://yul.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://ldu.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bdv.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://itk.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://opl.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://pvj.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xak.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://srn.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lpn.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://gvz.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fup.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iab.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yej.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lcq.jinqigufen.top

[F11] 复制与移动文件
来源：http://ufd.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gbl.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zei.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uwh.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syd.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tla.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://waq.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zxd.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xvx.hnqzz.top

[F12] CSV 读写
来源：http://qgh.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cil.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xoe.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://buv.nanxuanxn.top

TS:   // 同上
来源：http://dox.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nrl.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fnp.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ojz.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xbr.zycfv.cn

================================================================================
来源：http://wpr.ctjpmb.com

G. 面向对象
来源：http://yvy.iojbl.cn

================================================================================
来源：http://tzh.zhixingplan.top

[G01] 定义类
来源：http://enc.shangyingyoupin.top

Py:   class User: pass
来源：http://aml.mhx1999.top

PHP:  class User {}
来源：http://mag.tarul.cn

JS:   class User {}
来源：http://kny.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://mbl.epnwcf.com

Java: class User {}
来源：http://toi.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://edt.nanxinkj.top

Ruby: class User; end
来源：http://irz.tianlin.xyz

C#:   class User {}
来源：http://ibt.zdqjudy.top

[G02] 构造函数
来源：http://sbf.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://vag.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://vtu.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://lnu.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://ppd.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://gkb.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nwf.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://rhl.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://pfr.jinghuilouyu.cn

[G03] 实例属性
来源：http://lyl.hcnkem.com

Py:   self.name = "x"
来源：http://ams.birdmap.top

PHP:  public string $name = "x";
来源：http://hyj.guannengcc.top

JS:   this.name = "x";
来源：http://kew.jinqigufen.top

TS:   name: string = "x";
来源：http://wlp.ywan-chungtsiang.top

Java: private String name;
来源：http://ojj.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wxf.hongshengwenyu.top

Ruby: @name = "x"
来源：http://zvm.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://ile.hnxiangtu.top

[G04] 定义方法
来源：http://pfw.52xcode.cn

Py:   def greet(self): return self.name
来源：http://asa.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://jsx.yvedp.cn

JS:   greet() { return this.name; }
来源：http://kdl.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://mbt.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://dho.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://grj.sweek.top

Ruby: def greet; @name; end
来源：http://stv.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://iis.gotoacloud.top

[G05] 继承
来源：http://roo.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://jrg.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://qwr.xinyue.icu

JS:   class Admin extends User {}
来源：http://umj.pycfn.com

TS:   class Admin extends User {}
来源：http://eam.yangfankeji.com

Java: class Admin extends User {}
来源：http://wcw.cucudq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dxh.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://oxv.birdmap.top

C#:   class Admin : User {}
来源：http://gdz.yfazqb.com

[G06] 重写方法
来源：http://geh.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://wvw.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nib.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://agk.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://xeg.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://xbz.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://orc.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://mjx.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://gwd.daria6918.cn

[G07] 调用父类方法
来源：http://wod.smart0.xyz

Py:   super().greet()
来源：http://ddr.zhengqikj.top

PHP:  parent::greet();
来源：http://wxr.fzhhl.top

JS:   super.greet();
来源：http://isb.aizwys.cn

TS:   super.greet();
来源：http://tkb.quarkkingdee.top

Java: super.greet();
来源：http://bzn.guowangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blt.ctjpmb.com

Ruby: super
来源：http://jao.yj20258.top

C#:   base.Greet();
来源：http://mel.nanxinkj.top

[G08] 静态方法与属性
来源：http://prc.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tqb.epnwcf.com

PHP:  public static function f() {}
来源：http://ryw.tian-w.cn

JS:   static f() {}
来源：http://xaf.nwbrower.top

TS:   static f(): void {}
来源：http://ezz.pengpengdd.cyou

Java: static void f() {}
来源：http://bak.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qlg.hammf.cn

Ruby: def self.f; end
来源：http://mcg.havefunace.top

C#:   public static void F() {}
来源：http://hnk.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://raj.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://vgi.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wzn.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ljk.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://fqk.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://bzz.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://uxx.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pek.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://ggx.hysaishi.cn

[G10] 访问控制
来源：http://iyr.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://mfg.fktsv.cn

PHP:  public / protected / private
来源：http://hwr.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://pbt.dashuyun.cn

TS:   public / protected / private
来源：http://rhq.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://xoo.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ful.hysaishi.cn

Ruby: public / protected / private
来源：http://vhy.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://zaz.iojbl.cn

[G11] getter / setter
来源：http://res.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://yhg.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vqp.vehdjk.com

JS:   get name() { return this._name; }
来源：http://kku.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://mvu.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://vcz.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vkm.jinqigufen.top

Ruby: attr_accessor :name
来源：http://uli.316326.xyz

C#:   public string Name { get; set; }
来源：http://gdi.uphjek.com

[G12] 对象转字符串
来源：http://ayv.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://jbk.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ddz.yvedp.cn

JS:   toString() { return this.name; }
来源：http://fpv.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://gav.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://nex.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://bfo.smart0.xyz

Ruby: def to_s; @name; end
来源：http://bnj.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://ees.birdmap.top

[G13] 判断对象类型
来源：http://bke.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://vkk.zhijiandao.cn

PHP:  $u instanceof User
来源：http://izr.snrcjt.cn

JS:   u instanceof User
来源：http://vln.hysaishi.cn

TS:   u instanceof User
来源：http://wpj.hfpthk.cn

Java: u instanceof User
来源：http://efd.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://zaw.yongpay.top

Ruby: u.is_a?(User)
来源：http://wov.meibo888.top

C#:   u is User
来源：http://abu.yvedp.cn

[G14] 数据类 / record
来源：http://ovr.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lbi.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://vzl.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://afk.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://llc.daxiang520.top

Java: record User(String name, int age) {}
来源：http://tcv.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://qmn.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lbo.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://vwg.shangyingyoupin.top

[G15] 枚举
来源：http://rvr.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cva.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://uon.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cia.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kwb.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://rcb.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xes.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://vwx.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://czc.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://ntx.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tcz.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://xuv.cucudq.cn

JS:   Object.entries(obj)
来源：http://xmx.meibo888.top

TS:   Object.entries(obj)
来源：http://lct.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cau.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://pex.9152youxi.cn

Ruby: obj.instance_variables
来源：http://zfp.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://ata.hnqzz.top

================================================================================
来源：http://xim.hysaishi.cn

H. 异常与错误处理
来源：http://nqg.zhijiandao.cn

================================================================================
来源：http://fzu.cqqwz.cn

[H01] try / catch 基础
来源：http://bfl.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dgv.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efx.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qqd.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://huc.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cpj.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gxp.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://agm.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://apr.cashguo.top

[H02] finally / ensure 收尾
来源：http://cau.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mld.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jnq.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://tpw.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://yjm.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://pbx.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dkp.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jcn.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xjl.yanxiufei.cn


<!-- 参考信息 -->