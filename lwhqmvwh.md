代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hzr.tanke756.top

[E19] 多行文本按行拆分
来源：http://khh.jinqigufen.top

Py:   s.splitlines()
来源：http://tta.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://srq.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://dtx.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://mus.meibo888.top

Java: s.lines().toList()
来源：http://uza.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://dea.jyoumei.cn

Ruby: s.lines
来源：http://rmo.52xcode.cn

C#:   s.Split('\n')
来源：http://kem.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://rid.meibo888.top

Py:   if not s:
来源：http://ihw.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dif.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://orz.nanxuanxn.top

TS:   if (s === "") {}
来源：http://oai.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://vfw.tanke756.top

Go:   if s == "" {}
来源：http://esk.jinqigfzy.top

Ruby: if s.empty?
来源：http://qtt.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oig.bjfxy.top

[E21] 超长截断加省略号
来源：http://ulq.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bsu.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nsa.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cxo.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hco.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://krg.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://bsg.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gwo.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pgw.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://mlt.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://puz.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bck.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kni.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kvh.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ejx.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://twi.haohaochexian.top

Ruby: s.bytesize;  s.length
来源：http://wlv.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://umc.ywan-chungtsiang.top

================================================================================
来源：http://lfj.shuidangran.top

F. 文件与目录
来源：http://qbn.cqqwz.cn

================================================================================
来源：http://isz.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://ggw.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sgf.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://rcp.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rab.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://reu.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://tzi.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jbl.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://odr.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://sbu.yfazqb.com

[F02] 逐行读取文件
来源：http://qqi.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csh.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qkj.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gsw.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rnx.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vni.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ygf.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nxi.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ujq.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://pbi.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bbh.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gdl.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npk.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xch.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mey.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ghw.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://tln.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fpm.iojbl.cn

[F04] 追加写入文件
来源：http://htj.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gfb.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hvi.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdz.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://krb.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cjk.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wba.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qxi.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://szi.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://kav.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lki.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://jpk.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://bly.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://vez.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dfg.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rjv.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://eqv.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://mgq.meibo888.top

[F06] 删除文件
来源：http://gfu.xylfe.cn

Py:   os.remove("a.txt")
来源：http://bhz.tian-w.cn

PHP:  unlink("a.txt");
来源：http://gdx.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://skx.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ymj.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wka.birdmap.top

Go:   os.Remove("a.txt")
来源：http://nlr.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://njx.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://cgx.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://xcw.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fnn.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ohw.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rru.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wbs.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gzq.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sbt.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jxg.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kkf.cucudq.cn

[F08] 遍历目录
来源：http://pai.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lio.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bab.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://rcf.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://vyg.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nfq.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fep.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://yks.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://ucx.sweek.top

[F09] 获取文件大小
来源：http://gyr.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://rgq.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://xah.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://uru.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://not.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://hjy.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hwe.bjfxy.top

Ruby: File.size("a.txt")
来源：http://gdj.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://lyt.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ows.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fvm.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wcz.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sxn.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://nps.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gxk.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ull.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baj.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ehw.hongshengwenyu.top

[F11] 复制与移动文件
来源：http://eln.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lyr.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uga.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://efl.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzg.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://koy.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fcl.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nor.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wjl.dashuyun.cn

[F12] CSV 读写
来源：http://ati.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ppq.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ffk.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bgk.xinyue.icu

TS:   // 同上
来源：http://pow.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://prh.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hsv.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xzu.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://eej.fzhhl.top

================================================================================
来源：http://cvj.zycfv.cn

G. 面向对象
来源：http://qsh.zhiwuduotai.top

================================================================================
来源：http://ngp.nanxinkj.top

[G01] 定义类
来源：http://pjg.cucudq.cn

Py:   class User: pass
来源：http://qck.jinyuanbaomall.cn

PHP:  class User {}
来源：http://eog.yj20258888.top

JS:   class User {}
来源：http://ogy.cheryme.top

TS:   class User { name: string = ""; }
来源：http://lhi.sysykeji.top

Java: class User {}
来源：http://dtf.zdqjudy.top

Go:   type User struct { Name string }
来源：http://plt.yfazqb.com

Ruby: class User; end
来源：http://tnx.cucudq.cn

C#:   class User {}
来源：http://tue.hfpthk.cn

[G02] 构造函数
来源：http://oim.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://jtj.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://diz.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://lzj.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://fbr.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://jrh.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ffn.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://rrz.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://sja.hesvh.cn

[G03] 实例属性
来源：http://ald.shzxlz.cn

Py:   self.name = "x"
来源：http://duf.birdmap.top

PHP:  public string $name = "x";
来源：http://qwr.xinyue.icu

JS:   this.name = "x";
来源：http://gnb.ctjpmb.com

TS:   name: string = "x";
来源：http://inb.smart0.xyz

Java: private String name;
来源：http://odp.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rdc.fzhhl.top

Ruby: @name = "x"
来源：http://ksb.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://isz.sweek.top

[G04] 定义方法
来源：http://szr.ivvv.top

Py:   def greet(self): return self.name
来源：http://vgj.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pcs.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://ltb.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://pdo.sysykeji.top

Java: String greet() { return name; }
来源：http://wbj.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wlw.vehdjk.com

Ruby: def greet; @name; end
来源：http://mfg.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://szx.cheryme.top

[G05] 继承
来源：http://zaj.tarul.cn

Py:   class Admin(User): pass
来源：http://vuj.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://nqo.haohaochexian.top

JS:   class Admin extends User {}
来源：http://gjn.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://saq.52xcode.cn

Java: class Admin extends User {}
来源：http://kbx.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vzw.jianghu66.top

Ruby: class Admin < User; end
来源：http://vko.xziqi.cn

C#:   class Admin : User {}
来源：http://wsv.c1oappe.top

[G06] 重写方法
来源：http://yvu.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://bgz.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jsp.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://moj.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://boy.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://xfo.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dmf.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://avb.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://ydw.nwbrower.top

[G07] 调用父类方法
来源：http://uym.wangshuangyany.cn

Py:   super().greet()
来源：http://vwn.yangfankeji.com

PHP:  parent::greet();
来源：http://rjd.gogol.net.cn

JS:   super.greet();
来源：http://jou.kuanghao11.cn

TS:   super.greet();
来源：http://njf.zdqjudy.top

Java: super.greet();
来源：http://jlj.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://opw.jlsjyb.cn

Ruby: super
来源：http://avf.vehdjk.com

C#:   base.Greet();
来源：http://mts.vqdsnc.cn

[G08] 静态方法与属性
来源：http://lct.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cxk.snrcjt.cn

PHP:  public static function f() {}
来源：http://fyw.shanyushiyangtech.top

JS:   static f() {}
来源：http://orz.yuxming.cn

TS:   static f(): void {}
来源：http://zlq.gzhubu.top

Java: static void f() {}
来源：http://riy.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qcd.guannengcc.top

Ruby: def self.f; end
来源：http://mmb.hammf.cn

C#:   public static void F() {}
来源：http://aap.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://now.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://kpl.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xgu.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vne.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://yig.meibo888.top

Java: interface Shape { double area(); }
来源：http://zqk.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://lfg.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yru.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://xtn.xinyue.icu

[G10] 访问控制
来源：http://rey.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://vdl.jlsjyb.cn

PHP:  public / protected / private
来源：http://qvt.sysykeji.top

JS:   #private 字段；其余公开
来源：http://sgj.aizwys.cn

TS:   public / protected / private
来源：http://suy.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://hmh.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lav.jinqigfzy.top

Ruby: public / protected / private
来源：http://zvk.jyoumei.cn

C#:   public / protected / private / internal
来源：http://nmd.gotoacloud.top

[G11] getter / setter
来源：http://egx.ybcxt.top

Py:   @property 与 @x.setter
来源：http://rnv.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nwl.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://tqh.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://xsw.yongpay.top

Java: public String getName() { return name; }
来源：http://wfw.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://eni.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://hxj.yuxming.cn

C#:   public string Name { get; set; }
来源：http://uvy.gotoacloud.top

[G12] 对象转字符串
来源：http://ypp.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://ssu.guowangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wnm.xinyue.icu

JS:   toString() { return this.name; }
来源：http://eqd.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://nkk.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://jlj.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mwv.yongpay.top

Ruby: def to_s; @name; end
来源：http://wzz.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://hji.shzxlz.cn

[G13] 判断对象类型
来源：http://wzm.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://grf.jqgufenzy.top

PHP:  $u instanceof User
来源：http://rre.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://mqf.hnxiangtu.top

TS:   u instanceof User
来源：http://gvu.yuxming.cn

Java: u instanceof User
来源：http://jox.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qpo.hesvh.cn

Ruby: u.is_a?(User)
来源：http://hxe.yj20258.top

C#:   u is User
来源：http://syr.yueranfly.top

[G14] 数据类 / record
来源：http://oqv.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qqn.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://sun.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ybh.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://bnw.havefunace.top

Java: record User(String name, int age) {}
来源：http://htv.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://qqe.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zsc.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://nvb.feifeiyinyue.top

[G15] 枚举
来源：http://fha.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mri.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qox.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://giw.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jvv.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://kxp.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cel.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://lzo.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pvf.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://hig.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nzq.havefunace.top

PHP:  get_object_vars($obj);
来源：http://aub.nanxinkj.top

JS:   Object.entries(obj)
来源：http://hzk.pycfn.com

TS:   Object.entries(obj)
来源：http://rsl.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pgo.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jen.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://lxl.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://qux.wangdashe.top

================================================================================
来源：http://xor.sysykeji.top

H. 异常与错误处理
来源：http://hpl.gzhubu.top

================================================================================
来源：http://hkx.52xcode.cn

[H01] try / catch 基础
来源：http://rgq.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wei.jinqigufen.top


<!-- 参考信息 -->