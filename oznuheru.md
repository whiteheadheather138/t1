代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://afb.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://wez.fengsongda.top

Py:   s.splitlines()
来源：http://ogk.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jts.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://pxh.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://kws.ybcxt.top

Java: s.lines().toList()
来源：http://wpq.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://col.hcnkem.com

Ruby: s.lines
来源：http://mfp.fzhhl.top

C#:   s.Split('\n')
来源：http://ueo.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://ofj.nwbrower.top

Py:   if not s:
来源：http://atk.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ztq.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://omy.ydjk.org.cn

TS:   if (s === "") {}
来源：http://suh.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://ggg.chenjidiqi.icu

Go:   if s == "" {}
来源：http://ryt.ehwqpu.com

Ruby: if s.empty?
来源：http://mql.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://frv.daria6918.cn

[E21] 超长截断加省略号
来源：http://mzj.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dot.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jhd.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sdo.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pmh.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://haq.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://drr.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axx.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hax.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://kef.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gbv.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqr.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eqo.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ytw.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cet.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pgd.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://kee.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sgq.shuidangran.top

================================================================================
来源：http://sve.yanxiufei.cn

F. 文件与目录
来源：http://zpu.hnqzz.top

================================================================================
来源：http://nbj.pengpengdd.cyou

[F01] 读取整个文件
来源：http://dnz.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bwf.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://frg.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wya.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wdu.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://njz.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wnv.sysykeji.top

Ruby: File.read("a.txt")
来源：http://wyc.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://gdk.hywenlv.cn

[F02] 逐行读取文件
来源：http://ttq.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tnu.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jzz.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nql.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rhk.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hei.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lcr.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kez.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hyr.uphjek.com

[F03] 写入文件（覆盖）
来源：http://ocs.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fpj.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ogq.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zyi.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fbd.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kop.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tho.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://med.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hjq.yuxming.cn

[F04] 追加写入文件
来源：http://qrc.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nhg.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wso.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npa.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://shq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yag.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jdy.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ntg.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bzk.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://ske.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ugy.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://ggg.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://fgd.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://lts.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mqw.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kby.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://qka.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://tyx.zhengqikj.top

[F06] 删除文件
来源：http://ygz.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://zdz.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://hcx.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://knn.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://res.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yfy.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://usy.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://iht.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://ppk.yj20258.top

[F07] 创建目录（含多级）
来源：http://ugp.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://opz.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cua.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ykz.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tlz.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jli.epnwcf.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aoy.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bic.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tzf.aizwys.cn

[F08] 遍历目录
来源：http://rom.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lnr.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vmm.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://beq.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://fie.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tfj.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ldl.hnqzz.top

Ruby: Dir.children("dir")
来源：http://stf.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://gvx.gaohongyu789.top

[F09] 获取文件大小
来源：http://dvz.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://bqz.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://ltf.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://tfp.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://ubn.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://nsh.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xal.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://ysq.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://mra.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://wii.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qsy.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xlz.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wms.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://avy.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yxg.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wkt.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iat.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwh.guowangkeji.top

[F11] 复制与移动文件
来源：http://nlk.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fyj.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tgy.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ood.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nct.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iyg.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dsa.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gjq.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mhp.ivvv.top

[F12] CSV 读写
来源：http://dhj.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tpb.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nuq.yj20258888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rnf.zhongyouzk.top

TS:   // 同上
来源：http://vmx.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://usl.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ais.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aar.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wre.kuanghao11.cn

================================================================================
来源：http://hyj.hnqzz.top

G. 面向对象
来源：http://iiv.haohaochexian.top

================================================================================
来源：http://cwc.uphjek.com

[G01] 定义类
来源：http://hmn.c1oappe.top

Py:   class User: pass
来源：http://paa.xziqi.cn

PHP:  class User {}
来源：http://ryb.hnxiangtu.top

JS:   class User {}
来源：http://aev.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://cih.sufxvd.cn

Java: class User {}
来源：http://nsv.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://sbx.zycfv.cn

Ruby: class User; end
来源：http://gvq.shanyushiyangtech.top

C#:   class User {}
来源：http://xoe.ydjk.org.cn

[G02] 构造函数
来源：http://jee.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://oyr.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://aqt.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://bjg.ivvv.top

TS:   constructor(public name: string) {}
来源：http://adz.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://tou.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nel.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://eir.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://vsd.shanyushiyangkeji.top

[G03] 实例属性
来源：http://knn.yj20258888.top

Py:   self.name = "x"
来源：http://klk.ybcxt.top

PHP:  public string $name = "x";
来源：http://oie.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://oqa.sweek.top

TS:   name: string = "x";
来源：http://xiq.xziqi.cn

Java: private String name;
来源：http://zqz.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uru.zhengqikj.top

Ruby: @name = "x"
来源：http://jht.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://ibf.jinqigufen.top

[G04] 定义方法
来源：http://ucl.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://cau.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nci.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://euw.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://zvq.chenzaomai.com

Java: String greet() { return name; }
来源：http://lfy.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ftf.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://twl.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://unt.zdbjq.cn

[G05] 继承
来源：http://ymf.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://tsc.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://nmd.gotoacloud.top

JS:   class Admin extends User {}
来源：http://ziu.ppjwa.cn

TS:   class Admin extends User {}
来源：http://dre.yvedp.cn

Java: class Admin extends User {}
来源：http://adq.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://psg.cucudq.cn

Ruby: class Admin < User; end
来源：http://njl.jqgfzy.top

C#:   class Admin : User {}
来源：http://awi.nanxinkj.top

[G06] 重写方法
来源：http://iki.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://uox.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ibb.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://cbn.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://uek.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://wja.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yqe.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://pjp.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://gtm.zycfv.cn

[G07] 调用父类方法
来源：http://rhk.snrcjt.cn

Py:   super().greet()
来源：http://ogc.yonumen.top

PHP:  parent::greet();
来源：http://pfk.jianghu66.top

JS:   super.greet();
来源：http://ttz.xuetiantiany.cn

TS:   super.greet();
来源：http://bjr.zdbjq.cn

Java: super.greet();
来源：http://mhk.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gaw.iojbl.cn

Ruby: super
来源：http://ghb.snrcjt.cn

C#:   base.Greet();
来源：http://une.zhixingplan.top

[G08] 静态方法与属性
来源：http://ulc.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yhn.xinyue.icu

PHP:  public static function f() {}
来源：http://vbg.pycfn.com

JS:   static f() {}
来源：http://lps.jlsjyb.cn

TS:   static f(): void {}
来源：http://swb.pengpengdd.cyou

Java: static void f() {}
来源：http://rvh.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ocw.chenzaomai.com

Ruby: def self.f; end
来源：http://hip.yangfankeji.com

C#:   public static void F() {}
来源：http://xyd.pycfn.com

[G09] 接口 / 抽象类
来源：http://ycj.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://vqu.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://nqg.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cdc.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://syo.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://nje.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://mnx.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fzh.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://llx.snrcjt.cn

[G10] 访问控制
来源：http://crx.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://qyf.guannengcc.top

PHP:  public / protected / private
来源：http://eey.sysykeji.top

JS:   #private 字段；其余公开
来源：http://duy.yvedp.cn

TS:   public / protected / private
来源：http://vhb.meibo888.top

Java: public / protected / private / 默认包级
来源：http://cio.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xyq.xinyue.icu

Ruby: public / protected / private
来源：http://nhs.guannengcc.top

C#:   public / protected / private / internal
来源：http://ghp.tian-w.cn

[G11] getter / setter
来源：http://tvc.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://ilf.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://juy.sweek.top

JS:   get name() { return this._name; }
来源：http://wya.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://bnk.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://snt.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ovh.fehbvm.com

Ruby: attr_accessor :name
来源：http://dmt.fktsv.cn

C#:   public string Name { get; set; }
来源：http://jqt.zdbjq.cn

[G12] 对象转字符串
来源：http://lrs.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://umf.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://puq.tian-w.cn

JS:   toString() { return this.name; }
来源：http://hla.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://akj.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://dwd.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hcy.xuanzx.com

Ruby: def to_s; @name; end
来源：http://woj.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://suc.smart0.xyz

[G13] 判断对象类型
来源：http://bit.c1oappe.top

Py:   isinstance(u, User)
来源：http://ork.yongpay.top

PHP:  $u instanceof User
来源：http://dtn.jyoumei.cn

JS:   u instanceof User
来源：http://glb.aizwys.cn

TS:   u instanceof User
来源：http://jma.svipenyu.cn

Java: u instanceof User
来源：http://zeh.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://qvv.fktsv.cn

Ruby: u.is_a?(User)
来源：http://ibd.9152youxi.cn

C#:   u is User
来源：http://bwj.fktsv.cn

[G14] 数据类 / record
来源：http://sar.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ffm.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://niy.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://arx.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://wom.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://sdp.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://ajl.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jbi.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://dqn.ydjk.org.cn

[G15] 枚举
来源：http://qhq.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zxc.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qkc.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eun.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bjw.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://klg.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rih.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://wbk.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fze.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://arp.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wgy.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://kjs.hcnkem.com

JS:   Object.entries(obj)
来源：http://ybo.zhixingplan.top

TS:   Object.entries(obj)
来源：http://wtr.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ubi.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ihi.sweek.top

Ruby: obj.instance_variables
来源：http://sks.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://bti.yuxming.cn

================================================================================
来源：http://upp.xziqi.cn

H. 异常与错误处理
来源：http://dlx.zhijiandao.cn

================================================================================
来源：http://tgo.c1oappe.top

[H01] try / catch 基础
来源：http://nkv.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bwf.hywenlv.cn


<!-- 参考信息 -->