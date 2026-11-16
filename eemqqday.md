代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ari.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rnk.cashguo.top

C#:   1234567.ToString("N0")
来源：http://eio.pycfn.com

[E17] 首字母大写
来源：http://bso.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dsc.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://elt.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfc.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikz.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fgx.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gap.snrcjt.cn

Ruby: s.capitalize
来源：http://mzy.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jak.dashuyun.cn

[E18] 模板占位符替换
来源：http://tol.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bvz.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://crk.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uxc.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://qvi.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pen.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://idk.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sbs.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ojq.gzhubu.top

[E19] 多行文本按行拆分
来源：http://kje.yangfankeji.com

Py:   s.splitlines()
来源：http://snh.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ikp.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://afi.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://nqw.iojbl.cn

Java: s.lines().toList()
来源：http://ekt.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://ieh.vqdsnc.cn

Ruby: s.lines
来源：http://trt.zdqjudy.top

C#:   s.Split('\n')
来源：http://ljs.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://tzy.gaohongyu789.top

Py:   if not s:
来源：http://xjd.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fcx.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rva.tianlin.xyz

TS:   if (s === "") {}
来源：http://rbn.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://drl.smart0.xyz

Go:   if s == "" {}
来源：http://nev.yj20258888.top

Ruby: if s.empty?
来源：http://vzf.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://guq.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://btr.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tyr.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nfd.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tkp.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hxn.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bsr.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://che.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://alp.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://myc.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://yah.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aeu.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtw.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zku.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbs.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gal.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rjf.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://deq.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qvh.yanxiufei.cn

================================================================================
来源：http://mvq.jqgufenzy.top

F. 文件与目录
来源：http://sjr.yvedp.cn

================================================================================
来源：http://whd.jiagoushi.top

[F01] 读取整个文件
来源：http://ixw.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rsp.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://fwh.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hzb.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wxs.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nzg.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://npo.tian-w.cn

Ruby: File.read("a.txt")
来源：http://smw.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://pen.jqgfzy.top

[F02] 逐行读取文件
来源：http://asw.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tpi.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wvw.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sxb.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nfh.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ogq.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rny.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wdx.yvedp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qkk.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://szp.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdk.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ajq.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wkj.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cmb.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xlr.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xwi.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://zrv.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fxj.vqdsnc.cn

[F04] 追加写入文件
来源：http://ikr.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oqd.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yrd.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gsb.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gje.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cqi.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hgo.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://enq.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tsi.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://qnt.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ygx.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://iwv.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://xxm.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://zis.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://cwq.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tuq.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://eiw.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://oah.aibaodan.cn

[F06] 删除文件
来源：http://tzt.ydzc1.top

Py:   os.remove("a.txt")
来源：http://mmb.yuxming.cn

PHP:  unlink("a.txt");
来源：http://azz.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://yka.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://spm.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yrm.316326.xyz

Go:   os.Remove("a.txt")
来源：http://jgm.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://stb.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://ege.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://cdg.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ekr.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tbd.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://axz.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nie.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://thn.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ayf.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cug.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wyn.fktsv.cn

[F08] 遍历目录
来源：http://bvc.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://usb.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mlr.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://uep.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://uym.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xcv.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://njb.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://xun.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://djj.andypj.xyz

[F09] 获取文件大小
来源：http://ist.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://ujg.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://ziw.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://bsi.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://jqc.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://tsv.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lfc.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://esd.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://zdq.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://gay.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rez.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sts.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dpq.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://iwr.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iwr.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ktx.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lpw.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eeh.ivvv.top

[F11] 复制与移动文件
来源：http://qjm.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tuy.sjlbkw.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://juv.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nct.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgx.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ohf.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dye.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zop.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://woi.sysykeji.top

[F12] CSV 读写
来源：http://nxe.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sns.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hoh.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gsi.xinyue.icu

TS:   // 同上
来源：http://iak.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kfd.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gdw.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fyg.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://pbb.xingfuxueyuan.xyz

================================================================================
来源：http://vqy.hysaishi.cn

G. 面向对象
来源：http://qkz.zhoulong.xyz

================================================================================
来源：http://pxq.zdbjq.cn

[G01] 定义类
来源：http://lde.zhijiandao.cn

Py:   class User: pass
来源：http://wxv.uphjek.com

PHP:  class User {}
来源：http://pys.cucudq.cn

JS:   class User {}
来源：http://vsn.cashguo.top

TS:   class User { name: string = ""; }
来源：http://uri.xinyue.icu

Java: class User {}
来源：http://hcn.smart0.xyz

Go:   type User struct { Name string }
来源：http://azv.chenjidiqi.icu

Ruby: class User; end
来源：http://aai.chenzaomai.com

C#:   class User {}
来源：http://zku.jinyuanbaomall.cn

[G02] 构造函数
来源：http://eqv.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://vxn.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://knj.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://yrb.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://yrk.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://rxm.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ksc.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://tmf.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://gkg.tian-w.cn

[G03] 实例属性
来源：http://azp.52xcode.cn

Py:   self.name = "x"
来源：http://bmw.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://lgp.chenzaomai.com

JS:   this.name = "x";
来源：http://gqy.hcnkem.com

TS:   name: string = "x";
来源：http://aco.zhoulong.xyz

Java: private String name;
来源：http://jee.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hml.epnwcf.com

Ruby: @name = "x"
来源：http://khn.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://csc.zhongyouzk.top

[G04] 定义方法
来源：http://ytu.xziqi.cn

Py:   def greet(self): return self.name
来源：http://gee.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aib.52xcode.cn

JS:   greet() { return this.name; }
来源：http://afb.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://esw.nwbrower.top

Java: String greet() { return name; }
来源：http://gor.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fwx.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://rhi.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://nmq.gogol.net.cn

[G05] 继承
来源：http://lkg.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://cmn.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://pbj.guowangkeji.top

JS:   class Admin extends User {}
来源：http://ktr.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://gtn.sufxvd.cn

Java: class Admin extends User {}
来源：http://vwc.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://srr.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://ima.epnwcf.com

C#:   class Admin : User {}
来源：http://kzj.nanxinkj.top

[G06] 重写方法
来源：http://uav.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://zku.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uqn.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://mkt.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://xhx.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://pvm.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fct.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://fsb.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://bbb.bjfxy.top

[G07] 调用父类方法
来源：http://yjw.ywan-chungtsiang.top

Py:   super().greet()
来源：http://buc.9152youxi.cn

PHP:  parent::greet();
来源：http://gmd.yj20258.top

JS:   super.greet();
来源：http://tfj.uphjek.com

TS:   super.greet();
来源：http://xns.jlsjyb.cn

Java: super.greet();
来源：http://qsa.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zxd.xylfe.cn

Ruby: super
来源：http://srh.snrcjt.cn

C#:   base.Greet();
来源：http://ror.yvedp.cn

[G08] 静态方法与属性
来源：http://bzh.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bqw.zdqjudy.top

PHP:  public static function f() {}
来源：http://qyx.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://yhx.hesvh.cn

TS:   static f(): void {}
来源：http://knp.yfazqb.com

Java: static void f() {}
来源：http://kal.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dwl.sxryk.cn

Ruby: def self.f; end
来源：http://doz.jqgufenzy.top

C#:   public static void F() {}
来源：http://kew.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://ocu.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gfu.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://wkn.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lyj.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://lci.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://bvk.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://zdn.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rkm.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://ska.jinghuilouyu.cn

[G10] 访问控制
来源：http://jum.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://qoj.feifeiyinyue.top

PHP:  public / protected / private
来源：http://cvf.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://jzo.vqdsnc.cn

TS:   public / protected / private
来源：http://yjg.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://ion.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ypj.chenzaomai.com

Ruby: public / protected / private
来源：http://jpg.yongpay.top

C#:   public / protected / private / internal
来源：http://ugf.shzxlz.cn

[G11] getter / setter
来源：http://yyp.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://jja.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lom.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://ykj.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://mrb.sweek.top

Java: public String getName() { return name; }
来源：http://ulg.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jez.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://qpq.shuidangran.top

C#:   public string Name { get; set; }
来源：http://xhb.9152youxi.cn

[G12] 对象转字符串
来源：http://zqs.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://oed.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cpq.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://lix.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://kbq.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://ief.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cuj.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://lfr.cashguo.top

C#:   public override string ToString() => Name;
来源：http://eox.xziqi.cn

[G13] 判断对象类型
来源：http://zyq.epnwcf.com

Py:   isinstance(u, User)
来源：http://kwy.gzhubu.top

PHP:  $u instanceof User
来源：http://lro.yuanzhike.top

JS:   u instanceof User
来源：http://gtg.guowangkeji.top

TS:   u instanceof User
来源：http://lye.guannengcc.top

Java: u instanceof User
来源：http://evo.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://skj.xuanzx.com

Ruby: u.is_a?(User)
来源：http://pqo.cheryme.top

C#:   u is User
来源：http://nlz.smart0.xyz

[G14] 数据类 / record
来源：http://lop.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://afb.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ucf.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://nyw.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://gca.tarul.cn

Java: record User(String name, int age) {}
来源：http://esv.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://sny.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sql.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://lup.fktsv.cn

[G15] 枚举
来源：http://icx.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dqq.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ueg.bjfxy.top


<!-- 参考信息 -->