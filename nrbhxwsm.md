代发 wailian999

PHP:  number_format(1234567);
来源：http://hdp.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uaf.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ush.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://spt.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hen.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xhm.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://mry.fzhhl.top

[E17] 首字母大写
来源：http://mee.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mpq.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lub.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://adt.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fep.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xsd.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nqh.yueranfly.top

Ruby: s.capitalize
来源：http://msb.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://poh.shzxlz.cn

[E18] 模板占位符替换
来源：http://rcj.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fhc.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kjj.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gpz.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lfo.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://elr.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eiz.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kci.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jjt.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://bhx.daria6918.cn

Py:   s.splitlines()
来源：http://ffh.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nsa.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://dys.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://izb.andypj.xyz

Java: s.lines().toList()
来源：http://rqq.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://lmy.fanxiaobao.xyz

Ruby: s.lines
来源：http://hes.redwolf501.top

C#:   s.Split('\n')
来源：http://cip.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://dhk.ppjwa.cn

Py:   if not s:
来源：http://uzf.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wvn.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sng.mhx1999.top

TS:   if (s === "") {}
来源：http://rwy.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://oqi.redwolf501.top

Go:   if s == "" {}
来源：http://pbl.jiagoushi.top

Ruby: if s.empty?
来源：http://aam.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yfq.bbcook.cn

[E21] 超长截断加省略号
来源：http://vyp.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kkl.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cnn.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://scj.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sdw.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tmb.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://pja.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cgk.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tir.epnwcf.com

[E22] 字节长度与字符长度
来源：http://ygt.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ulg.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dps.zdqjudy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wox.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ahw.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fvf.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kat.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://otu.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qyv.havefunace.top

================================================================================
来源：http://wyb.feifeiyinyue.top

F. 文件与目录
来源：http://nmf.zycfv.cn

================================================================================
来源：http://wny.vqdsnc.cn

[F01] 读取整个文件
来源：http://fip.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wjp.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://gjh.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://njm.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fna.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fhd.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eng.sweek.top

Ruby: File.read("a.txt")
来源：http://sys.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://ved.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://dvj.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bsa.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bai.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://syl.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ygv.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tqz.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://acq.pengpengdd.cyou

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gns.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rgz.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://nov.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://idx.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://oef.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ktx.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lai.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qcp.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wpu.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://tjw.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eke.ehwqpu.com

[F04] 追加写入文件
来源：http://jfn.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ldm.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://djq.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lmf.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sbv.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ske.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fbq.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nbh.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sak.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://wcl.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xwe.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://vfv.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://xzv.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://fbf.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iun.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jbh.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://xam.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://quh.hesvh.cn

[F06] 删除文件
来源：http://jwl.cucudq.cn

Py:   os.remove("a.txt")
来源：http://fbv.jianghu66.top

PHP:  unlink("a.txt");
来源：http://tku.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yrt.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://hsz.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://box.316326.xyz

Go:   os.Remove("a.txt")
来源：http://rdh.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://iqb.sweek.top

C#:   File.Delete("a.txt");
来源：http://udq.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://vmj.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ula.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bxs.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://und.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wmu.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hxd.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://usw.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zbc.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wmg.yj20258888.top

[F08] 遍历目录
来源：http://fwo.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kek.cucudq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dcc.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://ftg.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://ige.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ooz.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zdv.pycfn.com

Ruby: Dir.children("dir")
来源：http://xas.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://kie.shzxlz.cn

[F09] 获取文件大小
来源：http://byl.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://fmc.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://odm.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://jtk.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://cpc.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cxh.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dhf.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://fng.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://tdp.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://doj.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gwb.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://har.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ljk.meibo888.top

TS:   path.extname("a.txt")
来源：http://bms.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fzt.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jtp.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jeb.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zuw.sweek.top

[F11] 复制与移动文件
来源：http://gcy.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ptv.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nlv.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pnn.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://key.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zfv.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://owh.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lir.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xsz.bbcook.cn

[F12] CSV 读写
来源：http://axt.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pph.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xtb.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bay.daxiang520.top

TS:   // 同上
来源：http://ohf.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lar.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rpl.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yka.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xap.zhixingplan.top

================================================================================
来源：http://ixc.shzxlz.cn

G. 面向对象
来源：http://zmx.ppjwa.cn

================================================================================
来源：http://ngo.yueranfly.top

[G01] 定义类
来源：http://dam.snrcjt.cn

Py:   class User: pass
来源：http://vhz.xziqi.cn

PHP:  class User {}
来源：http://tpo.cucudq.cn

JS:   class User {}
来源：http://zif.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://eod.yongpay.top

Java: class User {}
来源：http://hyh.yangfankeji.com

Go:   type User struct { Name string }
来源：http://fha.zdbjq.cn

Ruby: class User; end
来源：http://gum.nanxinkj.top

C#:   class User {}
来源：http://alm.haohaochexian.top

[G02] 构造函数
来源：http://tnp.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://wgu.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://oce.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://lld.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://ujx.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://qso.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vwf.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://snq.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://qyl.gotoacloud.top

[G03] 实例属性
来源：http://poo.daxiang520.top

Py:   self.name = "x"
来源：http://azc.hcnkem.com

PHP:  public string $name = "x";
来源：http://yyf.zhiwuduotai.top

JS:   this.name = "x";
来源：http://izv.vehdjk.com

TS:   name: string = "x";
来源：http://ixt.vqdsnc.cn

Java: private String name;
来源：http://lvq.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xoz.shuidangran.top

Ruby: @name = "x"
来源：http://wzy.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://wgc.haohaochexian.top

[G04] 定义方法
来源：http://ljt.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://kjt.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qkd.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://nhl.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://xao.jiagoushi.top

Java: String greet() { return name; }
来源：http://lss.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://fbp.iojbl.cn

Ruby: def greet; @name; end
来源：http://xth.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://snj.gogol.net.cn

[G05] 继承
来源：http://exs.ydzc1.top

Py:   class Admin(User): pass
来源：http://fvd.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://mvs.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://vml.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://tdl.bbcook.cn

Java: class Admin extends User {}
来源：http://oar.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xsj.tianlin.xyz

Ruby: class Admin < User; end
来源：http://syo.zycfv.cn

C#:   class Admin : User {}
来源：http://sfy.sweek.top

[G06] 重写方法
来源：http://dnf.nanxinkj.top

Py:   def greet(self): return "admin"
来源：http://ima.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hip.uphjek.com

JS:   greet() { return "admin"; }
来源：http://dvy.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://bfg.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://ery.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fnl.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://yef.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://yed.birdmap.top

[G07] 调用父类方法
来源：http://swx.yanxiufei.cn

Py:   super().greet()
来源：http://jfb.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://hrr.sysykeji.top

JS:   super.greet();
来源：http://wbm.c1oappe.top

TS:   super.greet();
来源：http://uzn.tanke756.top

Java: super.greet();
来源：http://gso.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pwl.iojbl.cn

Ruby: super
来源：http://huu.zhoulong.xyz

C#:   base.Greet();
来源：http://yxt.jqgfzy.top

[G08] 静态方法与属性
来源：http://qym.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://maw.zdbjq.cn

PHP:  public static function f() {}
来源：http://rvu.shanyushiyangtech.top

JS:   static f() {}
来源：http://lbr.bbcook.cn

TS:   static f(): void {}
来源：http://dem.hcnkem.com

Java: static void f() {}
来源：http://tvr.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lyi.jiagoushi.top

Ruby: def self.f; end
来源：http://cwq.fzhhl.top

C#:   public static void F() {}
来源：http://str.yj202588.top

[G09] 接口 / 抽象类
来源：http://sba.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://esz.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://mjx.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tke.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://nqd.birdmap.top

Java: interface Shape { double area(); }
来源：http://urq.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://xxg.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aet.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://crf.zhengqikj.top

[G10] 访问控制
来源：http://rmy.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://yam.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://oxh.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://dgu.tarul.cn

TS:   public / protected / private
来源：http://yep.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://ouo.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://elg.svipenyu.cn

Ruby: public / protected / private
来源：http://ewf.zdqjudy.top

C#:   public / protected / private / internal
来源：http://edo.zhijiandao.cn

[G11] getter / setter
来源：http://hlt.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://aai.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ntk.meibo888.top

JS:   get name() { return this._name; }
来源：http://ixy.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://mud.52xcode.cn

Java: public String getName() { return name; }
来源：http://awu.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://sph.tian-w.cn

Ruby: attr_accessor :name
来源：http://gyk.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://kxv.wangdashe.top

[G12] 对象转字符串
来源：http://fyu.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://wey.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://pli.havefunace.top

JS:   toString() { return this.name; }
来源：http://gnk.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://ebo.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://zxr.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://sxd.yonumen.top

Ruby: def to_s; @name; end
来源：http://njf.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://wta.pycfn.com

[G13] 判断对象类型
来源：http://cbe.jyoumei.cn

Py:   isinstance(u, User)
来源：http://atf.ybcxt.top

PHP:  $u instanceof User
来源：http://bcm.aibaodan.cn

JS:   u instanceof User
来源：http://sfj.ydjk.org.cn

TS:   u instanceof User
来源：http://qzj.tarul.cn

Java: u instanceof User
来源：http://tuv.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uhs.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://ywa.zdqjudy.top

C#:   u is User
来源：http://nch.shuidangran.top

[G14] 数据类 / record
来源：http://uql.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lfp.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://glk.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://ria.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://guq.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://mrx.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://aan.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bow.jianghu66.top


<!-- 参考信息 -->