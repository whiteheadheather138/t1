代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wxg.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://isr.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mri.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yko.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ipo.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mqm.xuanzx.com

Ruby: s.capitalize
来源：http://wta.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qkm.jinqigufen.top

[E18] 模板占位符替换
来源：http://exi.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sax.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ojg.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://dem.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hhn.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kfh.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ban.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ryg.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tyv.sxryk.cn

[E19] 多行文本按行拆分
来源：http://oeb.vehdjk.com

Py:   s.splitlines()
来源：http://krw.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uhc.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://rvw.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://yom.zdqjudy.top

Java: s.lines().toList()
来源：http://vic.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://mrh.vqdsnc.cn

Ruby: s.lines
来源：http://mis.cdnleiting.top

C#:   s.Split('\n')
来源：http://kum.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://rdb.cucudq.cn

Py:   if not s:
来源：http://kfk.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rcb.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cac.guowangkeji.top

TS:   if (s === "") {}
来源：http://qcn.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://vwi.yj20258.top

Go:   if s == "" {}
来源：http://lmt.sufxvd.cn

Ruby: if s.empty?
来源：http://fvo.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cpe.tanke756.top

[E21] 超长截断加省略号
来源：http://mvt.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vgr.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dun.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqx.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nhu.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nfn.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://dxl.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vkz.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://czj.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://aip.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jfu.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pzd.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjw.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mpe.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hdw.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vzn.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://fju.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lbl.redwolf501.top

================================================================================
来源：http://yxh.zhijiandao.cn

F. 文件与目录
来源：http://qzv.yonumen.top

================================================================================
来源：http://zaq.sysykeji.top

[F01] 读取整个文件
来源：http://flb.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kjp.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://xin.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ess.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kos.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zwh.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hqj.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://lxe.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://qvc.redwolf501.top

[F02] 逐行读取文件
来源：http://ged.yonumen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pmv.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eft.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tcj.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ozq.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axj.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lzg.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zbt.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mwm.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://ygy.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zii.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://myp.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wpz.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fan.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jth.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kzy.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://jow.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xxt.hfpthk.cn

[F04] 追加写入文件
来源：http://bcr.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yqw.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zoz.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://day.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aqd.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uqo.yj20258888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uzw.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vzn.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yeu.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://qpk.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nlx.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://rqp.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://yug.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://jzx.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zur.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ysj.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://bpp.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://wxt.fengsongda.top

[F06] 删除文件
来源：http://ghm.smart0.xyz

Py:   os.remove("a.txt")
来源：http://qzh.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://nkn.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://cng.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cde.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wuh.hammf.cn

Go:   os.Remove("a.txt")
来源：http://cpw.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://gbr.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://rzw.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://ifp.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mwl.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hjb.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vkt.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://plh.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ier.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gdh.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fse.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hhh.jianghu66.top

[F08] 遍历目录
来源：http://nwt.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qxf.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xrs.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://etu.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://tpv.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jdl.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://gcw.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://mpd.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://xhd.ctjpmb.com

[F09] 获取文件大小
来源：http://suo.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://uov.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://wqp.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://yqp.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://mvc.hesvh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kiz.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qqz.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://raz.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://ftq.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://bue.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jxf.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ahs.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://htj.tarul.cn

TS:   path.extname("a.txt")
来源：http://uzl.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tvt.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yha.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zef.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uyl.snrcjt.cn

[F11] 复制与移动文件
来源：http://kiu.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://smg.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://stq.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahz.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vxx.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tdz.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bid.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tfv.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dcy.sufxvd.cn

[F12] CSV 读写
来源：http://qwr.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vie.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zlg.yj20258888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ppf.fengsongda.top

TS:   // 同上
来源：http://upc.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pgm.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tzr.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xyi.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://att.9152youxi.cn

================================================================================
来源：http://ruc.vqdsnc.cn

G. 面向对象
来源：http://lce.gotoacloud.top

================================================================================
来源：http://ynr.ydjk.org.cn

[G01] 定义类
来源：http://kha.jinghuilouyu.cn

Py:   class User: pass
来源：http://znf.kuanghao11.cn

PHP:  class User {}
来源：http://uxw.ywan-chungtsiang.top

JS:   class User {}
来源：http://kza.tarul.cn

TS:   class User { name: string = ""; }
来源：http://hkf.sjlbkw.cn

Java: class User {}
来源：http://nbr.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://gdf.52xcode.cn

Ruby: class User; end
来源：http://zir.zhiwuduotai.top

C#:   class User {}
来源：http://hdf.hfpthk.cn

[G02] 构造函数
来源：http://wly.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://ios.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://hvg.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://cxp.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://chm.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://qco.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dru.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://oul.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://kqj.tarul.cn

[G03] 实例属性
来源：http://qps.shzxlz.cn

Py:   self.name = "x"
来源：http://vto.cheryme.top

PHP:  public string $name = "x";
来源：http://jta.jinqigfzy.top

JS:   this.name = "x";
来源：http://hqk.zhijiandao.cn

TS:   name: string = "x";
来源：http://jrh.xylfe.cn

Java: private String name;
来源：http://wxw.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zax.wangshuangyany.cn

Ruby: @name = "x"
来源：http://kzv.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://glv.yj20258888.top

[G04] 定义方法
来源：http://ywg.ybcxt.top

Py:   def greet(self): return self.name
来源：http://zjz.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tit.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://rxu.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://hzb.fktsv.cn

Java: String greet() { return name; }
来源：http://laj.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tzf.hywenlv.cn

Ruby: def greet; @name; end
来源：http://wly.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://mtw.fktsv.cn

[G05] 继承
来源：http://nri.mhx1999.top

Py:   class Admin(User): pass
来源：http://opf.aizwys.cn

PHP:  class Admin extends User {}
来源：http://soc.zycfv.cn

JS:   class Admin extends User {}
来源：http://pry.0kj1m.cn

TS:   class Admin extends User {}
来源：http://gwj.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://bwa.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ejy.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://rjl.zdbjq.cn

C#:   class Admin : User {}
来源：http://sqf.jyoumei.cn

[G06] 重写方法
来源：http://ehc.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://dju.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wzb.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://xjd.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://wuq.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://qco.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://duw.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://lqq.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://ifw.hywenlv.cn

[G07] 调用父类方法
来源：http://zkp.ybcxt.top

Py:   super().greet()
来源：http://axr.jianghu66.top

PHP:  parent::greet();
来源：http://idc.hongshengwenyu.top

JS:   super.greet();
来源：http://dth.xziqi.cn

TS:   super.greet();
来源：http://zqr.9152youxi.cn

Java: super.greet();
来源：http://oqa.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://trv.hesvh.cn

Ruby: super
来源：http://xsg.yonumen.top

C#:   base.Greet();
来源：http://qmw.shuidangran.top

[G08] 静态方法与属性
来源：http://lpm.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dtl.cashguo.top

PHP:  public static function f() {}
来源：http://qbx.hfpthk.cn

JS:   static f() {}
来源：http://eox.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://ukq.tanke756.top

Java: static void f() {}
来源：http://muf.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vit.hammf.cn

Ruby: def self.f; end
来源：http://zqm.zdqjudy.top

C#:   public static void F() {}
来源：http://zdo.yj202588.top

[G09] 接口 / 抽象类
来源：http://lvd.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://omp.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://qrs.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mmv.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://pyg.guannengcc.top

Java: interface Shape { double area(); }
来源：http://bmd.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://fff.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mll.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://bls.9152youxi.cn

[G10] 访问控制
来源：http://wwb.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://alb.iojbl.cn

PHP:  public / protected / private
来源：http://ubq.52xcode.cn

JS:   #private 字段；其余公开
来源：http://mlt.yanxiufei.cn

TS:   public / protected / private
来源：http://urc.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://nsi.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vpv.vqdsnc.cn

Ruby: public / protected / private
来源：http://omb.nanxinkj.top

C#:   public / protected / private / internal
来源：http://swl.shanyushiyangkeji.top

[G11] getter / setter
来源：http://ges.aizwys.cn

Py:   @property 与 @x.setter
来源：http://mcy.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://krc.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://byu.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://gco.bbcook.cn

Java: public String getName() { return name; }
来源：http://urm.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hwo.fengsongda.top

Ruby: attr_accessor :name
来源：http://iry.iojbl.cn

C#:   public string Name { get; set; }
来源：http://ode.tanke756.top

[G12] 对象转字符串
来源：http://wch.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://myg.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://avu.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://ign.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://syx.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://rnw.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fky.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://kqs.yongpay.top

C#:   public override string ToString() => Name;
来源：http://vvp.yonumen.top

[G13] 判断对象类型
来源：http://deh.fengsongda.top

Py:   isinstance(u, User)
来源：http://dvj.yueranfly.top

PHP:  $u instanceof User
来源：http://aig.ybcxt.top

JS:   u instanceof User
来源：http://ejm.bbcook.cn

TS:   u instanceof User
来源：http://fje.guannengcc.top

Java: u instanceof User
来源：http://ueq.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rtr.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://qsq.xuetiantiany.cn

C#:   u is User
来源：http://ejf.jinqigufen.top

[G14] 数据类 / record
来源：http://cgu.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gza.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://nbj.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hqy.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://frc.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://lse.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://war.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhi.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://sqj.xinyue.icu

[G15] 枚举
来源：http://slp.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://icr.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jcd.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hft.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cet.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://jlv.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://syc.xuanzx.com


<!-- 参考信息 -->