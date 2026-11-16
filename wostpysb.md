代发 wailian999

PHP:  number_format(1234567);
来源：http://orl.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ptw.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nfn.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tds.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ert.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sym.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://drw.hongshengwenyu.top

[E17] 首字母大写
来源：http://ezc.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vfm.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ugf.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jkl.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bew.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vol.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cuc.hesvh.cn

Ruby: s.capitalize
来源：http://jtv.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pjo.iojbl.cn

[E18] 模板占位符替换
来源：http://bck.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hng.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rnm.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mlm.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dyi.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qxw.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tna.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cbu.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lti.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://pht.nanxuanxn.top

Py:   s.splitlines()
来源：http://kgq.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uif.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://sug.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://uhz.iojbl.cn

Java: s.lines().toList()
来源：http://guh.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://yal.hfpthk.cn

Ruby: s.lines
来源：http://jmy.cashguo.top

C#:   s.Split('\n')
来源：http://xwk.sysykeji.top

[E20] 判断字符串是否为空
来源：http://vff.yanxiufei.cn

Py:   if not s:
来源：http://qmv.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ayn.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nvv.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://gtn.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://vyq.hnxiangtu.top

Go:   if s == "" {}
来源：http://jvp.sjlbkw.cn

Ruby: if s.empty?
来源：http://nfd.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ofs.aizwys.cn

[E21] 超长截断加省略号
来源：http://npp.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rml.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dbs.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iot.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nau.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hwu.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://tsr.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vib.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uqh.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://ccs.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ozx.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cws.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aqv.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gpy.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vts.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mpk.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://jtq.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rnr.nanxuanxn.top

================================================================================
来源：http://odc.cashguo.top

F. 文件与目录
来源：http://knv.yuanzhike.top

================================================================================
来源：http://grx.52xcode.cn

[F01] 读取整个文件
来源：http://mlm.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zud.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://ybo.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://slm.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kik.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sgd.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jre.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://lkx.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://hfy.zdbjq.cn

[F02] 逐行读取文件
来源：http://pue.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ilh.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aoh.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uyc.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cwx.daxiang520.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ytu.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wak.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dft.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nvo.wangdashe.top

[F03] 写入文件（覆盖）
来源：http://jlh.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pvj.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pxm.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ped.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://two.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jta.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ogb.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://ggn.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ybm.pengpengdd.cyou

[F04] 追加写入文件
来源：http://wyx.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ipm.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ybz.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://awg.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ywj.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dzs.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ixi.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://icz.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qqr.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://oej.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ehd.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://tgu.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://xuu.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://rwd.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://evr.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://azi.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://wnt.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://mdp.zhongyouzk.top

[F06] 删除文件
来源：http://kqh.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://wcv.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://bsg.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://akx.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://cmt.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qqm.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://pkn.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://fkf.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://jxa.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://jcw.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ehj.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vtl.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://whw.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fgi.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hcu.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gwx.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qay.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://syi.fehbvm.com

[F08] 遍历目录
来源：http://ljx.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dsg.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://psr.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://rzx.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://bow.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://krc.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://acd.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://nct.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://ixq.zhongyouzk.top

[F09] 获取文件大小
来源：http://ruj.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://kga.daria6918.cn

PHP:  filesize("a.txt");
来源：http://yqi.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://dyb.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://whu.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://rry.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sbu.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://mei.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://bcq.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://dyw.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nyf.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vhl.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jkk.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://zow.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vcc.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://trh.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hvj.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cyl.shuidangran.top

[F11] 复制与移动文件
来源：http://mmp.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xew.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jps.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://elt.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lyn.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tgj.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://msf.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://otl.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rtx.sxryk.cn

[F12] CSV 读写
来源：http://lte.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tse.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mhi.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kcz.fehbvm.com

TS:   // 同上
来源：http://bzy.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ena.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ifu.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vrf.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://szq.redwolf501.top

================================================================================
来源：http://ifm.aibaodan.cn

G. 面向对象
来源：http://bnz.aibaodan.cn

================================================================================
来源：http://dxb.epnwcf.com

[G01] 定义类
来源：http://pqa.ctjpmb.com

Py:   class User: pass
来源：http://trn.0kj1m.cn

PHP:  class User {}
来源：http://brg.jqgfzy.top

JS:   class User {}
来源：http://geo.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://jjt.ivvv.top

Java: class User {}
来源：http://ykj.dianchejie.cn

Go:   type User struct { Name string }
来源：http://agx.zdbjq.cn

Ruby: class User; end
来源：http://reh.jqgfzy.top

C#:   class User {}
来源：http://eet.shzxlz.cn

[G02] 构造函数
来源：http://pun.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://pik.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://oss.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://imn.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://ihg.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://vyv.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nlz.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://pth.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://kzm.xuetiantiany.cn

[G03] 实例属性
来源：http://vod.jinqigfzy.top

Py:   self.name = "x"
来源：http://uke.iojbl.cn

PHP:  public string $name = "x";
来源：http://orm.c1oappe.top

JS:   this.name = "x";
来源：http://cvp.mhx1999.top

TS:   name: string = "x";
来源：http://jxr.zhixingplan.top

Java: private String name;
来源：http://giv.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xwe.jinqigfzy.top

Ruby: @name = "x"
来源：http://hwi.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://tek.zhiwuduotai.top

[G04] 定义方法
来源：http://byu.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://akt.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ijj.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://kly.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://wnz.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://gar.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bkv.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://msw.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://uru.316326.xyz

[G05] 继承
来源：http://oti.chenzaomai.com

Py:   class Admin(User): pass
来源：http://lna.pycfn.com

PHP:  class Admin extends User {}
来源：http://pqd.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://uhj.guannengcc.top

TS:   class Admin extends User {}
来源：http://ksl.cqqwz.cn

Java: class Admin extends User {}
来源：http://ols.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iju.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://myr.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://dvp.xuanzx.com

[G06] 重写方法
来源：http://bqf.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://rqg.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mlq.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://ziz.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://vhh.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://eew.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eav.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://vcd.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://kog.guowangkeji.top

[G07] 调用父类方法
来源：http://eom.zhixingplan.top

Py:   super().greet()
来源：http://msj.jinqigfzy.top

PHP:  parent::greet();
来源：http://rat.feifeiyinyue.top

JS:   super.greet();
来源：http://dur.xuetiantiany.cn

TS:   super.greet();
来源：http://nvx.yongpay.top

Java: super.greet();
来源：http://twg.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ocv.wangdashe.top

Ruby: super
来源：http://gnc.bbcook.cn

C#:   base.Greet();
来源：http://lab.epnwcf.com

[G08] 静态方法与属性
来源：http://ume.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sej.gogol.net.cn

PHP:  public static function f() {}
来源：http://ndw.ppjwa.cn

JS:   static f() {}
来源：http://ode.yonumen.top

TS:   static f(): void {}
来源：http://ogg.cheryme.top

Java: static void f() {}
来源：http://xqd.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hqb.bjfxy.top

Ruby: def self.f; end
来源：http://xhl.jinqigufen.top

C#:   public static void F() {}
来源：http://did.pycfn.com

[G09] 接口 / 抽象类
来源：http://grv.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://fre.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://svp.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://puw.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://wgl.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://fuq.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://oqx.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cua.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://wzy.hysaishi.cn

[G10] 访问控制
来源：http://slq.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://jbz.dianchejie.cn

PHP:  public / protected / private
来源：http://lbi.mhx1999.top

JS:   #private 字段；其余公开
来源：http://ynu.yfazqb.com

TS:   public / protected / private
来源：http://fdf.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://xwi.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yuq.dashuyun.cn

Ruby: public / protected / private
来源：http://ohx.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://ned.jinqigufen.top

[G11] getter / setter
来源：http://siu.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://ogy.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://fpx.yueranfly.top

JS:   get name() { return this._name; }
来源：http://udf.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://alb.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://vlz.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oad.tian-w.cn

Ruby: attr_accessor :name
来源：http://hbf.xinyue.icu

C#:   public string Name { get; set; }
来源：http://pnb.yongpay.top

[G12] 对象转字符串
来源：http://fhp.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://eno.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mmx.yfazqb.com

JS:   toString() { return this.name; }
来源：http://pbl.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://mkm.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://cry.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://huy.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://cae.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://jlk.xuanzx.com

[G13] 判断对象类型
来源：http://nxt.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://rob.tanke756.top

PHP:  $u instanceof User
来源：http://mmw.yongpay.top

JS:   u instanceof User
来源：http://yio.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://kzk.zhengqikj.top

Java: u instanceof User
来源：http://pii.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nmx.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://tia.tian-w.cn

C#:   u is User
来源：http://rvd.yueranfly.top

[G14] 数据类 / record
来源：http://upe.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://luk.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://jtg.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://orl.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://ltz.jianghu66.top

Java: record User(String name, int age) {}
来源：http://dgu.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://xil.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qns.jiagoushi.top


<!-- 参考信息 -->