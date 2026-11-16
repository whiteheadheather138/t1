代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ema.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cvm.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ocs.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gpe.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pac.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dyb.iojbl.cn

Ruby: s.capitalize
来源：http://asi.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lpx.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://dpp.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tlq.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ibr.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kdk.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mip.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://otd.jinyuanbaomall.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fog.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xse.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hom.yfazqb.com

[E19] 多行文本按行拆分
来源：http://rio.shzxlz.cn

Py:   s.splitlines()
来源：http://jkq.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zow.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://frl.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://zqx.hnxiangtu.top

Java: s.lines().toList()
来源：http://kom.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://nqe.uphjek.com

Ruby: s.lines
来源：http://adr.yueranfly.top

C#:   s.Split('\n')
来源：http://zbv.xylfe.cn

[E20] 判断字符串是否为空
来源：http://kwi.daria6918.cn

Py:   if not s:
来源：http://yfz.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pdk.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aqb.gogol.net.cn

TS:   if (s === "") {}
来源：http://wjg.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://dlu.uphjek.com

Go:   if s == "" {}
来源：http://kjn.meibo888.top

Ruby: if s.empty?
来源：http://qfc.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://clz.yj20258888.top

[E21] 超长截断加省略号
来源：http://ois.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tnj.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://der.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vut.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wvy.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aoe.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://qmx.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ius.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qak.52xcode.cn

[E22] 字节长度与字符长度
来源：http://ckf.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vhj.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xdl.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mra.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ghe.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ndb.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sqk.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://prb.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://joi.guowangkeji.top

================================================================================
来源：http://uwj.zhoulong.xyz

F. 文件与目录
来源：http://dli.xziqi.cn

================================================================================
来源：http://igl.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://mor.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dyt.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://esp.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://djm.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cxt.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xnr.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rzv.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://jof.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://xis.vehdjk.com

[F02] 逐行读取文件
来源：http://pbv.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://krp.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blz.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wrr.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cht.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eaq.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lgz.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gzv.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ihj.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://nma.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pch.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vjm.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qol.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jxe.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dxf.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iep.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://iby.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://onh.meibo888.top

[F04] 追加写入文件
来源：http://rnq.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ldm.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xbe.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pua.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pfu.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jew.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xwa.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xnm.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wxu.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://oja.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iac.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://bdf.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://tkm.fehbvm.com

TS:   fs.existsSync("a.txt")
来源：http://mqc.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://dbx.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hwq.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://erp.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://vqp.shangyingyoupin.top

[F06] 删除文件
来源：http://hoi.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://czb.fzhhl.top

PHP:  unlink("a.txt");
来源：http://let.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://bmq.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jzu.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://plb.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://apv.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://neh.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://wgf.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://oma.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fay.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wtv.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jbt.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xdy.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fuy.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wgl.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gaa.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ldq.fzhhl.top

[F08] 遍历目录
来源：http://uld.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://nno.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vxu.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://cky.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://jwb.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hja.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qgi.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://szt.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://zii.aibaodan.cn

[F09] 获取文件大小
来源：http://ciw.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://xnk.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://vml.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://tsm.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://ret.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://jrd.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xml.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://yzl.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://gvv.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://wxc.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lqt.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ygb.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rhy.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://kho.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eqo.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qgo.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jvo.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://smv.yueranfly.top

[F11] 复制与移动文件
来源：http://hgt.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fcf.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://psh.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ytt.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fxf.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wbo.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vfq.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aav.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://usf.smart0.xyz

[F12] CSV 读写
来源：http://xkl.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ahh.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xez.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dub.shanyushiyangtech.top

TS:   // 同上
来源：http://wjc.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mfe.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ivf.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tfh.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://vdj.andypj.xyz

================================================================================
来源：http://ozy.jinghuilouyu.cn

G. 面向对象
来源：http://zad.andypj.xyz

================================================================================
来源：http://hqq.shanyushiyangkeji.top

[G01] 定义类
来源：http://hcr.jqgfzy.top

Py:   class User: pass
来源：http://slm.nanxuanxn.top

PHP:  class User {}
来源：http://hzr.cdnleiting.top

JS:   class User {}
来源：http://fqs.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://enx.ybcxt.top

Java: class User {}
来源：http://yfc.zhixingplan.top

Go:   type User struct { Name string }
来源：http://ckv.hfpthk.cn

Ruby: class User; end
来源：http://hsx.guannengcc.top

C#:   class User {}
来源：http://jzk.ywan-chungtsiang.top

[G02] 构造函数
来源：http://tnj.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://clt.wangshuangyany.cn

PHP:  public function __construct(public string $name) {}
来源：http://xoq.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://ygs.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://knc.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://ctq.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wsq.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://mvh.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://ysa.guannengcc.top

[G03] 实例属性
来源：http://wpm.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://rod.yueranfly.top

PHP:  public string $name = "x";
来源：http://rcx.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://pml.hfpthk.cn

TS:   name: string = "x";
来源：http://vnr.gaohongyu789.top

Java: private String name;
来源：http://cpo.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iyt.sxryk.cn

Ruby: @name = "x"
来源：http://cnw.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://gxn.yvedp.cn

[G04] 定义方法
来源：http://xuq.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://kgu.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dbj.sysykeji.top

JS:   greet() { return this.name; }
来源：http://arp.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://lxp.316326.xyz

Java: String greet() { return name; }
来源：http://ikk.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tbg.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://znq.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://nmg.hywenlv.cn

[G05] 继承
来源：http://yiy.yuanzhike.top

Py:   class Admin(User): pass
来源：http://eub.52xcode.cn

PHP:  class Admin extends User {}
来源：http://anm.wangdashe.top

JS:   class Admin extends User {}
来源：http://pjz.cdnleiting.top

TS:   class Admin extends User {}
来源：http://yxz.zhixingplan.top

Java: class Admin extends User {}
来源：http://jfc.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vrm.yj202588.top

Ruby: class Admin < User; end
来源：http://vtf.ybcxt.top

C#:   class Admin : User {}
来源：http://ayw.xuetiantiany.cn

[G06] 重写方法
来源：http://glx.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://zli.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://loe.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://szs.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://esy.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://byw.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nyj.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://gnl.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://odc.316326.xyz

[G07] 调用父类方法
来源：http://yxo.tarul.cn

Py:   super().greet()
来源：http://spv.iojbl.cn

PHP:  parent::greet();
来源：http://iil.chenzaomai.com

JS:   super.greet();
来源：http://voh.ywan-chungtsiang.top

TS:   super.greet();
来源：http://ygp.fanxiaobao.xyz

Java: super.greet();
来源：http://vgl.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hto.nwbrower.top

Ruby: super
来源：http://ift.chenjidiqi.icu

C#:   base.Greet();
来源：http://njx.zhijiandao.cn

[G08] 静态方法与属性
来源：http://kof.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xtu.hesvh.cn

PHP:  public static function f() {}
来源：http://hts.haohaochexian.top

JS:   static f() {}
来源：http://atw.quarkkingdee.top

TS:   static f(): void {}
来源：http://uhv.jqgufenzy.top

Java: static void f() {}
来源：http://ilo.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gqk.ehwqpu.com

Ruby: def self.f; end
来源：http://egt.tarul.cn

C#:   public static void F() {}
来源：http://wtc.redwolf501.top

[G09] 接口 / 抽象类
来源：http://oof.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://igb.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eib.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://itq.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://tbf.smart0.xyz

Java: interface Shape { double area(); }
来源：http://kgw.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://jhz.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jyx.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://nya.yangfankeji.com

[G10] 访问控制
来源：http://nnr.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://lep.gaohongyu789.top

PHP:  public / protected / private
来源：http://xtz.52xcode.cn

JS:   #private 字段；其余公开
来源：http://uva.xylfe.cn

TS:   public / protected / private
来源：http://soe.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://cbv.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://svf.zhongyouzk.top

Ruby: public / protected / private
来源：http://oob.dashuyun.cn

C#:   public / protected / private / internal
来源：http://exn.zhongyouzk.top

[G11] getter / setter
来源：http://cwb.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://whi.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://wtt.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://mew.sweek.top

TS:   get name(): string { return this._name; }
来源：http://cgv.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://cau.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nsg.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://yxg.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://tdb.jqgfzy.top

[G12] 对象转字符串
来源：http://yde.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://zfw.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://koc.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://cws.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://buh.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://zxk.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://ait.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://nth.ivvv.top

C#:   public override string ToString() => Name;
来源：http://bsk.yueranfly.top

[G13] 判断对象类型
来源：http://ovv.cqqwz.cn

Py:   isinstance(u, User)
来源：http://uiu.kuanghao11.cn

PHP:  $u instanceof User
来源：http://krn.iojbl.cn

JS:   u instanceof User
来源：http://gqp.ydzc1.top

TS:   u instanceof User
来源：http://bdu.yj20258.top

Java: u instanceof User
来源：http://wwx.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yiq.ydzc1.top

Ruby: u.is_a?(User)
来源：http://zwb.jqgufenzy.top

C#:   u is User
来源：http://tak.jyoumei.cn

[G14] 数据类 / record
来源：http://nqv.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gcn.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://zvr.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ivh.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://flg.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://fon.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://nxo.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qtq.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://orx.zhixingplan.top

[G15] 枚举
来源：http://hau.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://skr.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://edw.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wlx.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jue.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://tdb.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wsb.fengsongda.top


<!-- 参考信息 -->