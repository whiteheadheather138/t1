代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sjg.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xag.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hla.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptf.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eox.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://oso.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aps.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tqn.yuxming.cn

[E22] 字节长度与字符长度
来源：http://awl.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bcj.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ppm.hcnkem.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vbv.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rbf.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lzg.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vjm.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://fuv.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ola.chenjidiqi.icu

================================================================================
来源：http://rbq.ivvv.top

F. 文件与目录
来源：http://oqo.quarkkingdee.top

================================================================================
来源：http://oxs.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://iux.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zsn.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://upi.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cyu.shanyushiyangtech.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vcs.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://hff.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gew.wangdashe.top

Ruby: File.read("a.txt")
来源：http://vzv.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://urj.zdqjudy.top

[F02] 逐行读取文件
来源：http://ayq.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sda.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://krm.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwz.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tcj.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://txg.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lkq.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://azg.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dzk.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://rgo.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dbn.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://buc.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nnl.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfn.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jsh.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xyf.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://eqb.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qyb.hfpthk.cn

[F04] 追加写入文件
来源：http://pua.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eng.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ifm.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://trx.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vuu.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wth.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://knw.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xaq.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urc.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://ary.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kcq.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://qbg.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://nor.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://pth.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jqp.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qna.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://bte.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://qhg.nanxinkj.top

[F06] 删除文件
来源：http://tui.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://wzs.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://inx.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vwn.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://dfq.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ddg.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://hfn.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://qia.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://avg.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://bgk.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pnm.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ehk.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sek.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ysv.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aiv.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bug.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvr.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baw.dianchejie.cn

[F08] 遍历目录
来源：http://gqs.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mre.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nvm.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://fam.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://mtt.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xuo.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://czc.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://lfh.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://ycb.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://iig.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://tha.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://fqa.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://njc.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://zfi.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bux.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yxb.nwbrower.top

Ruby: File.size("a.txt")
来源：http://qbj.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://ait.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://xlv.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://imn.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yjw.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qto.c1oappe.top

TS:   path.extname("a.txt")
来源：http://cyl.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tmk.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gii.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uvv.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://edu.fengsongda.top

[F11] 复制与移动文件
来源：http://ytf.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ave.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dxa.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ryc.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bic.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kqs.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://caw.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iqo.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zap.wangdashe.top

[F12] CSV 读写
来源：http://xrn.fzhhl.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xtt.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://som.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dkp.dianchejie.cn

TS:   // 同上
来源：http://vhc.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fre.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nhq.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://axo.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sld.jyoumei.cn

================================================================================
来源：http://mld.zhixingplan.top

G. 面向对象
来源：http://dci.daria6918.cn

================================================================================
来源：http://bbw.sjlbkw.cn

[G01] 定义类
来源：http://vbr.ybcxt.top

Py:   class User: pass
来源：http://cjn.fengsongda.top

PHP:  class User {}
来源：http://hps.sweek.top

JS:   class User {}
来源：http://fly.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://oqs.xuanzx.com

Java: class User {}
来源：http://qnk.hfpthk.cn

Go:   type User struct { Name string }
来源：http://ugn.ctjpmb.com

Ruby: class User; end
来源：http://rle.guannengcc.top

C#:   class User {}
来源：http://zaf.xinyue.icu

[G02] 构造函数
来源：http://fmz.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://mpr.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://igu.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://cun.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://ein.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://ojq.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dqp.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://kbq.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://kdo.ppjwa.cn

[G03] 实例属性
来源：http://swc.yuxming.cn

Py:   self.name = "x"
来源：http://inb.fzhhl.top

PHP:  public string $name = "x";
来源：http://eqd.zhiwuduotai.top

JS:   this.name = "x";
来源：http://ekc.bjfxy.top

TS:   name: string = "x";
来源：http://ldo.shanyushiyangtech.top

Java: private String name;
来源：http://gre.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qwz.chenlongwang.top

Ruby: @name = "x"
来源：http://rpk.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://yvp.iojbl.cn

[G04] 定义方法
来源：http://ygb.meibo888.top

Py:   def greet(self): return self.name
来源：http://qzk.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mtc.daria6918.cn

JS:   greet() { return this.name; }
来源：http://cyc.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://nas.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://upt.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://kev.jinqigufen.top

Ruby: def greet; @name; end
来源：http://qvo.birdmap.top

C#:   public string Greet() => Name;
来源：http://cll.gogol.net.cn

[G05] 继承
来源：http://ulb.jyoumei.cn

Py:   class Admin(User): pass
来源：http://yft.yj202588.top

PHP:  class Admin extends User {}
来源：http://rgq.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://cyn.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://dvb.chenlongwang.top

Java: class Admin extends User {}
来源：http://xql.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tkj.yangfankeji.com

Ruby: class Admin < User; end
来源：http://eks.redwolf501.top

C#:   class Admin : User {}
来源：http://stl.daria6918.cn

[G06] 重写方法
来源：http://ixc.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://rnh.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ndh.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://hjc.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://hmf.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://wbl.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pmb.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://hkf.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://fff.dianchejie.cn

[G07] 调用父类方法
来源：http://qva.hywenlv.cn

Py:   super().greet()
来源：http://oge.xuanzx.com

PHP:  parent::greet();
来源：http://fsb.daria6918.cn

JS:   super.greet();
来源：http://dmd.zhongyouzk.top

TS:   super.greet();
来源：http://bcv.ybcxt.top

Java: super.greet();
来源：http://kdo.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://law.cdnleiting.top

Ruby: super
来源：http://min.ybcxt.top

C#:   base.Greet();
来源：http://tsa.nwbrower.top

[G08] 静态方法与属性
来源：http://qzp.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://grn.zdbjq.cn

PHP:  public static function f() {}
来源：http://mro.52xcode.cn

JS:   static f() {}
来源：http://yom.gaohongyu789.top

TS:   static f(): void {}
来源：http://pzi.jianghu66.top

Java: static void f() {}
来源：http://dcq.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hfk.gogol.net.cn

Ruby: def self.f; end
来源：http://sfa.yvedp.cn

C#:   public static void F() {}
来源：http://nzk.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://rse.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://yym.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pqm.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vjo.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://xfh.hcnkem.com

Java: interface Shape { double area(); }
来源：http://bhd.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://jpq.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uvg.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://avy.guowangkeji.top

[G10] 访问控制
来源：http://gdi.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://iwe.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://wkd.shuidangran.top

JS:   #private 字段；其余公开
来源：http://qxn.cucudq.cn

TS:   public / protected / private
来源：http://xmb.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://lfa.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bzz.ydjk.org.cn

Ruby: public / protected / private
来源：http://ygd.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://wtv.xylfe.cn

[G11] getter / setter
来源：http://wqg.guannengcc.top

Py:   @property 与 @x.setter
来源：http://hqa.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nmw.sxryk.cn

JS:   get name() { return this._name; }
来源：http://emt.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://lrd.epnwcf.com

Java: public String getName() { return name; }
来源：http://iik.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://nnw.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://ssh.hnqzz.top

C#:   public string Name { get; set; }
来源：http://oqq.yongpay.top

[G12] 对象转字符串
来源：http://fxl.ivvv.top

Py:   def __str__(self): return self.name
来源：http://iiq.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ohj.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://mgk.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://nsl.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://phf.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://skw.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://gdx.hammf.cn

C#:   public override string ToString() => Name;
来源：http://anh.hesvh.cn

[G13] 判断对象类型
来源：http://kgi.yfazqb.com

Py:   isinstance(u, User)
来源：http://bcm.cashguo.top

PHP:  $u instanceof User
来源：http://drz.fengsongda.top

JS:   u instanceof User
来源：http://acm.vehdjk.com

TS:   u instanceof User
来源：http://mio.jianghu66.top

Java: u instanceof User
来源：http://beh.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://phk.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://jak.xingfuxueyuan.xyz

C#:   u is User
来源：http://ybh.fzhhl.top

[G14] 数据类 / record
来源：http://byn.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lku.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://frr.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://ruq.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://ybs.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://xrd.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://xtc.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uhl.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://mle.ydzc1.top

[G15] 枚举
来源：http://mxr.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zcv.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://cpv.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wui.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wht.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://aeb.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jhp.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://ydj.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://meg.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://qlu.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://smf.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://php.jinqigufen.top

JS:   Object.entries(obj)
来源：http://kib.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://gxh.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oik.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://yro.ppjwa.cn

Ruby: obj.instance_variables
来源：http://qwn.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://vkx.yuxming.cn

================================================================================
来源：http://uox.aibaodan.cn

H. 异常与错误处理
来源：http://aki.dashuyun.cn

================================================================================
来源：http://rgu.zycfv.cn

[H01] try / catch 基础
来源：http://mbi.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wes.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rpy.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wbz.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hgj.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hay.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jaq.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tja.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://agk.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://fjy.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://ejl.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cjm.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lrx.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jpx.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://mne.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sph.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://atw.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fiz.hnqzz.top

[H03] 主动抛出异常
来源：http://ukl.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://pru.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dpg.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://nex.smart0.xyz


<!-- 参考信息 -->