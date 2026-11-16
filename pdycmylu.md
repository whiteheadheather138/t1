代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xzv.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://bbc.chenjidiqi.icu

Py:   s.splitlines()
来源：http://wpm.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vky.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://zip.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://eys.mhx1999.top

Java: s.lines().toList()
来源：http://imf.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://rmb.xziqi.cn

Ruby: s.lines
来源：http://zpa.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://dhl.meibo888.top

[E20] 判断字符串是否为空
来源：http://qld.svipenyu.cn

Py:   if not s:
来源：http://cig.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gja.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oyz.yj202588.top

TS:   if (s === "") {}
来源：http://fwy.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://veu.guowangkeji.top

Go:   if s == "" {}
来源：http://jww.nwbrower.top

Ruby: if s.empty?
来源：http://ffr.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://utj.sysykeji.top

[E21] 超长截断加省略号
来源：http://mdl.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ahy.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ktk.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://moa.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xvj.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://whi.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://epq.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fhm.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fch.wangdashe.top

[E22] 字节长度与字符长度
来源：http://jre.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gkm.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ytb.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cdb.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rbu.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mek.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ixb.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://vqv.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hzm.xylfe.cn

================================================================================
来源：http://ivt.jyoumei.cn

F. 文件与目录
来源：http://hkz.xuetiantiany.cn

================================================================================
来源：http://ibk.kuanghao11.cn

[F01] 读取整个文件
来源：http://xro.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baf.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://ulg.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bmc.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iwu.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qqb.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yrz.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://ubv.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://nog.hysaishi.cn

[F02] 逐行读取文件
来源：http://awp.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xty.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oez.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ltq.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://shb.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pmb.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vnn.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cps.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qmy.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://tvc.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bpv.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://clv.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epp.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gmg.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sai.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yjf.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://mnh.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://usb.aizwys.cn

[F04] 追加写入文件
来源：http://tzk.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lxm.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yca.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zim.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nvb.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kho.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oez.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gto.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xke.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://lzc.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://auc.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://cjf.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://frq.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://yxo.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xed.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://azt.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://hga.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://qww.cashguo.top

[F06] 删除文件
来源：http://dsd.uphjek.com

Py:   os.remove("a.txt")
来源：http://utg.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://lat.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aqm.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://sal.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kui.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://orr.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://gmw.316326.xyz

C#:   File.Delete("a.txt");
来源：http://udc.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://bnh.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tmb.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iey.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fjs.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zuv.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xvt.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kvz.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nds.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jsb.vqdsnc.cn

[F08] 遍历目录
来源：http://xeb.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ker.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mzw.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://bne.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://omv.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xem.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ygv.birdmap.top

Ruby: Dir.children("dir")
来源：http://lpu.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://ihe.redwolf501.top

[F09] 获取文件大小
来源：http://odz.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://bth.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://ngf.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://mhd.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://tdb.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://zsx.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jgz.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://pxk.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://cmv.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://kgy.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aha.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lnz.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://amv.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://tzp.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yes.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ahs.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aed.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xst.vqdsnc.cn

[F11] 复制与移动文件
来源：http://vjv.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://edw.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rnr.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://obp.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iqn.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vzc.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hwo.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nwa.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dzl.cucudq.cn

[F12] CSV 读写
来源：http://mub.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://edp.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bta.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lor.chenjidiqi.icu

TS:   // 同上
来源：http://ttu.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yvd.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rqk.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vsc.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://itg.jinghuilouyu.cn

================================================================================
来源：http://uwf.gogol.net.cn

G. 面向对象
来源：http://fhz.tianlin.xyz

================================================================================
来源：http://kvb.guowangkeji.top

[G01] 定义类
来源：http://rhm.jyoumei.cn

Py:   class User: pass
来源：http://qos.ivvv.top

PHP:  class User {}
来源：http://brx.ybcxt.top

JS:   class User {}
来源：http://pyt.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://tex.jinghuilouyu.cn

Java: class User {}
来源：http://gha.fengsongda.top

Go:   type User struct { Name string }
来源：http://ifq.sxryk.cn

Ruby: class User; end
来源：http://wnw.ybcxt.top

C#:   class User {}
来源：http://irl.wangdashe.top

[G02] 构造函数
来源：http://hin.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://suj.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://djk.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://nmu.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://lgb.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://wle.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bql.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://yoi.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://uee.hammf.cn

[G03] 实例属性
来源：http://qag.zhiwuduotai.top

Py:   self.name = "x"
来源：http://jeo.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://yri.yfazqb.com

JS:   this.name = "x";
来源：http://bke.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://bfc.sysykeji.top

Java: private String name;
来源：http://fig.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dcy.fktsv.cn

Ruby: @name = "x"
来源：http://wbh.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://itm.zhijiandao.cn

[G04] 定义方法
来源：http://rwb.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://qyj.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://nbm.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://hsz.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://abx.tianlin.xyz

Java: String greet() { return name; }
来源：http://xjh.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tdb.fzhhl.top

Ruby: def greet; @name; end
来源：http://dgi.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://nbd.ppjwa.cn

[G05] 继承
来源：http://gnn.vehdjk.com

Py:   class Admin(User): pass
来源：http://aje.nwbrower.top

PHP:  class Admin extends User {}
来源：http://olc.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://uqp.hysaishi.cn

TS:   class Admin extends User {}
来源：http://ssq.yanxiufei.cn

Java: class Admin extends User {}
来源：http://iiu.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cph.xinyue.icu

Ruby: class Admin < User; end
来源：http://jar.meibo888.top

C#:   class Admin : User {}
来源：http://qgb.52xcode.cn

[G06] 重写方法
来源：http://sef.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://wys.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sqy.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://mvo.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://ttv.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://zmr.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rqq.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://svy.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://eji.haohaochexian.top

[G07] 调用父类方法
来源：http://ogu.andypj.xyz

Py:   super().greet()
来源：http://rme.cqqwz.cn

PHP:  parent::greet();
来源：http://ilf.havefunace.top

JS:   super.greet();
来源：http://wzy.jianghu66.top

TS:   super.greet();
来源：http://vhh.tanke756.top

Java: super.greet();
来源：http://etx.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fee.epnwcf.com

Ruby: super
来源：http://pwq.316326.xyz

C#:   base.Greet();
来源：http://cuf.hfpthk.cn

[G08] 静态方法与属性
来源：http://poy.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lwg.fzhhl.top

PHP:  public static function f() {}
来源：http://izs.shuidangran.top

JS:   static f() {}
来源：http://pzy.guowangkeji.top

TS:   static f(): void {}
来源：http://tlo.xuanzx.com

Java: static void f() {}
来源：http://lcr.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nxf.tarul.cn

Ruby: def self.f; end
来源：http://yzz.yueranfly.top

C#:   public static void F() {}
来源：http://ohe.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://rie.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://boe.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://odp.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ecm.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://nvg.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://jau.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://dur.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gbr.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://sor.yueranfly.top

[G10] 访问控制
来源：http://arj.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://nbh.pengpengdd.cyou

PHP:  public / protected / private
来源：http://ddw.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://bxu.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://miy.cashguo.top

Java: public / protected / private / 默认包级
来源：http://xlc.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qlx.chenlongwang.top

Ruby: public / protected / private
来源：http://qbn.meibo888.top

C#:   public / protected / private / internal
来源：http://grs.fehbvm.com

[G11] getter / setter
来源：http://ajq.zycfv.cn

Py:   @property 与 @x.setter
来源：http://ier.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://nen.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://noz.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://pef.daxiang520.top

Java: public String getName() { return name; }
来源：http://dqq.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hau.cucudq.cn

Ruby: attr_accessor :name
来源：http://yon.sweek.top

C#:   public string Name { get; set; }
来源：http://xxt.sufxvd.cn

[G12] 对象转字符串
来源：http://zrm.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://jkd.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xtw.nwbrower.top

JS:   toString() { return this.name; }
来源：http://oxj.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://pvz.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://dbg.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ffo.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://jsb.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://atv.9152youxi.cn

[G13] 判断对象类型
来源：http://cuw.cheryme.top

Py:   isinstance(u, User)
来源：http://brt.zdbjq.cn

PHP:  $u instanceof User
来源：http://lla.gogol.net.cn

JS:   u instanceof User
来源：http://idk.hesvh.cn

TS:   u instanceof User
来源：http://odr.jianghu66.top

Java: u instanceof User
来源：http://dwz.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tgj.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://dhn.haohaochexian.top

C#:   u is User
来源：http://ukg.ydjk.org.cn

[G14] 数据类 / record
来源：http://zwn.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://axj.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://jqp.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://rif.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://rmc.nwbrower.top

Java: record User(String name, int age) {}
来源：http://jnv.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://hdz.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jzi.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://bjo.iojbl.cn

[G15] 枚举
来源：http://asw.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wtx.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://emi.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rfp.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ren.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://fsm.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bvb.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://vjb.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xja.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://jwe.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dui.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://paa.cashguo.top

JS:   Object.entries(obj)
来源：http://aam.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://mxv.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rbf.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xcv.hnqzz.top

Ruby: obj.instance_variables
来源：http://kpz.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://qns.snrcjt.cn

================================================================================
来源：http://bwg.zdqjudy.top

H. 异常与错误处理
来源：http://goc.wangshuangyany.cn

================================================================================
来源：http://rkv.0kj1m.cn

[H01] try / catch 基础
来源：http://kzv.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pcc.vqdsnc.cn


<!-- 参考信息 -->