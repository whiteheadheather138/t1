代发 wailian999

[E18] 模板占位符替换
来源：http://eqd.daxiang520.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xui.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vnu.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fkd.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xjb.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rbg.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yod.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qdg.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gof.hnqzz.top

[E19] 多行文本按行拆分
来源：http://fgt.yuxming.cn

Py:   s.splitlines()
来源：http://hwb.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ahd.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://wql.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://hts.hnqzz.top

Java: s.lines().toList()
来源：http://ois.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://kaa.ybcxt.top

Ruby: s.lines
来源：http://urp.ydzc1.top

C#:   s.Split('\n')
来源：http://kbk.c1oappe.top

[E20] 判断字符串是否为空
来源：http://suh.yuanzhike.top

Py:   if not s:
来源：http://mho.zhengqikj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://itp.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wtc.tanke756.top

TS:   if (s === "") {}
来源：http://vkh.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://kyo.xuanzx.com

Go:   if s == "" {}
来源：http://qwv.ybcxt.top

Ruby: if s.empty?
来源：http://rrd.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gdr.hfpthk.cn

[E21] 超长截断加省略号
来源：http://ocq.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cmg.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ypk.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bor.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rro.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kke.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://ohb.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xai.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kac.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://sln.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qdz.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ejh.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jhk.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://keg.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ylf.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mna.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://abk.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iiz.yfazqb.com

================================================================================
来源：http://ahy.jyoumei.cn

F. 文件与目录
来源：http://waf.shanyushiyangtech.top

================================================================================
来源：http://rfw.pengpengdd.cyou

[F01] 读取整个文件
来源：http://vbf.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yvl.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://xnb.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://flw.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zfi.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tco.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tkw.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://owo.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://tcw.cashguo.top

[F02] 逐行读取文件
来源：http://wzi.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ojz.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hiz.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rag.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pen.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wya.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tuq.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vjl.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wuy.316326.xyz

[F03] 写入文件（覆盖）
来源：http://cjw.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bzy.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xaf.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ppp.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vdy.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pkk.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hms.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://ptq.jianghu66.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gef.dashuyun.cn

[F04] 追加写入文件
来源：http://wih.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tby.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ctb.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yva.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hrj.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fpb.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qoo.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://omc.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jqh.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://bkp.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://szf.meibo888.top

PHP:  file_exists("a.txt");
来源：http://pex.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://niw.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://xqs.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dis.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vya.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://mal.yongpay.top

C#:   File.Exists("a.txt")
来源：http://brq.zdbjq.cn

[F06] 删除文件
来源：http://hix.xuanzx.com

Py:   os.remove("a.txt")
来源：http://ruo.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://cuu.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://dhd.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pjq.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bwh.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://prh.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://hfo.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://czv.hesvh.cn

[F07] 创建目录（含多级）
来源：http://shp.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dsv.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://usl.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xts.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cqx.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ped.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qco.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gfp.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://caf.fanxiaobao.xyz

[F08] 遍历目录
来源：http://yme.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://zyt.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jgt.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://pto.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://lsr.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://stf.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://plo.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://bqa.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://hdh.sjlbkw.cn

[F09] 获取文件大小
来源：http://mdk.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://oqi.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://ycz.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://xsq.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://xjp.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gzj.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nri.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://wcs.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://rsi.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://iif.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://frb.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gqw.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://arm.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://ank.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mxy.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qhk.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ljj.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mvq.jlsjyb.cn

[F11] 复制与移动文件
来源：http://oib.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://llr.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jdn.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eto.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sbm.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gdg.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vry.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gwd.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mxr.mhx1999.top

[F12] CSV 读写
来源：http://yfb.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wjs.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kcu.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ccx.zdbjq.cn

TS:   // 同上
来源：http://pco.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rpp.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://avh.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qjw.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ooe.sysykeji.top

================================================================================
来源：http://dhy.nwbrower.top

G. 面向对象
来源：http://tsa.jinyuanbaomall.cn

================================================================================
来源：http://jwt.fktsv.cn

[G01] 定义类
来源：http://gcp.ywan-chungtsiang.top

Py:   class User: pass
来源：http://yvz.ydzc1.top

PHP:  class User {}
来源：http://amu.zhengqikj.top

JS:   class User {}
来源：http://vlk.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://smj.snrcjt.cn

Java: class User {}
来源：http://wyq.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://tkp.gaohongyu789.top

Ruby: class User; end
来源：http://qxr.hcnkem.com

C#:   class User {}
来源：http://puf.nanxinkj.top

[G02] 构造函数
来源：http://acx.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://fgr.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://bsx.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://abw.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://zqo.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://rwr.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ggf.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://qqk.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://pzp.zhaomingkeji.xyz

[G03] 实例属性
来源：http://dmn.gaohongyu789.top

Py:   self.name = "x"
来源：http://mrn.ivvv.top

PHP:  public string $name = "x";
来源：http://qog.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://abq.zhongyouzk.top

TS:   name: string = "x";
来源：http://znq.jinyuanbaomall.cn

Java: private String name;
来源：http://uai.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uqm.mhx1999.top

Ruby: @name = "x"
来源：http://htt.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://deh.snrcjt.cn

[G04] 定义方法
来源：http://mpv.birdmap.top

Py:   def greet(self): return self.name
来源：http://yql.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lrs.316326.xyz

JS:   greet() { return this.name; }
来源：http://wzy.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://vrd.jlsjyb.cn

Java: String greet() { return name; }
来源：http://fro.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://thy.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://cou.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://vxy.jinyuanbaomall.cn

[G05] 继承
来源：http://slh.jinqigufen.top

Py:   class Admin(User): pass
来源：http://rks.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://wvi.dashuyun.cn

JS:   class Admin extends User {}
来源：http://dva.dashuyun.cn

TS:   class Admin extends User {}
来源：http://piz.zhixingplan.top

Java: class Admin extends User {}
来源：http://kly.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qox.9152youxi.cn

Ruby: class Admin < User; end
来源：http://lhv.jyoumei.cn

C#:   class Admin : User {}
来源：http://tmv.jianghu66.top

[G06] 重写方法
来源：http://wbv.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://kgi.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sxj.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://uyv.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://geb.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://vfl.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://duk.ivvv.top

Ruby: def greet; "admin"; end
来源：http://inp.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://yth.zhijiandao.cn

[G07] 调用父类方法
来源：http://dpl.yvedp.cn

Py:   super().greet()
来源：http://gcg.jyoumei.cn

PHP:  parent::greet();
来源：http://ceq.fktsv.cn

JS:   super.greet();
来源：http://wdl.yj202588.top

TS:   super.greet();
来源：http://kef.gzhubu.top

Java: super.greet();
来源：http://tvk.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tsq.havefunace.top

Ruby: super
来源：http://cwe.bjfxy.top

C#:   base.Greet();
来源：http://six.guannengcc.top

[G08] 静态方法与属性
来源：http://jxf.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gai.snrcjt.cn

PHP:  public static function f() {}
来源：http://wce.chenzaomai.com

JS:   static f() {}
来源：http://ghb.hongshengwenyu.top

TS:   static f(): void {}
来源：http://bzm.xinyue.icu

Java: static void f() {}
来源：http://jww.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lwh.quarkkingdee.top

Ruby: def self.f; end
来源：http://ama.wangdashe.top

C#:   public static void F() {}
来源：http://gyz.c1oappe.top

[G09] 接口 / 抽象类
来源：http://smm.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://wae.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lsw.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dkq.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://ljj.hammf.cn

Java: interface Shape { double area(); }
来源：http://lns.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://hos.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rmq.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://gjm.ctjpmb.com

[G10] 访问控制
来源：http://ubq.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://csm.ehwqpu.com

PHP:  public / protected / private
来源：http://bdt.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://wgi.chenzaomai.com

TS:   public / protected / private
来源：http://dcu.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://jor.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://lpb.cqqwz.cn

Ruby: public / protected / private
来源：http://iov.bjfxy.top

C#:   public / protected / private / internal
来源：http://myq.chenzaomai.com

[G11] getter / setter
来源：http://tvk.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://zhv.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://cym.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://kwb.zdqjudy.top

TS:   get name(): string { return this._name; }
来源：http://ghv.svipenyu.cn

Java: public String getName() { return name; }
来源：http://dmc.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://udo.zdqjudy.top

Ruby: attr_accessor :name
来源：http://rfv.ybcxt.top

C#:   public string Name { get; set; }
来源：http://cto.andypj.xyz

[G12] 对象转字符串
来源：http://bnf.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://sbw.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://sfu.shuidangran.top

JS:   toString() { return this.name; }
来源：http://njf.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://zhi.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://gaa.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://nws.bbcook.cn

Ruby: def to_s; @name; end
来源：http://mtz.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://soi.sjlbkw.cn

[G13] 判断对象类型
来源：http://fgj.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://zlp.yueranfly.top

PHP:  $u instanceof User
来源：http://anv.iojbl.cn

JS:   u instanceof User
来源：http://ruk.yueranfly.top

TS:   u instanceof User
来源：http://svt.hysaishi.cn

Java: u instanceof User
来源：http://wat.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uos.xuanzx.com

Ruby: u.is_a?(User)
来源：http://otl.yj20258.top

C#:   u is User
来源：http://lhj.tian-w.cn

[G14] 数据类 / record
来源：http://epu.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cgm.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://nvs.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kru.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://hqn.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://hwi.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://btf.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qqy.ivvv.top

C#:   record User(string Name, int Age);
来源：http://rwg.ctjpmb.com

[G15] 枚举
来源：http://laf.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://whe.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xib.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rij.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gtj.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://nxo.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gqg.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://gfm.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xoc.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://atb.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hyr.ivvv.top

PHP:  get_object_vars($obj);
来源：http://bft.xylfe.cn

JS:   Object.entries(obj)
来源：http://acj.ivvv.top

TS:   Object.entries(obj)
来源：http://ozl.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://znh.sxryk.cn


<!-- 参考信息 -->