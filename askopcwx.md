代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kmu.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kbz.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://awc.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hqj.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://usq.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bth.sxryk.cn

[E16] 数字千分位
来源：http://evb.andypj.xyz

Py:   f"{1234567:,}"
来源：http://eow.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://igo.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eqz.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sls.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wdg.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gha.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fto.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://qqm.hesvh.cn

[E17] 首字母大写
来源：http://mlj.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgv.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dqi.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://frp.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hdt.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hgf.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ktr.aibaodan.cn

Ruby: s.capitalize
来源：http://eyk.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gus.fehbvm.com

[E18] 模板占位符替换
来源：http://ier.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ezn.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://flk.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://rvy.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hge.iojbl.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jjh.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fvq.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ovy.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vhw.yj20258888.top

[E19] 多行文本按行拆分
来源：http://fpi.dianchejie.cn

Py:   s.splitlines()
来源：http://hjv.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mfu.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://mzi.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://aod.gzhubu.top

Java: s.lines().toList()
来源：http://rrq.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://wzv.9152youxi.cn

Ruby: s.lines
来源：http://xqw.xziqi.cn

C#:   s.Split('\n')
来源：http://mgp.fktsv.cn

[E20] 判断字符串是否为空
来源：http://pxf.52xcode.cn

Py:   if not s:
来源：http://usv.yj202588.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ncu.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://usq.jiagoushi.top

TS:   if (s === "") {}
来源：http://uhe.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://vba.iojbl.cn

Go:   if s == "" {}
来源：http://cft.zhongyouzk.top

Ruby: if s.empty?
来源：http://djv.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://irq.0kj1m.cn

[E21] 超长截断加省略号
来源：http://eov.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yvq.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vxd.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndg.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tbw.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yzk.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://qjl.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fdu.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dcx.yfazqb.com

[E22] 字节长度与字符长度
来源：http://drp.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sor.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uay.epnwcf.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://evw.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gib.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vyt.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lcz.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://rrb.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ksg.hesvh.cn

================================================================================
来源：http://meo.jlsjyb.cn

F. 文件与目录
来源：http://wqw.pycfn.com

================================================================================
来源：http://zdc.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://ajj.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uva.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://xao.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qnq.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cnk.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://sdq.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sij.yj20258.top

Ruby: File.read("a.txt")
来源：http://vdf.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://vyu.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://sea.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kto.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pfz.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jyi.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yoh.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fld.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ane.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vvo.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yap.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://ads.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bxt.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://stn.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://elv.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pan.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://peu.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lau.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://zsb.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uhb.bjfxy.top

[F04] 追加写入文件
来源：http://alm.zycfv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xrf.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bvm.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ujp.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kuz.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oqc.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nuj.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lts.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jmg.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://ise.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ils.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://lcs.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://ema.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://iua.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tmc.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nti.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://oek.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://ljf.vqdsnc.cn

[F06] 删除文件
来源：http://gvr.yfazqb.com

Py:   os.remove("a.txt")
来源：http://bvw.xuanzx.com

PHP:  unlink("a.txt");
来源：http://egq.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kgn.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://egi.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fqk.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://fro.ivvv.top

Ruby: File.delete("a.txt")
来源：http://wzy.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://ltb.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://yyv.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ycl.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dmu.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yng.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmm.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vrn.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://czl.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dvb.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kga.fengsongda.top

[F08] 遍历目录
来源：http://ful.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ezw.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uvq.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://ebz.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://fap.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zzd.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://piz.ybcxt.top

Ruby: Dir.children("dir")
来源：http://rnn.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://dlh.9152youxi.cn

[F09] 获取文件大小
来源：http://njv.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://kto.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://otp.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://jrh.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://zsd.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://ljx.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://twb.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://eiu.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://inx.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://dxv.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wwi.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ahb.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bks.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://ngm.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ims.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wyg.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zdg.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lnq.pycfn.com

[F11] 复制与移动文件
来源：http://vmn.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xpv.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nmk.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gsq.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://src.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://djg.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://czg.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gza.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mft.zdbjq.cn

[F12] CSV 读写
来源：http://wsa.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vnh.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://muh.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tnp.fzhhl.top

TS:   // 同上
来源：http://ajq.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jzk.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yrq.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://usl.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wkt.fanxiaobao.xyz

================================================================================
来源：http://jtx.wangdashe.top

G. 面向对象
来源：http://xsp.zhoulong.xyz

================================================================================
来源：http://uuo.zhixingplan.top

[G01] 定义类
来源：http://tlw.gogol.net.cn

Py:   class User: pass
来源：http://ibo.shanyushiyangkeji.top

PHP:  class User {}
来源：http://xsi.zhengqikj.top

JS:   class User {}
来源：http://gcw.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://zrh.snrcjt.cn

Java: class User {}
来源：http://vps.ehwqpu.com

Go:   type User struct { Name string }
来源：http://upi.jinqigufen.top

Ruby: class User; end
来源：http://knn.bjfxy.top

C#:   class User {}
来源：http://eta.vehdjk.com

[G02] 构造函数
来源：http://aky.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://rqv.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://xea.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://nxy.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://fmo.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://zri.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oxa.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://rob.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://tco.uphjek.com

[G03] 实例属性
来源：http://hdm.cdnleiting.top

Py:   self.name = "x"
来源：http://wvb.svipenyu.cn

PHP:  public string $name = "x";
来源：http://zkj.daria6918.cn

JS:   this.name = "x";
来源：http://osq.ehwqpu.com

TS:   name: string = "x";
来源：http://npb.shzxlz.cn

Java: private String name;
来源：http://ypu.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xjs.yanxiufei.cn

Ruby: @name = "x"
来源：http://kwn.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://xhj.fehbvm.com

[G04] 定义方法
来源：http://ixi.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://awj.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qzv.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://knq.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://otc.yvedp.cn

Java: String greet() { return name; }
来源：http://dim.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lrh.vehdjk.com

Ruby: def greet; @name; end
来源：http://xhl.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://edf.daria6918.cn

[G05] 继承
来源：http://zly.xuanzx.com

Py:   class Admin(User): pass
来源：http://hcg.meibo888.top

PHP:  class Admin extends User {}
来源：http://spc.haohaochexian.top

JS:   class Admin extends User {}
来源：http://jre.jianghu66.top

TS:   class Admin extends User {}
来源：http://uzw.vehdjk.com

Java: class Admin extends User {}
来源：http://ayl.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tiq.yfazqb.com

Ruby: class Admin < User; end
来源：http://szc.ybcxt.top

C#:   class Admin : User {}
来源：http://hom.guowangkeji.top

[G06] 重写方法
来源：http://ken.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://ngb.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rhi.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://phi.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://iks.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://xlu.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vqr.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://boa.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://zah.zhongyouzk.top

[G07] 调用父类方法
来源：http://ajh.xinyue.icu

Py:   super().greet()
来源：http://wni.fengsongda.top

PHP:  parent::greet();
来源：http://vmb.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://iol.cheryme.top

TS:   super.greet();
来源：http://hut.tian-w.cn

Java: super.greet();
来源：http://dir.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vdj.vehdjk.com

Ruby: super
来源：http://wzn.nwbrower.top

C#:   base.Greet();
来源：http://wce.yj20258.top

[G08] 静态方法与属性
来源：http://aeb.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vqn.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://oom.yanxiufei.cn

JS:   static f() {}
来源：http://yif.birdmap.top

TS:   static f(): void {}
来源：http://ulv.chenlongwang.top

Java: static void f() {}
来源：http://ebw.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://esp.quarkkingdee.top

Ruby: def self.f; end
来源：http://xvt.tanke756.top

C#:   public static void F() {}
来源：http://zke.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://bgl.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://wzf.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gxs.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yvf.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://mpt.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://bzb.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://aib.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ieo.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://oqz.birdmap.top

[G10] 访问控制
来源：http://uzs.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://dig.cheryme.top

PHP:  public / protected / private
来源：http://xfv.yj20258.top

JS:   #private 字段；其余公开
来源：http://lou.guannengcc.top

TS:   public / protected / private
来源：http://dib.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://uob.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://psh.yvedp.cn

Ruby: public / protected / private
来源：http://glc.meibo888.top

C#:   public / protected / private / internal
来源：http://tjm.feifeiyinyue.top

[G11] getter / setter
来源：http://leo.9152youxi.cn

Py:   @property 与 @x.setter
来源：http://kxl.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pqp.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://tzy.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://uzx.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://mvz.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tni.cucudq.cn

Ruby: attr_accessor :name
来源：http://moy.aizwys.cn

C#:   public string Name { get; set; }
来源：http://ull.yfazqb.com

[G12] 对象转字符串
来源：http://aen.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://klu.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://vsq.redwolf501.top

JS:   toString() { return this.name; }
来源：http://gte.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://uql.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://dwt.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://csg.hnqzz.top

Ruby: def to_s; @name; end
来源：http://szg.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://ldc.jlsjyb.cn

[G13] 判断对象类型
来源：http://xnt.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://rrs.tian-w.cn

PHP:  $u instanceof User
来源：http://fmm.feifeiyinyue.top

JS:   u instanceof User
来源：http://gbd.cucudq.cn

TS:   u instanceof User
来源：http://eio.c1oappe.top

Java: u instanceof User
来源：http://ziw.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bte.fktsv.cn

Ruby: u.is_a?(User)
来源：http://lnj.iojbl.cn

C#:   u is User
来源：http://scn.yj202588.top


<!-- 参考信息 -->