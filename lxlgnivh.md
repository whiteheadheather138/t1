代发 wailian999

Go:   if s == "" {}
来源：http://rwp.fktsv.cn

Ruby: if s.empty?
来源：http://uhx.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kkd.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://txc.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qbv.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dir.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://evi.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ouh.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dou.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://ucq.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://knc.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://huj.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://ejl.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qbn.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yst.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ojt.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tjc.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pyg.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://afs.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://fiq.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rcw.zhengqikj.top

================================================================================
来源：http://ybr.dianchejie.cn

F. 文件与目录
来源：http://hdd.hcnkem.com

================================================================================
来源：http://nyk.cdnleiting.top

[F01] 读取整个文件
来源：http://vum.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iqw.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://zkd.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://afl.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sdm.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vyd.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lda.birdmap.top

Ruby: File.read("a.txt")
来源：http://iyx.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://sve.meibo888.top

[F02] 逐行读取文件
来源：http://qab.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jas.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xml.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ksl.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rev.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://arl.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lcn.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xnv.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yuy.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://jxl.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uwq.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jlt.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gak.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://phi.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ner.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hwo.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ajq.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aqz.ydjk.org.cn

[F04] 追加写入文件
来源：http://ylo.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://juq.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lvp.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kee.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dzt.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ryg.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jil.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fri.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xux.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://egg.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iue.tarul.cn

PHP:  file_exists("a.txt");
来源：http://bmc.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://nir.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://hjt.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://xuz.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pwm.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://tfr.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://acq.ivvv.top

[F06] 删除文件
来源：http://pck.nwbrower.top

Py:   os.remove("a.txt")
来源：http://avt.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://gwt.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cci.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hmb.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qds.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://tal.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://qlb.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://orx.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://xym.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zwy.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gnv.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rme.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://owp.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fsa.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fwm.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://foh.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fyf.jinqigfzy.top

[F08] 遍历目录
来源：http://qmv.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aze.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dcu.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://efv.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://jmu.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yzi.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ebk.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://wnp.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://fki.xziqi.cn

[F09] 获取文件大小
来源：http://uzb.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://fsa.vehdjk.com

PHP:  filesize("a.txt");
来源：http://jrv.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://vsg.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://cgj.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://jaf.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fxm.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://nkq.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://ugz.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://cpc.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hct.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://suu.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://okp.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://bdm.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nwt.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tgb.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hja.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pun.mhx1999.top

[F11] 复制与移动文件
来源：http://nlg.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yhf.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uiq.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zqi.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ssc.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tqe.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zyp.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ltd.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nfk.nanxinkj.top

[F12] CSV 读写
来源：http://zmr.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tef.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xax.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gxa.xuanzx.com

TS:   // 同上
来源：http://wbb.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sep.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://epp.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mpe.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hin.zhengqikj.top

================================================================================
来源：http://gsw.shanyushiyangtech.top

G. 面向对象
来源：http://zel.tarul.cn

================================================================================
来源：http://rax.aizwys.cn

[G01] 定义类
来源：http://dlq.kuanghao11.cn

Py:   class User: pass
来源：http://bsv.cdnleiting.top

PHP:  class User {}
来源：http://ipt.chenzaomai.com

JS:   class User {}
来源：http://khz.yj20258.top

TS:   class User { name: string = ""; }
来源：http://oph.hesvh.cn

Java: class User {}
来源：http://jpv.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://hxo.guannengcc.top

Ruby: class User; end
来源：http://veh.zhixingplan.top

C#:   class User {}
来源：http://ljr.sxryk.cn

[G02] 构造函数
来源：http://neh.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://wdz.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://xgk.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://kyi.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://ror.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://bmf.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://epw.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://uud.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://mqo.cheryme.top

[G03] 实例属性
来源：http://tmw.aibaodan.cn

Py:   self.name = "x"
来源：http://zsw.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://hph.gaohongyu789.top

JS:   this.name = "x";
来源：http://kly.zhijiandao.cn

TS:   name: string = "x";
来源：http://csu.fanxiaobao.xyz

Java: private String name;
来源：http://iol.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hgw.52xcode.cn

Ruby: @name = "x"
来源：http://aef.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://ecj.sxryk.cn

[G04] 定义方法
来源：http://kdr.xylfe.cn

Py:   def greet(self): return self.name
来源：http://vqr.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ryz.yonumen.top

JS:   greet() { return this.name; }
来源：http://sob.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://yzj.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://ixe.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wpb.shuidangran.top

Ruby: def greet; @name; end
来源：http://gjc.hammf.cn

C#:   public string Greet() => Name;
来源：http://bnr.wangshuangyany.cn

[G05] 继承
来源：http://rox.fktsv.cn

Py:   class Admin(User): pass
来源：http://mbb.xuanzx.com

PHP:  class Admin extends User {}
来源：http://kwx.tarul.cn

JS:   class Admin extends User {}
来源：http://emb.jianghu66.top

TS:   class Admin extends User {}
来源：http://dew.zhoulong.xyz

Java: class Admin extends User {}
来源：http://siy.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vge.316326.xyz

Ruby: class Admin < User; end
来源：http://mso.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://mwr.zhijiandao.cn

[G06] 重写方法
来源：http://jbr.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://lor.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://jfx.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://xmn.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://bmv.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://hgg.hysaishi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oyg.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://sxt.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://elb.bjfxy.top

[G07] 调用父类方法
来源：http://tfa.wangdashe.top

Py:   super().greet()
来源：http://yxq.cheryme.top

PHP:  parent::greet();
来源：http://fir.snrcjt.cn

JS:   super.greet();
来源：http://bqz.cashguo.top

TS:   super.greet();
来源：http://nut.tianlin.xyz

Java: super.greet();
来源：http://ejl.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tgk.cucudq.cn

Ruby: super
来源：http://stq.yfazqb.com

C#:   base.Greet();
来源：http://wxb.sufxvd.cn

[G08] 静态方法与属性
来源：http://mov.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ymq.ctjpmb.com

PHP:  public static function f() {}
来源：http://lec.zycfv.cn

JS:   static f() {}
来源：http://nou.yj20258888.top

TS:   static f(): void {}
来源：http://htz.daxiang520.top

Java: static void f() {}
来源：http://ffc.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fdz.yueranfly.top

Ruby: def self.f; end
来源：http://fmi.birdmap.top

C#:   public static void F() {}
来源：http://kyr.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://nyy.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://znj.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://pjs.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://psq.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://kvd.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://cqj.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://hkd.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://irk.xinyue.icu

C#:   interface IShape { double Area(); }
来源：http://lok.xylfe.cn

[G10] 访问控制
来源：http://caf.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://gcx.snrcjt.cn

PHP:  public / protected / private
来源：http://ayd.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://hhq.redwolf501.top

TS:   public / protected / private
来源：http://qmh.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://tcj.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://szg.yj202588.top

Ruby: public / protected / private
来源：http://ekw.vehdjk.com

C#:   public / protected / private / internal
来源：http://gdm.jinyuanbaomall.cn

[G11] getter / setter
来源：http://ugg.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://yoj.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dqe.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://hxx.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://vkv.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://qxs.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qqw.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://acr.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://wse.cdnleiting.top

[G12] 对象转字符串
来源：http://xfq.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://hsj.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bva.tanke756.top

JS:   toString() { return this.name; }
来源：http://nfg.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://tjk.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://sid.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://has.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://fvg.yj202588.top

C#:   public override string ToString() => Name;
来源：http://cka.cqqwz.cn

[G13] 判断对象类型
来源：http://qmb.wangdashe.top

Py:   isinstance(u, User)
来源：http://zrr.yangfankeji.com

PHP:  $u instanceof User
来源：http://agp.mhx1999.top

JS:   u instanceof User
来源：http://cfu.daria6918.cn

TS:   u instanceof User
来源：http://lda.zhoulong.xyz

Java: u instanceof User
来源：http://zym.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ctt.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://taa.zdbjq.cn

C#:   u is User
来源：http://tni.sweek.top

[G14] 数据类 / record
来源：http://twg.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wxj.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://tej.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://noe.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://qat.yfazqb.com

Java: record User(String name, int age) {}
来源：http://eyv.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://qbt.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aeq.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://bma.feifeiyinyue.top

[G15] 枚举
来源：http://tzw.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://svy.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://miq.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xfb.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yre.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://hvb.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fnp.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://xwo.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cnk.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://acj.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fvw.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://ivv.c1oappe.top

JS:   Object.entries(obj)
来源：http://vva.jqgfzy.top

TS:   Object.entries(obj)
来源：http://ven.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hip.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jym.jiagoushi.top

Ruby: obj.instance_variables
来源：http://uuu.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://syq.birdmap.top

================================================================================
来源：http://ivt.dianchejie.cn

H. 异常与错误处理
来源：http://mlg.zhoulong.xyz

================================================================================
来源：http://xgg.vqdsnc.cn

[H01] try / catch 基础
来源：http://ufm.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://haj.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://byo.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://btw.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wnc.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://juc.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kaf.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qua.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ksc.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://oee.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lvk.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://clu.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zsq.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nlw.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wug.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vck.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zpb.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ply.dianchejie.cn


<!-- 参考信息 -->