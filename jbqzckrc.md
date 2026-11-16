代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blr.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kwm.gzhubu.top

[E16] 数字千分位
来源：http://uki.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://cbn.gzhubu.top

PHP:  number_format(1234567);
来源：http://idd.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cdj.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://alt.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xdm.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qls.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ybh.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://wyh.daria6918.cn

[E17] 首字母大写
来源：http://guu.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ucd.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rsb.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfb.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bzp.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kkm.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bsg.chenjidiqi.icu

Ruby: s.capitalize
来源：http://stf.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://htg.daria6918.cn

[E18] 模板占位符替换
来源：http://bod.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zul.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lje.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xai.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zgo.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://otn.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ixq.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dhc.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ops.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://doq.dianchejie.cn

Py:   s.splitlines()
来源：http://tea.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bfw.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://kge.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://qmj.yanxiufei.cn

Java: s.lines().toList()
来源：http://oul.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://zqa.xziqi.cn

Ruby: s.lines
来源：http://gxm.yonumen.top

C#:   s.Split('\n')
来源：http://xaf.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://fma.zhongyouzk.top

Py:   if not s:
来源：http://kdt.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ccv.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pfj.xziqi.cn

TS:   if (s === "") {}
来源：http://acd.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://ipg.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://dzg.ehwqpu.com

Ruby: if s.empty?
来源：http://pnt.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bsn.jianghu66.top

[E21] 超长截断加省略号
来源：http://jxc.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pjb.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hyc.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://enf.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fhy.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bzr.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://hpq.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ekr.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ljg.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://voc.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://enp.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vew.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lrc.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sgr.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lxb.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mkt.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://rqm.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zbz.hywenlv.cn

================================================================================
来源：http://yam.yvedp.cn

F. 文件与目录
来源：http://nzc.daria6918.cn

================================================================================
来源：http://vgi.jinqigufen.top

[F01] 读取整个文件
来源：http://pvg.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eyh.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://mew.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dao.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pxg.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://zdz.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iyx.ybcxt.top

Ruby: File.read("a.txt")
来源：http://rzl.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://agl.zdqjudy.top

[F02] 逐行读取文件
来源：http://zpg.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fts.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ode.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yoz.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://miy.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://llc.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kfi.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://huc.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qey.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://iuj.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wxa.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mrl.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xvs.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdf.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://plp.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uok.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://ewl.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hwt.nanxuanxn.top

[F04] 追加写入文件
来源：http://uej.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ina.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vmb.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://afq.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ref.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vct.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://plg.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vfc.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wfk.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://eap.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bxm.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://qaw.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://zll.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://oqd.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://vwb.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aox.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://oej.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://wdc.dashuyun.cn

[F06] 删除文件
来源：http://krw.sweek.top

Py:   os.remove("a.txt")
来源：http://eew.mhx1999.top

PHP:  unlink("a.txt");
来源：http://zyw.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vdn.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://lmi.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aax.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://btq.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://ysd.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://jxd.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://gif.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wde.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pdq.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bci.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pyw.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fyq.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tkf.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tzw.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bvt.gaohongyu789.top

[F08] 遍历目录
来源：http://ick.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sli.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qyr.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://dpk.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://vwt.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qba.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ods.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://otj.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://oww.guowangkeji.top

[F09] 获取文件大小
来源：http://npv.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://ooj.gzhubu.top

PHP:  filesize("a.txt");
来源：http://sxd.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://mme.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://txd.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://rrg.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pct.redwolf501.top

Ruby: File.size("a.txt")
来源：http://alt.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://ewm.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://zfi.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://laz.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fcv.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qij.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://dhc.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://viw.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tll.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bvg.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eit.yuxming.cn

[F11] 复制与移动文件
来源：http://oba.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iyp.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iuu.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ckk.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nia.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pqn.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sln.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tfz.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wvj.gotoacloud.top

[F12] CSV 读写
来源：http://rnn.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iso.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wyf.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ozq.tianlin.xyz

TS:   // 同上
来源：http://bap.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tpu.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fbp.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kbx.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://txu.smart0.xyz

================================================================================
来源：http://ymm.fktsv.cn

G. 面向对象
来源：http://xho.sjlbkw.cn

================================================================================
来源：http://yrf.gzhubu.top

[G01] 定义类
来源：http://xhq.chenzaomai.com

Py:   class User: pass
来源：http://gxo.yongpay.top

PHP:  class User {}
来源：http://myr.yj20258888.top

JS:   class User {}
来源：http://frx.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://ivp.zdqjudy.top

Java: class User {}
来源：http://qgc.havefunace.top

Go:   type User struct { Name string }
来源：http://rit.sjlbkw.cn

Ruby: class User; end
来源：http://zod.sjlbkw.cn

C#:   class User {}
来源：http://mcw.guowangkeji.top

[G02] 构造函数
来源：http://enx.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://ejd.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://jhx.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://tpv.yonumen.top

TS:   constructor(public name: string) {}
来源：http://ada.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://qhf.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oou.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://owi.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://qbj.guannengcc.top

[G03] 实例属性
来源：http://dft.gaohongyu789.top

Py:   self.name = "x"
来源：http://cfh.nanxinkj.top

PHP:  public string $name = "x";
来源：http://eno.hywenlv.cn

JS:   this.name = "x";
来源：http://cgn.chenjidiqi.icu

TS:   name: string = "x";
来源：http://gpg.ctjpmb.com

Java: private String name;
来源：http://efb.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bic.hfpthk.cn

Ruby: @name = "x"
来源：http://qkt.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://uip.quarkkingdee.top

[G04] 定义方法
来源：http://tus.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://lzj.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ici.tanke756.top

JS:   greet() { return this.name; }
来源：http://lmd.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://zsa.yfazqb.com

Java: String greet() { return name; }
来源：http://kee.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cjr.jyoumei.cn

Ruby: def greet; @name; end
来源：http://htb.smart0.xyz

C#:   public string Greet() => Name;
来源：http://mxg.ywan-chungtsiang.top

[G05] 继承
来源：http://yzo.dashuyun.cn

Py:   class Admin(User): pass
来源：http://xmb.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://eqv.jinqigfzy.top

JS:   class Admin extends User {}
来源：http://etv.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://zuf.hnqzz.top

Java: class Admin extends User {}
来源：http://kla.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sil.tianlin.xyz

Ruby: class Admin < User; end
来源：http://xgy.dianchejie.cn

C#:   class Admin : User {}
来源：http://xeq.9152youxi.cn

[G06] 重写方法
来源：http://etn.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://jwl.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://djy.tarul.cn

JS:   greet() { return "admin"; }
来源：http://xlv.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://aoi.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://ehi.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cdm.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://swa.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://swe.yueranfly.top

[G07] 调用父类方法
来源：http://ubr.fktsv.cn

Py:   super().greet()
来源：http://muq.fehbvm.com

PHP:  parent::greet();
来源：http://qxf.dianchejie.cn

JS:   super.greet();
来源：http://lvy.quarkkingdee.top

TS:   super.greet();
来源：http://jji.zhixingplan.top

Java: super.greet();
来源：http://lgz.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rwc.andypj.xyz

Ruby: super
来源：http://giq.zdqjudy.top

C#:   base.Greet();
来源：http://zda.hfpthk.cn

[G08] 静态方法与属性
来源：http://ezc.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zty.svipenyu.cn

PHP:  public static function f() {}
来源：http://qzb.daxiang520.top

JS:   static f() {}
来源：http://wtb.shuidangran.top

TS:   static f(): void {}
来源：http://kjq.vqdsnc.cn

Java: static void f() {}
来源：http://dfj.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ulg.zdbjq.cn

Ruby: def self.f; end
来源：http://giv.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://ozp.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://apw.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://gqk.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ykz.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hkt.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://pze.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://dlc.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://fjw.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://frj.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://bqr.quarkkingdee.top

[G10] 访问控制
来源：http://xlj.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://qhp.vqdsnc.cn

PHP:  public / protected / private
来源：http://mnl.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://gtb.cheryme.top

TS:   public / protected / private
来源：http://ftq.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://neq.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://omk.fzhhl.top

Ruby: public / protected / private
来源：http://psa.daxiang520.top

C#:   public / protected / private / internal
来源：http://gxl.shanyushiyangtech.top

[G11] getter / setter
来源：http://xvx.guannengcc.top

Py:   @property 与 @x.setter
来源：http://ijo.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nxo.vehdjk.com

JS:   get name() { return this._name; }
来源：http://xzi.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://ftr.jyoumei.cn

Java: public String getName() { return name; }
来源：http://xgb.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lsi.cucudq.cn

Ruby: attr_accessor :name
来源：http://hcs.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://nhw.jianghu66.top

[G12] 对象转字符串
来源：http://pmk.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://kil.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vho.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://oax.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://jde.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://vzh.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kzy.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://jeb.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://xpt.yj20258.top

[G13] 判断对象类型
来源：http://xaj.yueranfly.top

Py:   isinstance(u, User)
来源：http://wad.tian-w.cn

PHP:  $u instanceof User
来源：http://uva.feifeiyinyue.top

JS:   u instanceof User
来源：http://zpj.jqgufenzy.top

TS:   u instanceof User
来源：http://pqo.hnxiangtu.top

Java: u instanceof User
来源：http://tzb.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kfd.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://rko.sxryk.cn

C#:   u is User
来源：http://toj.dianchejie.cn

[G14] 数据类 / record
来源：http://wzm.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rro.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://vzk.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://slo.zhijiandao.cn


<!-- 参考信息 -->