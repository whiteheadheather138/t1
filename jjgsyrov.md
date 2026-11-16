代发 wailian999

PHP:  number_format(1234567);
来源：http://ggm.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cfu.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://szn.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tlp.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jsp.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iwu.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://akj.quarkkingdee.top

[E17] 首字母大写
来源：http://tzz.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ttm.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bcl.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oay.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kkf.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ukq.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wao.52xcode.cn

Ruby: s.capitalize
来源：http://tcl.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wij.ybcxt.top

[E18] 模板占位符替换
来源：http://qtl.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://syb.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vzu.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://veu.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aew.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ppk.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://awb.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ovo.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rrs.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://zhr.zhiwuduotai.top

Py:   s.splitlines()
来源：http://ymg.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kba.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://myv.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://auw.aizwys.cn

Java: s.lines().toList()
来源：http://snp.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://qad.uphjek.com

Ruby: s.lines
来源：http://krr.zhijiandao.cn

C#:   s.Split('\n')
来源：http://dmp.fengsongda.top

[E20] 判断字符串是否为空
来源：http://ana.vqdsnc.cn

Py:   if not s:
来源：http://gts.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dky.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dxd.yongpay.top

TS:   if (s === "") {}
来源：http://zsy.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://pxe.svipenyu.cn

Go:   if s == "" {}
来源：http://hfl.zdqjudy.top

Ruby: if s.empty?
来源：http://zss.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bvr.yueranfly.top

[E21] 超长截断加省略号
来源：http://lbo.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bsh.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bsv.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zaq.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzw.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gdd.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://dio.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rdh.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ycc.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://trk.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aai.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yhh.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lyg.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://liy.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ebz.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lru.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://wtr.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jut.uphjek.com

================================================================================
来源：http://wzn.tanke756.top

F. 文件与目录
来源：http://iec.snrcjt.cn

================================================================================
来源：http://epc.sxryk.cn

[F01] 读取整个文件
来源：http://pxu.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yni.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://ijv.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gge.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yas.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wrv.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qcd.hnqzz.top

Ruby: File.read("a.txt")
来源：http://hvs.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://yly.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://sdo.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fwn.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zut.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rrm.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://glk.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ive.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tzu.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://udo.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwo.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://qrm.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://glv.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://roc.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rgb.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://btg.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fsx.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qwu.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://aig.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oxc.epnwcf.com

[F04] 追加写入文件
来源：http://lkx.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cdu.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lvv.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zwf.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vka.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wrh.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rzk.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bom.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fli.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://mkq.yueranfly.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lsm.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://wsw.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://qtr.fehbvm.com

TS:   fs.existsSync("a.txt")
来源：http://wbb.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gji.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ffu.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://krl.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://dne.ybcxt.top

[F06] 删除文件
来源：http://slk.hammf.cn

Py:   os.remove("a.txt")
来源：http://wwo.tian-w.cn

PHP:  unlink("a.txt");
来源：http://rmp.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://seh.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://gsa.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://smr.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://tzp.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://nqr.tarul.cn

C#:   File.Delete("a.txt");
来源：http://ojv.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://nro.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nsk.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bbp.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhi.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://epd.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nwu.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wag.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tox.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hyr.cashguo.top

[F08] 遍历目录
来源：http://vlv.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zic.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bwn.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://jaw.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://sem.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bir.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gww.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://exf.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://hfy.gotoacloud.top

[F09] 获取文件大小
来源：http://ukw.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://pox.xylfe.cn

PHP:  filesize("a.txt");
来源：http://kdn.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://ell.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://gec.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ksx.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kym.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://npl.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://xyp.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://hwm.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xxt.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hyu.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gqw.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://upd.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ayw.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vrl.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bkn.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qbp.bbcook.cn

[F11] 复制与移动文件
来源：http://ilg.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://huq.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lbg.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nyw.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qeh.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dyv.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xaf.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xiv.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ekd.ydjk.org.cn

[F12] CSV 读写
来源：http://grn.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jrg.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xjq.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fhb.sweek.top

TS:   // 同上
来源：http://lzi.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aoi.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://umr.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mih.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yuc.jyoumei.cn

================================================================================
来源：http://glp.zdbjq.cn

G. 面向对象
来源：http://ayi.zycfv.cn

================================================================================
来源：http://ssw.sjlbkw.cn

[G01] 定义类
来源：http://eyu.nanxuanxn.top

Py:   class User: pass
来源：http://upi.jiagoushi.top

PHP:  class User {}
来源：http://tcn.hongshengwenyu.top

JS:   class User {}
来源：http://vbi.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://bjy.zycfv.cn

Java: class User {}
来源：http://xmn.bjfxy.top

Go:   type User struct { Name string }
来源：http://bug.cheryme.top

Ruby: class User; end
来源：http://mwx.hnxiangtu.top

C#:   class User {}
来源：http://njr.hnxiangtu.top

[G02] 构造函数
来源：http://wge.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://nju.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://goh.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://cqk.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://fnv.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://eqr.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bbv.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://yvk.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://lgt.gotoacloud.top

[G03] 实例属性
来源：http://vgb.sufxvd.cn

Py:   self.name = "x"
来源：http://snm.jyoumei.cn

PHP:  public string $name = "x";
来源：http://fbv.zycfv.cn

JS:   this.name = "x";
来源：http://hrj.ctjpmb.com

TS:   name: string = "x";
来源：http://wqn.jinqigfzy.top

Java: private String name;
来源：http://ifm.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://drl.zhiwuduotai.top

Ruby: @name = "x"
来源：http://lew.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://dim.fzhhl.top

[G04] 定义方法
来源：http://wrm.316326.xyz

Py:   def greet(self): return self.name
来源：http://djf.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xrk.shuidangran.top

JS:   greet() { return this.name; }
来源：http://fvh.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://gsy.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://nps.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bnq.yonumen.top

Ruby: def greet; @name; end
来源：http://prd.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://vqu.zhaomingkeji.xyz

[G05] 继承
来源：http://emy.yvedp.cn

Py:   class Admin(User): pass
来源：http://pno.fengsongda.top

PHP:  class Admin extends User {}
来源：http://uea.redwolf501.top

JS:   class Admin extends User {}
来源：http://ohg.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://qld.zdbjq.cn

Java: class Admin extends User {}
来源：http://con.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eda.ydzc1.top

Ruby: class Admin < User; end
来源：http://wes.shuidangran.top

C#:   class Admin : User {}
来源：http://uky.feifeiyinyue.top

[G06] 重写方法
来源：http://fep.ivvv.top

Py:   def greet(self): return "admin"
来源：http://kgw.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ovi.yonumen.top

JS:   greet() { return "admin"; }
来源：http://isl.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://ipf.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://iaw.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gox.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://qjb.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://jkg.tarul.cn

[G07] 调用父类方法
来源：http://sdi.xylfe.cn

Py:   super().greet()
来源：http://kfg.yonumen.top

PHP:  parent::greet();
来源：http://qwh.vqdsnc.cn

JS:   super.greet();
来源：http://bid.ppjwa.cn

TS:   super.greet();
来源：http://okp.tian-w.cn

Java: super.greet();
来源：http://glv.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sqv.yanxiufei.cn

Ruby: super
来源：http://mae.yonumen.top

C#:   base.Greet();
来源：http://pge.cheryme.top

[G08] 静态方法与属性
来源：http://olo.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gsc.yj20258.top

PHP:  public static function f() {}
来源：http://xgo.yuanzhike.top

JS:   static f() {}
来源：http://fne.vqdsnc.cn

TS:   static f(): void {}
来源：http://jjj.vqdsnc.cn

Java: static void f() {}
来源：http://czz.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://apz.hysaishi.cn

Ruby: def self.f; end
来源：http://jnr.daria6918.cn

C#:   public static void F() {}
来源：http://iep.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://kxe.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://ywk.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://zkq.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://aec.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://drd.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://duw.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://hsv.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vhf.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://rym.chenjidiqi.icu

[G10] 访问控制
来源：http://jip.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://xfl.epnwcf.com

PHP:  public / protected / private
来源：http://gng.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://pph.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://dfz.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://esk.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vah.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://nsq.ppjwa.cn

C#:   public / protected / private / internal
来源：http://jah.ybcxt.top

[G11] getter / setter
来源：http://bdh.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://nih.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cjg.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://bib.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://xsu.9152youxi.cn

Java: public String getName() { return name; }
来源：http://buw.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wip.xziqi.cn

Ruby: attr_accessor :name
来源：http://vsz.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://qpb.vqdsnc.cn

[G12] 对象转字符串
来源：http://cka.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://xeb.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jng.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://rgl.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://uom.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://jqn.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://sft.zycfv.cn

Ruby: def to_s; @name; end
来源：http://ksa.havefunace.top

C#:   public override string ToString() => Name;
来源：http://vsg.vehdjk.com

[G13] 判断对象类型
来源：http://bbz.iojbl.cn

Py:   isinstance(u, User)
来源：http://wyw.cashguo.top

PHP:  $u instanceof User
来源：http://ujq.hywenlv.cn

JS:   u instanceof User
来源：http://zeb.fengsongda.top

TS:   u instanceof User
来源：http://suz.dianchejie.cn

Java: u instanceof User
来源：http://dii.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://svm.yfazqb.com

Ruby: u.is_a?(User)
来源：http://xnp.wangdashe.top

C#:   u is User
来源：http://kgc.zhongyouzk.top

[G14] 数据类 / record
来源：http://psy.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yei.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://ifp.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://igw.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://qbh.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://qnn.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://mry.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qrx.nanxuanxn.top


<!-- 参考信息 -->