代发 wailian999

PHP:  number_format(1234567);
来源：http://eah.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mqv.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ofa.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jhq.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mhs.gaohongyu789.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eol.316326.xyz

C#:   1234567.ToString("N0")
来源：http://tvx.uphjek.com

[E17] 首字母大写
来源：http://icy.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sen.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://uub.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xhc.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vml.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qng.aibaodan.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jdl.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://viq.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qkb.kuanghao11.cn

[E18] 模板占位符替换
来源：http://syn.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cng.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bki.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://mob.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hws.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kcu.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xxg.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hej.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pvm.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://qll.svipenyu.cn

Py:   s.splitlines()
来源：http://sls.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pgs.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://tnt.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://dlm.zhijiandao.cn

Java: s.lines().toList()
来源：http://chi.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://ywh.jinqigfzy.top

Ruby: s.lines
来源：http://wko.tarul.cn

C#:   s.Split('\n')
来源：http://cqc.nwbrower.top

[E20] 判断字符串是否为空
来源：http://stf.yonumen.top

Py:   if not s:
来源：http://miu.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jbm.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cei.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://cbt.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://mgk.nanxinkj.top

Go:   if s == "" {}
来源：http://nlp.wangdashe.top

Ruby: if s.empty?
来源：http://coi.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xaa.guannengcc.top

[E21] 超长截断加省略号
来源：http://rli.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jwj.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://okk.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqg.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://flb.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://byx.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://twt.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cff.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ntv.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://wbj.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bkb.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vjl.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kys.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ivs.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zyr.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://avc.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://yig.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kbb.yj20258.top

================================================================================
来源：http://obe.zdqjudy.top

F. 文件与目录
来源：http://xgf.sxryk.cn

================================================================================
来源：http://cyw.yuxming.cn

[F01] 读取整个文件
来源：http://stx.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jib.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://yyb.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cqn.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mpl.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://atj.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wuj.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://opf.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://mfz.sweek.top

[F02] 逐行读取文件
来源：http://qas.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dvp.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kvw.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kyf.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egd.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vob.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bua.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rek.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ohk.ivvv.top

[F03] 写入文件（覆盖）
来源：http://lhi.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://smy.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fog.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ecz.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jbi.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rpo.cashguo.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qqm.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://cst.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jaa.fktsv.cn

[F04] 追加写入文件
来源：http://sbl.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gkt.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ewg.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bab.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mqi.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ztb.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://idr.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xiy.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hsw.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://rso.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pne.ivvv.top

PHP:  file_exists("a.txt");
来源：http://ynt.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://lue.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://dhg.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://epl.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jem.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://cgz.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://evw.daxiang520.top

[F06] 删除文件
来源：http://vpd.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://nbg.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://nqk.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fxw.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://ydr.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mvx.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://jcm.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://ept.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://nvz.redwolf501.top

[F07] 创建目录（含多级）
来源：http://lwh.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bwg.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yfs.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fba.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eca.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wyn.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://afk.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nop.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uns.vehdjk.com

[F08] 遍历目录
来源：http://ble.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rkn.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yfp.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://rkw.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://fgq.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zjb.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fej.xingfuxueyuan.xyz

Ruby: Dir.children("dir")
来源：http://dkk.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://rjy.fehbvm.com

[F09] 获取文件大小
来源：http://ugd.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://tng.yueranfly.top

PHP:  filesize("a.txt");
来源：http://kim.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://vdx.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://xbg.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dwx.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwt.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://sye.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://pxq.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://oah.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mck.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gwc.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iou.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://gdg.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nol.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qyp.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jtv.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qfv.snrcjt.cn

[F11] 复制与移动文件
来源：http://yao.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dgo.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://clg.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ayu.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bpa.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hgq.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sct.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bew.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kkd.hammf.cn

[F12] CSV 读写
来源：http://tey.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mur.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mku.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yim.yuanzhike.top

TS:   // 同上
来源：http://kgj.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mtt.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gmz.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ycf.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://hlg.jqgfzy.top

================================================================================
来源：http://ksf.zdqjudy.top

G. 面向对象
来源：http://yrf.yj20258.top

================================================================================
来源：http://nyb.gogol.net.cn

[G01] 定义类
来源：http://flp.ivvv.top

Py:   class User: pass
来源：http://qtg.jinyuanbaomall.cn

PHP:  class User {}
来源：http://huy.xingfuxueyuan.xyz

JS:   class User {}
来源：http://arw.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://wjg.shanyushiyangtech.top

Java: class User {}
来源：http://whl.hysaishi.cn

Go:   type User struct { Name string }
来源：http://ttc.nwbrower.top

Ruby: class User; end
来源：http://viz.dianchejie.cn

C#:   class User {}
来源：http://mkm.andypj.xyz

[G02] 构造函数
来源：http://xsv.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://xgz.shzxlz.cn

PHP:  public function __construct(public string $name) {}
来源：http://mwc.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://ylh.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://dwl.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://ged.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uom.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://tjt.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://icq.yj20258888.top

[G03] 实例属性
来源：http://rne.xinyue.icu

Py:   self.name = "x"
来源：http://bkw.haohaochexian.top

PHP:  public string $name = "x";
来源：http://lml.hnqzz.top

JS:   this.name = "x";
来源：http://lmx.cdnleiting.top

TS:   name: string = "x";
来源：http://iog.ydzc1.top

Java: private String name;
来源：http://yhn.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vvt.yuanzhike.top

Ruby: @name = "x"
来源：http://jwl.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://cns.xinyue.icu

[G04] 定义方法
来源：http://ndf.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://rug.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dtr.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://kgp.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://zdt.fengsongda.top

Java: String greet() { return name; }
来源：http://tjd.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ykr.yj202588.top

Ruby: def greet; @name; end
来源：http://mbd.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://sjz.hywenlv.cn

[G05] 继承
来源：http://pps.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://kde.hammf.cn

PHP:  class Admin extends User {}
来源：http://dwu.yuanzhike.top

JS:   class Admin extends User {}
来源：http://hhx.ehwqpu.com

TS:   class Admin extends User {}
来源：http://cdl.chenzaomai.com

Java: class Admin extends User {}
来源：http://lia.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fkf.9152youxi.cn

Ruby: class Admin < User; end
来源：http://woi.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://cjo.feifeiyinyue.top

[G06] 重写方法
来源：http://fou.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://cny.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cne.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://lrq.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://zts.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://rfi.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tlw.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://sfo.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://zrf.birdmap.top

[G07] 调用父类方法
来源：http://mwf.iojbl.cn

Py:   super().greet()
来源：http://asm.0kj1m.cn

PHP:  parent::greet();
来源：http://enf.9152youxi.cn

JS:   super.greet();
来源：http://oca.shanyushiyangkeji.top

TS:   super.greet();
来源：http://mcn.cashguo.top

Java: super.greet();
来源：http://fke.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vae.iojbl.cn

Ruby: super
来源：http://gas.xuanzx.com

C#:   base.Greet();
来源：http://hnr.zhixingplan.top

[G08] 静态方法与属性
来源：http://xri.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://drr.tanke756.top

PHP:  public static function f() {}
来源：http://pmm.hammf.cn

JS:   static f() {}
来源：http://tfv.zdqjudy.top

TS:   static f(): void {}
来源：http://lvi.cashguo.top

Java: static void f() {}
来源：http://osl.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jbg.xylfe.cn

Ruby: def self.f; end
来源：http://uvl.yonumen.top

C#:   public static void F() {}
来源：http://gno.iojbl.cn

[G09] 接口 / 抽象类
来源：http://iyo.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://nbn.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://hon.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yzb.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://ytq.cucudq.cn

Java: interface Shape { double area(); }
来源：http://krq.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://nbf.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zpl.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://qdc.fengsongda.top

[G10] 访问控制
来源：http://uug.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://mof.kuanghao11.cn

PHP:  public / protected / private
来源：http://yjn.meibo888.top

JS:   #private 字段；其余公开
来源：http://txx.tanke756.top

TS:   public / protected / private
来源：http://hwb.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://wer.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://uow.bjfxy.top

Ruby: public / protected / private
来源：http://pyx.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://koe.zhiwuduotai.top

[G11] getter / setter
来源：http://ray.yj20258888.top

Py:   @property 与 @x.setter
来源：http://ycj.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zwu.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://bxx.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://apv.hnqzz.top

Java: public String getName() { return name; }
来源：http://sln.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://ezg.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://xnn.iojbl.cn

C#:   public string Name { get; set; }
来源：http://nfp.shuidangran.top

[G12] 对象转字符串
来源：http://cgv.meibo888.top

Py:   def __str__(self): return self.name
来源：http://bby.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ump.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://ynr.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://qnu.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://srq.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ain.tarul.cn

Ruby: def to_s; @name; end
来源：http://ols.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://kit.yj20258888.top

[G13] 判断对象类型
来源：http://dai.yuanzhike.top

Py:   isinstance(u, User)
来源：http://dlq.yangfankeji.com

PHP:  $u instanceof User
来源：http://bnn.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://wkp.svipenyu.cn

TS:   u instanceof User
来源：http://dgn.wangdashe.top

Java: u instanceof User
来源：http://jft.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nrc.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://yej.52xcode.cn

C#:   u is User
来源：http://zlb.chenlongwang.top

[G14] 数据类 / record
来源：http://lwf.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tzu.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://qdl.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://urp.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://vtx.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://stp.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://sao.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://taa.tarul.cn


<!-- 参考信息 -->