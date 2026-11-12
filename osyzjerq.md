代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fwx.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hvc.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vtt.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://izg.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ckf.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://prl.fktsv.cn

[E16] 数字千分位
来源：http://ccj.gzhubu.top

Py:   f"{1234567:,}"
来源：http://iqv.zycfv.cn

PHP:  number_format(1234567);
来源：http://uve.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ksb.jqgfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mox.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xjc.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vii.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ejq.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://una.fzhhl.top

[E17] 首字母大写
来源：http://asu.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jfw.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://smh.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://njj.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fzg.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vqy.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mec.snrcjt.cn

Ruby: s.capitalize
来源：http://bni.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://txz.0kj1m.cn

[E18] 模板占位符替换
来源：http://gat.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://giz.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kgy.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bbl.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nro.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ltv.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://akz.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uov.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fsq.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://nad.xuanzx.com

Py:   s.splitlines()
来源：http://qqk.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qiv.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://vdi.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://umg.shangyingyoupin.top

Java: s.lines().toList()
来源：http://yzs.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://uga.yvedp.cn

Ruby: s.lines
来源：http://tij.guowangkeji.top

C#:   s.Split('\n')
来源：http://qsm.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://jpq.yonumen.top

Py:   if not s:
来源：http://bpt.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tok.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iwf.yangfankeji.com

TS:   if (s === "") {}
来源：http://qtm.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://mjh.sufxvd.cn

Go:   if s == "" {}
来源：http://cnw.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://esx.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://abq.zdbjq.cn

[E21] 超长截断加省略号
来源：http://tjz.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cif.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rox.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lpc.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhk.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hnm.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://qiq.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ray.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bqk.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://fcx.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ddv.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bbj.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dju.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bgw.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jqq.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sfq.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://ypx.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yew.chenzaomai.com

================================================================================
来源：http://nko.yangfankeji.com

F. 文件与目录
来源：http://eoe.ppjwa.cn

================================================================================
来源：http://yjo.ppjwa.cn

[F01] 读取整个文件
来源：http://tqb.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://auo.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://duq.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://voh.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ugj.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bsg.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://roc.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://aep.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://gus.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://urv.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uxk.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qic.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cwx.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzb.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jky.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sur.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sbq.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ahe.havefunace.top

[F03] 写入文件（覆盖）
来源：http://mtt.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bul.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gnt.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fhm.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pyb.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aqw.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://geu.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://zsq.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xlv.quarkkingdee.top

[F04] 追加写入文件
来源：http://jqy.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lqh.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mgf.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dvs.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mht.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://boo.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rme.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xlx.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qym.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://kdn.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sse.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://fip.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://wqb.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://iig.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jjp.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cyb.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://fhe.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://kyo.yj20258.top

[F06] 删除文件
来源：http://zxh.andypj.xyz

Py:   os.remove("a.txt")
来源：http://qmz.gzhubu.top

PHP:  unlink("a.txt");
来源：http://hak.cashguo.top

JS:   fs.unlinkSync("a.txt")
来源：http://bof.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://afs.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gfo.yj20258.top

Go:   os.Remove("a.txt")
来源：http://imz.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://fab.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://voz.yj20258.top

[F07] 创建目录（含多级）
来源：http://ztv.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hdu.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jom.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wtm.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aex.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xhg.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cra.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lsk.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mpr.hongshengwenyu.top

[F08] 遍历目录
来源：http://fhv.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zqu.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jvy.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://dsj.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://jsw.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dvo.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bfj.tian-w.cn

Ruby: Dir.children("dir")
来源：http://gir.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://coh.hammf.cn

[F09] 获取文件大小
来源：http://yyo.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://jvz.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://ilk.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://ugf.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://shu.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ltn.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tif.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://skf.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://uyh.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://cpl.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vbo.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dmd.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yso.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://dbv.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zvn.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wmn.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wkf.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ikm.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://zps.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fre.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mqy.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ihg.fengsongda.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wiq.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ric.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kvx.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bfp.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://swl.birdmap.top

[F12] CSV 读写
来源：http://zew.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lom.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://onk.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijt.ydzc1.top

TS:   // 同上
来源：http://evo.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://amx.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eyg.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hqq.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://moe.ppjwa.cn

================================================================================
来源：http://qyd.quarkkingdee.top

G. 面向对象
来源：http://gwc.smart0.xyz

================================================================================
来源：http://ofm.9152youxi.cn

[G01] 定义类
来源：http://ffr.sweek.top

Py:   class User: pass
来源：http://zfp.hysaishi.cn

PHP:  class User {}
来源：http://edo.vqdsnc.cn

JS:   class User {}
来源：http://duc.havefunace.top

TS:   class User { name: string = ""; }
来源：http://zkn.hywenlv.cn

Java: class User {}
来源：http://efc.aibaodan.cn

Go:   type User struct { Name string }
来源：http://tty.hfpthk.cn

Ruby: class User; end
来源：http://nne.yanxiufei.cn

C#:   class User {}
来源：http://uhq.jqgufenzy.top

[G02] 构造函数
来源：http://qvv.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://vsg.wangshuangyany.cn

PHP:  public function __construct(public string $name) {}
来源：http://szl.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://zwl.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://toc.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://yoa.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ukp.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://kwi.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://ymt.epnwcf.com

[G03] 实例属性
来源：http://sgc.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://qbm.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://tiq.aibaodan.cn

JS:   this.name = "x";
来源：http://yxp.chenjidiqi.icu

TS:   name: string = "x";
来源：http://fxl.snrcjt.cn

Java: private String name;
来源：http://wde.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sjq.vqdsnc.cn

Ruby: @name = "x"
来源：http://zgl.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://icw.chenzaomai.com

[G04] 定义方法
来源：http://mmx.tanke756.top

Py:   def greet(self): return self.name
来源：http://ars.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fuu.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://rto.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://bvu.tianlin.xyz

Java: String greet() { return name; }
来源：http://koe.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mcx.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://fsp.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://rxk.gzhubu.top

[G05] 继承
来源：http://xwm.hnqzz.top

Py:   class Admin(User): pass
来源：http://djv.uphjek.com

PHP:  class Admin extends User {}
来源：http://qah.0kj1m.cn

JS:   class Admin extends User {}
来源：http://swg.316326.xyz

TS:   class Admin extends User {}
来源：http://kyl.snrcjt.cn

Java: class Admin extends User {}
来源：http://nfz.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rsu.ydzc1.top

Ruby: class Admin < User; end
来源：http://ajv.shzxlz.cn

C#:   class Admin : User {}
来源：http://hor.ppjwa.cn

[G06] 重写方法
来源：http://bvr.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://anc.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qpf.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://dvk.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://czt.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://jan.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sws.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://kjs.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://mir.hnqzz.top

[G07] 调用父类方法
来源：http://qlz.zhongyouzk.top

Py:   super().greet()
来源：http://uuh.dashuyun.cn

PHP:  parent::greet();
来源：http://jcw.zhaomingkeji.xyz

JS:   super.greet();
来源：http://eby.sweek.top

TS:   super.greet();
来源：http://iev.sysykeji.top

Java: super.greet();
来源：http://xio.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uft.yj20258.top

Ruby: super
来源：http://vag.shangyingyoupin.top

C#:   base.Greet();
来源：http://gxh.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://ugu.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vif.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://fpy.ivvv.top

JS:   static f() {}
来源：http://lhw.yuxming.cn

TS:   static f(): void {}
来源：http://jif.sysykeji.top

Java: static void f() {}
来源：http://pbh.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://joi.hcnkem.com

Ruby: def self.f; end
来源：http://anr.snrcjt.cn

C#:   public static void F() {}
来源：http://mef.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://sfu.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://lmr.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://rtz.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xkp.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://iru.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://pio.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://dyv.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sts.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://vwv.jqgufenzy.top

[G10] 访问控制
来源：http://wlw.ybcxt.top

Py:   约定 _protected / __private（不强制）
来源：http://pzc.mhx1999.top

PHP:  public / protected / private
来源：http://tmj.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://ksl.yuxming.cn

TS:   public / protected / private
来源：http://nea.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://fht.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://nbq.pycfn.com

Ruby: public / protected / private
来源：http://tai.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://cor.fanxiaobao.xyz

[G11] getter / setter
来源：http://hka.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://wum.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rtm.nwbrower.top

JS:   get name() { return this._name; }
来源：http://sjc.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://rzu.ehwqpu.com

Java: public String getName() { return name; }
来源：http://ebb.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://plv.sysykeji.top

Ruby: attr_accessor :name
来源：http://eui.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://vhf.ybcxt.top

[G12] 对象转字符串
来源：http://sjg.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://gov.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jjv.pycfn.com

JS:   toString() { return this.name; }
来源：http://crj.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://nzh.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://okh.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://thz.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://eic.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://rda.yj20258888.top

[G13] 判断对象类型
来源：http://wif.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://zae.sufxvd.cn

PHP:  $u instanceof User
来源：http://yoq.shanyushiyangtech.top

JS:   u instanceof User
来源：http://nww.havefunace.top

TS:   u instanceof User
来源：http://bps.guowangkeji.top

Java: u instanceof User
来源：http://ops.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://klx.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://hsb.gzhubu.top

C#:   u is User
来源：http://lyf.bjfxy.top


<!-- 参考信息 -->