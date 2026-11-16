代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hgg.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ryb.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tuw.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pwb.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pse.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kuz.redwolf501.top

[E16] 数字千分位
来源：http://kbo.meibo888.top

Py:   f"{1234567:,}"
来源：http://wap.jianghu66.top

PHP:  number_format(1234567);
来源：http://cdn.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rsg.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mwf.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wiq.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://esl.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pqx.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://rlp.52xcode.cn

[E17] 首字母大写
来源：http://mek.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://frv.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eqx.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ygf.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lnb.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nxk.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zsd.ydzc1.top

Ruby: s.capitalize
来源：http://lkl.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wzb.yj20258.top

[E18] 模板占位符替换
来源：http://eut.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gys.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://grn.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://apx.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://osy.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ydd.hongshengwenyu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lsf.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uns.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ewg.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://fja.uphjek.com

Py:   s.splitlines()
来源：http://yeh.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://svg.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://wtn.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://lmu.yanxiufei.cn

Java: s.lines().toList()
来源：http://ibu.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://vvy.jianghu66.top

Ruby: s.lines
来源：http://xfc.yj20258.top

C#:   s.Split('\n')
来源：http://lrb.hammf.cn

[E20] 判断字符串是否为空
来源：http://mks.sjlbkw.cn

Py:   if not s:
来源：http://iis.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pjq.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kkk.ydjk.org.cn

TS:   if (s === "") {}
来源：http://ziv.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://uxx.tian-w.cn

Go:   if s == "" {}
来源：http://obw.ivvv.top

Ruby: if s.empty?
来源：http://api.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gel.shzxlz.cn

[E21] 超长截断加省略号
来源：http://qvw.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xbd.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ymz.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkg.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbs.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rtd.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://rsb.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nbg.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zwj.nwbrower.top

[E22] 字节长度与字符长度
来源：http://lvp.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kuv.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ytv.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xso.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhc.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rte.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mmi.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://aoi.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rlk.ydzc1.top

================================================================================
来源：http://vab.sjlbkw.cn

F. 文件与目录
来源：http://rsh.ehwqpu.com

================================================================================
来源：http://iju.xuetiantiany.cn

[F01] 读取整个文件
来源：http://ddn.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qcf.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://xjn.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ffu.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dnt.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jdc.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lue.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://bel.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://gut.andypj.xyz

[F02] 逐行读取文件
来源：http://wls.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mob.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://usz.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awv.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uta.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sqb.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xzg.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dcj.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vhe.meibo888.top

[F03] 写入文件（覆盖）
来源：http://lpx.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vur.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://seh.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffz.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqo.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sps.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fba.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://ukw.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tof.zhiwuduotai.top

[F04] 追加写入文件
来源：http://mfo.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mgz.0kj1m.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tsr.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://alt.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ddx.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yxr.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://prx.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hru.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://atw.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://uhn.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xje.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://zod.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://cmt.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://bex.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dmc.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nic.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://frs.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://bme.andypj.xyz

[F06] 删除文件
来源：http://cec.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://mmi.epnwcf.com

PHP:  unlink("a.txt");
来源：http://yrz.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://omv.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://bik.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mzq.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://nmy.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://pto.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://tyk.tarul.cn

[F07] 创建目录（含多级）
来源：http://isc.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://puu.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tmp.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hyv.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ajz.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uqy.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qdr.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aay.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://osh.andypj.xyz

[F08] 遍历目录
来源：http://tep.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yzt.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rci.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://ycz.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://jjz.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vwf.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://umr.cucudq.cn

Ruby: Dir.children("dir")
来源：http://zzm.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://xrv.pengpengdd.cyou

[F09] 获取文件大小
来源：http://oro.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://okg.shuidangran.top

PHP:  filesize("a.txt");
来源：http://vfu.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://owu.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://fsu.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://ixg.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fkl.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://aeb.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://kfl.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://sww.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uep.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xde.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gzp.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://eek.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xzy.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mcz.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ynj.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dnc.zhoulong.xyz

[F11] 复制与移动文件
来源：http://haj.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nco.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vuy.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hur.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mhq.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mhh.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ueh.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nji.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jxa.hnxiangtu.top

[F12] CSV 读写
来源：http://lbq.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zfi.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tkl.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qum.cqqwz.cn

TS:   // 同上
来源：http://zxu.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sgm.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vfq.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://prc.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fms.ehwqpu.com

================================================================================
来源：http://rsn.jianghu66.top

G. 面向对象
来源：http://kmy.nwbrower.top

================================================================================
来源：http://wln.yonumen.top

[G01] 定义类
来源：http://yzi.zdbjq.cn

Py:   class User: pass
来源：http://rqd.daxiang520.top

PHP:  class User {}
来源：http://vfz.gzhubu.top

JS:   class User {}
来源：http://yvv.yongpay.top

TS:   class User { name: string = ""; }
来源：http://adn.kuanghao11.cn

Java: class User {}
来源：http://mmf.hywenlv.cn

Go:   type User struct { Name string }
来源：http://dta.hnxiangtu.top

Ruby: class User; end
来源：http://byi.316326.xyz

C#:   class User {}
来源：http://uut.shangyingyoupin.top

[G02] 构造函数
来源：http://twx.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://ooo.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://biu.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://xjf.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://rez.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://wev.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ppr.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://eyb.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://aea.pycfn.com

[G03] 实例属性
来源：http://wqs.cqqwz.cn

Py:   self.name = "x"
来源：http://cdl.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://cee.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://fjy.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://tqi.hcnkem.com

Java: private String name;
来源：http://pqq.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yuw.yanxiufei.cn

Ruby: @name = "x"
来源：http://ibz.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://jez.fzhhl.top

[G04] 定义方法
来源：http://rjs.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://gvv.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ygb.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://qdh.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://oqb.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://gbv.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://zjj.gogol.net.cn

Ruby: def greet; @name; end
来源：http://wls.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://uxq.aibaodan.cn

[G05] 继承
来源：http://bkm.uphjek.com

Py:   class Admin(User): pass
来源：http://bav.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://ibb.snrcjt.cn

JS:   class Admin extends User {}
来源：http://cau.guowangkeji.top

TS:   class Admin extends User {}
来源：http://nye.epnwcf.com

Java: class Admin extends User {}
来源：http://rfd.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ouf.xylfe.cn

Ruby: class Admin < User; end
来源：http://bil.0kj1m.cn

C#:   class Admin : User {}
来源：http://lzz.hfpthk.cn

[G06] 重写方法
来源：http://iys.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://gae.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://whr.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://kdn.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://uam.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://gbw.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ywq.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://vfe.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://rlf.yongpay.top

[G07] 调用父类方法
来源：http://byh.jyoumei.cn

Py:   super().greet()
来源：http://oog.tarul.cn

PHP:  parent::greet();
来源：http://njc.dashuyun.cn

JS:   super.greet();
来源：http://aam.feifeiyinyue.top

TS:   super.greet();
来源：http://sks.aizwys.cn

Java: super.greet();
来源：http://ltq.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kvg.sysykeji.top

Ruby: super
来源：http://jbe.cashguo.top

C#:   base.Greet();
来源：http://tmo.nanxinkj.top

[G08] 静态方法与属性
来源：http://mey.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jht.nanxuanxn.top

PHP:  public static function f() {}
来源：http://kzy.fehbvm.com

JS:   static f() {}
来源：http://rfk.zdqjudy.top

TS:   static f(): void {}
来源：http://ezb.yueranfly.top

Java: static void f() {}
来源：http://ven.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bnc.guowangkeji.top

Ruby: def self.f; end
来源：http://qck.yongpay.top

C#:   public static void F() {}
来源：http://dup.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://ymt.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://lic.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://lbv.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cvw.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://hmn.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://jbg.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://asl.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kti.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://ilf.shzxlz.cn

[G10] 访问控制
来源：http://ucl.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://ifm.yueranfly.top

PHP:  public / protected / private
来源：http://int.bjfxy.top

JS:   #private 字段；其余公开
来源：http://jnh.cdnleiting.top

TS:   public / protected / private
来源：http://djc.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://doh.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://iee.vqdsnc.cn

Ruby: public / protected / private
来源：http://fdn.redwolf501.top

C#:   public / protected / private / internal
来源：http://jjd.tanke756.top

[G11] getter / setter
来源：http://jcg.smart0.xyz

Py:   @property 与 @x.setter
来源：http://tyd.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://zvj.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://ear.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://dwc.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://yfh.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oen.sufxvd.cn

Ruby: attr_accessor :name
来源：http://ysx.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://iit.fzhhl.top

[G12] 对象转字符串
来源：http://mbw.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://uhw.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://fck.redwolf501.top

JS:   toString() { return this.name; }
来源：http://xzg.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://win.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://uxj.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://cag.daria6918.cn

Ruby: def to_s; @name; end
来源：http://thd.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://qyk.pengpengdd.cyou

[G13] 判断对象类型
来源：http://vpo.yongpay.top

Py:   isinstance(u, User)
来源：http://wlu.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://iez.nanxuanxn.top

JS:   u instanceof User
来源：http://fmc.fzhhl.top

TS:   u instanceof User
来源：http://ihf.dianchejie.cn

Java: u instanceof User
来源：http://lgv.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rmu.yueranfly.top

Ruby: u.is_a?(User)
来源：http://rar.havefunace.top

C#:   u is User
来源：http://zjl.ppjwa.cn


<!-- 参考信息 -->