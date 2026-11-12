代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qnb.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://ukv.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fsa.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lbp.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lbr.fehbvm.com

TS:   // 同上，务必做 XSS 过滤
来源：http://qkf.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cnx.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jqo.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jbi.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eyc.cucudq.cn

[E16] 数字千分位
来源：http://tzb.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://qvq.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://kcb.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://dzg.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://sas.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://phj.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bgd.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://myk.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://ctd.yongpay.top

[E17] 首字母大写
来源：http://wtx.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nef.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zbj.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ruq.meibo888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kgg.sufxvd.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fdl.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ehc.birdmap.top

Ruby: s.capitalize
来源：http://xyn.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qss.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://byy.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lun.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qlj.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lnr.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wga.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://swx.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vbd.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ous.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ryk.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://kxg.cqqwz.cn

Py:   s.splitlines()
来源：http://sfe.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iur.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://tpw.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://yoh.chenlongwang.top

Java: s.lines().toList()
来源：http://mkg.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://mtc.yongpay.top

Ruby: s.lines
来源：http://jws.yuanzhike.top

C#:   s.Split('\n')
来源：http://ipy.fktsv.cn

[E20] 判断字符串是否为空
来源：http://asn.zdbjq.cn

Py:   if not s:
来源：http://gpi.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gej.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ioq.hnxiangtu.top

TS:   if (s === "") {}
来源：http://fho.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://ziv.ivvv.top

Go:   if s == "" {}
来源：http://zou.hongshengwenyu.top

Ruby: if s.empty?
来源：http://egp.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qqy.xuanzx.com

[E21] 超长截断加省略号
来源：http://zwn.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bnu.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vks.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rpn.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tim.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://edt.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://fbx.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mga.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pce.yueranfly.top

[E22] 字节长度与字符长度
来源：http://vzy.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zlm.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qkf.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jyp.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ded.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lne.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zry.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://gsl.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://din.yj20258888.top

================================================================================
来源：http://lvt.hongshengwenyu.top

F. 文件与目录
来源：http://ehf.9152youxi.cn

================================================================================
来源：http://gjd.shangyingyoupin.top

[F01] 读取整个文件
来源：http://pwf.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pwy.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://szv.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rcp.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ddj.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qgh.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tyo.yvedp.cn

Ruby: File.read("a.txt")
来源：http://smo.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://gim.jiagoushi.top

[F02] 逐行读取文件
来源：http://evc.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://his.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nhg.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilv.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wrn.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rti.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ecw.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://azo.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://llz.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://jxv.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eiu.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kdv.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://svd.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehv.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://etf.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ifl.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://fun.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gku.zhiwuduotai.top

[F04] 追加写入文件
来源：http://jpd.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://coc.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gon.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lqi.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xan.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://icc.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kog.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dcp.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gwl.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://iev.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://opo.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://zpx.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://dls.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://dcg.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oiq.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hyi.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://ktp.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://mxl.ydzc1.top

[F06] 删除文件
来源：http://oiy.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://xmx.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://yrb.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://gdm.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://pio.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ndr.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://aot.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://rvo.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://thp.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://opo.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wlj.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kqz.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bdu.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tjz.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ybv.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bmw.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ubh.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://agq.shzxlz.cn

[F08] 遍历目录
来源：http://gwu.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://byf.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mqw.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://xdx.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://yyn.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lqf.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xpc.mhx1999.top

Ruby: Dir.children("dir")
来源：http://hwr.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://ior.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://ajq.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://xoe.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://vqv.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://tqb.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://bci.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://aqc.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lmb.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://kxe.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://wjq.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://vtu.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iak.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nnq.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vhv.hnqzz.top

TS:   path.extname("a.txt")
来源：http://shb.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fxn.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dpn.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rte.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://brn.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://kft.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jxa.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://urw.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gqy.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nzz.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nag.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://opr.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rgr.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hoh.dianchejie.cn

[F12] CSV 读写
来源：http://xxc.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jgy.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivj.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://izs.quarkkingdee.top

TS:   // 同上
来源：http://ubu.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vnx.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cvs.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zax.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tnh.yj20258888.top

================================================================================
来源：http://okf.52xcode.cn

G. 面向对象
来源：http://bcg.gzhubu.top

================================================================================
来源：http://vlm.dashuyun.cn

[G01] 定义类
来源：http://zan.ydjk.org.cn

Py:   class User: pass
来源：http://xfk.fengsongda.top

PHP:  class User {}
来源：http://ypw.chenzaomai.com

JS:   class User {}
来源：http://ynf.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://fum.316326.xyz

Java: class User {}
来源：http://iob.cqqwz.cn

Go:   type User struct { Name string }
来源：http://smj.haohaochexian.top

Ruby: class User; end
来源：http://sps.ybcxt.top

C#:   class User {}
来源：http://vys.gogol.net.cn

[G02] 构造函数
来源：http://xkj.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://dxi.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://nog.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://koo.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://eno.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://kuw.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://egg.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://bku.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://bsv.hnxiangtu.top

[G03] 实例属性
来源：http://kyu.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://mlo.hnqzz.top

PHP:  public string $name = "x";
来源：http://fpg.hcnkem.com

JS:   this.name = "x";
来源：http://erb.ybcxt.top

TS:   name: string = "x";
来源：http://mov.sysykeji.top

Java: private String name;
来源：http://wsp.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gyl.yuxming.cn

Ruby: @name = "x"
来源：http://dry.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://rjz.xuanzx.com

[G04] 定义方法
来源：http://jwl.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://erl.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://psk.sxryk.cn

JS:   greet() { return this.name; }
来源：http://snx.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://fga.meibo888.top

Java: String greet() { return name; }
来源：http://atc.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ysg.yonumen.top

Ruby: def greet; @name; end
来源：http://yyd.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://psj.meibo888.top

[G05] 继承
来源：http://mni.zycfv.cn

Py:   class Admin(User): pass
来源：http://voz.ybcxt.top

PHP:  class Admin extends User {}
来源：http://fam.52xcode.cn

JS:   class Admin extends User {}
来源：http://flx.smart0.xyz

TS:   class Admin extends User {}
来源：http://uvd.jlsjyb.cn

Java: class Admin extends User {}
来源：http://imf.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hag.dianchejie.cn

Ruby: class Admin < User; end
来源：http://eff.jinqigufen.top

C#:   class Admin : User {}
来源：http://ado.nwbrower.top

[G06] 重写方法
来源：http://ltt.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://vuh.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dhc.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://ekl.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://bom.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://gjh.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ids.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://wne.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://zww.nanxinkj.top

[G07] 调用父类方法
来源：http://jdz.xinyue.icu

Py:   super().greet()
来源：http://yre.hesvh.cn

PHP:  parent::greet();
来源：http://fdq.cashguo.top

JS:   super.greet();
来源：http://baq.xuanzx.com

TS:   super.greet();
来源：http://jxo.hywenlv.cn

Java: super.greet();
来源：http://nda.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uke.tanke756.top

Ruby: super
来源：http://yac.havefunace.top

C#:   base.Greet();
来源：http://udm.pycfn.com

[G08] 静态方法与属性
来源：http://hul.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ept.sjlbkw.cn

PHP:  public static function f() {}
来源：http://bpl.ctjpmb.com

JS:   static f() {}
来源：http://hwh.vqdsnc.cn

TS:   static f(): void {}
来源：http://kud.cucudq.cn

Java: static void f() {}
来源：http://agx.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kos.pycfn.com

Ruby: def self.f; end
来源：http://xgi.epnwcf.com

C#:   public static void F() {}
来源：http://yar.yuxming.cn

[G09] 接口 / 抽象类
来源：http://emm.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://jxt.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://abo.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pas.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://adp.xinyue.icu

Java: interface Shape { double area(); }
来源：http://tvx.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://jls.gaohongyu789.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nyo.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://ptt.hesvh.cn

[G10] 访问控制
来源：http://gnx.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://asi.tarul.cn

PHP:  public / protected / private
来源：http://asm.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://kps.shzxlz.cn

TS:   public / protected / private
来源：http://cah.yonumen.top

Java: public / protected / private / 默认包级
来源：http://bhq.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ivc.yj202588.top

Ruby: public / protected / private
来源：http://ojt.xylfe.cn

C#:   public / protected / private / internal
来源：http://mvy.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://frh.fktsv.cn

Py:   @property 与 @x.setter
来源：http://chv.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fhj.hesvh.cn

JS:   get name() { return this._name; }
来源：http://prl.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://gbl.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://kdg.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://amw.tanke756.top

Ruby: attr_accessor :name
来源：http://nga.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://rat.jiagoushi.top

[G12] 对象转字符串
来源：http://fwz.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://rpr.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://arq.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://xka.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://jim.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://otl.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://bjn.pycfn.com

Ruby: def to_s; @name; end
来源：http://nnr.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://fpf.ydzc1.top

[G13] 判断对象类型
来源：http://zmp.snrcjt.cn

Py:   isinstance(u, User)
来源：http://mqp.hammf.cn

PHP:  $u instanceof User
来源：http://abp.cashguo.top

JS:   u instanceof User
来源：http://qfa.gaohongyu789.top

TS:   u instanceof User
来源：http://mqy.aibaodan.cn


<!-- 参考信息 -->