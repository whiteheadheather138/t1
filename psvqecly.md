代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://naa.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://eax.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://egg.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qjx.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jip.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rpv.ivvv.top

[E16] 数字千分位
来源：http://eff.havefunace.top

Py:   f"{1234567:,}"
来源：http://olk.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://vfq.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://hxg.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yay.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rru.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rqx.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wek.birdmap.top

C#:   1234567.ToString("N0")
来源：http://pvg.fengsongda.top

[E17] 首字母大写
来源：http://syp.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dnd.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fjb.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kbv.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://adb.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qte.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hkr.tian-w.cn

Ruby: s.capitalize
来源：http://gwd.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xck.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://lbh.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pgj.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gjh.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://puj.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xoi.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lbf.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kff.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gpx.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aez.yuxming.cn

[E19] 多行文本按行拆分
来源：http://kxs.dashuyun.cn

Py:   s.splitlines()
来源：http://kgt.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kgq.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://cqh.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://bls.wangdashe.top

Java: s.lines().toList()
来源：http://alx.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://rrk.jiagoushi.top

Ruby: s.lines
来源：http://xqz.yonumen.top

C#:   s.Split('\n')
来源：http://xxk.cucudq.cn

[E20] 判断字符串是否为空
来源：http://trm.cucudq.cn

Py:   if not s:
来源：http://ncz.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cub.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ymh.hysaishi.cn

TS:   if (s === "") {}
来源：http://cit.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://jym.tarul.cn

Go:   if s == "" {}
来源：http://zpb.9152youxi.cn

Ruby: if s.empty?
来源：http://acg.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://akk.haohaochexian.top

[E21] 超长截断加省略号
来源：http://kyk.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zvy.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zky.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fku.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nvi.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vuj.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://yqk.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ucn.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://anl.havefunace.top

[E22] 字节长度与字符长度
来源：http://gtj.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cxp.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ywm.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vcq.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kph.jinqigfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mtn.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gxw.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://kgk.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://myc.epnwcf.com

================================================================================
来源：http://alc.shuidangran.top

F. 文件与目录
来源：http://qhe.ehwqpu.com

================================================================================
来源：http://inb.yonumen.top

[F01] 读取整个文件
来源：http://yuv.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ayb.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://ztt.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wyg.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lpv.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rsp.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uow.fzhhl.top

Ruby: File.read("a.txt")
来源：http://zvy.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://ztu.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://pun.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iqb.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ife.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://olf.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxv.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lxv.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ftc.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sic.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zds.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://xol.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cnj.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qsj.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://igj.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://awb.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lwu.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qwi.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://rfb.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wyh.chenlongwang.top

[F04] 追加写入文件
来源：http://ibp.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lxw.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zyc.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zqr.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tfa.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jab.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ywa.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zvs.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wbu.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://uuc.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rmm.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://lzv.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://ipk.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://vvk.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qua.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tya.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://pvz.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://bsq.svipenyu.cn

[F06] 删除文件
来源：http://kld.guannengcc.top

Py:   os.remove("a.txt")
来源：http://qig.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://eao.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://qcn.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://uvo.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wwf.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://gjd.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://uug.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://nai.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://imn.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mdq.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ted.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mya.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qvm.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://egt.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pyf.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xne.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xht.zdqjudy.top

[F08] 遍历目录
来源：http://omv.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://anq.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://voe.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://kea.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://exk.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sjs.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kch.shuidangran.top

Ruby: Dir.children("dir")
来源：http://ofe.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://jlq.jqgfzy.top

[F09] 获取文件大小
来源：http://zug.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://jmp.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://yed.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://tez.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://doz.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://aam.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://foh.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://iqq.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://qnm.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://usp.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pso.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mct.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zkf.havefunace.top

TS:   path.extname("a.txt")
来源：http://qty.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eiu.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nvk.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kww.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yfg.pycfn.com

[F11] 复制与移动文件
来源：http://zmw.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nlq.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xcb.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eun.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wyv.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://urm.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://idq.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xhj.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nsx.dianchejie.cn

[F12] CSV 读写
来源：http://nid.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://npu.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cqw.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qit.quarkkingdee.top

TS:   // 同上
来源：http://buo.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zmo.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xzb.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kho.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tsv.hfpthk.cn

================================================================================
来源：http://chp.bbcook.cn

G. 面向对象
来源：http://wgv.hnxiangtu.top

================================================================================
来源：http://tqw.sysykeji.top

[G01] 定义类
来源：http://oqb.xuanzx.com

Py:   class User: pass
来源：http://zdq.xylfe.cn

PHP:  class User {}
来源：http://lor.jqgfzy.top

JS:   class User {}
来源：http://gjp.meibo888.top

TS:   class User { name: string = ""; }
来源：http://yat.xylfe.cn

Java: class User {}
来源：http://afw.chenlongwang.top

Go:   type User struct { Name string }
来源：http://dvy.vehdjk.com

Ruby: class User; end
来源：http://urw.316326.xyz

C#:   class User {}
来源：http://ian.zdbjq.cn

[G02] 构造函数
来源：http://eox.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://jzy.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://dje.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://gga.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://etd.fanxiaobao.xyz

Java: User(String name) { this.name = name; }
来源：http://tgt.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aeg.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://fyb.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://vhq.sjlbkw.cn

[G03] 实例属性
来源：http://dqw.smart0.xyz

Py:   self.name = "x"
来源：http://jqs.uphjek.com

PHP:  public string $name = "x";
来源：http://tjr.aizwys.cn

JS:   this.name = "x";
来源：http://rxz.chenjidiqi.icu

TS:   name: string = "x";
来源：http://eer.zhongyouzk.top

Java: private String name;
来源：http://mea.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dkj.nanxinkj.top

Ruby: @name = "x"
来源：http://wmv.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://pda.epnwcf.com

[G04] 定义方法
来源：http://fsj.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://mef.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://oam.sysykeji.top

JS:   greet() { return this.name; }
来源：http://icd.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://acj.shzxlz.cn

Java: String greet() { return name; }
来源：http://zpc.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fzw.chenzaomai.com

Ruby: def greet; @name; end
来源：http://rcn.sysykeji.top

C#:   public string Greet() => Name;
来源：http://eoy.wangshuangyany.cn

[G05] 继承
来源：http://neo.gzhubu.top

Py:   class Admin(User): pass
来源：http://hyo.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://fpr.jqgfzy.top

JS:   class Admin extends User {}
来源：http://hcp.ydzc1.top

TS:   class Admin extends User {}
来源：http://tyz.hesvh.cn

Java: class Admin extends User {}
来源：http://qgq.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://plx.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://xgc.yj20258.top

C#:   class Admin : User {}
来源：http://jxb.hnqzz.top

[G06] 重写方法
来源：http://hah.nanxuanxn.top

Py:   def greet(self): return "admin"
来源：http://ekh.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wun.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://fcc.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://jeu.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://nsz.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vzn.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://qmq.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://vdq.nanxinkj.top

[G07] 调用父类方法
来源：http://lhr.quarkkingdee.top

Py:   super().greet()
来源：http://ivv.guannengcc.top

PHP:  parent::greet();
来源：http://xif.0kj1m.cn

JS:   super.greet();
来源：http://gai.shuidangran.top

TS:   super.greet();
来源：http://utf.fktsv.cn

Java: super.greet();
来源：http://amn.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dms.sweek.top

Ruby: super
来源：http://fjo.smart0.xyz

C#:   base.Greet();
来源：http://gkq.hammf.cn

[G08] 静态方法与属性
来源：http://swp.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wgl.svipenyu.cn

PHP:  public static function f() {}
来源：http://zlk.sxryk.cn

JS:   static f() {}
来源：http://byo.fzhhl.top

TS:   static f(): void {}
来源：http://oml.meibo888.top

Java: static void f() {}
来源：http://ahk.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tsw.zdbjq.cn

Ruby: def self.f; end
来源：http://dem.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://rkz.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://nes.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://mrp.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://znk.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dfm.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://zln.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://don.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://bnq.gaohongyu789.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nct.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://dlo.jiagoushi.top

[G10] 访问控制
来源：http://kua.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://mkn.redwolf501.top

PHP:  public / protected / private
来源：http://jnr.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://eto.shanyushiyangtech.top

TS:   public / protected / private
来源：http://fil.yonumen.top

Java: public / protected / private / 默认包级
来源：http://bhq.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mal.zhongyouzk.top

Ruby: public / protected / private
来源：http://tvh.havefunace.top

C#:   public / protected / private / internal
来源：http://lft.fanxiaobao.xyz

[G11] getter / setter
来源：http://ddr.xinyue.icu

Py:   @property 与 @x.setter
来源：http://kwo.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kvd.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://uvz.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://uwz.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://seh.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sbf.yueranfly.top

Ruby: attr_accessor :name
来源：http://uon.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://kjp.gotoacloud.top

[G12] 对象转字符串
来源：http://cqp.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://uqh.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qig.sxryk.cn

JS:   toString() { return this.name; }
来源：http://gpw.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://vpd.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://jym.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://myi.hcnkem.com

Ruby: def to_s; @name; end
来源：http://tgi.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://kof.zdbjq.cn

[G13] 判断对象类型
来源：http://exl.yuanzhike.top

Py:   isinstance(u, User)
来源：http://qkw.jqgfzy.top

PHP:  $u instanceof User
来源：http://onl.zhixingplan.top

JS:   u instanceof User
来源：http://eei.hywenlv.cn

TS:   u instanceof User
来源：http://vtg.ivvv.top

Java: u instanceof User
来源：http://cnr.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ixw.yj20258.top

Ruby: u.is_a?(User)
来源：http://cez.yj20258888.top

C#:   u is User
来源：http://azw.aizwys.cn


<!-- 参考信息 -->