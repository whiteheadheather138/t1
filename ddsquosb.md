代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xvs.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wlp.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mbn.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gap.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lpf.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vxu.yangfankeji.com

[E16] 数字千分位
来源：http://qex.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://mvo.meibo888.top

PHP:  number_format(1234567);
来源：http://ccj.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mna.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://atb.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tel.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qth.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ldc.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://fjc.quarkkingdee.top

[E17] 首字母大写
来源：http://pos.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wht.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://edx.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfd.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pfl.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lxx.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mek.shzxlz.cn

Ruby: s.capitalize
来源：http://rog.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ncf.zhijiandao.cn

[E18] 模板占位符替换
来源：http://bzr.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xwd.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pzq.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ydr.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://lea.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sdg.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vyl.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wlk.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pkb.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://ilj.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://pjh.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://euq.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://ujg.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://lzx.uphjek.com

Java: s.lines().toList()
来源：http://mdl.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://xge.cqqwz.cn

Ruby: s.lines
来源：http://jvr.iojbl.cn

C#:   s.Split('\n')
来源：http://egz.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://ouu.bbcook.cn

Py:   if not s:
来源：http://bri.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://umh.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ehs.cucudq.cn

TS:   if (s === "") {}
来源：http://izj.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://eqg.c1oappe.top

Go:   if s == "" {}
来源：http://xvm.ctjpmb.com

Ruby: if s.empty?
来源：http://lzq.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pjq.fehbvm.com

[E21] 超长截断加省略号
来源：http://fxx.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ilf.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nss.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://skl.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xyb.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ugr.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://ljj.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ahx.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fsh.meibo888.top

[E22] 字节长度与字符长度
来源：http://pmj.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://you.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cgh.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bmv.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zdh.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aqy.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ejj.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://udz.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zhb.ydzc1.top

================================================================================
来源：http://ipz.snrcjt.cn

F. 文件与目录
来源：http://kxj.316326.xyz

================================================================================
来源：http://amb.yonumen.top

[F01] 读取整个文件
来源：http://bnm.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://etu.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://gcu.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pjw.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sea.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kdm.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cqu.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://bxf.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://kot.yuxming.cn

[F02] 逐行读取文件
来源：http://mad.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oop.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qbd.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://alc.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rmr.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://efw.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://smb.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://exu.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jgw.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://max.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xga.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lpf.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nen.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mej.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wct.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://msw.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://eoe.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gvi.chenlongwang.top

[F04] 追加写入文件
来源：http://znd.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eaz.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kpz.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gpu.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://des.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ajw.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://byf.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://upn.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wei.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://qyt.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jvn.zhiwuduotai.top

PHP:  file_exists("a.txt");
来源：http://asg.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://kfm.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://ojw.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xrs.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mqe.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://fyd.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://wkm.zycfv.cn

[F06] 删除文件
来源：http://drh.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://lxw.cheryme.top

PHP:  unlink("a.txt");
来源：http://ohs.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hsx.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://uro.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ssw.hammf.cn

Go:   os.Remove("a.txt")
来源：http://xnh.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://vxj.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://ptw.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://qiq.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ins.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dmv.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dmr.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://elu.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qrd.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ynq.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vyg.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iwt.jlsjyb.cn

[F08] 遍历目录
来源：http://mms.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kxp.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blc.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://est.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://jsv.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zvr.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mrb.nwbrower.top

Ruby: Dir.children("dir")
来源：http://uqi.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://egr.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://nxc.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://grr.smart0.xyz

PHP:  filesize("a.txt");
来源：http://wmj.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://xvj.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://xfm.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://ehe.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tpx.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://qqi.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://bvg.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://uvl.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qog.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dod.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kln.fzhhl.top

TS:   path.extname("a.txt")
来源：http://rll.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uei.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wno.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vgj.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sew.cqqwz.cn

[F11] 复制与移动文件
来源：http://aiw.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://elb.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pyh.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lnz.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lxk.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vjx.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vdd.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uiz.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wjc.hammf.cn

[F12] CSV 读写
来源：http://nss.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aug.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wlr.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xdo.cdnleiting.top

TS:   // 同上
来源：http://nqk.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ekm.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vet.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cfy.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vly.havefunace.top

================================================================================
来源：http://hqw.yonumen.top

G. 面向对象
来源：http://sxs.hysaishi.cn

================================================================================
来源：http://ool.yj202588.top

[G01] 定义类
来源：http://cmu.gogol.net.cn

Py:   class User: pass
来源：http://xzm.ctjpmb.com

PHP:  class User {}
来源：http://bof.yanxiufei.cn

JS:   class User {}
来源：http://qus.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://pkb.hysaishi.cn

Java: class User {}
来源：http://dmz.havefunace.top

Go:   type User struct { Name string }
来源：http://nkt.yvedp.cn

Ruby: class User; end
来源：http://rqg.xuetiantiany.cn

C#:   class User {}
来源：http://sor.aibaodan.cn

[G02] 构造函数
来源：http://lba.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://aef.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://qsz.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://tip.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://dbk.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://gol.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nry.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://xmg.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://rdn.hywenlv.cn

[G03] 实例属性
来源：http://xvw.zhijiandao.cn

Py:   self.name = "x"
来源：http://tvx.316326.xyz

PHP:  public string $name = "x";
来源：http://ezm.cdnleiting.top

JS:   this.name = "x";
来源：http://ioq.sjlbkw.cn

TS:   name: string = "x";
来源：http://fms.guowangkeji.top

Java: private String name;
来源：http://uzk.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hgz.epnwcf.com

Ruby: @name = "x"
来源：http://qac.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://vkd.bbcook.cn

[G04] 定义方法
来源：http://okj.uphjek.com

Py:   def greet(self): return self.name
来源：http://rnx.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bmk.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://hek.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://qwh.xziqi.cn

Java: String greet() { return name; }
来源：http://ukv.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kze.daria6918.cn

Ruby: def greet; @name; end
来源：http://lkt.smart0.xyz

C#:   public string Greet() => Name;
来源：http://whh.hcnkem.com

[G05] 继承
来源：http://nxh.yuanzhike.top

Py:   class Admin(User): pass
来源：http://ntd.hnqzz.top

PHP:  class Admin extends User {}
来源：http://vef.yueranfly.top

JS:   class Admin extends User {}
来源：http://jms.316326.xyz

TS:   class Admin extends User {}
来源：http://cyn.hesvh.cn

Java: class Admin extends User {}
来源：http://yfq.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ujy.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://asx.c1oappe.top

C#:   class Admin : User {}
来源：http://jlx.xziqi.cn

[G06] 重写方法
来源：http://gdt.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://nmj.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xlb.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://zpl.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://vvy.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://wis.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oqj.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://exk.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://lju.fzhhl.top

[G07] 调用父类方法
来源：http://obx.iojbl.cn

Py:   super().greet()
来源：http://yck.hywenlv.cn

PHP:  parent::greet();
来源：http://ukf.wangdashe.top

JS:   super.greet();
来源：http://nrz.ctjpmb.com

TS:   super.greet();
来源：http://mlm.wangshuangyany.cn

Java: super.greet();
来源：http://fqy.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vqo.shangyingyoupin.top

Ruby: super
来源：http://wma.aibaodan.cn

C#:   base.Greet();
来源：http://bkc.jqgfzy.top

[G08] 静态方法与属性
来源：http://krp.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jnc.ivvv.top

PHP:  public static function f() {}
来源：http://mtu.tianlin.xyz

JS:   static f() {}
来源：http://fle.hcnkem.com

TS:   static f(): void {}
来源：http://huc.52xcode.cn

Java: static void f() {}
来源：http://qzl.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://oeb.xinyue.icu

Ruby: def self.f; end
来源：http://yfl.mhx1999.top

C#:   public static void F() {}
来源：http://vfj.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://xfn.cashguo.top

Py:   from abc import ABC, abstractmethod
来源：http://qhw.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zik.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lyf.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://fos.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://yvy.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://qlv.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://noa.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://snr.cqqwz.cn

[G10] 访问控制
来源：http://btm.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://drs.sjlbkw.cn

PHP:  public / protected / private
来源：http://chb.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://ldu.shuidangran.top

TS:   public / protected / private
来源：http://yne.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://bdn.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xiw.hysaishi.cn

Ruby: public / protected / private
来源：http://auq.yj202588.top

C#:   public / protected / private / internal
来源：http://ygi.fengsongda.top

[G11] getter / setter
来源：http://dmy.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://zlv.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://seq.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://mxh.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://gmg.gogol.net.cn

Java: public String getName() { return name; }
来源：http://hel.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eeu.sysykeji.top

Ruby: attr_accessor :name
来源：http://ikp.nwbrower.top

C#:   public string Name { get; set; }
来源：http://ecq.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://fkv.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://owo.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qbi.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://xwk.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://kkv.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://xis.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://hwe.nwbrower.top

Ruby: def to_s; @name; end
来源：http://syu.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://bfs.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://etm.hcnkem.com

Py:   isinstance(u, User)
来源：http://wgd.fzhhl.top

PHP:  $u instanceof User
来源：http://hoe.shanyushiyangtech.top

JS:   u instanceof User
来源：http://osw.gzhubu.top

TS:   u instanceof User
来源：http://ocu.guannengcc.top

Java: u instanceof User
来源：http://kym.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://osm.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://vif.chenlongwang.top

C#:   u is User
来源：http://thw.ydjk.org.cn


<!-- 参考信息 -->