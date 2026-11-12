代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sko.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gsr.tianlin.xyz

[E16] 数字千分位
来源：http://ald.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://phv.52xcode.cn

PHP:  number_format(1234567);
来源：http://kba.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wab.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yaz.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xkz.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jmv.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kwh.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://xds.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://iuq.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bdp.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ndk.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkg.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://euc.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xyt.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yur.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://keh.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nqf.hesvh.cn

[E18] 模板占位符替换
来源：http://nox.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qho.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://piu.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mpj.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://kvj.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ycu.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yqw.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dhr.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://poj.daxiang520.top

[E19] 多行文本按行拆分
来源：http://eey.pycfn.com

Py:   s.splitlines()
来源：http://ccj.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uwr.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://bcf.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://qvw.zdqjudy.top

Java: s.lines().toList()
来源：http://jmn.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://pot.nwbrower.top

Ruby: s.lines
来源：http://gmj.svipenyu.cn

C#:   s.Split('\n')
来源：http://nqg.sweek.top

[E20] 判断字符串是否为空
来源：http://vvn.wangshuangyany.cn

Py:   if not s:
来源：http://zzm.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hkl.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ycp.fengsongda.top

TS:   if (s === "") {}
来源：http://dfw.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://daz.hongshengwenyu.top

Go:   if s == "" {}
来源：http://ubc.yj202588.top

Ruby: if s.empty?
来源：http://mbb.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yav.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://ndh.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pav.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://azx.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sbf.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jwt.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rne.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://hdo.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://omt.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pxs.smart0.xyz

[E22] 字节长度与字符长度
来源：http://lzz.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tym.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wrc.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jim.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdj.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fuh.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qig.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://cqo.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jup.dashuyun.cn

================================================================================
来源：http://tct.cashguo.top

F. 文件与目录
来源：http://qkj.bbcook.cn

================================================================================
来源：http://nvf.meibo888.top

[F01] 读取整个文件
来源：http://azs.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ece.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://sbs.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jka.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sik.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hzm.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vot.epnwcf.com

Ruby: File.read("a.txt")
来源：http://itz.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://nik.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://cby.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dpc.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uld.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dwg.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yuw.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kud.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aup.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yfo.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lle.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://kda.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tub.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xsc.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zxv.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://luw.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ura.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://omw.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://hlc.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://par.zycfv.cn

[F04] 追加写入文件
来源：http://kzb.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cik.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zvh.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oxp.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zbq.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cgc.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mqf.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iet.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ktu.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://rcd.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://img.yongpay.top

PHP:  file_exists("a.txt");
来源：http://qfn.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://fdv.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://qcs.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eef.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jcl.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://mdb.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://yvn.dashuyun.cn

[F06] 删除文件
来源：http://vdu.yj202588.top

Py:   os.remove("a.txt")
来源：http://zqm.tanke756.top

PHP:  unlink("a.txt");
来源：http://sjb.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ebk.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rvc.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hte.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://zwb.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://nur.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://qku.wangdashe.top

[F07] 创建目录（含多级）
来源：http://kog.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bej.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mxx.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxz.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vao.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rqk.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aqf.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gpp.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ttu.pengpengdd.cyou

[F08] 遍历目录
来源：http://obj.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wds.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hqp.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://osr.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://ghw.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://plw.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://csh.nwbrower.top

Ruby: Dir.children("dir")
来源：http://qyo.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://fdv.mhx1999.top

[F09] 获取文件大小
来源：http://ues.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://kbt.ybcxt.top

PHP:  filesize("a.txt");
来源：http://amm.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://xkc.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://gmt.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://ibt.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nae.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://nfh.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://alr.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://abi.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zrg.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dzz.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zxi.hammf.cn

TS:   path.extname("a.txt")
来源：http://tkv.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://coc.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wtw.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kwe.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uaz.kuanghao11.cn

[F11] 复制与移动文件
来源：http://xbb.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://erf.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gde.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zzy.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ykh.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxn.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xml.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uhy.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qsc.hcnkem.com

[F12] CSV 读写
来源：http://yzj.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://plg.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zgy.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tln.quarkkingdee.top

TS:   // 同上
来源：http://ybw.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://muh.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://miw.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aqb.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://wnt.xziqi.cn

================================================================================
来源：http://xgj.yvedp.cn

G. 面向对象
来源：http://ucg.zhengqikj.top

================================================================================
来源：http://iav.xuanzx.com

[G01] 定义类
来源：http://mon.sjlbkw.cn

Py:   class User: pass
来源：http://fus.xuanzx.com

PHP:  class User {}
来源：http://snf.epnwcf.com

JS:   class User {}
来源：http://ylq.sweek.top

TS:   class User { name: string = ""; }
来源：http://zgy.havefunace.top

Java: class User {}
来源：http://gze.zycfv.cn

Go:   type User struct { Name string }
来源：http://jkz.yuxming.cn

Ruby: class User; end
来源：http://keo.zdqjudy.top

C#:   class User {}
来源：http://nlo.zhengqikj.top

[G02] 构造函数
来源：http://fml.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://rbp.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://ijp.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://pys.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://fip.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://dub.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://syv.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://efs.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://rpz.cashguo.top

[G03] 实例属性
来源：http://ovq.haohaochexian.top

Py:   self.name = "x"
来源：http://bmz.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://tym.hysaishi.cn

JS:   this.name = "x";
来源：http://kbo.ydjk.org.cn

TS:   name: string = "x";
来源：http://vzj.hysaishi.cn

Java: private String name;
来源：http://rhg.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cex.xuanzx.com

Ruby: @name = "x"
来源：http://bjo.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://iph.sxryk.cn

[G04] 定义方法
来源：http://wkp.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://oya.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qgb.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://oie.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://kqw.shzxlz.cn

Java: String greet() { return name; }
来源：http://tdy.zhixingplan.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pyv.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://vjy.wangdashe.top

C#:   public string Greet() => Name;
来源：http://tku.zhoulong.xyz

[G05] 继承
来源：http://ina.ybcxt.top

Py:   class Admin(User): pass
来源：http://esp.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://hae.andypj.xyz

JS:   class Admin extends User {}
来源：http://mxr.zhixingplan.top

TS:   class Admin extends User {}
来源：http://cxv.sufxvd.cn

Java: class Admin extends User {}
来源：http://ibc.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yhq.52xcode.cn

Ruby: class Admin < User; end
来源：http://pyg.52xcode.cn

C#:   class Admin : User {}
来源：http://efy.yanxiufei.cn

[G06] 重写方法
来源：http://aow.316326.xyz

Py:   def greet(self): return "admin"
来源：http://tjy.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://coh.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://ovi.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://puu.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://uma.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mqj.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://vti.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://kvw.wangshuangyany.cn

[G07] 调用父类方法
来源：http://vsy.fanxiaobao.xyz

Py:   super().greet()
来源：http://rsw.shzxlz.cn

PHP:  parent::greet();
来源：http://tlj.zycfv.cn

JS:   super.greet();
来源：http://ceo.iojbl.cn

TS:   super.greet();
来源：http://pdd.dianchejie.cn

Java: super.greet();
来源：http://ovd.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bze.daxiang520.top

Ruby: super
来源：http://bhd.fehbvm.com

C#:   base.Greet();
来源：http://epb.meibo888.top

[G08] 静态方法与属性
来源：http://vkd.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://phd.haohaochexian.top

PHP:  public static function f() {}
来源：http://rwq.yj20258888.top

JS:   static f() {}
来源：http://uuh.zdbjq.cn

TS:   static f(): void {}
来源：http://fwd.shanyushiyangtech.top

Java: static void f() {}
来源：http://fus.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mpz.ydjk.org.cn

Ruby: def self.f; end
来源：http://gzz.fzhhl.top

C#:   public static void F() {}
来源：http://vfl.tarul.cn

[G09] 接口 / 抽象类
来源：http://doi.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://szd.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rku.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rjx.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://ltd.daxiang520.top

Java: interface Shape { double area(); }
来源：http://yvv.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://joi.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yqt.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://pzj.hammf.cn

[G10] 访问控制
来源：http://fyp.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://etk.gzhubu.top

PHP:  public / protected / private
来源：http://aov.yongpay.top

JS:   #private 字段；其余公开
来源：http://six.hnxiangtu.top

TS:   public / protected / private
来源：http://zok.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://iap.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nbs.jqgfzy.top

Ruby: public / protected / private
来源：http://hqh.redwolf501.top

C#:   public / protected / private / internal
来源：http://mce.gaohongyu789.top

[G11] getter / setter
来源：http://ntn.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://wwt.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ssv.daria6918.cn

JS:   get name() { return this._name; }
来源：http://kbx.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://sal.shuidangran.top

Java: public String getName() { return name; }
来源：http://rmn.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://ylf.iojbl.cn

Ruby: attr_accessor :name
来源：http://aew.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://zxu.meibo888.top

[G12] 对象转字符串
来源：http://qcb.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://orq.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qbv.yj202588.top

JS:   toString() { return this.name; }
来源：http://bkd.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://cgs.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://elk.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://wxt.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://osx.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://fig.hesvh.cn

[G13] 判断对象类型
来源：http://ofh.guowangkeji.top

Py:   isinstance(u, User)
来源：http://yyq.chenzaomai.com

PHP:  $u instanceof User
来源：http://jcn.jlsjyb.cn

JS:   u instanceof User
来源：http://svz.dianchejie.cn

TS:   u instanceof User
来源：http://kvh.andypj.xyz

Java: u instanceof User
来源：http://ync.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gal.cucudq.cn

Ruby: u.is_a?(User)
来源：http://ano.ydjk.org.cn

C#:   u is User
来源：http://wtr.aibaodan.cn

[G14] 数据类 / record
来源：http://gzg.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://crg.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://wmv.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://gqq.quarkkingdee.top


<!-- 参考信息 -->