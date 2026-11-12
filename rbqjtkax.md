代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tgy.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://skd.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://dlx.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wku.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bkb.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jtt.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nvt.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://smo.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bql.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jsl.xziqi.cn

[E16] 数字千分位
来源：http://uvo.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://jpn.316326.xyz

PHP:  number_format(1234567);
来源：http://xos.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aue.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qvu.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://psb.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mnz.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nit.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://ekf.gogol.net.cn

[E17] 首字母大写
来源：http://wtd.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hzl.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dsa.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ogv.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cnn.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rhc.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uoj.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://psy.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lpg.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://tbs.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mgc.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kxv.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hfo.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://utt.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hud.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfd.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gxw.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://msp.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://lbh.vqdsnc.cn

Py:   s.splitlines()
来源：http://zch.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dsv.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://rzw.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://nbj.pycfn.com

Java: s.lines().toList()
来源：http://dfu.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://pnj.shanyushiyangkeji.top

Ruby: s.lines
来源：http://agx.zhixingplan.top

C#:   s.Split('\n')
来源：http://wfr.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://ohz.yanxiufei.cn

Py:   if not s:
来源：http://oqh.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ths.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wux.yangfankeji.com

TS:   if (s === "") {}
来源：http://azr.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://bjb.0kj1m.cn

Go:   if s == "" {}
来源：http://jpv.yueranfly.top

Ruby: if s.empty?
来源：http://lgh.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nbf.cucudq.cn

[E21] 超长截断加省略号
来源：http://hoc.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gag.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpd.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbq.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wsj.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hnh.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://cfl.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rfl.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ssd.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://jzq.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rjo.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axa.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ttu.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dbq.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xai.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ien.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://npv.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ubo.yuanzhike.top

================================================================================
来源：http://bor.ywan-chungtsiang.top

F. 文件与目录
来源：http://sji.vqdsnc.cn

================================================================================
来源：http://lsc.wangdashe.top

[F01] 读取整个文件
来源：http://goy.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ewz.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://mkf.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pob.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zuz.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ycf.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://til.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://dxt.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://cmm.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://svb.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pdi.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zxb.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vxm.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xyi.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ytt.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://snl.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jrl.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lyf.316326.xyz

[F03] 写入文件（覆盖）
来源：http://zci.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vpz.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://noa.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izr.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gnr.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gpv.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mbw.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://lqq.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kay.meibo888.top

[F04] 追加写入文件
来源：http://ywt.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xfr.nanxuanxn.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rfl.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pwt.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ugy.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nia.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kqn.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sce.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ptu.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://zhd.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hwv.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://xum.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://xgb.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://qzg.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zhk.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wdk.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://doe.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://sve.hnxiangtu.top

[F06] 删除文件
来源：http://qha.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://ywl.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://zmc.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://ovw.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://jou.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hfv.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://eep.pycfn.com

Ruby: File.delete("a.txt")
来源：http://eiy.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://dej.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://bjk.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rtw.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://voy.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ikq.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ulq.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hag.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ihb.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qnb.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://unl.0kj1m.cn

[F08] 遍历目录
来源：http://wip.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bbz.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vyw.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://fxn.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://usr.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oqp.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bpl.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://jmu.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://dka.ppjwa.cn

[F09] 获取文件大小
来源：http://pop.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://hov.aizwys.cn

PHP:  filesize("a.txt");
来源：http://pxx.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://wmr.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://bbm.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://kmh.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://irx.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://ecw.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://gaf.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://lmd.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vpk.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vqf.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://miq.xziqi.cn

TS:   path.extname("a.txt")
来源：http://kiu.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ada.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://usi.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rfv.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qjt.havefunace.top

[F11] 复制与移动文件
来源：http://fgt.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uqh.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yaa.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ntk.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bge.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://adk.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://csi.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ixa.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sxy.yangfankeji.com

[F12] CSV 读写
来源：http://oni.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://skd.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://htp.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cdv.hysaishi.cn

TS:   // 同上
来源：http://sgl.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ozj.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tue.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jhe.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ozr.ctjpmb.com

================================================================================
来源：http://rxa.andypj.xyz

G. 面向对象
来源：http://nmy.yvedp.cn

================================================================================
来源：http://sdi.zhiwuduotai.top

[G01] 定义类
来源：http://uiv.yfazqb.com

Py:   class User: pass
来源：http://heg.guowangkeji.top

PHP:  class User {}
来源：http://hcc.andypj.xyz

JS:   class User {}
来源：http://xum.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://hre.9152youxi.cn

Java: class User {}
来源：http://zql.shuidangran.top

Go:   type User struct { Name string }
来源：http://ejx.cdnleiting.top

Ruby: class User; end
来源：http://iej.daria6918.cn

C#:   class User {}
来源：http://tvq.kuanghao11.cn

[G02] 构造函数
来源：http://eun.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://nux.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://ihx.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://fsy.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://tek.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://wby.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tpd.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://wnx.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://dmp.zycfv.cn

[G03] 实例属性
来源：http://vtt.guannengcc.top

Py:   self.name = "x"
来源：http://upm.meibo888.top

PHP:  public string $name = "x";
来源：http://ajm.dianchejie.cn

JS:   this.name = "x";
来源：http://gdv.bjfxy.top

TS:   name: string = "x";
来源：http://gpd.aizwys.cn

Java: private String name;
来源：http://rou.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cvd.havefunace.top

Ruby: @name = "x"
来源：http://mlr.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://xog.chenlongwang.top

[G04] 定义方法
来源：http://ypy.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://niu.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qqu.havefunace.top

JS:   greet() { return this.name; }
来源：http://mwr.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://kie.jlsjyb.cn

Java: String greet() { return name; }
来源：http://gui.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zey.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://wdk.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://czu.fehbvm.com

[G05] 继承
来源：http://nkk.nwbrower.top

Py:   class Admin(User): pass
来源：http://xqy.smart0.xyz

PHP:  class Admin extends User {}
来源：http://ekd.bjfxy.top

JS:   class Admin extends User {}
来源：http://qnq.ehwqpu.com

TS:   class Admin extends User {}
来源：http://tcg.9152youxi.cn

Java: class Admin extends User {}
来源：http://zkw.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xwj.hywenlv.cn

Ruby: class Admin < User; end
来源：http://yzt.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://rho.wangshuangyany.cn

[G06] 重写方法
来源：http://rvu.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://jkp.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hgm.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://xkg.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://eev.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://exg.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://alc.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://qeg.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://hab.meibo888.top

[G07] 调用父类方法
来源：http://gfh.fzhhl.top

Py:   super().greet()
来源：http://xai.shzxlz.cn

PHP:  parent::greet();
来源：http://bzu.fzhhl.top

JS:   super.greet();
来源：http://nzd.yvedp.cn

TS:   super.greet();
来源：http://sax.jqgufenzy.top

Java: super.greet();
来源：http://yyo.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kpm.jqgufenzy.top

Ruby: super
来源：http://kgh.andypj.xyz

C#:   base.Greet();
来源：http://vqg.iojbl.cn

[G08] 静态方法与属性
来源：http://tho.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzy.guannengcc.top

PHP:  public static function f() {}
来源：http://lvr.yfazqb.com

JS:   static f() {}
来源：http://ipu.guannengcc.top

TS:   static f(): void {}
来源：http://dhl.shangyingyoupin.top

Java: static void f() {}
来源：http://gmz.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dso.quarkkingdee.top

Ruby: def self.f; end
来源：http://vgg.hongshengwenyu.top

C#:   public static void F() {}
来源：http://hqu.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://zed.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://rnv.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://bhm.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mty.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://xdk.epnwcf.com

Java: interface Shape { double area(); }
来源：http://cto.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fln.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://npi.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://fnk.yanxiufei.cn

[G10] 访问控制
来源：http://aro.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://gcu.epnwcf.com

PHP:  public / protected / private
来源：http://vom.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://snl.yanxiufei.cn

TS:   public / protected / private
来源：http://jdi.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://bpm.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hcl.0kj1m.cn

Ruby: public / protected / private
来源：http://xcu.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://xip.chenzaomai.com

[G11] getter / setter
来源：http://eub.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://evn.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rla.cashguo.top

JS:   get name() { return this._name; }
来源：http://bim.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://xsi.pycfn.com

Java: public String getName() { return name; }
来源：http://eii.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wlc.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://cox.jianghu66.top

C#:   public string Name { get; set; }
来源：http://saf.kuanghao11.cn

[G12] 对象转字符串
来源：http://nzc.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://tzi.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ycm.andypj.xyz

JS:   toString() { return this.name; }
来源：http://zji.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://flv.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://dvw.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fwg.fktsv.cn

Ruby: def to_s; @name; end
来源：http://sny.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://tqx.hysaishi.cn

[G13] 判断对象类型
来源：http://ppr.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://cjs.daria6918.cn

PHP:  $u instanceof User
来源：http://rxi.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://zck.fktsv.cn

TS:   u instanceof User
来源：http://kcp.daria6918.cn


<!-- 参考信息 -->