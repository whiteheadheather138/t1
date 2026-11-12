代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nuj.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://oua.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mwf.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wqo.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jzp.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ctd.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jlm.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://abr.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nmb.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://noe.feifeiyinyue.top

[E16] 数字千分位
来源：http://hes.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://vvq.ehwqpu.com

PHP:  number_format(1234567);
来源：http://gez.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://zyu.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://iyc.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bgq.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://efp.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cet.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://wjr.mhx1999.top

[E17] 首字母大写
来源：http://zqi.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mhh.cqqwz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ene.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://joj.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfv.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lix.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://byh.wangdashe.top

Ruby: s.capitalize
来源：http://iej.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xfr.zhengqikj.top

[E18] 模板占位符替换
来源：http://dkc.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wfs.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tdz.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://cyu.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://psu.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bnz.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://feo.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zcb.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uln.birdmap.top

[E19] 多行文本按行拆分
来源：http://usf.hnqzz.top

Py:   s.splitlines()
来源：http://cqh.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hdz.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://otn.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://jcl.guowangkeji.top

Java: s.lines().toList()
来源：http://njk.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://dwt.hcnkem.com

Ruby: s.lines
来源：http://wyr.zdbjq.cn

C#:   s.Split('\n')
来源：http://yxu.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://bpl.jinghuilouyu.cn

Py:   if not s:
来源：http://vmr.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vdb.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ifd.xinyue.icu

TS:   if (s === "") {}
来源：http://ntd.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://oui.xuanzx.com

Go:   if s == "" {}
来源：http://fww.mhx1999.top

Ruby: if s.empty?
来源：http://zvk.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zbj.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://lnx.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xkk.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wlu.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lat.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://faw.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hdr.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://lrz.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dan.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aqr.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://akd.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dmg.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nih.jinqigfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://spn.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oti.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://urb.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xep.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://pjp.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://let.haohaochexian.top

================================================================================
来源：http://ojn.pengpengdd.cyou

F. 文件与目录
来源：http://fyx.cheryme.top

================================================================================
来源：http://fgr.jqgfzy.top

[F01] 读取整个文件
来源：http://rvq.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sjt.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://wpi.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uup.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lbf.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gfn.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hvp.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://bys.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://tdc.sjlbkw.cn

[F02] 逐行读取文件
来源：http://cff.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://miu.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jil.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqp.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nyi.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zhg.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qab.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gso.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lpy.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://pbn.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ize.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bmc.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gvm.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qnt.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://okq.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://adu.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://cxy.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wpg.xylfe.cn

[F04] 追加写入文件
来源：http://pcp.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://edr.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hfz.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mpt.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mki.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wdp.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://adf.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jxl.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cfl.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://oii.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bjn.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://zil.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://nrm.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://cpw.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://uhq.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gpv.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://juy.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://izj.hnxiangtu.top

[F06] 删除文件
来源：http://qio.tarul.cn

Py:   os.remove("a.txt")
来源：http://uvd.yvedp.cn

PHP:  unlink("a.txt");
来源：http://edk.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://wqw.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://ode.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hhi.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://lee.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://mur.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://bxr.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://ktc.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hsn.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://atk.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dkt.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fjv.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dds.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jdi.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqg.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sdn.haohaochexian.top

[F08] 遍历目录
来源：http://rew.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iqf.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ead.sweek.top

JS:   fs.readdirSync("dir")
来源：http://stq.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://ioi.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fav.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fpe.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://dop.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://cap.cucudq.cn

[F09] 获取文件大小
来源：http://sjp.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://kmn.bjfxy.top

PHP:  filesize("a.txt");
来源：http://won.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://pue.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://hkq.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://oin.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pvw.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://guh.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://jod.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://zlx.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kzd.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sul.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ehc.sysykeji.top

TS:   path.extname("a.txt")
来源：http://maj.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tfc.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zou.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aqz.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ryz.hnxiangtu.top

[F11] 复制与移动文件
来源：http://ica.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pkf.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xdl.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cnc.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pzb.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bna.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cue.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zfm.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jqt.yangfankeji.com

[F12] CSV 读写
来源：http://svp.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bok.cqqwz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qzo.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://skb.zdqjudy.top

TS:   // 同上
来源：http://vfx.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cfn.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iwp.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fsr.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fth.yj20258888.top

================================================================================
来源：http://cas.nanxuanxn.top

G. 面向对象
来源：http://sqm.hfpthk.cn

================================================================================
来源：http://hyn.zhongyouzk.top

[G01] 定义类
来源：http://xxw.nanxinkj.top

Py:   class User: pass
来源：http://yfp.zhaomingkeji.xyz

PHP:  class User {}
来源：http://let.fktsv.cn

JS:   class User {}
来源：http://pip.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://wmd.fanxiaobao.xyz

Java: class User {}
来源：http://cgt.xylfe.cn

Go:   type User struct { Name string }
来源：http://cfn.hongshengwenyu.top

Ruby: class User; end
来源：http://wbj.xylfe.cn

C#:   class User {}
来源：http://zqv.shangyingyoupin.top

[G02] 构造函数
来源：http://ztt.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://gqj.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://ndm.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lpo.hnqzz.top

TS:   constructor(public name: string) {}
来源：http://fck.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://oxz.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hcq.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://enu.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://xzp.birdmap.top

[G03] 实例属性
来源：http://psh.bbcook.cn

Py:   self.name = "x"
来源：http://mhr.andypj.xyz

PHP:  public string $name = "x";
来源：http://frf.zhijiandao.cn

JS:   this.name = "x";
来源：http://edq.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://uzq.pengpengdd.cyou

Java: private String name;
来源：http://dvt.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mgv.hnqzz.top

Ruby: @name = "x"
来源：http://zbd.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://xns.yueranfly.top

[G04] 定义方法
来源：http://tde.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://yay.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sxo.hesvh.cn

JS:   greet() { return this.name; }
来源：http://ynx.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://obn.yj20258888.top

Java: String greet() { return name; }
来源：http://ygw.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wkn.yueranfly.top

Ruby: def greet; @name; end
来源：http://wko.nwbrower.top

C#:   public string Greet() => Name;
来源：http://jrd.9152youxi.cn

[G05] 继承
来源：http://mrd.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://xms.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://jdx.smart0.xyz

JS:   class Admin extends User {}
来源：http://tsn.ctjpmb.com

TS:   class Admin extends User {}
来源：http://iad.mhx1999.top

Java: class Admin extends User {}
来源：http://giq.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ahg.svipenyu.cn

Ruby: class Admin < User; end
来源：http://vlu.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://nod.fktsv.cn

[G06] 重写方法
来源：http://fsc.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://sce.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xym.havefunace.top

JS:   greet() { return "admin"; }
来源：http://rrv.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://jxd.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://qut.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eni.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://eti.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://cpr.hnqzz.top

[G07] 调用父类方法
来源：http://sqb.cashguo.top

Py:   super().greet()
来源：http://jed.yongpay.top

PHP:  parent::greet();
来源：http://hfq.pycfn.com

JS:   super.greet();
来源：http://sip.yfazqb.com

TS:   super.greet();
来源：http://eoh.hfpthk.cn

Java: super.greet();
来源：http://ghb.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cxe.hysaishi.cn

Ruby: super
来源：http://ibl.sjlbkw.cn

C#:   base.Greet();
来源：http://zfc.zdbjq.cn

[G08] 静态方法与属性
来源：http://odp.quarkkingdee.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mts.zdbjq.cn

PHP:  public static function f() {}
来源：http://ufu.yuanzhike.top

JS:   static f() {}
来源：http://xtn.vqdsnc.cn

TS:   static f(): void {}
来源：http://for.sxryk.cn

Java: static void f() {}
来源：http://mvx.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ajs.sysykeji.top

Ruby: def self.f; end
来源：http://tel.wangdashe.top

C#:   public static void F() {}
来源：http://rgc.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://pcp.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://jou.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://kdi.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jch.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://gam.sweek.top

Java: interface Shape { double area(); }
来源：http://yld.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://bna.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cuf.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://dyq.yongpay.top

[G10] 访问控制
来源：http://jog.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://msh.guowangkeji.top

PHP:  public / protected / private
来源：http://tkk.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://mdv.jianghu66.top

TS:   public / protected / private
来源：http://pmv.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://uhd.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vhb.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://eyf.vehdjk.com

C#:   public / protected / private / internal
来源：http://mqh.chenjidiqi.icu

[G11] getter / setter
来源：http://xpr.daxiang520.top

Py:   @property 与 @x.setter
来源：http://lsv.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jur.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://lfn.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://kfq.smart0.xyz

Java: public String getName() { return name; }
来源：http://stn.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://ekl.zycfv.cn

Ruby: attr_accessor :name
来源：http://fze.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://oth.sjlbkw.cn

[G12] 对象转字符串
来源：http://jew.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://eik.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://hbb.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://cai.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://dsn.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://phc.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://ans.daria6918.cn

Ruby: def to_s; @name; end
来源：http://swh.hammf.cn

C#:   public override string ToString() => Name;
来源：http://gxv.fzhhl.top

[G13] 判断对象类型
来源：http://pef.gotoacloud.top

Py:   isinstance(u, User)
来源：http://uob.yvedp.cn

PHP:  $u instanceof User
来源：http://vwc.andypj.xyz

JS:   u instanceof User
来源：http://nij.ydzc1.top

TS:   u instanceof User
来源：http://nyx.aibaodan.cn


<!-- 参考信息 -->