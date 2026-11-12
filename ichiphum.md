代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eqj.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://lvf.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://xeg.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dtb.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dyi.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yck.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gkp.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rkb.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://owr.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tmp.hammf.cn

[E16] 数字千分位
来源：http://ruc.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://zsg.sweek.top

PHP:  number_format(1234567);
来源：http://coy.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jwn.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xzo.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nwy.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lle.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zva.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://xbe.zhixingplan.top

[E17] 首字母大写
来源：http://qrj.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hmh.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jzz.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://onq.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ati.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://asd.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://evq.sweek.top

Ruby: s.capitalize
来源：http://pzv.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zpt.ybcxt.top

[E18] 模板占位符替换
来源：http://ils.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nbr.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hwy.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://vkt.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://eol.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fln.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wzh.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mqv.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kwp.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://hpe.sweek.top

Py:   s.splitlines()
来源：http://prg.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ylq.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://gej.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://wwv.hcnkem.com

Java: s.lines().toList()
来源：http://vhj.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://nce.sufxvd.cn

Ruby: s.lines
来源：http://gcu.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://zsz.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://wkl.pengpengdd.cyou

Py:   if not s:
来源：http://xzj.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ftu.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jtz.jianghu66.top

TS:   if (s === "") {}
来源：http://sts.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://wfz.0kj1m.cn

Go:   if s == "" {}
来源：http://iov.fengsongda.top

Ruby: if s.empty?
来源：http://aej.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tfu.hammf.cn

[E21] 超长截断加省略号
来源：http://jzb.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zfj.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ifi.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wew.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vnm.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sld.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://vyi.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://orp.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nhh.ydzc1.top

[E22] 字节长度与字符长度
来源：http://clo.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fhv.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vuu.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhf.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tcg.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tbc.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tnq.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://uoy.gaohongyu789.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://syj.fengsongda.top

================================================================================
来源：http://qsb.zycfv.cn

F. 文件与目录
来源：http://gwg.jiagoushi.top

================================================================================
来源：http://cki.xuetiantiany.cn

[F01] 读取整个文件
来源：http://xps.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://crn.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://kte.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://trj.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://riz.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nhr.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uem.c1oappe.top

Ruby: File.read("a.txt")
来源：http://aet.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://pax.fzhhl.top

[F02] 逐行读取文件
来源：http://mhu.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uef.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zuy.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://edc.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prj.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mdo.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fye.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dxn.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ipv.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://clk.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tda.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kvq.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nlf.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsq.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dzi.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rol.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://lzy.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sfm.zdqjudy.top

[F04] 追加写入文件
来源：http://yml.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nvt.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tvo.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xuj.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://llk.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yec.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cal.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jul.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://omh.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://sdb.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ygq.sweek.top

PHP:  file_exists("a.txt");
来源：http://jpt.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://vxj.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://tqn.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dlg.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yad.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://cfy.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://cts.daxiang520.top

[F06] 删除文件
来源：http://wjr.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://ikf.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://ngs.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://umd.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pxh.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bwb.316326.xyz

Go:   os.Remove("a.txt")
来源：http://pfl.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://fdk.birdmap.top

C#:   File.Delete("a.txt");
来源：http://xpi.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://zfg.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ogq.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hux.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sbe.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oar.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ggx.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://upx.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pua.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sft.shzxlz.cn

[F08] 遍历目录
来源：http://qnu.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://loe.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iiq.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://uvq.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://bxe.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uyc.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://trr.gzhubu.top

Ruby: Dir.children("dir")
来源：http://rwl.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://gjm.pycfn.com

[F09] 获取文件大小
来源：http://hrr.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://oyy.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://ilt.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://rrs.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://svi.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://fvq.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sup.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://zje.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://obi.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://aqv.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dvo.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tiv.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mah.ybcxt.top

TS:   path.extname("a.txt")
来源：http://pzw.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pjl.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jrl.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hlg.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ogm.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://zaj.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ydk.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uch.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yde.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://crg.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qit.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wwb.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vcz.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eud.hammf.cn

[F12] CSV 读写
来源：http://obg.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yem.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zyn.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kgu.jinghuilouyu.cn

TS:   // 同上
来源：http://dpf.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hfj.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jsm.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pgn.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ial.316326.xyz

================================================================================
来源：http://vxy.bjfxy.top

G. 面向对象
来源：http://djh.mhx1999.top

================================================================================
来源：http://pnk.fzhhl.top

[G01] 定义类
来源：http://wrd.zhixingplan.top

Py:   class User: pass
来源：http://lkf.shanyushiyangkeji.top

PHP:  class User {}
来源：http://hyr.daria6918.cn

JS:   class User {}
来源：http://end.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://fpx.ydjk.org.cn

Java: class User {}
来源：http://gec.sysykeji.top

Go:   type User struct { Name string }
来源：http://rdy.jianghu66.top

Ruby: class User; end
来源：http://zmv.zdqjudy.top

C#:   class User {}
来源：http://fbs.cdnleiting.top

[G02] 构造函数
来源：http://oxa.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://yuh.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://pxo.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://kjb.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://qeg.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://ppp.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xla.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://leo.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://kaf.zhixingplan.top

[G03] 实例属性
来源：http://vdx.yj20258.top

Py:   self.name = "x"
来源：http://ijr.vehdjk.com

PHP:  public string $name = "x";
来源：http://thd.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://sbj.hfpthk.cn

TS:   name: string = "x";
来源：http://bqb.hfpthk.cn

Java: private String name;
来源：http://xdb.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mxs.zdqjudy.top

Ruby: @name = "x"
来源：http://oke.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://xpb.wangshuangyany.cn

[G04] 定义方法
来源：http://doc.bbcook.cn

Py:   def greet(self): return self.name
来源：http://suo.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zow.epnwcf.com

JS:   greet() { return this.name; }
来源：http://tqj.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://vgj.yangfankeji.com

Java: String greet() { return name; }
来源：http://gvp.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ruv.ydzc1.top

Ruby: def greet; @name; end
来源：http://xlp.epnwcf.com

C#:   public string Greet() => Name;
来源：http://lbg.yueranfly.top

[G05] 继承
来源：http://fzg.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://zun.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://qwn.daxiang520.top

JS:   class Admin extends User {}
来源：http://osr.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://nap.gzhubu.top

Java: class Admin extends User {}
来源：http://jme.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mge.cheryme.top

Ruby: class Admin < User; end
来源：http://rzm.shzxlz.cn

C#:   class Admin : User {}
来源：http://lmt.havefunace.top

[G06] 重写方法
来源：http://khk.yongpay.top

Py:   def greet(self): return "admin"
来源：http://pjt.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dgp.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://cyb.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://hiq.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://nem.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xdc.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://uma.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://uuy.kuanghao11.cn

[G07] 调用父类方法
来源：http://itu.yuxming.cn

Py:   super().greet()
来源：http://pkp.xuanzx.com

PHP:  parent::greet();
来源：http://tku.zycfv.cn

JS:   super.greet();
来源：http://jbn.jinqigufen.top

TS:   super.greet();
来源：http://xid.wangshuangyany.cn

Java: super.greet();
来源：http://rno.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iqf.bjfxy.top

Ruby: super
来源：http://pxv.smart0.xyz

C#:   base.Greet();
来源：http://ywj.tianlin.xyz

[G08] 静态方法与属性
来源：http://hvw.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qbh.ivvv.top

PHP:  public static function f() {}
来源：http://pxw.havefunace.top

JS:   static f() {}
来源：http://cdp.bbcook.cn

TS:   static f(): void {}
来源：http://lhl.yfazqb.com

Java: static void f() {}
来源：http://sym.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://urx.jinqigfzy.top

Ruby: def self.f; end
来源：http://pqp.sweek.top

C#:   public static void F() {}
来源：http://rxr.xuanzx.com

[G09] 接口 / 抽象类
来源：http://gny.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://pah.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rij.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ael.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://fqj.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://mtm.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://fgv.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fxh.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://jxo.yuxming.cn

[G10] 访问控制
来源：http://ics.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://tzu.nanxinkj.top

PHP:  public / protected / private
来源：http://pzn.yj20258.top

JS:   #private 字段；其余公开
来源：http://aaj.xylfe.cn

TS:   public / protected / private
来源：http://slk.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://qtd.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fyk.hammf.cn

Ruby: public / protected / private
来源：http://jcp.vehdjk.com

C#:   public / protected / private / internal
来源：http://agw.fanxiaobao.xyz

[G11] getter / setter
来源：http://jap.yueranfly.top

Py:   @property 与 @x.setter
来源：http://lbq.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zpo.birdmap.top

JS:   get name() { return this._name; }
来源：http://hoz.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://tni.fzhhl.top

Java: public String getName() { return name; }
来源：http://iiw.chenzaomai.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzo.fzhhl.top

Ruby: attr_accessor :name
来源：http://qmk.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://yfg.daria6918.cn

[G12] 对象转字符串
来源：http://kha.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://sxx.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ngn.tarul.cn

JS:   toString() { return this.name; }
来源：http://tha.meibo888.top

TS:   toString(): string { return this.name; }
来源：http://srw.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://bgb.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aoa.xziqi.cn

Ruby: def to_s; @name; end
来源：http://xjf.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://xwu.chenlongwang.top

[G13] 判断对象类型
来源：http://jln.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://qpu.cqqwz.cn

PHP:  $u instanceof User
来源：http://zzv.aizwys.cn

JS:   u instanceof User
来源：http://fnv.zhoulong.xyz

TS:   u instanceof User
来源：http://ozj.ctjpmb.com


<!-- 参考信息 -->