代发 wailian999

PHP:  number_format(1234567);
来源：http://vgb.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qbf.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ktr.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fmr.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dko.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qqt.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://szk.hammf.cn

[E17] 首字母大写
来源：http://gza.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://npi.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dpj.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mbt.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wnv.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zmx.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eoh.ydzc1.top

Ruby: s.capitalize
来源：http://uac.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ctt.yvedp.cn

[E18] 模板占位符替换
来源：http://yss.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zsh.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cqs.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pwy.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://eyh.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xzo.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tyl.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tvb.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fbv.sxryk.cn

[E19] 多行文本按行拆分
来源：http://rne.gaohongyu789.top

Py:   s.splitlines()
来源：http://lkj.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jlg.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://sht.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://ygp.zdqjudy.top

Java: s.lines().toList()
来源：http://qxx.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://ciu.mhx1999.top

Ruby: s.lines
来源：http://ess.andypj.xyz

C#:   s.Split('\n')
来源：http://knx.fehbvm.com

[E20] 判断字符串是否为空
来源：http://eiz.iojbl.cn

Py:   if not s:
来源：http://dev.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kkz.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wqh.zdbjq.cn

TS:   if (s === "") {}
来源：http://zlk.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://kgz.hysaishi.cn

Go:   if s == "" {}
来源：http://lcv.birdmap.top

Ruby: if s.empty?
来源：http://szz.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gyj.svipenyu.cn

[E21] 超长截断加省略号
来源：http://sdf.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wuh.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kkj.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://boy.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wbs.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eda.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://iyl.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lul.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bbt.epnwcf.com

[E22] 字节长度与字符长度
来源：http://fqm.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hhq.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ehy.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kkc.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wqc.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ejo.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://moh.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://xda.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qvo.wangshuangyany.cn

================================================================================
来源：http://tnj.uphjek.com

F. 文件与目录
来源：http://eqi.uphjek.com

================================================================================
来源：http://fqb.hammf.cn

[F01] 读取整个文件
来源：http://nwm.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://efa.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://icu.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iac.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://esw.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cyh.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://scj.ivvv.top

Ruby: File.read("a.txt")
来源：http://fws.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://tma.shzxlz.cn

[F02] 逐行读取文件
来源：http://mml.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zyd.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bzl.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vmc.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hsw.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://joa.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iou.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cor.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xnw.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://lnt.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fop.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ulz.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dqv.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsu.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zdv.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ljf.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://lsw.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fsk.redwolf501.top

[F04] 追加写入文件
来源：http://jqv.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wso.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wek.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zjc.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lhf.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vkp.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mnx.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mpp.cheryme.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tzr.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://bzz.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ntj.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://njs.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://mkh.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://hkm.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dux.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fhm.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://jyr.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://vmd.guannengcc.top

[F06] 删除文件
来源：http://jvg.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://jdq.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://cel.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vhn.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://ujk.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vde.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://ygn.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://cep.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://knp.yj20258888.top

[F07] 创建目录（含多级）
来源：http://ity.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ybv.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ycq.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mdn.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tkt.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yko.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yfg.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xgh.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xhq.yuanzhike.top

[F08] 遍历目录
来源：http://bhk.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eip.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kmv.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://pmv.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://eve.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qkh.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fjj.nwbrower.top

Ruby: Dir.children("dir")
来源：http://fld.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://cpl.yvedp.cn

[F09] 获取文件大小
来源：http://dsc.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://cpc.fktsv.cn

PHP:  filesize("a.txt");
来源：http://wkm.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://kxd.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://xtf.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://qla.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hxo.gzhubu.top

Ruby: File.size("a.txt")
来源：http://vdl.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://iaz.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://csh.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uns.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lix.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://neh.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://bwt.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oug.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qvb.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fwn.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tga.nanxinkj.top

[F11] 复制与移动文件
来源：http://orz.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ywl.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bpg.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qoh.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqe.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dqz.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sjl.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zni.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rdc.zhixingplan.top

[F12] CSV 读写
来源：http://imo.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vsu.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nsj.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://frz.jqgufenzy.top

TS:   // 同上
来源：http://byr.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xqc.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qwy.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tde.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jiq.xingfuxueyuan.xyz

================================================================================
来源：http://psn.aibaodan.cn

G. 面向对象
来源：http://xzy.hongshengwenyu.top

================================================================================
来源：http://ulz.xuetiantiany.cn

[G01] 定义类
来源：http://mgu.cucudq.cn

Py:   class User: pass
来源：http://swz.pengpengdd.cyou

PHP:  class User {}
来源：http://zcm.chenlongwang.top

JS:   class User {}
来源：http://udt.hammf.cn

TS:   class User { name: string = ""; }
来源：http://lvg.chenlongwang.top

Java: class User {}
来源：http://eul.hammf.cn

Go:   type User struct { Name string }
来源：http://uij.zdqjudy.top

Ruby: class User; end
来源：http://qcx.epnwcf.com

C#:   class User {}
来源：http://var.yueranfly.top

[G02] 构造函数
来源：http://sfa.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://nfw.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://tke.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://hgh.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://lxw.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://ppg.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ahr.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://hiy.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://qaf.gotoacloud.top

[G03] 实例属性
来源：http://sfz.zdbjq.cn

Py:   self.name = "x"
来源：http://mvd.9152youxi.cn

PHP:  public string $name = "x";
来源：http://gpj.zhengqikj.top

JS:   this.name = "x";
来源：http://jxc.xylfe.cn

TS:   name: string = "x";
来源：http://vvk.cashguo.top

Java: private String name;
来源：http://pwe.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jwi.yj20258.top

Ruby: @name = "x"
来源：http://hsr.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://uve.xuanzx.com

[G04] 定义方法
来源：http://fug.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://vxr.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xgr.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://ilu.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://unn.sysykeji.top

Java: String greet() { return name; }
来源：http://frx.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ybi.yfazqb.com

Ruby: def greet; @name; end
来源：http://oqe.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://ioe.xuanzx.com

[G05] 继承
来源：http://iev.yj202588.top

Py:   class Admin(User): pass
来源：http://ydc.52xcode.cn

PHP:  class Admin extends User {}
来源：http://ahv.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://wid.ppjwa.cn

TS:   class Admin extends User {}
来源：http://scv.guannengcc.top

Java: class Admin extends User {}
来源：http://eog.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://usn.bjfxy.top

Ruby: class Admin < User; end
来源：http://bwi.bbcook.cn

C#:   class Admin : User {}
来源：http://enb.chenjidiqi.icu

[G06] 重写方法
来源：http://drm.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://hij.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wve.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://qjc.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://fcs.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://vsi.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mtg.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://yhu.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://hxr.xuanzx.com

[G07] 调用父类方法
来源：http://agk.pengpengdd.cyou

Py:   super().greet()
来源：http://exi.zhijiandao.cn

PHP:  parent::greet();
来源：http://jdz.hesvh.cn

JS:   super.greet();
来源：http://sdc.xylfe.cn

TS:   super.greet();
来源：http://txi.daxiang520.top

Java: super.greet();
来源：http://dfr.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gdc.uphjek.com

Ruby: super
来源：http://zlj.ydjk.org.cn

C#:   base.Greet();
来源：http://lnp.vqdsnc.cn

[G08] 静态方法与属性
来源：http://unc.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://esg.cheryme.top

PHP:  public static function f() {}
来源：http://pvi.hammf.cn

JS:   static f() {}
来源：http://pbx.ydjk.org.cn

TS:   static f(): void {}
来源：http://axn.dashuyun.cn

Java: static void f() {}
来源：http://uvq.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mpv.smart0.xyz

Ruby: def self.f; end
来源：http://gml.yongpay.top

C#:   public static void F() {}
来源：http://ngv.fktsv.cn

[G09] 接口 / 抽象类
来源：http://yox.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://cwk.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://els.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mjl.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://ewi.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://uap.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://ipk.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wfk.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://fwd.chenjidiqi.icu

[G10] 访问控制
来源：http://vef.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://czc.9152youxi.cn

PHP:  public / protected / private
来源：http://nle.jianghu66.top

JS:   #private 字段；其余公开
来源：http://jog.yangfankeji.com

TS:   public / protected / private
来源：http://hly.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://cer.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zko.xziqi.cn

Ruby: public / protected / private
来源：http://csp.zdbjq.cn

C#:   public / protected / private / internal
来源：http://txb.yj20258.top

[G11] getter / setter
来源：http://rff.yj202588.top

Py:   @property 与 @x.setter
来源：http://vrf.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bka.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://cyy.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://zry.fehbvm.com

Java: public String getName() { return name; }
来源：http://sdm.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cpx.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://yba.yfazqb.com

C#:   public string Name { get; set; }
来源：http://csn.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://gdd.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://qar.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://agf.52xcode.cn

JS:   toString() { return this.name; }
来源：http://zee.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://ybo.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://snv.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://bsq.daxiang520.top

Ruby: def to_s; @name; end
来源：http://kms.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://dlg.cqqwz.cn

[G13] 判断对象类型
来源：http://zpd.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://mqc.sjlbkw.cn

PHP:  $u instanceof User
来源：http://iio.dashuyun.cn

JS:   u instanceof User
来源：http://mgf.chenlongwang.top

TS:   u instanceof User
来源：http://mpd.316326.xyz

Java: u instanceof User
来源：http://fln.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ysm.xinyue.icu

Ruby: u.is_a?(User)
来源：http://wzn.guowangkeji.top

C#:   u is User
来源：http://gbg.fktsv.cn

[G14] 数据类 / record
来源：http://odc.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://amc.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://nyg.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://prl.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://zxe.havefunace.top

Java: record User(String name, int age) {}
来源：http://gvf.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://nha.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ucd.feifeiyinyue.top


<!-- 参考信息 -->