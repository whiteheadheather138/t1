代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qtt.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hky.hesvh.cn

TS:   if (s === "") {}
来源：http://ipe.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://rev.nanxuanxn.top

Go:   if s == "" {}
来源：http://fan.ivvv.top

Ruby: if s.empty?
来源：http://dbf.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fyc.yangfankeji.com

[E21] 超长截断加省略号
来源：http://pql.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pyz.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eqt.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xqm.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzv.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://amv.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://qjn.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pfh.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sid.uphjek.com

[E22] 字节长度与字符长度
来源：http://wcq.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mah.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://whv.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jte.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fez.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ine.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pec.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://asv.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dhh.zdqjudy.top

================================================================================
来源：http://dmt.bjfxy.top

F. 文件与目录
来源：http://jzw.chenlongwang.top

================================================================================
来源：http://bqo.pengpengdd.cyou

[F01] 读取整个文件
来源：http://ymm.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cwe.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://gfb.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ghp.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://okx.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fkr.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nbi.yongpay.top

Ruby: File.read("a.txt")
来源：http://ycg.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://cxb.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://vpt.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://giw.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uko.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zsj.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tfu.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wkf.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://okv.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lvo.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mgw.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://dpm.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oeh.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hia.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tkt.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gik.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sjt.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://plu.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://rdy.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xca.shuidangran.top

[F04] 追加写入文件
来源：http://nvv.chenzaomai.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xbm.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tgq.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qnf.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://evn.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://poc.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fnf.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vyd.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ewv.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://gnz.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ukd.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://dfs.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://vyj.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://dhz.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ruf.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nvm.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://hpl.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://tmv.tian-w.cn

[F06] 删除文件
来源：http://aah.mhx1999.top

Py:   os.remove("a.txt")
来源：http://evd.c1oappe.top

PHP:  unlink("a.txt");
来源：http://dck.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aob.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://bkf.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hfc.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://uxg.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://mfc.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://nnw.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://tpl.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pfh.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ecl.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ipz.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ode.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vlp.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aly.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bmt.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zam.zycfv.cn

[F08] 遍历目录
来源：http://vsl.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xsh.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vbx.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://skk.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://mnc.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mzd.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://unt.fehbvm.com

Ruby: Dir.children("dir")
来源：http://kpg.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://vvi.yueranfly.top

[F09] 获取文件大小
来源：http://ebg.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://ztx.havefunace.top

PHP:  filesize("a.txt");
来源：http://ist.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://evt.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://vxx.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://ice.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://miv.yvedp.cn

Ruby: File.size("a.txt")
来源：http://lci.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://kqf.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://gtk.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gia.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jqg.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dbt.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://qum.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://adv.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lzf.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oln.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jnn.zdqjudy.top

[F11] 复制与移动文件
来源：http://rrn.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bbz.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ndp.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dbs.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fqy.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wbj.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uhc.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hce.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ect.chenzaomai.com

[F12] CSV 读写
来源：http://kyd.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nxx.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ynw.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://inq.shanyushiyangkeji.top

TS:   // 同上
来源：http://xgx.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bvp.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://esg.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bfe.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lni.yueranfly.top

================================================================================
来源：http://qdb.smart0.xyz

G. 面向对象
来源：http://blg.gaohongyu789.top

================================================================================
来源：http://xma.fzhhl.top

[G01] 定义类
来源：http://lxv.xinyue.icu

Py:   class User: pass
来源：http://oau.chenjidiqi.icu

PHP:  class User {}
来源：http://cpn.zhengqikj.top

JS:   class User {}
来源：http://uhq.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://fvm.epnwcf.com

Java: class User {}
来源：http://enz.gzhubu.top

Go:   type User struct { Name string }
来源：http://ejp.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://tdy.yueranfly.top

C#:   class User {}
来源：http://evr.yj20258888.top

[G02] 构造函数
来源：http://kic.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://pot.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ucf.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://wrw.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://hzv.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://lee.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oav.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://wfk.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://fhi.hcnkem.com

[G03] 实例属性
来源：http://qwm.jiagoushi.top

Py:   self.name = "x"
来源：http://vuj.daxiang520.top

PHP:  public string $name = "x";
来源：http://bod.tanke756.top

JS:   this.name = "x";
来源：http://kxn.sxryk.cn

TS:   name: string = "x";
来源：http://aru.yanxiufei.cn

Java: private String name;
来源：http://wbd.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xpk.jiagoushi.top

Ruby: @name = "x"
来源：http://xft.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://ijq.gogol.net.cn

[G04] 定义方法
来源：http://nfi.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://tvv.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://axr.shuidangran.top

JS:   greet() { return this.name; }
来源：http://wzu.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://awh.fehbvm.com

Java: String greet() { return name; }
来源：http://itw.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://psc.tian-w.cn

Ruby: def greet; @name; end
来源：http://tnp.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://tio.jlsjyb.cn

[G05] 继承
来源：http://mfm.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://nzr.ivvv.top

PHP:  class Admin extends User {}
来源：http://gbs.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://ten.ctjpmb.com

TS:   class Admin extends User {}
来源：http://yoi.svipenyu.cn

Java: class Admin extends User {}
来源：http://ose.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kcq.wangdashe.top

Ruby: class Admin < User; end
来源：http://mab.zhengqikj.top

C#:   class Admin : User {}
来源：http://fci.yj202588.top

[G06] 重写方法
来源：http://fdw.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://knh.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zfa.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://qxi.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://okc.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://efw.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xly.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://kgv.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://sjo.sxryk.cn

[G07] 调用父类方法
来源：http://dcn.shanyushiyangkeji.top

Py:   super().greet()
来源：http://rdg.hysaishi.cn

PHP:  parent::greet();
来源：http://weq.haohaochexian.top

JS:   super.greet();
来源：http://ehl.jinqigufen.top

TS:   super.greet();
来源：http://vcc.fanxiaobao.xyz

Java: super.greet();
来源：http://dml.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://upj.shuidangran.top

Ruby: super
来源：http://rsa.0kj1m.cn

C#:   base.Greet();
来源：http://bhm.316326.xyz

[G08] 静态方法与属性
来源：http://xzt.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bku.yongpay.top

PHP:  public static function f() {}
来源：http://hml.ehwqpu.com

JS:   static f() {}
来源：http://fex.chenjidiqi.icu

TS:   static f(): void {}
来源：http://dzj.yj202588.top

Java: static void f() {}
来源：http://fgz.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://joh.zhixingplan.top

Ruby: def self.f; end
来源：http://pew.jianghu66.top

C#:   public static void F() {}
来源：http://ebt.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://yqt.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://vqd.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://sqi.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kvt.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://osx.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://btt.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://yyk.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xas.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://wdu.xuetiantiany.cn

[G10] 访问控制
来源：http://ifx.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://ury.fktsv.cn

PHP:  public / protected / private
来源：http://iqf.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://ezj.hnqzz.top

TS:   public / protected / private
来源：http://bek.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://ybr.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://bxh.smart0.xyz

Ruby: public / protected / private
来源：http://mbl.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://xmk.c1oappe.top

[G11] getter / setter
来源：http://fhw.yongpay.top

Py:   @property 与 @x.setter
来源：http://bab.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pvm.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://ner.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://fbq.yongpay.top

Java: public String getName() { return name; }
来源：http://gdc.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://xdn.smart0.xyz

Ruby: attr_accessor :name
来源：http://glo.tianlin.xyz

C#:   public string Name { get; set; }
来源：http://ott.ydzc1.top

[G12] 对象转字符串
来源：http://vpo.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://cgx.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://roc.yj202588.top

JS:   toString() { return this.name; }
来源：http://ius.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://vrk.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://zmc.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://amo.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://aso.cashguo.top

C#:   public override string ToString() => Name;
来源：http://car.iojbl.cn

[G13] 判断对象类型
来源：http://bih.ppjwa.cn

Py:   isinstance(u, User)
来源：http://eeg.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://wkn.tian-w.cn

JS:   u instanceof User
来源：http://evh.fehbvm.com

TS:   u instanceof User
来源：http://bok.hesvh.cn

Java: u instanceof User
来源：http://ojc.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://zdz.bbcook.cn

Ruby: u.is_a?(User)
来源：http://dbj.jlsjyb.cn

C#:   u is User
来源：http://wmu.pycfn.com

[G14] 数据类 / record
来源：http://sja.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://luf.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://eiw.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://thw.sweek.top

TS:   type User = { name: string; age: number };
来源：http://jpw.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://lin.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://qvy.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cmd.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://rtd.sweek.top

[G15] 枚举
来源：http://blf.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ozv.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xdo.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eyo.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bka.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://eio.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://swb.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://vfr.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cml.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://gpm.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cfv.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://ixc.dianchejie.cn

JS:   Object.entries(obj)
来源：http://pna.yonumen.top

TS:   Object.entries(obj)
来源：http://mhk.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://awq.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ruk.haohaochexian.top

Ruby: obj.instance_variables
来源：http://bkp.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://hpi.aizwys.cn

================================================================================
来源：http://now.bbcook.cn

H. 异常与错误处理
来源：http://ass.vehdjk.com

================================================================================
来源：http://xbh.yonumen.top

[H01] try / catch 基础
来源：http://avk.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cdf.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nri.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://szx.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xwk.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ioi.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xpr.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wjo.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tve.vehdjk.com

[H02] finally / ensure 收尾
来源：http://nqo.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://hug.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://glo.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dsj.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://blv.hammf.cn


<!-- 参考信息 -->