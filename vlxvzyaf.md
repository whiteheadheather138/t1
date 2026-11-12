代发 wailian999

Go:   if s == "" {}
来源：http://axv.yongpay.top

Ruby: if s.empty?
来源：http://pyy.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ohv.yvedp.cn

[E21] 超长截断加省略号
来源：http://rby.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://csp.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ton.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bnv.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ruf.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kpy.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://isg.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://osb.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cxz.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://hwo.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ilz.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://onl.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ryc.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://egb.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rls.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wrd.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://ymk.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://amj.wangshuangyany.cn

================================================================================
来源：http://iya.bjfxy.top

F. 文件与目录
来源：http://tjm.meibo888.top

================================================================================
来源：http://uhg.cashguo.top

[F01] 读取整个文件
来源：http://oup.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://owp.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://rpb.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tyk.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uni.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nku.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://agx.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://dcz.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://aeb.dashuyun.cn

[F02] 逐行读取文件
来源：http://cly.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jzg.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cet.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ewk.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zob.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ymx.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egd.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aiw.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oft.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://hzh.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vgb.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qst.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://agx.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xcr.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bdv.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ivd.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://jce.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hca.vqdsnc.cn

[F04] 追加写入文件
来源：http://ljo.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ede.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://itm.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdv.chenjidiqi.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://srh.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gsk.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jbe.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zef.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wwt.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://twn.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hek.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://vbb.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://iba.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://ymf.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://fll.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ses.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://moc.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://lbb.zhijiandao.cn

[F06] 删除文件
来源：http://uwz.redwolf501.top

Py:   os.remove("a.txt")
来源：http://gwt.gzhubu.top

PHP:  unlink("a.txt");
来源：http://xjg.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mhh.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rmw.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://axr.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://hlo.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://fwq.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://hbi.sysykeji.top

[F07] 创建目录（含多级）
来源：http://ycy.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cvb.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://acb.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sbf.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxz.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wyf.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vcs.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sit.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fgg.shangyingyoupin.top

[F08] 遍历目录
来源：http://rgt.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vih.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pou.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://tef.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://lme.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wye.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://oot.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://gzb.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://byv.sweek.top

[F09] 获取文件大小
来源：http://wnf.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ash.xziqi.cn

PHP:  filesize("a.txt");
来源：http://scz.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://jtw.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://upp.hesvh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://avm.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dzx.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://ada.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://rhj.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://vci.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://muz.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xuk.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://olb.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://ftv.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fnm.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cvd.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cmk.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://law.yueranfly.top

[F11] 复制与移动文件
来源：http://eor.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vdu.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ewx.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lko.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmn.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qvw.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tpq.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jhz.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yfh.fzhhl.top

[F12] CSV 读写
来源：http://vyq.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zoc.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iru.snrcjt.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nci.hammf.cn

TS:   // 同上
来源：http://hne.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bis.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xbk.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jvb.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://gpx.9152youxi.cn

================================================================================
来源：http://zmm.kuanghao11.cn

G. 面向对象
来源：http://asu.redwolf501.top

================================================================================
来源：http://vnp.0kj1m.cn

[G01] 定义类
来源：http://iuf.tanke756.top

Py:   class User: pass
来源：http://gmz.jqgufenzy.top

PHP:  class User {}
来源：http://xfa.yongpay.top

JS:   class User {}
来源：http://jow.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://yhu.nanxinkj.top

Java: class User {}
来源：http://wss.tanke756.top

Go:   type User struct { Name string }
来源：http://sjf.yj20258.top

Ruby: class User; end
来源：http://tzn.yangfankeji.com

C#:   class User {}
来源：http://scm.jlsjyb.cn

[G02] 构造函数
来源：http://fqi.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://acf.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://xyf.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://axm.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://yop.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://fek.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lrq.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://uev.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://pau.cashguo.top

[G03] 实例属性
来源：http://aar.xuetiantiany.cn

Py:   self.name = "x"
来源：http://qux.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://zlx.guowangkeji.top

JS:   this.name = "x";
来源：http://asm.chenzaomai.com

TS:   name: string = "x";
来源：http://slm.shzxlz.cn

Java: private String name;
来源：http://lsb.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qfm.yuxming.cn

Ruby: @name = "x"
来源：http://tyw.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://nxr.yanxiufei.cn

[G04] 定义方法
来源：http://rsh.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://wku.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tnw.meibo888.top

JS:   greet() { return this.name; }
来源：http://vee.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://kbp.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://mkz.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jzi.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://lvr.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://eup.chenlongwang.top

[G05] 继承
来源：http://bwc.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://mlt.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://mma.52xcode.cn

JS:   class Admin extends User {}
来源：http://uww.epnwcf.com

TS:   class Admin extends User {}
来源：http://hwt.yvedp.cn

Java: class Admin extends User {}
来源：http://zhv.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hji.epnwcf.com

Ruby: class Admin < User; end
来源：http://mtt.shzxlz.cn

C#:   class Admin : User {}
来源：http://ecw.sysykeji.top

[G06] 重写方法
来源：http://kte.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://jtx.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yym.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://cjn.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://dhp.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://hfs.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://akk.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://kdl.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://buu.zhijiandao.cn

[G07] 调用父类方法
来源：http://mvs.hongshengwenyu.top

Py:   super().greet()
来源：http://krs.hywenlv.cn

PHP:  parent::greet();
来源：http://tlr.hesvh.cn

JS:   super.greet();
来源：http://sip.quarkkingdee.top

TS:   super.greet();
来源：http://qpu.haohaochexian.top

Java: super.greet();
来源：http://iqn.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kxe.cheryme.top

Ruby: super
来源：http://fqg.fehbvm.com

C#:   base.Greet();
来源：http://xfs.xinyue.icu

[G08] 静态方法与属性
来源：http://ohd.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iql.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://exn.yfazqb.com

JS:   static f() {}
来源：http://ewh.c1oappe.top

TS:   static f(): void {}
来源：http://pcg.zhengqikj.top

Java: static void f() {}
来源：http://njz.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pbv.jyoumei.cn

Ruby: def self.f; end
来源：http://pgz.gotoacloud.top

C#:   public static void F() {}
来源：http://nvl.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://lri.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://dgm.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nel.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rob.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://brf.yj20258888.top

Java: interface Shape { double area(); }
来源：http://hlj.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://gyc.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hpg.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://iey.gaohongyu789.top

[G10] 访问控制
来源：http://ylw.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://lde.dianchejie.cn

PHP:  public / protected / private
来源：http://kyt.yj20258.top

JS:   #private 字段；其余公开
来源：http://cyn.cucudq.cn

TS:   public / protected / private
来源：http://kut.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://mbt.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cpr.andypj.xyz

Ruby: public / protected / private
来源：http://wke.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://itn.jinqigfzy.top

[G11] getter / setter
来源：http://upk.zycfv.cn

Py:   @property 与 @x.setter
来源：http://bkk.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vrt.tanke756.top

JS:   get name() { return this._name; }
来源：http://ggv.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://axb.sweek.top

Java: public String getName() { return name; }
来源：http://uqt.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://adm.tanke756.top

Ruby: attr_accessor :name
来源：http://ubh.ydzc1.top

C#:   public string Name { get; set; }
来源：http://mzt.dashuyun.cn

[G12] 对象转字符串
来源：http://kvh.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://atq.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://odo.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://qfq.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://qqp.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://fpl.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pdt.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://tae.yj202588.top

C#:   public override string ToString() => Name;
来源：http://gms.shzxlz.cn

[G13] 判断对象类型
来源：http://rok.ivvv.top

Py:   isinstance(u, User)
来源：http://cfm.xylfe.cn

PHP:  $u instanceof User
来源：http://vrs.ppjwa.cn

JS:   u instanceof User
来源：http://goi.fanxiaobao.xyz

TS:   u instanceof User
来源：http://dtq.sufxvd.cn

Java: u instanceof User
来源：http://eml.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lkc.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://gyo.meibo888.top

C#:   u is User
来源：http://del.wangshuangyany.cn

[G14] 数据类 / record
来源：http://ybo.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ngh.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://whb.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://yph.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://knv.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://imv.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://wku.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yzj.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://gpi.zhongyouzk.top

[G15] 枚举
来源：http://tbp.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ofz.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fxn.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gpe.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iiy.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://vxe.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://flc.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://bvx.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gjp.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://kaf.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xrw.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://vib.hesvh.cn

JS:   Object.entries(obj)
来源：http://vwe.andypj.xyz

TS:   Object.entries(obj)
来源：http://znj.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://slv.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tda.bbcook.cn

Ruby: obj.instance_variables
来源：http://tnk.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://irg.zhaomingkeji.xyz

================================================================================
来源：http://nub.sufxvd.cn

H. 异常与错误处理
来源：http://qcl.ehwqpu.com

================================================================================
来源：http://zqy.dashuyun.cn

[H01] try / catch 基础
来源：http://osi.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zzo.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oqh.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kfk.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rci.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vyr.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://elc.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sly.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jxq.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://agq.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://qzn.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://qya.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fxz.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dma.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://iya.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gxv.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://vfs.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://kfl.nanxuanxn.top


<!-- 参考信息 -->