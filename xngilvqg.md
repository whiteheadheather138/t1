代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oxo.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iqv.jiagoushi.top

Ruby: s.capitalize
来源：http://ppa.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gae.jyoumei.cn

[E18] 模板占位符替换
来源：http://sqm.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ylx.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zqm.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://low.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fpv.yueranfly.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ktx.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dxz.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ydi.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fji.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://iau.cheryme.top

Py:   s.splitlines()
来源：http://bht.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://voh.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://gug.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://phs.9152youxi.cn

Java: s.lines().toList()
来源：http://vgr.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://mfa.c1oappe.top

Ruby: s.lines
来源：http://jzv.xylfe.cn

C#:   s.Split('\n')
来源：http://mzo.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://usn.jqgufenzy.top

Py:   if not s:
来源：http://onk.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ibb.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mme.yj20258.top

TS:   if (s === "") {}
来源：http://aom.zhiwuduotai.top

Java: if (s.isEmpty()) {}
来源：http://gke.redwolf501.top

Go:   if s == "" {}
来源：http://qxy.gaohongyu789.top

Ruby: if s.empty?
来源：http://eni.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nfg.ivvv.top

[E21] 超长截断加省略号
来源：http://ewk.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ahb.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ikf.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yvl.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wsn.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rit.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://vzu.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wjf.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gxy.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://mtk.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hhx.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uxu.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vrn.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://evn.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zwb.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qmk.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://hfe.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cya.tarul.cn

================================================================================
来源：http://cjr.hcnkem.com

F. 文件与目录
来源：http://mck.feifeiyinyue.top

================================================================================
来源：http://vpz.tian-w.cn

[F01] 读取整个文件
来源：http://ucm.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wcu.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://kzn.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lxg.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kre.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vhp.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mys.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://lbq.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://dox.52xcode.cn

[F02] 逐行读取文件
来源：http://fvs.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sdk.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://whb.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kla.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qmf.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mzi.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wdg.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qqr.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mpd.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://wds.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qyt.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ceh.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hba.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfp.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fjw.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wyv.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://gdj.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zzz.guannengcc.top

[F04] 追加写入文件
来源：http://wag.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sqg.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pjm.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xao.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nwz.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vfm.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dxd.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://twz.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jkg.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://rso.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ujv.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://pnw.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://ldg.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://sqi.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nae.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kja.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://tcv.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://pks.ctjpmb.com

[F06] 删除文件
来源：http://ntu.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://sey.ybcxt.top

PHP:  unlink("a.txt");
来源：http://sgj.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://iwr.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://twy.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hne.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://myb.pycfn.com

Ruby: File.delete("a.txt")
来源：http://axi.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://cju.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://gdk.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ioo.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xno.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mkn.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zfh.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://khl.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jaw.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gnq.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oen.yonumen.top

[F08] 遍历目录
来源：http://vtf.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pzr.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rfh.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://bkb.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://jop.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jke.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zeo.yonumen.top

Ruby: Dir.children("dir")
来源：http://aow.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://vns.smart0.xyz

[F09] 获取文件大小
来源：http://qmw.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://eqq.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://szk.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://znq.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://stu.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://qwj.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xit.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://zds.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://psz.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://lhw.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://huz.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mdh.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tjc.fengsongda.top

TS:   path.extname("a.txt")
来源：http://sju.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://btw.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dnz.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fei.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dnd.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://jml.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kum.shanyushiyangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://auw.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://coz.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qqb.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://krb.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mhi.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://set.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dse.tarul.cn

[F12] CSV 读写
来源：http://yxz.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zjy.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tci.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wzi.hammf.cn

TS:   // 同上
来源：http://htt.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lrh.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://frl.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rok.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jcv.vqdsnc.cn

================================================================================
来源：http://bdo.fengsongda.top

G. 面向对象
来源：http://vms.bjfxy.top

================================================================================
来源：http://wye.fehbvm.com

[G01] 定义类
来源：http://wcl.fehbvm.com

Py:   class User: pass
来源：http://xwq.svipenyu.cn

PHP:  class User {}
来源：http://rcx.kuanghao11.cn

JS:   class User {}
来源：http://ohp.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://zjo.ydjk.org.cn

Java: class User {}
来源：http://dzp.epnwcf.com

Go:   type User struct { Name string }
来源：http://xeo.nanxuanxn.top

Ruby: class User; end
来源：http://yhp.quarkkingdee.top

C#:   class User {}
来源：http://erj.cashguo.top

[G02] 构造函数
来源：http://zwu.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://gtf.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://dkv.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://kye.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://rbh.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://nrk.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://weo.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://tdf.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://qzt.ydjk.org.cn

[G03] 实例属性
来源：http://cqc.haohaochexian.top

Py:   self.name = "x"
来源：http://mso.chenzaomai.com

PHP:  public string $name = "x";
来源：http://rnn.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://fik.yangfankeji.com

TS:   name: string = "x";
来源：http://ina.epnwcf.com

Java: private String name;
来源：http://kmf.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hpv.fengsongda.top

Ruby: @name = "x"
来源：http://pfl.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://bls.smart0.xyz

[G04] 定义方法
来源：http://cnf.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://wdx.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ikc.ybcxt.top

JS:   greet() { return this.name; }
来源：http://vqs.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://reh.jinqigufen.top

Java: String greet() { return name; }
来源：http://jei.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oto.aibaodan.cn

Ruby: def greet; @name; end
来源：http://jye.gzhubu.top

C#:   public string Greet() => Name;
来源：http://tpr.vqdsnc.cn

[G05] 继承
来源：http://tbe.ehwqpu.com

Py:   class Admin(User): pass
来源：http://jfu.tarul.cn

PHP:  class Admin extends User {}
来源：http://jvj.hfpthk.cn

JS:   class Admin extends User {}
来源：http://lut.xuanzx.com

TS:   class Admin extends User {}
来源：http://idt.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://rkp.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lnw.zdbjq.cn

Ruby: class Admin < User; end
来源：http://rvr.tanke756.top

C#:   class Admin : User {}
来源：http://kig.epnwcf.com

[G06] 重写方法
来源：http://hil.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://uxc.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://esr.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://tpn.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://fwa.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://gnv.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zbz.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://wru.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://fpp.cheryme.top

[G07] 调用父类方法
来源：http://asp.shzxlz.cn

Py:   super().greet()
来源：http://xhe.sjlbkw.cn

PHP:  parent::greet();
来源：http://fdr.ctjpmb.com

JS:   super.greet();
来源：http://ekc.gotoacloud.top

TS:   super.greet();
来源：http://lox.gzhubu.top

Java: super.greet();
来源：http://fck.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cql.yonumen.top

Ruby: super
来源：http://mun.hesvh.cn

C#:   base.Greet();
来源：http://kit.jyoumei.cn

[G08] 静态方法与属性
来源：http://fwn.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bqr.zhengqikj.top

PHP:  public static function f() {}
来源：http://dsp.zhixingplan.top

JS:   static f() {}
来源：http://lwe.sjlbkw.cn

TS:   static f(): void {}
来源：http://nhr.fktsv.cn

Java: static void f() {}
来源：http://ghy.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wax.jianghu66.top

Ruby: def self.f; end
来源：http://phc.xziqi.cn

C#:   public static void F() {}
来源：http://kmg.yfazqb.com

[G09] 接口 / 抽象类
来源：http://xmn.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://rhz.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://ktw.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sny.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://nuu.hammf.cn

Java: interface Shape { double area(); }
来源：http://rwp.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://xwc.jqgfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dcf.0kj1m.cn

C#:   interface IShape { double Area(); }
来源：http://mcc.zycfv.cn

[G10] 访问控制
来源：http://ceb.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://tup.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://sdx.52xcode.cn

JS:   #private 字段；其余公开
来源：http://jbw.fktsv.cn

TS:   public / protected / private
来源：http://vcn.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://leo.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wck.gotoacloud.top

Ruby: public / protected / private
来源：http://zsv.havefunace.top

C#:   public / protected / private / internal
来源：http://rnh.sxryk.cn

[G11] getter / setter
来源：http://yka.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://jmq.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://mmr.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://lmk.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://sok.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://imb.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hbx.sysykeji.top

Ruby: attr_accessor :name
来源：http://xal.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://qjm.wangshuangyany.cn

[G12] 对象转字符串
来源：http://wyy.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://yqz.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://iwb.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://hnh.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://ugv.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://dkb.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://dbt.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://qcd.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://fjj.yueranfly.top

[G13] 判断对象类型
来源：http://rgv.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://cht.zdbjq.cn

PHP:  $u instanceof User
来源：http://uod.wangshuangyany.cn

JS:   u instanceof User
来源：http://bqo.sysykeji.top

TS:   u instanceof User
来源：http://gyh.jqgufenzy.top

Java: u instanceof User
来源：http://pfs.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jwx.cheryme.top

Ruby: u.is_a?(User)
来源：http://psg.zhaomingkeji.xyz

C#:   u is User
来源：http://ivo.zhongyouzk.top

[G14] 数据类 / record
来源：http://aku.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dnl.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://knz.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://cip.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://rny.yfazqb.com

Java: record User(String name, int age) {}
来源：http://ppb.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://man.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://obd.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://hcj.zhengqikj.top

[G15] 枚举
来源：http://ehe.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zpk.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://evn.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xpz.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://suj.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://nuy.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mlr.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://rgx.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wdj.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://wpy.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ivz.yangfankeji.com


<!-- 参考信息 -->