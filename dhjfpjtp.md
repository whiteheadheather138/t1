代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kjf.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://pdw.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lrx.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://izc.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bkr.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://crj.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dbc.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hmc.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ult.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xzw.bjfxy.top

[E16] 数字千分位
来源：http://prm.jianghu66.top

Py:   f"{1234567:,}"
来源：http://ede.fengsongda.top

PHP:  number_format(1234567);
来源：http://cfl.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hra.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://chv.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oay.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yrs.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nwz.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://dwq.daria6918.cn

[E17] 首字母大写
来源：http://mzx.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://emp.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cnm.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fcw.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aev.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xcz.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oie.tanke756.top

Ruby: s.capitalize
来源：http://wuk.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nat.shzxlz.cn

[E18] 模板占位符替换
来源：http://wap.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sqj.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uja.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://fdm.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nhk.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fbe.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://koi.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xix.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nvu.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://kqo.chenlongwang.top

Py:   s.splitlines()
来源：http://cxk.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ihd.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://lez.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://out.tanke756.top

Java: s.lines().toList()
来源：http://vfl.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://nhk.hesvh.cn

Ruby: s.lines
来源：http://yls.hywenlv.cn

C#:   s.Split('\n')
来源：http://bwg.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://msx.kuanghao11.cn

Py:   if not s:
来源：http://ueo.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cbb.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mum.jqgfzy.top

TS:   if (s === "") {}
来源：http://njx.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://djb.c1oappe.top

Go:   if s == "" {}
来源：http://aun.cucudq.cn

Ruby: if s.empty?
来源：http://wee.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vpu.tarul.cn

[E21] 超长截断加省略号
来源：http://ojt.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nps.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iwm.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hml.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdk.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ntu.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://ivv.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dwf.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://asj.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://did.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://flk.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://crf.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxt.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ucd.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://klk.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hmt.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://lry.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tda.yongpay.top

================================================================================
来源：http://dtv.jinqigufen.top

F. 文件与目录
来源：http://uhd.shzxlz.cn

================================================================================
来源：http://bdj.shuidangran.top

[F01] 读取整个文件
来源：http://qsm.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ilj.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://zcj.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dxo.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ntw.jqgufenzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://toy.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qhw.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://dvs.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://pyo.zycfv.cn

[F02] 逐行读取文件
来源：http://rpg.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ztk.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iqx.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kqa.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qrr.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kmb.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tgf.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://txd.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gpk.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://pdd.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nhq.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nqc.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vof.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nlp.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://veq.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rpd.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://gts.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qoi.zdbjq.cn

[F04] 追加写入文件
来源：http://ara.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kjm.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://akr.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jbf.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zae.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vea.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iqc.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wpv.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zlb.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://ggi.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wnq.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://drb.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://jru.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://azx.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uqd.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rjh.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://jxv.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://cyw.pengpengdd.cyou

[F06] 删除文件
来源：http://ygy.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://pnf.daxiang520.top

PHP:  unlink("a.txt");
来源：http://jfx.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lhj.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://udj.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ksc.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://xhb.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://bua.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://dzx.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://uwn.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ehs.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vmr.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qpz.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wpk.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ztx.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vrv.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rsm.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iiv.gogol.net.cn

[F08] 遍历目录
来源：http://wte.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nzg.cucudq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://typ.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://vuz.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://dxz.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyr.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wjs.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://bri.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://ibu.jianghu66.top

[F09] 获取文件大小
来源：http://zxw.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://asp.tian-w.cn

PHP:  filesize("a.txt");
来源：http://pzj.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://glf.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://noh.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://fyi.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qys.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://gho.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://znz.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://sco.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dkb.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vvy.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vyy.hcnkem.com

TS:   path.extname("a.txt")
来源：http://zss.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://epg.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pkq.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uwz.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://izt.zhijiandao.cn

[F11] 复制与移动文件
来源：http://dpx.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qlj.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://njg.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bnr.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tul.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kxl.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nnn.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qoi.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vxc.hesvh.cn

[F12] CSV 读写
来源：http://xtt.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ohq.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oqb.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://foh.andypj.xyz

TS:   // 同上
来源：http://pby.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jtt.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ttd.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zyt.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ivm.jinqigufen.top

================================================================================
来源：http://bxh.epnwcf.com

G. 面向对象
来源：http://oit.hysaishi.cn

================================================================================
来源：http://qhl.wangdashe.top

[G01] 定义类
来源：http://dls.haohaochexian.top

Py:   class User: pass
来源：http://xad.jinyuanbaomall.cn

PHP:  class User {}
来源：http://kmy.jinqigfzy.top

JS:   class User {}
来源：http://evn.havefunace.top

TS:   class User { name: string = ""; }
来源：http://hqm.ehwqpu.com

Java: class User {}
来源：http://did.shuidangran.top

Go:   type User struct { Name string }
来源：http://xvy.zycfv.cn

Ruby: class User; end
来源：http://kbi.guannengcc.top

C#:   class User {}
来源：http://qhi.hnxiangtu.top

[G02] 构造函数
来源：http://jio.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://rqe.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://odo.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://cqa.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://faf.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://pet.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gke.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://tqh.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://klu.yj202588.top

[G03] 实例属性
来源：http://hjf.ivvv.top

Py:   self.name = "x"
来源：http://slh.0kj1m.cn

PHP:  public string $name = "x";
来源：http://pom.hywenlv.cn

JS:   this.name = "x";
来源：http://eqm.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://tzz.tianlin.xyz

Java: private String name;
来源：http://ugy.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://llm.iojbl.cn

Ruby: @name = "x"
来源：http://ylw.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://nuz.sxryk.cn

[G04] 定义方法
来源：http://qcu.hammf.cn

Py:   def greet(self): return self.name
来源：http://vfp.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mez.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://zwp.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://jfa.pycfn.com

Java: String greet() { return name; }
来源：http://kdb.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://dmx.shzxlz.cn

Ruby: def greet; @name; end
来源：http://btp.redwolf501.top

C#:   public string Greet() => Name;
来源：http://buu.hcnkem.com

[G05] 继承
来源：http://kan.dashuyun.cn

Py:   class Admin(User): pass
来源：http://tji.sysykeji.top

PHP:  class Admin extends User {}
来源：http://itu.ctjpmb.com

JS:   class Admin extends User {}
来源：http://luu.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://njq.nwbrower.top

Java: class Admin extends User {}
来源：http://qem.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kxe.316326.xyz

Ruby: class Admin < User; end
来源：http://qyo.shuidangran.top

C#:   class Admin : User {}
来源：http://rkc.hammf.cn

[G06] 重写方法
来源：http://mxt.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://lyz.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tpp.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://qev.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://sif.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://bai.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://udx.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://amb.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://jat.sweek.top

[G07] 调用父类方法
来源：http://cpv.yonumen.top

Py:   super().greet()
来源：http://lgs.vqdsnc.cn

PHP:  parent::greet();
来源：http://bjy.hammf.cn

JS:   super.greet();
来源：http://cdr.zdqjudy.top

TS:   super.greet();
来源：http://lxd.fzhhl.top

Java: super.greet();
来源：http://mwr.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yqj.chenlongwang.top

Ruby: super
来源：http://ahv.svipenyu.cn

C#:   base.Greet();
来源：http://ymr.52xcode.cn

[G08] 静态方法与属性
来源：http://hjo.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ggp.ybcxt.top

PHP:  public static function f() {}
来源：http://szy.aibaodan.cn

JS:   static f() {}
来源：http://wvd.guannengcc.top

TS:   static f(): void {}
来源：http://ucm.xylfe.cn

Java: static void f() {}
来源：http://mne.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pms.gzhubu.top

Ruby: def self.f; end
来源：http://fzf.ydzc1.top

C#:   public static void F() {}
来源：http://igm.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://okq.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pje.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://fdt.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qug.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://yxf.xylfe.cn

Java: interface Shape { double area(); }
来源：http://zvr.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://lxy.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yes.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://win.havefunace.top

[G10] 访问控制
来源：http://ify.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://ixa.jqgfzy.top

PHP:  public / protected / private
来源：http://kye.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://bcb.ybcxt.top

TS:   public / protected / private
来源：http://sqh.yongpay.top

Java: public / protected / private / 默认包级
来源：http://api.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qno.sysykeji.top

Ruby: public / protected / private
来源：http://zpn.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://ooq.pengpengdd.cyou

[G11] getter / setter
来源：http://kyq.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://wbj.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://djx.iojbl.cn

JS:   get name() { return this._name; }
来源：http://lwk.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://gaw.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://byj.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jva.cashguo.top

Ruby: attr_accessor :name
来源：http://bjg.redwolf501.top

C#:   public string Name { get; set; }
来源：http://cdj.yfazqb.com

[G12] 对象转字符串
来源：http://qph.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://wrl.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://cqi.guannengcc.top

JS:   toString() { return this.name; }
来源：http://pmg.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://qci.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://wup.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://pkz.gzhubu.top

Ruby: def to_s; @name; end
来源：http://rrx.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://enj.0kj1m.cn

[G13] 判断对象类型
来源：http://vob.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://sdh.svipenyu.cn

PHP:  $u instanceof User
来源：http://lmm.vehdjk.com

JS:   u instanceof User
来源：http://sow.cqqwz.cn

TS:   u instanceof User
来源：http://bxw.kuanghao11.cn


<!-- 参考信息 -->