代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mla.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mfs.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kwf.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wpq.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gxl.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cls.gaohongyu789.top

[E16] 数字千分位
来源：http://yfh.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://ten.fzhhl.top

PHP:  number_format(1234567);
来源：http://ukr.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://alm.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gex.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://azo.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lya.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fye.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://tgu.jinqigufen.top

[E17] 首字母大写
来源：http://dvi.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ylq.zycfv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gov.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ghu.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://noe.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ksm.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kxn.shangyingyoupin.top

Ruby: s.capitalize
来源：http://ihb.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://abq.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://aak.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kxk.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ebu.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gwd.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vyl.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sab.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://abw.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://anu.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hkc.bjfxy.top

[E19] 多行文本按行拆分
来源：http://fcy.daria6918.cn

Py:   s.splitlines()
来源：http://qun.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://acd.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://hbk.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://yza.yuanzhike.top

Java: s.lines().toList()
来源：http://hym.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://fco.sysykeji.top

Ruby: s.lines
来源：http://jhz.kuanghao11.cn

C#:   s.Split('\n')
来源：http://wxe.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://ioq.kuanghao11.cn

Py:   if not s:
来源：http://cof.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zau.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://swg.hfpthk.cn

TS:   if (s === "") {}
来源：http://kvh.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://tvr.vehdjk.com

Go:   if s == "" {}
来源：http://dns.chenzaomai.com

Ruby: if s.empty?
来源：http://opn.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://flv.dashuyun.cn

[E21] 超长截断加省略号
来源：http://skh.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qrq.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vak.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xdn.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ouf.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cpy.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://leh.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yry.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xbj.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://lib.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wls.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ptc.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pqz.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ubj.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jup.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mce.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://wev.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ekr.redwolf501.top

================================================================================
来源：http://pbx.redwolf501.top

F. 文件与目录
来源：http://uzr.sysykeji.top

================================================================================
来源：http://ysx.shuidangran.top

[F01] 读取整个文件
来源：http://you.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://utm.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://gfu.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eqz.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nxp.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fkd.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://urx.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://dgb.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://hbz.daria6918.cn

[F02] 逐行读取文件
来源：http://lzo.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mup.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ata.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uay.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vnh.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tyf.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zzd.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rod.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dlm.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://yxc.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lua.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cqv.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://moo.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kgt.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lbz.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gdr.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://rdf.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uoq.cqqwz.cn

[F04] 追加写入文件
来源：http://uyi.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nll.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eth.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://olr.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mbw.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cym.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fmm.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lew.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kcm.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://pbg.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qlm.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://rwz.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://cji.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://gys.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fac.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cpp.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://bpq.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://yda.meibo888.top

[F06] 删除文件
来源：http://mch.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://uoy.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://nsd.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://klr.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://amy.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bid.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://ale.pycfn.com

Ruby: File.delete("a.txt")
来源：http://uey.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://emj.hesvh.cn

[F07] 创建目录（含多级）
来源：http://tgc.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bpy.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rln.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gnx.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bwr.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jwp.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xtc.pengpengdd.cyou

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ynu.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ebj.dashuyun.cn

[F08] 遍历目录
来源：http://zzo.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ltr.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kyh.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://iaj.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://hxp.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ncu.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nuq.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://soy.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://ydr.yanxiufei.cn

[F09] 获取文件大小
来源：http://utp.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://bpn.xziqi.cn

PHP:  filesize("a.txt");
来源：http://cyu.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://kvu.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://eot.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://pms.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wze.fengsongda.top

Ruby: File.size("a.txt")
来源：http://wrj.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://mss.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://zfc.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gue.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gdi.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vpb.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://uzo.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pyw.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ozr.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pvt.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tyc.yvedp.cn

[F11] 复制与移动文件
来源：http://ohm.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kzi.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eic.52xcode.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vwy.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nhx.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rzz.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dga.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wff.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://doi.jlsjyb.cn

[F12] CSV 读写
来源：http://esg.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pwx.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dst.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zlg.epnwcf.com

TS:   // 同上
来源：http://kbq.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tua.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rau.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gwc.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hgn.jinqigfzy.top

================================================================================
来源：http://pvh.jinqigufen.top

G. 面向对象
来源：http://wzd.quarkkingdee.top

================================================================================
来源：http://lom.yvedp.cn

[G01] 定义类
来源：http://frx.gzhubu.top

Py:   class User: pass
来源：http://rkc.guowangkeji.top

PHP:  class User {}
来源：http://wir.yuanzhike.top

JS:   class User {}
来源：http://bpp.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://wjv.svipenyu.cn

Java: class User {}
来源：http://der.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://gga.zdqjudy.top

Ruby: class User; end
来源：http://msq.ctjpmb.com

C#:   class User {}
来源：http://noo.smart0.xyz

[G02] 构造函数
来源：http://bqp.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://duj.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://efx.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://ylr.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://wdz.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://qyk.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://igo.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://nfa.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://rrj.9152youxi.cn

[G03] 实例属性
来源：http://hzw.ybcxt.top

Py:   self.name = "x"
来源：http://mtv.cashguo.top

PHP:  public string $name = "x";
来源：http://yxh.wangdashe.top

JS:   this.name = "x";
来源：http://vnd.ybcxt.top

TS:   name: string = "x";
来源：http://ulq.jyoumei.cn

Java: private String name;
来源：http://rcy.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wdm.zhixingplan.top

Ruby: @name = "x"
来源：http://sgg.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://cqd.yfazqb.com

[G04] 定义方法
来源：http://tjs.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://kcw.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hxg.guannengcc.top

JS:   greet() { return this.name; }
来源：http://cjn.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://vvl.yonumen.top

Java: String greet() { return name; }
来源：http://uda.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aoz.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://tew.fzhhl.top

C#:   public string Greet() => Name;
来源：http://kyk.chenlongwang.top

[G05] 继承
来源：http://uzb.0kj1m.cn

Py:   class Admin(User): pass
来源：http://kcj.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://fce.9152youxi.cn

JS:   class Admin extends User {}
来源：http://mxo.jyoumei.cn

TS:   class Admin extends User {}
来源：http://gjh.yuanzhike.top

Java: class Admin extends User {}
来源：http://the.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fjo.mhx1999.top

Ruby: class Admin < User; end
来源：http://btg.hysaishi.cn

C#:   class Admin : User {}
来源：http://luv.ywan-chungtsiang.top

[G06] 重写方法
来源：http://rvf.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://zht.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://grd.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://ppq.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://gqa.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://emc.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oab.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://pwv.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://fqb.iojbl.cn

[G07] 调用父类方法
来源：http://jor.andypj.xyz

Py:   super().greet()
来源：http://tds.ppjwa.cn

PHP:  parent::greet();
来源：http://bsy.jqgufenzy.top

JS:   super.greet();
来源：http://fta.zhoulong.xyz

TS:   super.greet();
来源：http://lex.aibaodan.cn

Java: super.greet();
来源：http://htt.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bqk.shanyushiyangkeji.top

Ruby: super
来源：http://yla.cashguo.top

C#:   base.Greet();
来源：http://iuh.tanke756.top

[G08] 静态方法与属性
来源：http://deq.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jou.andypj.xyz

PHP:  public static function f() {}
来源：http://yet.cashguo.top

JS:   static f() {}
来源：http://vpa.gotoacloud.top

TS:   static f(): void {}
来源：http://hsm.shzxlz.cn

Java: static void f() {}
来源：http://wjb.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://vig.sysykeji.top

Ruby: def self.f; end
来源：http://mqg.hammf.cn

C#:   public static void F() {}
来源：http://ler.epnwcf.com

[G09] 接口 / 抽象类
来源：http://sdu.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://jua.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://rvm.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://phx.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://quc.yfazqb.com

Java: interface Shape { double area(); }
来源：http://eex.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://lju.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypv.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://fdo.zhijiandao.cn

[G10] 访问控制
来源：http://mxf.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://htw.birdmap.top

PHP:  public / protected / private
来源：http://zbs.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://mvx.pycfn.com

TS:   public / protected / private
来源：http://hzd.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://hpp.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gww.aizwys.cn

Ruby: public / protected / private
来源：http://qjc.gaohongyu789.top

C#:   public / protected / private / internal
来源：http://ghj.cucudq.cn

[G11] getter / setter
来源：http://lri.52xcode.cn

Py:   @property 与 @x.setter
来源：http://lpn.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nar.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://tyc.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://ktp.yfazqb.com

Java: public String getName() { return name; }
来源：http://lvs.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzt.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://bhi.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://ver.dashuyun.cn

[G12] 对象转字符串
来源：http://oyw.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://nhz.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ihy.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://hzy.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://hnv.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://ljq.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://rlj.cheryme.top

Ruby: def to_s; @name; end
来源：http://efw.tanke756.top

C#:   public override string ToString() => Name;
来源：http://gcj.fktsv.cn

[G13] 判断对象类型
来源：http://mrs.c1oappe.top

Py:   isinstance(u, User)
来源：http://gfn.vqdsnc.cn

PHP:  $u instanceof User
来源：http://cdb.yuanzhike.top

JS:   u instanceof User
来源：http://uay.xziqi.cn

TS:   u instanceof User
来源：http://yok.vqdsnc.cn

Java: u instanceof User
来源：http://yxu.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mdy.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://nex.sysykeji.top

C#:   u is User
来源：http://wlq.shangyingyoupin.top


<!-- 参考信息 -->