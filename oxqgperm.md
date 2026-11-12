代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gwq.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://dhi.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uzv.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://god.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dli.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qul.vehdjk.com

[E16] 数字千分位
来源：http://mto.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://qpc.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://ngl.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uzu.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dci.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tlg.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjr.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gjm.havefunace.top

C#:   1234567.ToString("N0")
来源：http://nxf.hongshengwenyu.top

[E17] 首字母大写
来源：http://sde.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hiy.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://moc.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rby.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://juf.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hup.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xon.cashguo.top

Ruby: s.capitalize
来源：http://rav.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ike.uphjek.com

[E18] 模板占位符替换
来源：http://irk.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fsg.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yko.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://edk.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uqi.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oqx.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nyo.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ukc.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://byy.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://pwz.hysaishi.cn

Py:   s.splitlines()
来源：http://jdj.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eis.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://vna.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://cko.daria6918.cn

Java: s.lines().toList()
来源：http://rwp.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://bbp.sysykeji.top

Ruby: s.lines
来源：http://jnj.wangdashe.top

C#:   s.Split('\n')
来源：http://mex.yfazqb.com

[E20] 判断字符串是否为空
来源：http://uvy.sweek.top

Py:   if not s:
来源：http://trl.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pjd.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cfp.xinyue.icu

TS:   if (s === "") {}
来源：http://oxp.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://jhs.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://xyh.zhiwuduotai.top

Ruby: if s.empty?
来源：http://vas.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ksq.zdbjq.cn

[E21] 超长截断加省略号
来源：http://cmt.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vjv.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vol.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rxs.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ces.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zhw.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://gnq.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nzp.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bmm.shzxlz.cn

[E22] 字节长度与字符长度
来源：http://pri.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzc.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mks.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mmz.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://url.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hbl.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rdk.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://jbn.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cjp.bbcook.cn

================================================================================
来源：http://hkn.yfazqb.com

F. 文件与目录
来源：http://hek.epnwcf.com

================================================================================
来源：http://bqo.sweek.top

[F01] 读取整个文件
来源：http://imj.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ppf.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://kwm.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qid.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://shd.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pok.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://njk.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://jny.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://vwm.sjlbkw.cn

[F02] 逐行读取文件
来源：http://owk.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://acv.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://llo.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ubh.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cgu.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lrn.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bsi.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lcn.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zhs.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://kdc.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bqq.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xip.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vvn.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wsw.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://amn.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ayu.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://kfo.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwm.fktsv.cn

[F04] 追加写入文件
来源：http://kal.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iov.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vqz.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lyp.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bts.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vao.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jch.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://stw.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ban.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://kwb.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aun.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://vas.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://fsp.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://xcc.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zks.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ggq.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://shd.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://shq.zycfv.cn

[F06] 删除文件
来源：http://vvh.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://buo.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://fgs.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://lyk.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://wmr.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mcu.yj202588.top

Go:   os.Remove("a.txt")
来源：http://sos.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://fhu.pycfn.com

C#:   File.Delete("a.txt");
来源：http://brk.vehdjk.com

[F07] 创建目录（含多级）
来源：http://atd.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://brk.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pkr.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sek.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uou.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hng.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zmb.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ssf.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xnn.hammf.cn

[F08] 遍历目录
来源：http://nyq.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://xlf.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iki.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://exs.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://flx.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wec.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://flq.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://uwx.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://iyr.snrcjt.cn

[F09] 获取文件大小
来源：http://yyp.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://zbp.zycfv.cn

PHP:  filesize("a.txt");
来源：http://wpg.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://cal.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://fqf.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://gmb.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fbd.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://xrp.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://zjb.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://pwc.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oyt.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mjk.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zqn.daria6918.cn

TS:   path.extname("a.txt")
来源：http://xmx.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ojp.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://anu.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wlc.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dbx.vehdjk.com

[F11] 复制与移动文件
来源：http://qde.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mml.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pai.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bbv.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://akq.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xry.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ykv.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://avq.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hfo.hfpthk.cn

[F12] CSV 读写
来源：http://wku.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gqz.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iyw.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nks.shzxlz.cn

TS:   // 同上
来源：http://kii.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mnf.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lkb.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vfb.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://snm.jlsjyb.cn

================================================================================
来源：http://xaa.tianlin.xyz

G. 面向对象
来源：http://ndj.shangyingyoupin.top

================================================================================
来源：http://aaa.birdmap.top

[G01] 定义类
来源：http://who.shanyushiyangkeji.top

Py:   class User: pass
来源：http://zva.zdbjq.cn

PHP:  class User {}
来源：http://hkh.cdnleiting.top

JS:   class User {}
来源：http://mjm.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://rzo.quarkkingdee.top

Java: class User {}
来源：http://eco.aizwys.cn

Go:   type User struct { Name string }
来源：http://zfl.9152youxi.cn

Ruby: class User; end
来源：http://owz.xuanzx.com

C#:   class User {}
来源：http://qqc.c1oappe.top

[G02] 构造函数
来源：http://nfr.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://qfl.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://zjh.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://yqk.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://her.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://jcx.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qil.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://zol.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://ziw.quarkkingdee.top

[G03] 实例属性
来源：http://lgv.aibaodan.cn

Py:   self.name = "x"
来源：http://nsh.aibaodan.cn

PHP:  public string $name = "x";
来源：http://ivo.0kj1m.cn

JS:   this.name = "x";
来源：http://jts.sysykeji.top

TS:   name: string = "x";
来源：http://fdv.chenjidiqi.icu

Java: private String name;
来源：http://xpc.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pge.cdnleiting.top

Ruby: @name = "x"
来源：http://pun.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://luu.yueranfly.top

[G04] 定义方法
来源：http://rkt.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://wan.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sll.daxiang520.top

JS:   greet() { return this.name; }
来源：http://fpc.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://ppz.9152youxi.cn

Java: String greet() { return name; }
来源：http://yms.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gxq.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://etc.xylfe.cn

C#:   public string Greet() => Name;
来源：http://ooj.epnwcf.com

[G05] 继承
来源：http://suo.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://apr.shuidangran.top

PHP:  class Admin extends User {}
来源：http://gwb.cdnleiting.top

JS:   class Admin extends User {}
来源：http://vio.daxiang520.top

TS:   class Admin extends User {}
来源：http://qog.jlsjyb.cn

Java: class Admin extends User {}
来源：http://xog.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tdf.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://cai.hfpthk.cn

C#:   class Admin : User {}
来源：http://blf.yfazqb.com

[G06] 重写方法
来源：http://tfs.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://fks.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://shz.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://nlf.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://yod.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://hsn.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rzc.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://fqi.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://crh.aizwys.cn

[G07] 调用父类方法
来源：http://tmx.shanyushiyangkeji.top

Py:   super().greet()
来源：http://psf.xylfe.cn

PHP:  parent::greet();
来源：http://qfd.zhijiandao.cn

JS:   super.greet();
来源：http://oyj.pycfn.com

TS:   super.greet();
来源：http://phq.havefunace.top

Java: super.greet();
来源：http://hks.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://caq.fktsv.cn

Ruby: super
来源：http://lfw.hammf.cn

C#:   base.Greet();
来源：http://gim.haohaochexian.top

[G08] 静态方法与属性
来源：http://qnr.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mqb.52xcode.cn

PHP:  public static function f() {}
来源：http://ait.cdnleiting.top

JS:   static f() {}
来源：http://svq.snrcjt.cn

TS:   static f(): void {}
来源：http://xkz.shanyushiyangtech.top

Java: static void f() {}
来源：http://ozr.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uek.feifeiyinyue.top

Ruby: def self.f; end
来源：http://auc.kuanghao11.cn

C#:   public static void F() {}
来源：http://oer.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://bsk.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://twd.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://cmx.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://geb.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://dxg.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://spe.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://lqk.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zzf.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://pai.ydjk.org.cn

[G10] 访问控制
来源：http://smu.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://qud.ivvv.top

PHP:  public / protected / private
来源：http://dvj.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://hcy.nanxuanxn.top

TS:   public / protected / private
来源：http://udo.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://fjo.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qcq.hfpthk.cn

Ruby: public / protected / private
来源：http://rch.vehdjk.com

C#:   public / protected / private / internal
来源：http://zac.wangdashe.top

[G11] getter / setter
来源：http://spn.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://uox.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ugv.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://ork.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://osv.daxiang520.top

Java: public String getName() { return name; }
来源：http://ksv.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fcg.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://klu.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://ahq.wangshuangyany.cn

[G12] 对象转字符串
来源：http://nqv.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://xdo.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cap.cashguo.top

JS:   toString() { return this.name; }
来源：http://cez.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://bdy.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://rjc.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ljj.c1oappe.top

Ruby: def to_s; @name; end
来源：http://cku.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://edh.jiagoushi.top

[G13] 判断对象类型
来源：http://cln.sweek.top

Py:   isinstance(u, User)
来源：http://ysh.tarul.cn

PHP:  $u instanceof User
来源：http://iun.svipenyu.cn

JS:   u instanceof User
来源：http://ifm.chenlongwang.top

TS:   u instanceof User
来源：http://cfd.fzhhl.top

Java: u instanceof User
来源：http://zrt.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sxd.cheryme.top

Ruby: u.is_a?(User)
来源：http://npq.gzhubu.top

C#:   u is User
来源：http://tne.fktsv.cn


<!-- 参考信息 -->