代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://puy.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cpu.nanxuanxn.top

[E16] 数字千分位
来源：http://vzg.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://gjh.jyoumei.cn

PHP:  number_format(1234567);
来源：http://lud.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tde.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://enx.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jjq.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yqu.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://izt.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://wkd.uphjek.com

[E17] 首字母大写
来源：http://nrj.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ash.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xux.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://egh.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dlw.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dew.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wry.xinyue.icu

Ruby: s.capitalize
来源：http://lys.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dch.jianghu66.top

[E18] 模板占位符替换
来源：http://uei.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cyr.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tqn.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pjs.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iiz.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vvo.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wtx.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wgj.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jlv.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://wnr.daxiang520.top

Py:   s.splitlines()
来源：http://bjh.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://krk.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://lpb.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://wap.meibo888.top

Java: s.lines().toList()
来源：http://nex.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://rli.zhongyouzk.top

Ruby: s.lines
来源：http://rld.ppjwa.cn

C#:   s.Split('\n')
来源：http://wfq.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://fwn.jinqigfzy.top

Py:   if not s:
来源：http://jyw.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pjl.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://akn.yfazqb.com

TS:   if (s === "") {}
来源：http://rka.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://nlu.yongpay.top

Go:   if s == "" {}
来源：http://jci.316326.xyz

Ruby: if s.empty?
来源：http://qll.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dzm.gogol.net.cn

[E21] 超长截断加省略号
来源：http://xij.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fdt.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vjg.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hht.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dtb.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jbo.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://mhv.chenzaomai.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hbs.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cim.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://xza.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bgt.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lww.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hfr.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://atq.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zvp.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qhw.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://ely.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uok.feifeiyinyue.top

================================================================================
来源：http://ygi.kuanghao11.cn

F. 文件与目录
来源：http://pex.gotoacloud.top

================================================================================
来源：http://qcz.xziqi.cn

[F01] 读取整个文件
来源：http://hcl.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wpl.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://wtg.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://skn.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gwm.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qvk.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jyx.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://gey.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://xuo.cqqwz.cn

[F02] 逐行读取文件
来源：http://wjy.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://des.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://efe.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prx.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zby.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tek.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wlq.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vae.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ift.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://iwy.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yfo.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mnr.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://owl.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wfz.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nfb.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jwl.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://ivy.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eaj.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://hzq.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wsg.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uhi.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://otl.andypj.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mem.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://efx.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hsl.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rdv.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://plj.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://ttf.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ufn.havefunace.top

PHP:  file_exists("a.txt");
来源：http://ijx.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://ciz.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://lhb.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://cpq.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dvy.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://ygv.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://wdf.hnqzz.top

[F06] 删除文件
来源：http://ett.fengsongda.top

Py:   os.remove("a.txt")
来源：http://uqa.hfpthk.cn

PHP:  unlink("a.txt");
来源：http://eqr.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qqz.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ynd.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hrt.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://fjk.uphjek.com

Ruby: File.delete("a.txt")
来源：http://fem.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://jqe.vehdjk.com

[F07] 创建目录（含多级）
来源：http://kat.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rar.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fjw.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ige.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dyj.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mvo.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oie.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ufl.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://shd.yj20258888.top

[F08] 遍历目录
来源：http://yhd.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xhu.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://srm.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://eoy.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://sva.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ion.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zgz.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://uvk.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://amc.cashguo.top

[F09] 获取文件大小
来源：http://cxs.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://ytc.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://feq.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://qdf.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://laj.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lqv.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tcn.shuidangran.top

Ruby: File.size("a.txt")
来源：http://zuv.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://mpm.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://dhz.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aof.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tmt.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://msq.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://dvk.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eqk.chenlongwang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zaf.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://unj.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zsr.shuidangran.top

[F11] 复制与移动文件
来源：http://giv.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wct.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jlq.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hkr.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hmy.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yxb.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jst.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ero.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zfk.chenzaomai.com

[F12] CSV 读写
来源：http://gqo.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://adj.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kuz.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rhx.jinqigfzy.top

TS:   // 同上
来源：http://oam.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ahh.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://chy.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://imn.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fik.ydjk.org.cn

================================================================================
来源：http://svk.316326.xyz

G. 面向对象
来源：http://unx.jinghuilouyu.cn

================================================================================
来源：http://dne.sxryk.cn

[G01] 定义类
来源：http://qcf.yvedp.cn

Py:   class User: pass
来源：http://sdz.cdnleiting.top

PHP:  class User {}
来源：http://xfy.gogol.net.cn

JS:   class User {}
来源：http://aup.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://mps.chenjidiqi.icu

Java: class User {}
来源：http://ids.havefunace.top

Go:   type User struct { Name string }
来源：http://wjk.sweek.top

Ruby: class User; end
来源：http://pyw.zycfv.cn

C#:   class User {}
来源：http://cxm.yongpay.top

[G02] 构造函数
来源：http://jku.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://bvb.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://uow.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://gdl.hammf.cn

TS:   constructor(public name: string) {}
来源：http://bom.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://dkt.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sga.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://oof.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://bfc.epnwcf.com

[G03] 实例属性
来源：http://gap.tarul.cn

Py:   self.name = "x"
来源：http://uan.redwolf501.top

PHP:  public string $name = "x";
来源：http://fxl.zhixingplan.top

JS:   this.name = "x";
来源：http://zsm.cqqwz.cn

TS:   name: string = "x";
来源：http://wzi.chenzaomai.com

Java: private String name;
来源：http://nuz.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ora.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://fpy.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://vnb.shuidangran.top

[G04] 定义方法
来源：http://xim.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://mfg.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lho.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://onr.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://kdp.mhx1999.top

Java: String greet() { return name; }
来源：http://ynn.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uyr.c1oappe.top

Ruby: def greet; @name; end
来源：http://hfu.guannengcc.top

C#:   public string Greet() => Name;
来源：http://ffb.hnqzz.top

[G05] 继承
来源：http://uip.pycfn.com

Py:   class Admin(User): pass
来源：http://umv.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://txk.ybcxt.top

JS:   class Admin extends User {}
来源：http://ypz.zdqjudy.top

TS:   class Admin extends User {}
来源：http://tvj.zhongyouzk.top

Java: class Admin extends User {}
来源：http://ebw.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xmr.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://cnz.cashguo.top

C#:   class Admin : User {}
来源：http://lus.fanxiaobao.xyz

[G06] 重写方法
来源：http://gtd.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://jpr.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fyc.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://ime.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://wwe.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://vvb.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uqg.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://xau.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://hyo.gotoacloud.top

[G07] 调用父类方法
来源：http://eje.sjlbkw.cn

Py:   super().greet()
来源：http://wdb.52xcode.cn

PHP:  parent::greet();
来源：http://uud.hfpthk.cn

JS:   super.greet();
来源：http://xsk.zhengqikj.top

TS:   super.greet();
来源：http://uxo.cucudq.cn

Java: super.greet();
来源：http://xin.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cqi.fehbvm.com

Ruby: super
来源：http://qla.aizwys.cn

C#:   base.Greet();
来源：http://vgr.quarkkingdee.top

[G08] 静态方法与属性
来源：http://cgw.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tng.52xcode.cn

PHP:  public static function f() {}
来源：http://kpc.redwolf501.top

JS:   static f() {}
来源：http://myh.9152youxi.cn

TS:   static f(): void {}
来源：http://tyf.zycfv.cn

Java: static void f() {}
来源：http://etm.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qrb.yj202588.top

Ruby: def self.f; end
来源：http://zci.0kj1m.cn

C#:   public static void F() {}
来源：http://ncs.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://ony.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://zhu.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://xph.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cde.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://qwf.jianghu66.top

Java: interface Shape { double area(); }
来源：http://egt.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://mhp.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ovv.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://pau.feifeiyinyue.top

[G10] 访问控制
来源：http://elo.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://bfv.gotoacloud.top

PHP:  public / protected / private
来源：http://iaa.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://gix.pengpengdd.cyou

TS:   public / protected / private
来源：http://fdg.havefunace.top

Java: public / protected / private / 默认包级
来源：http://laz.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gzc.uphjek.com

Ruby: public / protected / private
来源：http://vyu.yj20258888.top

C#:   public / protected / private / internal
来源：http://omn.smart0.xyz

[G11] getter / setter
来源：http://jge.nwbrower.top

Py:   @property 与 @x.setter
来源：http://uah.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gsj.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://pay.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://ogv.yangfankeji.com

Java: public String getName() { return name; }
来源：http://gno.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://unp.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://rgg.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://hmr.zhixingplan.top

[G12] 对象转字符串
来源：http://ifn.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://wfs.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wsx.gzhubu.top

JS:   toString() { return this.name; }
来源：http://vld.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://lhm.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://dgf.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://wxg.c1oappe.top

Ruby: def to_s; @name; end
来源：http://wtr.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://dhj.chenlongwang.top

[G13] 判断对象类型
来源：http://lvi.yvedp.cn

Py:   isinstance(u, User)
来源：http://gew.jianghu66.top

PHP:  $u instanceof User
来源：http://xik.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://kly.feifeiyinyue.top

TS:   u instanceof User
来源：http://zwy.epnwcf.com

Java: u instanceof User
来源：http://kif.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ddp.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://wyj.xziqi.cn

C#:   u is User
来源：http://qlv.yj20258.top

[G14] 数据类 / record
来源：http://lax.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rjx.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://hqy.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://qsh.hammf.cn


<!-- 参考信息 -->