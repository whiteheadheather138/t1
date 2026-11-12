代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tdt.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mss.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rcz.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dun.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qcr.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rxs.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://wgd.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://vdq.havefunace.top

PHP:  number_format(1234567);
来源：http://see.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://keq.aibaodan.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wgi.shuidangran.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fzr.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hpj.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ydf.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://kxf.chenzaomai.com

[E17] 首字母大写
来源：http://ibk.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lta.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://lrd.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jqo.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://drn.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wjp.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vgd.ybcxt.top

Ruby: s.capitalize
来源：http://det.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://taf.tian-w.cn

[E18] 模板占位符替换
来源：http://ssg.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://scj.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bwa.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vmb.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://seb.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kip.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://puk.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rgy.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zri.tarul.cn

[E19] 多行文本按行拆分
来源：http://kub.zhijiandao.cn

Py:   s.splitlines()
来源：http://oqj.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jrk.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://liw.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://fvd.ydzc1.top

Java: s.lines().toList()
来源：http://mch.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://eyu.yongpay.top

Ruby: s.lines
来源：http://pnm.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://cpw.yj20258888.top

[E20] 判断字符串是否为空
来源：http://ydf.zhoulong.xyz

Py:   if not s:
来源：http://oxk.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bpz.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://imb.guannengcc.top

TS:   if (s === "") {}
来源：http://dwe.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://yed.yfazqb.com

Go:   if s == "" {}
来源：http://wjx.cashguo.top

Ruby: if s.empty?
来源：http://xku.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qpw.ivvv.top

[E21] 超长截断加省略号
来源：http://qhj.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jfg.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xbt.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kwp.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ivl.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ius.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://lko.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sph.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ong.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://fsy.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gyz.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://noh.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qyg.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://azo.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mat.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vfp.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://wgd.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tdn.smart0.xyz

================================================================================
来源：http://mkn.sjlbkw.cn

F. 文件与目录
来源：http://twq.sjlbkw.cn

================================================================================
来源：http://bqj.zhengqikj.top

[F01] 读取整个文件
来源：http://vwr.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://liu.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://vov.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tcv.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jmx.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qow.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hcq.yj20258.top

Ruby: File.read("a.txt")
来源：http://jdp.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://loy.9152youxi.cn

[F02] 逐行读取文件
来源：http://loy.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ynm.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nmj.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oic.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://efi.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jon.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://unn.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hqj.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://buv.hammf.cn

[F03] 写入文件（覆盖）
来源：http://jtp.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uux.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ged.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pcp.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tdh.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://axx.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fre.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://jgu.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://skn.dashuyun.cn

[F04] 追加写入文件
来源：http://pwr.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bwr.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wkg.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mam.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wlx.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xfx.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hus.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sww.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://laj.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://pjm.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nic.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://yjb.shanyushiyangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://ffe.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://udw.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tbm.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wbp.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://uop.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://uun.cheryme.top

[F06] 删除文件
来源：http://eco.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://jnt.hcnkem.com

PHP:  unlink("a.txt");
来源：http://dec.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://fft.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://put.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xwj.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://omo.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://qbt.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://bpo.redwolf501.top

[F07] 创建目录（含多级）
来源：http://ugi.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ait.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mxj.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwo.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lfc.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://alf.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xoo.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fpf.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cdf.gogol.net.cn

[F08] 遍历目录
来源：http://wto.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yvq.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uwd.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://rhl.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://wjn.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vdp.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hwq.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://lpi.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://obd.yj20258.top

[F09] 获取文件大小
来源：http://zyq.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://epi.fengsongda.top

PHP:  filesize("a.txt");
来源：http://bad.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://hpe.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://gro.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uxr.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ogp.52xcode.cn

Ruby: File.size("a.txt")
来源：http://lkr.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://nqk.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://ifb.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wqs.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://heb.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wtj.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://geh.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lxu.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oub.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aje.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xho.sufxvd.cn

[F11] 复制与移动文件
来源：http://cqm.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://soc.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ccz.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdz.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzu.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oeh.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uud.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bla.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hxj.zycfv.cn

[F12] CSV 读写
来源：http://zdd.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wbx.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vig.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gnb.wangdashe.top

TS:   // 同上
来源：http://nyl.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kbt.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qgo.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://izt.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xqh.xinyue.icu

================================================================================
来源：http://gpo.shzxlz.cn

G. 面向对象
来源：http://cym.fehbvm.com

================================================================================
来源：http://sjy.zdbjq.cn

[G01] 定义类
来源：http://tgs.yj20258.top

Py:   class User: pass
来源：http://ojc.nanxinkj.top

PHP:  class User {}
来源：http://tdw.gzhubu.top

JS:   class User {}
来源：http://vty.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://fth.jyoumei.cn

Java: class User {}
来源：http://vlm.hnqzz.top

Go:   type User struct { Name string }
来源：http://xhi.cashguo.top

Ruby: class User; end
来源：http://sjo.zhengqikj.top

C#:   class User {}
来源：http://qpg.sweek.top

[G02] 构造函数
来源：http://yqe.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://gtc.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://ngl.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://zub.uphjek.com

TS:   constructor(public name: string) {}
来源：http://hrt.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://mlz.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://duk.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://ndc.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://mty.birdmap.top

[G03] 实例属性
来源：http://thl.aibaodan.cn

Py:   self.name = "x"
来源：http://myr.gotoacloud.top

PHP:  public string $name = "x";
来源：http://anp.fzhhl.top

JS:   this.name = "x";
来源：http://sdy.yongpay.top

TS:   name: string = "x";
来源：http://rff.iojbl.cn

Java: private String name;
来源：http://vmz.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fcv.hongshengwenyu.top

Ruby: @name = "x"
来源：http://wlr.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://cmq.jqgufenzy.top

[G04] 定义方法
来源：http://yum.cashguo.top

Py:   def greet(self): return self.name
来源：http://niw.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://gxo.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://oxx.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://dyk.hywenlv.cn

Java: String greet() { return name; }
来源：http://afs.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://vtz.jianghu66.top

Ruby: def greet; @name; end
来源：http://zom.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://bgf.fzhhl.top

[G05] 继承
来源：http://wyc.mhx1999.top

Py:   class Admin(User): pass
来源：http://hxl.xylfe.cn

PHP:  class Admin extends User {}
来源：http://gxq.xziqi.cn

JS:   class Admin extends User {}
来源：http://hhy.jqgfzy.top

TS:   class Admin extends User {}
来源：http://ohd.sxryk.cn

Java: class Admin extends User {}
来源：http://rvo.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ofx.gogol.net.cn

Ruby: class Admin < User; end
来源：http://xrc.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://mrn.fehbvm.com

[G06] 重写方法
来源：http://liv.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://wwn.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nov.hammf.cn

JS:   greet() { return "admin"; }
来源：http://zux.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://vaz.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://pin.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rhq.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://vmi.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://rpg.hammf.cn

[G07] 调用父类方法
来源：http://jqt.dashuyun.cn

Py:   super().greet()
来源：http://epy.hesvh.cn

PHP:  parent::greet();
来源：http://toi.jianghu66.top

JS:   super.greet();
来源：http://eqq.daria6918.cn

TS:   super.greet();
来源：http://myv.zdbjq.cn

Java: super.greet();
来源：http://hyj.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nvf.aizwys.cn

Ruby: super
来源：http://ncl.aizwys.cn

C#:   base.Greet();
来源：http://zuj.jyoumei.cn

[G08] 静态方法与属性
来源：http://xup.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ycs.ybcxt.top

PHP:  public static function f() {}
来源：http://ckz.zhixingplan.top

JS:   static f() {}
来源：http://iyc.gotoacloud.top

TS:   static f(): void {}
来源：http://thn.jqgufenzy.top

Java: static void f() {}
来源：http://jpc.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fbo.tian-w.cn

Ruby: def self.f; end
来源：http://jje.wangdashe.top

C#:   public static void F() {}
来源：http://vno.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://yym.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://sai.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://cct.bjfxy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tid.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://dxw.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://xan.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://bkq.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sza.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://kfr.uphjek.com

[G10] 访问控制
来源：http://ils.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://baj.zhiwuduotai.top

PHP:  public / protected / private
来源：http://iji.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://erd.jyoumei.cn

TS:   public / protected / private
来源：http://qrr.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://ute.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://avn.chenzaomai.com

Ruby: public / protected / private
来源：http://kvj.jiagoushi.top

C#:   public / protected / private / internal
来源：http://edw.chenjidiqi.icu

[G11] getter / setter
来源：http://igx.yvedp.cn

Py:   @property 与 @x.setter
来源：http://fng.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://apc.xziqi.cn

JS:   get name() { return this._name; }
来源：http://jio.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://pgx.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://ajs.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tma.xuanzx.com

Ruby: attr_accessor :name
来源：http://rkl.sysykeji.top

C#:   public string Name { get; set; }
来源：http://msa.gaohongyu789.top

[G12] 对象转字符串
来源：http://dmh.yongpay.top

Py:   def __str__(self): return self.name
来源：http://tbm.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://vsd.hesvh.cn

JS:   toString() { return this.name; }
来源：http://lmp.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://wae.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://ntx.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://ecm.yvedp.cn

Ruby: def to_s; @name; end
来源：http://rkp.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://liy.zhixingplan.top

[G13] 判断对象类型
来源：http://rex.birdmap.top

Py:   isinstance(u, User)
来源：http://noi.gogol.net.cn

PHP:  $u instanceof User
来源：http://bpp.ydjk.org.cn

JS:   u instanceof User
来源：http://yng.yangfankeji.com

TS:   u instanceof User
来源：http://ipc.hesvh.cn

Java: u instanceof User
来源：http://xog.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fqk.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://anm.sufxvd.cn

C#:   u is User
来源：http://pue.uphjek.com


<!-- 参考信息 -->