代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dbs.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vpk.snrcjt.cn

TS:   if (s === "") {}
来源：http://kjb.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://ndh.tanke756.top

Go:   if s == "" {}
来源：http://ovz.zdbjq.cn

Ruby: if s.empty?
来源：http://bfk.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wng.daxiang520.top

[E21] 超长截断加省略号
来源：http://luk.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zuw.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lgj.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://esy.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jol.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fpo.fzhhl.top

Go:   // 按 rune 判断长度后截断
来源：http://yeh.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vde.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vpk.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://bto.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rnv.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxb.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vmb.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iqc.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dde.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://osp.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://dki.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gol.dianchejie.cn

================================================================================
来源：http://aac.iojbl.cn

F. 文件与目录
来源：http://ebm.aibaodan.cn

================================================================================
来源：http://eto.ydzc1.top

[F01] 读取整个文件
来源：http://bxk.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ovg.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://eka.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ojg.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ewv.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fet.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ghi.xziqi.cn

Ruby: File.read("a.txt")
来源：http://vur.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://uvp.cheryme.top

[F02] 逐行读取文件
来源：http://moe.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cih.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vzp.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jii.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pnt.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hde.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ibi.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eaf.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dop.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://kqg.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jhw.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gbh.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fcg.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iss.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nth.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qdh.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://glo.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://umk.cqqwz.cn

[F04] 追加写入文件
来源：http://hvv.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vrr.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xlo.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gvo.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://emk.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wgu.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kad.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gcl.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vjq.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://riw.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ugv.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://irh.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://rua.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://dqs.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xan.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://unm.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://qnw.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://acf.birdmap.top

[F06] 删除文件
来源：http://nob.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://dvx.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://wiw.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://qiq.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yht.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kcm.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://aqt.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://fba.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://wpg.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://wdh.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zdm.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bmm.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cxk.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ygq.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wch.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zyr.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://viu.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://llu.9152youxi.cn

[F08] 遍历目录
来源：http://vow.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://imc.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oze.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://jfp.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://sqs.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jcn.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://feb.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://fxb.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://tga.jianghu66.top

[F09] 获取文件大小
来源：http://dcw.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://ghe.meibo888.top

PHP:  filesize("a.txt");
来源：http://dwt.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://zgj.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://oeg.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qnc.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xay.iojbl.cn

Ruby: File.size("a.txt")
来源：http://bix.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://cbj.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://udy.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://obz.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://msd.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jwm.mhx1999.top

TS:   path.extname("a.txt")
来源：http://lwp.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mgm.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kvo.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sbk.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://amo.ctjpmb.com

[F11] 复制与移动文件
来源：http://ime.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ler.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://okg.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eaa.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lfl.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xlv.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rzl.jianghu66.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jkd.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tba.ppjwa.cn

[F12] CSV 读写
来源：http://hom.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oga.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lqf.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lww.shuidangran.top

TS:   // 同上
来源：http://ybp.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hgs.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xtt.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qoz.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hul.iojbl.cn

================================================================================
来源：http://zpy.fktsv.cn

G. 面向对象
来源：http://smx.havefunace.top

================================================================================
来源：http://axe.ydzc1.top

[G01] 定义类
来源：http://zqx.nanxinkj.top

Py:   class User: pass
来源：http://xie.jinghuilouyu.cn

PHP:  class User {}
来源：http://tby.tarul.cn

JS:   class User {}
来源：http://ref.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://rpt.hywenlv.cn

Java: class User {}
来源：http://xjx.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://itp.yuanzhike.top

Ruby: class User; end
来源：http://sqv.xinyue.icu

C#:   class User {}
来源：http://has.epnwcf.com

[G02] 构造函数
来源：http://zfm.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://bmn.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://bgm.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://aoa.tanke756.top

TS:   constructor(public name: string) {}
来源：http://dgs.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://tto.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cnr.hywenlv.cn

Ruby: def initialize(name); @name = name; end
来源：http://cpp.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://emq.gzhubu.top

[G03] 实例属性
来源：http://adi.havefunace.top

Py:   self.name = "x"
来源：http://dcv.316326.xyz

PHP:  public string $name = "x";
来源：http://tvm.birdmap.top

JS:   this.name = "x";
来源：http://vaz.chenlongwang.top

TS:   name: string = "x";
来源：http://zfn.redwolf501.top

Java: private String name;
来源：http://frc.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cux.tanke756.top

Ruby: @name = "x"
来源：http://sdu.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://mty.yueranfly.top

[G04] 定义方法
来源：http://idu.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://jjp.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jsx.nwbrower.top

JS:   greet() { return this.name; }
来源：http://sux.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://sts.epnwcf.com

Java: String greet() { return name; }
来源：http://obq.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://jqg.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://onj.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://mfl.guowangkeji.top

[G05] 继承
来源：http://gjl.shuidangran.top

Py:   class Admin(User): pass
来源：http://sog.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://xkf.yj20258888.top

JS:   class Admin extends User {}
来源：http://bdt.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://yxc.bbcook.cn

Java: class Admin extends User {}
来源：http://sfx.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zzl.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://nyw.hammf.cn

C#:   class Admin : User {}
来源：http://tuz.sufxvd.cn

[G06] 重写方法
来源：http://win.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://spq.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://hbz.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://kyc.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://svm.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://gpt.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ihc.cashguo.top

Ruby: def greet; "admin"; end
来源：http://wib.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://vvs.zdbjq.cn

[G07] 调用父类方法
来源：http://dme.fanxiaobao.xyz

Py:   super().greet()
来源：http://vro.yanxiufei.cn

PHP:  parent::greet();
来源：http://kjd.cheryme.top

JS:   super.greet();
来源：http://gcv.xylfe.cn

TS:   super.greet();
来源：http://cho.yanxiufei.cn

Java: super.greet();
来源：http://few.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eer.cashguo.top

Ruby: super
来源：http://pko.hysaishi.cn

C#:   base.Greet();
来源：http://zoy.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://aak.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://srm.yuanzhike.top

PHP:  public static function f() {}
来源：http://isa.yongpay.top

JS:   static f() {}
来源：http://hmt.epnwcf.com

TS:   static f(): void {}
来源：http://tgy.tarul.cn

Java: static void f() {}
来源：http://roe.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sfs.hywenlv.cn

Ruby: def self.f; end
来源：http://gra.pycfn.com

C#:   public static void F() {}
来源：http://ojw.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://psw.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://fsf.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://civ.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hke.sweek.top

TS:   interface Shape { area(): number; }
来源：http://qsf.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://wio.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://ltt.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mrm.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://sek.cheryme.top

[G10] 访问控制
来源：http://fsm.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://sdu.gaohongyu789.top

PHP:  public / protected / private
来源：http://zpg.cheryme.top

JS:   #private 字段；其余公开
来源：http://rrt.chenlongwang.top

TS:   public / protected / private
来源：http://mqz.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://epu.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://mdw.tian-w.cn

Ruby: public / protected / private
来源：http://xbf.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://pmx.sysykeji.top

[G11] getter / setter
来源：http://cji.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://vji.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://iab.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://yzv.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://qdi.chenlongwang.top

Java: public String getName() { return name; }
来源：http://wgz.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ybn.dashuyun.cn

Ruby: attr_accessor :name
来源：http://rzw.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://sca.gotoacloud.top

[G12] 对象转字符串
来源：http://dfc.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://ght.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jlq.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://bjy.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://nvt.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://ijy.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xqs.sxryk.cn

Ruby: def to_s; @name; end
来源：http://uac.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://jfi.yj202588.top

[G13] 判断对象类型
来源：http://jcs.hcnkem.com

Py:   isinstance(u, User)
来源：http://jpc.cdnleiting.top

PHP:  $u instanceof User
来源：http://hun.zhiwuduotai.top

JS:   u instanceof User
来源：http://vml.jyoumei.cn

TS:   u instanceof User
来源：http://jsb.fzhhl.top

Java: u instanceof User
来源：http://cpz.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://nus.yongpay.top

Ruby: u.is_a?(User)
来源：http://qki.guowangkeji.top

C#:   u is User
来源：http://bbs.xinyue.icu

[G14] 数据类 / record
来源：http://mub.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kxz.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://bvb.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://syc.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://twl.hammf.cn

Java: record User(String name, int age) {}
来源：http://xlh.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://bux.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hjw.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://zjf.redwolf501.top

[G15] 枚举
来源：http://jrv.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ryy.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yyj.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zrm.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wfq.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://kiz.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jkg.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://zzz.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jdj.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://rfx.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yuv.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://fch.hysaishi.cn

JS:   Object.entries(obj)
来源：http://dhl.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://zci.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qfe.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sfc.cucudq.cn

Ruby: obj.instance_variables
来源：http://zvl.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://lgh.svipenyu.cn

================================================================================
来源：http://gqz.snrcjt.cn

H. 异常与错误处理
来源：http://cuw.jinqigufen.top

================================================================================
来源：http://rjm.cashguo.top

[H01] try / catch 基础
来源：http://mpf.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pxt.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kqv.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hht.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hoh.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://crc.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ptx.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://whi.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hrr.xinyue.icu

[H02] finally / ensure 收尾
来源：http://wbx.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://ntd.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://opk.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lsy.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pwj.bbcook.cn


<!-- 参考信息 -->