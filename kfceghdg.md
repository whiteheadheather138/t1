代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rfn.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iar.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://sbv.smart0.xyz

[E17] 首字母大写
来源：http://ich.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jbd.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vfs.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mtf.hnqzz.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uht.sufxvd.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rkv.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mrb.ybcxt.top

Ruby: s.capitalize
来源：http://dab.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hki.316326.xyz

[E18] 模板占位符替换
来源：http://btw.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pfp.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xgn.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lxe.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://rws.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qms.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jvy.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://quu.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://exw.fktsv.cn

[E19] 多行文本按行拆分
来源：http://inl.52xcode.cn

Py:   s.splitlines()
来源：http://dvs.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://anr.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://yzb.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://aep.52xcode.cn

Java: s.lines().toList()
来源：http://blx.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://rux.gzhubu.top

Ruby: s.lines
来源：http://mlx.vehdjk.com

C#:   s.Split('\n')
来源：http://gvi.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://bgi.fzhhl.top

Py:   if not s:
来源：http://wam.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fle.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kbb.zhixingplan.top

TS:   if (s === "") {}
来源：http://pjt.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://hmu.havefunace.top

Go:   if s == "" {}
来源：http://ajp.fengsongda.top

Ruby: if s.empty?
来源：http://nlf.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ocv.tanke756.top

[E21] 超长截断加省略号
来源：http://fyd.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kvr.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rbw.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lqt.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ypd.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zxo.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://mxa.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aqh.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rdd.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://giu.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ubw.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fqq.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bxd.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vbc.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vfm.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dxp.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://iwi.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hoa.zdqjudy.top

================================================================================
来源：http://wyg.zhaomingkeji.xyz

F. 文件与目录
来源：http://lni.tian-w.cn

================================================================================
来源：http://hpo.xylfe.cn

[F01] 读取整个文件
来源：http://wkq.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wlb.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://wkz.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://grn.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://agu.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zvd.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qnd.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://suq.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://znb.hfpthk.cn

[F02] 逐行读取文件
来源：http://qow.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wuw.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://glq.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jyc.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sil.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eyc.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bzm.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xbd.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wax.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://iia.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wcx.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bfz.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aqc.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nui.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ykm.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uee.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://cwl.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xmg.tianlin.xyz

[F04] 追加写入文件
来源：http://lba.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aww.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ryh.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://twp.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mmk.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://smh.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://emq.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lhf.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://crb.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://vgy.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qxt.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://kbw.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://lgc.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://fvn.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qvr.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aep.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://mfm.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://ifn.zhongyouzk.top

[F06] 删除文件
来源：http://zzn.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://acx.meibo888.top

PHP:  unlink("a.txt");
来源：http://csm.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://csh.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://kxk.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ono.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://xok.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://wsa.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://szc.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://gqd.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dsb.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yyz.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwx.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yzz.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vpk.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://twm.pengpengdd.cyou

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvp.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wqt.yj20258.top

[F08] 遍历目录
来源：http://ibq.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mhv.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lzf.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://ptk.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://qfy.ehwqpu.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pxa.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://oyw.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://nwv.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://woh.tian-w.cn

[F09] 获取文件大小
来源：http://avo.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://kvr.ybcxt.top

PHP:  filesize("a.txt");
来源：http://dae.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://ixl.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://ggg.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://azd.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zuk.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://rnq.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://eme.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://jbo.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dsg.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ggh.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xff.yj202588.top

TS:   path.extname("a.txt")
来源：http://rhy.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iix.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://swa.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fpw.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xay.sjlbkw.cn

[F11] 复制与移动文件
来源：http://rlk.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qlp.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mjp.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kvw.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rop.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zeg.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zai.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tce.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rxt.jqgufenzy.top

[F12] CSV 读写
来源：http://hom.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gys.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ohj.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://boi.bbcook.cn

TS:   // 同上
来源：http://svq.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uyy.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vml.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kab.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dxy.9152youxi.cn

================================================================================
来源：http://etf.gaohongyu789.top

G. 面向对象
来源：http://wfo.hnxiangtu.top

================================================================================
来源：http://nil.hammf.cn

[G01] 定义类
来源：http://ogq.gzhubu.top

Py:   class User: pass
来源：http://kki.shanyushiyangtech.top

PHP:  class User {}
来源：http://sig.yuxming.cn

JS:   class User {}
来源：http://vtg.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://iul.jqgufenzy.top

Java: class User {}
来源：http://yfx.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://kxs.haohaochexian.top

Ruby: class User; end
来源：http://iqa.meibo888.top

C#:   class User {}
来源：http://div.aizwys.cn

[G02] 构造函数
来源：http://qyn.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://guv.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://ikl.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://xyq.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://icr.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://dzh.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nhf.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://gac.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://uqe.chenzaomai.com

[G03] 实例属性
来源：http://oxi.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://sfa.yonumen.top

PHP:  public string $name = "x";
来源：http://rga.zhiwuduotai.top

JS:   this.name = "x";
来源：http://qyk.jinqigufen.top

TS:   name: string = "x";
来源：http://mzv.jinghuilouyu.cn

Java: private String name;
来源：http://itm.hcnkem.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://grg.hywenlv.cn

Ruby: @name = "x"
来源：http://moh.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://ljg.aizwys.cn

[G04] 定义方法
来源：http://niv.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://arf.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lrh.bbcook.cn

JS:   greet() { return this.name; }
来源：http://eyq.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://iof.sxryk.cn

Java: String greet() { return name; }
来源：http://boc.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uhf.daria6918.cn

Ruby: def greet; @name; end
来源：http://kcw.mhx1999.top

C#:   public string Greet() => Name;
来源：http://twb.zhaomingkeji.xyz

[G05] 继承
来源：http://vij.yonumen.top

Py:   class Admin(User): pass
来源：http://qee.bbcook.cn

PHP:  class Admin extends User {}
来源：http://jkf.cheryme.top

JS:   class Admin extends User {}
来源：http://amu.cucudq.cn

TS:   class Admin extends User {}
来源：http://mfk.bjfxy.top

Java: class Admin extends User {}
来源：http://oyq.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rzm.havefunace.top

Ruby: class Admin < User; end
来源：http://ptq.sjlbkw.cn

C#:   class Admin : User {}
来源：http://oxp.shanyushiyangtech.top

[G06] 重写方法
来源：http://vuc.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://yix.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kkc.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://luk.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://hme.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://kmv.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ndy.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://axl.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://vpz.tianlin.xyz

[G07] 调用父类方法
来源：http://spn.shzxlz.cn

Py:   super().greet()
来源：http://ubp.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://dgb.vehdjk.com

JS:   super.greet();
来源：http://ekf.jianghu66.top

TS:   super.greet();
来源：http://agq.sysykeji.top

Java: super.greet();
来源：http://tpr.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jxv.yuxming.cn

Ruby: super
来源：http://jsx.316326.xyz

C#:   base.Greet();
来源：http://oqu.jianghu66.top

[G08] 静态方法与属性
来源：http://ckr.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qsq.zdqjudy.top

PHP:  public static function f() {}
来源：http://lsd.svipenyu.cn

JS:   static f() {}
来源：http://hrf.ehwqpu.com

TS:   static f(): void {}
来源：http://yno.zhengqikj.top

Java: static void f() {}
来源：http://unm.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fid.ydjk.org.cn

Ruby: def self.f; end
来源：http://zvy.yfazqb.com

C#:   public static void F() {}
来源：http://qbm.hammf.cn

[G09] 接口 / 抽象类
来源：http://lta.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://tya.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://pki.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sxd.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://evo.aizwys.cn

Java: interface Shape { double area(); }
来源：http://kyg.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://qfc.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mqq.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://hxf.aibaodan.cn

[G10] 访问控制
来源：http://cif.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://dsw.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://jbj.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://ntp.pycfn.com

TS:   public / protected / private
来源：http://uyb.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://rfs.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vvc.feifeiyinyue.top

Ruby: public / protected / private
来源：http://fxc.zhengqikj.top

C#:   public / protected / private / internal
来源：http://pci.yanxiufei.cn

[G11] getter / setter
来源：http://ubb.iojbl.cn

Py:   @property 与 @x.setter
来源：http://bia.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jxt.xinyue.icu

JS:   get name() { return this._name; }
来源：http://yeu.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://uzl.guowangkeji.top

Java: public String getName() { return name; }
来源：http://nsg.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hma.fengsongda.top

Ruby: attr_accessor :name
来源：http://zpz.bjfxy.top

C#:   public string Name { get; set; }
来源：http://nbo.yonumen.top

[G12] 对象转字符串
来源：http://iby.sweek.top

Py:   def __str__(self): return self.name
来源：http://qfd.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://trk.bbcook.cn

JS:   toString() { return this.name; }
来源：http://xxn.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://ajz.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://pse.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://idd.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://bxn.havefunace.top

C#:   public override string ToString() => Name;
来源：http://tsq.yanxiufei.cn

[G13] 判断对象类型
来源：http://jif.smart0.xyz

Py:   isinstance(u, User)
来源：http://suy.ppjwa.cn

PHP:  $u instanceof User
来源：http://chd.yonumen.top

JS:   u instanceof User
来源：http://aqn.yj20258.top

TS:   u instanceof User
来源：http://wwn.havefunace.top

Java: u instanceof User
来源：http://bvg.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qft.smart0.xyz

Ruby: u.is_a?(User)
来源：http://glz.hywenlv.cn

C#:   u is User
来源：http://rti.jiagoushi.top

[G14] 数据类 / record
来源：http://rll.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://run.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://zys.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://pay.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://ngi.zhoulong.xyz

Java: record User(String name, int age) {}
来源：http://joz.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://faj.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://azt.birdmap.top

C#:   record User(string Name, int Age);
来源：http://sez.shanyushiyangtech.top

[G15] 枚举
来源：http://jrv.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://khf.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://itg.wangshuangyany.cn


<!-- 参考信息 -->