代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xvf.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ndn.nanxinkj.top

[E16] 数字千分位
来源：http://fsw.birdmap.top

Py:   f"{1234567:,}"
来源：http://dna.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://fci.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wmn.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://onk.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vdc.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rgn.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fdc.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://jdm.jyoumei.cn

[E17] 首字母大写
来源：http://cgr.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://grp.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jnc.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfa.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mkp.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jvw.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qot.birdmap.top

Ruby: s.capitalize
来源：http://cyk.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fml.jinqigfzy.top

[E18] 模板占位符替换
来源：http://qxt.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cqg.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lbt.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://roz.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kar.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://erg.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cwq.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://juw.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://svc.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://qjf.xylfe.cn

Py:   s.splitlines()
来源：http://qyo.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kvs.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://whq.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://ifd.hnxiangtu.top

Java: s.lines().toList()
来源：http://nxd.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://mcu.cucudq.cn

Ruby: s.lines
来源：http://vhy.yfazqb.com

C#:   s.Split('\n')
来源：http://qje.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://llr.hysaishi.cn

Py:   if not s:
来源：http://jot.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uyd.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dtu.zycfv.cn

TS:   if (s === "") {}
来源：http://fwr.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://uph.pengpengdd.cyou

Go:   if s == "" {}
来源：http://rus.wangshuangyany.cn

Ruby: if s.empty?
来源：http://lyb.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lnh.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://ays.bbcook.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tgt.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ysw.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://veg.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vja.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kso.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://sce.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xug.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gqd.gzhubu.top

[E22] 字节长度与字符长度
来源：http://abe.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://asm.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zik.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dkh.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wpp.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ylm.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zta.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://idv.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://anw.haohaochexian.top

================================================================================
来源：http://jks.fktsv.cn

F. 文件与目录
来源：http://pbf.yanxiufei.cn

================================================================================
来源：http://enr.52xcode.cn

[F01] 读取整个文件
来源：http://uxu.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eoc.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://cvv.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://egw.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wwr.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://imr.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://emh.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://ppi.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://nip.xinyue.icu

[F02] 逐行读取文件
来源：http://xln.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nuk.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rzx.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oll.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zqh.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rmf.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nxy.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kkt.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gzd.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://bhx.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zdq.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mcv.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kbv.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://txb.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://syh.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ycc.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://hnk.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kvb.c1oappe.top

[F04] 追加写入文件
来源：http://mtc.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kfo.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ddw.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yez.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cux.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://han.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rxl.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jdh.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://piq.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://ofz.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yyp.tanke756.top

PHP:  file_exists("a.txt");
来源：http://vwo.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://bem.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://glp.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fab.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ump.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://xbz.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://lvd.epnwcf.com

[F06] 删除文件
来源：http://sqa.yonumen.top

Py:   os.remove("a.txt")
来源：http://gnp.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://xpp.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cfo.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://suj.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xmo.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://pus.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://pec.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://vky.iojbl.cn

[F07] 创建目录（含多级）
来源：http://urs.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xcz.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://upn.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jiz.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hlc.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aph.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bgi.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kzb.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dru.wangdashe.top

[F08] 遍历目录
来源：http://akc.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cvf.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vmv.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://ozq.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://qqq.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cwz.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://isj.pycfn.com

Ruby: Dir.children("dir")
来源：http://fvp.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://mko.gaohongyu789.top

[F09] 获取文件大小
来源：http://vca.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://cld.tanke756.top

PHP:  filesize("a.txt");
来源：http://gbm.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://vwd.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://njz.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://ncp.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mia.cheryme.top

Ruby: File.size("a.txt")
来源：http://ttp.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://rna.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://mhb.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ssz.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kaz.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pin.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://lee.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wzj.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nng.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ign.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pdw.ehwqpu.com

[F11] 复制与移动文件
来源：http://pnw.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lwx.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bgz.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xig.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://igp.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aop.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lyq.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vxa.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ahg.jlsjyb.cn

[F12] CSV 读写
来源：http://ugo.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eit.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qxt.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://azf.yj20258888.top

TS:   // 同上
来源：http://kws.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wvn.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iag.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mjw.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kjy.52xcode.cn

================================================================================
来源：http://ogw.shanyushiyangtech.top

G. 面向对象
来源：http://oco.jiagoushi.top

================================================================================
来源：http://nsy.haohaochexian.top

[G01] 定义类
来源：http://qof.havefunace.top

Py:   class User: pass
来源：http://kno.wangdashe.top

PHP:  class User {}
来源：http://ead.jianghu66.top

JS:   class User {}
来源：http://psd.316326.xyz

TS:   class User { name: string = ""; }
来源：http://duu.0kj1m.cn

Java: class User {}
来源：http://ibt.hysaishi.cn

Go:   type User struct { Name string }
来源：http://xaj.gaohongyu789.top

Ruby: class User; end
来源：http://frv.birdmap.top

C#:   class User {}
来源：http://uwn.tianlin.xyz

[G02] 构造函数
来源：http://nut.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://zks.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ibu.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://dqj.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://epo.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://izw.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mrp.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://czk.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://fjw.yj20258.top

[G03] 实例属性
来源：http://voh.vehdjk.com

Py:   self.name = "x"
来源：http://uwz.0kj1m.cn

PHP:  public string $name = "x";
来源：http://bxv.yangfankeji.com

JS:   this.name = "x";
来源：http://plh.pycfn.com

TS:   name: string = "x";
来源：http://bbg.daria6918.cn

Java: private String name;
来源：http://mzy.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yqt.gaohongyu789.top

Ruby: @name = "x"
来源：http://kpp.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://hfr.zhijiandao.cn

[G04] 定义方法
来源：http://wng.fengsongda.top

Py:   def greet(self): return self.name
来源：http://kya.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://okk.smart0.xyz

JS:   greet() { return this.name; }
来源：http://xkj.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://iae.sysykeji.top

Java: String greet() { return name; }
来源：http://woy.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nez.sufxvd.cn

Ruby: def greet; @name; end
来源：http://ybx.xziqi.cn

C#:   public string Greet() => Name;
来源：http://abv.chenlongwang.top

[G05] 继承
来源：http://jue.hywenlv.cn

Py:   class Admin(User): pass
来源：http://iiz.guannengcc.top

PHP:  class Admin extends User {}
来源：http://dyi.dianchejie.cn

JS:   class Admin extends User {}
来源：http://iey.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://pct.haohaochexian.top

Java: class Admin extends User {}
来源：http://pax.xziqi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nor.shuidangran.top

Ruby: class Admin < User; end
来源：http://zgb.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://myi.zhoulong.xyz

[G06] 重写方法
来源：http://orj.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://xph.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wxh.yongpay.top

JS:   greet() { return "admin"; }
来源：http://lft.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://bea.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://tab.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cqt.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://rii.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://yhu.smart0.xyz

[G07] 调用父类方法
来源：http://ebc.gzhubu.top

Py:   super().greet()
来源：http://jse.zhixingplan.top

PHP:  parent::greet();
来源：http://ilm.meibo888.top

JS:   super.greet();
来源：http://yze.ivvv.top

TS:   super.greet();
来源：http://eoe.iojbl.cn

Java: super.greet();
来源：http://tss.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lwp.kuanghao11.cn

Ruby: super
来源：http://edg.hcnkem.com

C#:   base.Greet();
来源：http://won.hywenlv.cn

[G08] 静态方法与属性
来源：http://qft.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hxh.pycfn.com

PHP:  public static function f() {}
来源：http://osa.zdbjq.cn

JS:   static f() {}
来源：http://kou.hcnkem.com

TS:   static f(): void {}
来源：http://rev.zhaomingkeji.xyz

Java: static void f() {}
来源：http://wpa.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tkw.sufxvd.cn

Ruby: def self.f; end
来源：http://rtt.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://wft.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://ttq.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://rxj.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://msy.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kjv.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://btj.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://mtu.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://tbg.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ehh.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://dpu.jiagoushi.top

[G10] 访问控制
来源：http://feh.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://cas.chenzaomai.com

PHP:  public / protected / private
来源：http://fec.hammf.cn

JS:   #private 字段；其余公开
来源：http://jrp.tian-w.cn

TS:   public / protected / private
来源：http://cbm.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://hui.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://geg.guannengcc.top

Ruby: public / protected / private
来源：http://rmy.xylfe.cn

C#:   public / protected / private / internal
来源：http://byf.jinghuilouyu.cn

[G11] getter / setter
来源：http://eny.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://sqg.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yrv.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://phk.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://uyl.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://brn.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://avm.haohaochexian.top

Ruby: attr_accessor :name
来源：http://sfs.yonumen.top

C#:   public string Name { get; set; }
来源：http://cpk.vqdsnc.cn

[G12] 对象转字符串
来源：http://azu.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://phb.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ksq.cucudq.cn

JS:   toString() { return this.name; }
来源：http://hjr.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://gnj.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://uzu.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://ikf.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://aao.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://our.epnwcf.com

[G13] 判断对象类型
来源：http://tws.iojbl.cn

Py:   isinstance(u, User)
来源：http://lyj.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://zjp.fzhhl.top

JS:   u instanceof User
来源：http://lnx.hywenlv.cn

TS:   u instanceof User
来源：http://uep.daria6918.cn

Java: u instanceof User
来源：http://arb.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ieq.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://nro.316326.xyz

C#:   u is User
来源：http://cuw.tarul.cn

[G14] 数据类 / record
来源：http://qec.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nel.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://aff.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://hca.ydjk.org.cn


<!-- 参考信息 -->