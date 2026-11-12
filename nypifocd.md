代发 wailian999

PHP:  number_format(1234567);
来源：http://huq.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tvn.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bej.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vue.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://syu.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qei.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://kqj.cashguo.top

[E17] 首字母大写
来源：http://tvg.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sqw.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://psi.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://exb.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vfc.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gpw.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gnm.havefunace.top

Ruby: s.capitalize
来源：http://eqw.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hnu.cashguo.top

[E18] 模板占位符替换
来源：http://uhu.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://htj.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aaf.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zeh.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wxy.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lga.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lyd.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ndh.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otg.tian-w.cn

[E19] 多行文本按行拆分
来源：http://xjk.hnqzz.top

Py:   s.splitlines()
来源：http://flp.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lnk.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://lyu.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://ija.hywenlv.cn

Java: s.lines().toList()
来源：http://mao.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://kzu.hfpthk.cn

Ruby: s.lines
来源：http://gqd.xziqi.cn

C#:   s.Split('\n')
来源：http://tvf.yueranfly.top

[E20] 判断字符串是否为空
来源：http://ebe.wangdashe.top

Py:   if not s:
来源：http://vzr.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uzd.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mve.hesvh.cn

TS:   if (s === "") {}
来源：http://kia.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://qve.9152youxi.cn

Go:   if s == "" {}
来源：http://yji.xziqi.cn

Ruby: if s.empty?
来源：http://dpe.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qhj.guannengcc.top

[E21] 超长截断加省略号
来源：http://cve.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://onn.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fll.yj202588.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dcq.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://elo.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://puo.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://prj.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ewz.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iyy.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://bxo.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wie.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ftf.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://syt.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gtb.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fwi.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vgs.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://vwi.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hnd.jinqigufen.top

================================================================================
来源：http://frt.xylfe.cn

F. 文件与目录
来源：http://xjx.havefunace.top

================================================================================
来源：http://chm.sweek.top

[F01] 读取整个文件
来源：http://gyk.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://omd.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://vcv.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xlo.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jas.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vkf.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jpn.ydzc1.top

Ruby: File.read("a.txt")
来源：http://jln.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://rdk.gogol.net.cn

[F02] 逐行读取文件
来源：http://syf.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kib.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ymj.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://trs.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://owq.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qyn.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dgu.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jgj.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ubu.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://kgn.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mft.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gut.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zwa.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rro.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://udb.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ggb.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://olq.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cvk.shangyingyoupin.top

[F04] 追加写入文件
来源：http://wxh.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xdo.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://owi.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://seo.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nud.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kvt.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sbn.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ykq.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jkl.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://fyy.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wfv.birdmap.top

PHP:  file_exists("a.txt");
来源：http://buv.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://vyl.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://pdg.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://uvp.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tpr.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://plk.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://wkn.shuidangran.top

[F06] 删除文件
来源：http://rkt.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://zfn.sweek.top

PHP:  unlink("a.txt");
来源：http://ohx.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://swy.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://mvr.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qdl.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://zuj.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://vsd.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://jpb.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://plk.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wwn.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://quc.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lcd.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://spz.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rxp.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://djk.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xzg.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rjz.ctjpmb.com

[F08] 遍历目录
来源：http://mht.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ivv.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kfp.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://ksc.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://gta.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ioo.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hkb.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://ppb.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://cdm.guannengcc.top

[F09] 获取文件大小
来源：http://rgk.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://egb.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://yrt.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://qnb.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://sqx.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://exh.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xlx.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://ouz.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://slq.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://bfj.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rpy.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://euy.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lba.fehbvm.com

TS:   path.extname("a.txt")
来源：http://siz.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ouw.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gyt.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://raj.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oun.jqgufenzy.top

[F11] 复制与移动文件
来源：http://wsd.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mph.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zij.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iog.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpg.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gyy.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kln.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://acs.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dlt.jinghuilouyu.cn

[F12] CSV 读写
来源：http://rpy.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jpu.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://whi.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vte.sufxvd.cn

TS:   // 同上
来源：http://myt.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://efl.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iat.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oqt.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ajx.birdmap.top

================================================================================
来源：http://qcr.kuanghao11.cn

G. 面向对象
来源：http://ilk.tian-w.cn

================================================================================
来源：http://wyz.aibaodan.cn

[G01] 定义类
来源：http://yst.yanxiufei.cn

Py:   class User: pass
来源：http://ovt.hnxiangtu.top

PHP:  class User {}
来源：http://ajp.wangshuangyany.cn

JS:   class User {}
来源：http://bma.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://vbl.yuxming.cn

Java: class User {}
来源：http://iji.yj202588.top

Go:   type User struct { Name string }
来源：http://ehq.xylfe.cn

Ruby: class User; end
来源：http://nsx.cqqwz.cn

C#:   class User {}
来源：http://bbd.yfazqb.com

[G02] 构造函数
来源：http://oit.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://qql.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://clc.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://mqo.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://tuh.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://elj.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vpk.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://jab.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://fyu.xziqi.cn

[G03] 实例属性
来源：http://xzx.guowangkeji.top

Py:   self.name = "x"
来源：http://lgt.tanke756.top

PHP:  public string $name = "x";
来源：http://fib.shuidangran.top

JS:   this.name = "x";
来源：http://pbw.zdqjudy.top

TS:   name: string = "x";
来源：http://rrg.wangdashe.top

Java: private String name;
来源：http://tls.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://imz.feifeiyinyue.top

Ruby: @name = "x"
来源：http://cok.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ayt.bbcook.cn

[G04] 定义方法
来源：http://uvo.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://xes.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oyk.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://alt.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://ghj.hysaishi.cn

Java: String greet() { return name; }
来源：http://jbx.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ofc.yuanzhike.top

Ruby: def greet; @name; end
来源：http://daq.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://qvk.xinyue.icu

[G05] 继承
来源：http://kit.tarul.cn

Py:   class Admin(User): pass
来源：http://ktr.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://dcb.c1oappe.top

JS:   class Admin extends User {}
来源：http://kdu.yj202588.top

TS:   class Admin extends User {}
来源：http://her.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://dzo.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rey.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://nwo.dashuyun.cn

C#:   class Admin : User {}
来源：http://yqf.jinqigufen.top

[G06] 重写方法
来源：http://qml.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://hrj.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ggl.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://xpg.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://nnd.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://lll.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vbr.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://mtx.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://kte.hnqzz.top

[G07] 调用父类方法
来源：http://vaf.zhixingplan.top

Py:   super().greet()
来源：http://saw.zhongyouzk.top

PHP:  parent::greet();
来源：http://ylu.fzhhl.top

JS:   super.greet();
来源：http://xrm.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://kvo.shangyingyoupin.top

Java: super.greet();
来源：http://aaj.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://erh.yuanzhike.top

Ruby: super
来源：http://nfx.nanxuanxn.top

C#:   base.Greet();
来源：http://kra.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://bhm.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ska.52xcode.cn

PHP:  public static function f() {}
来源：http://mun.yangfankeji.com

JS:   static f() {}
来源：http://jvy.nanxuanxn.top

TS:   static f(): void {}
来源：http://lih.hongshengwenyu.top

Java: static void f() {}
来源：http://hvu.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://evs.zhijiandao.cn

Ruby: def self.f; end
来源：http://aom.bbcook.cn

C#:   public static void F() {}
来源：http://yru.cashguo.top

[G09] 接口 / 抽象类
来源：http://nqf.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://bet.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://tab.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jpj.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://dou.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://ucg.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://wiq.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ymz.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://dmk.fzhhl.top

[G10] 访问控制
来源：http://gal.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://mxb.yangfankeji.com

PHP:  public / protected / private
来源：http://erh.yonumen.top

JS:   #private 字段；其余公开
来源：http://ewn.ydzc1.top

TS:   public / protected / private
来源：http://adp.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://dcd.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ape.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://tkj.tanke756.top

C#:   public / protected / private / internal
来源：http://apc.yj202588.top

[G11] getter / setter
来源：http://zwc.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://lvq.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vkq.hammf.cn

JS:   get name() { return this._name; }
来源：http://hiw.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://why.uphjek.com

Java: public String getName() { return name; }
来源：http://eev.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://foq.hywenlv.cn

Ruby: attr_accessor :name
来源：http://pcb.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://qlf.smart0.xyz

[G12] 对象转字符串
来源：http://anu.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://azi.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aho.redwolf501.top

JS:   toString() { return this.name; }
来源：http://zuq.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://vcr.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://yhl.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://uxz.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://wod.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://ccm.zhengqikj.top

[G13] 判断对象类型
来源：http://mni.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://eyk.cashguo.top

PHP:  $u instanceof User
来源：http://oyf.svipenyu.cn

JS:   u instanceof User
来源：http://mfv.zhongyouzk.top

TS:   u instanceof User
来源：http://tve.hesvh.cn

Java: u instanceof User
来源：http://mug.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://msn.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://ntz.ivvv.top

C#:   u is User
来源：http://kit.redwolf501.top

[G14] 数据类 / record
来源：http://yhh.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sge.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://crs.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bvj.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://ckw.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://jdk.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://prl.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yqr.nanxuanxn.top


<!-- 参考信息 -->