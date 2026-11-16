代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nbm.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fzy.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hvd.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://axb.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hbb.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ltr.kuanghao11.cn

[E16] 数字千分位
来源：http://wev.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://fnb.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://mhr.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qhx.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cpp.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kzt.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://laa.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ehq.meibo888.top

C#:   1234567.ToString("N0")
来源：http://qqz.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://ggv.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bwj.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pvd.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://irr.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxr.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gjz.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yoo.sufxvd.cn

Ruby: s.capitalize
来源：http://puc.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://frq.ydjk.org.cn

[E18] 模板占位符替换
来源：http://vxb.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hhd.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wxy.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tun.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zcl.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nyx.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qas.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jyn.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gzc.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://eop.ydjk.org.cn

Py:   s.splitlines()
来源：http://nqm.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jfl.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://uec.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://fjm.xuetiantiany.cn

Java: s.lines().toList()
来源：http://jwf.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://lgk.gotoacloud.top

Ruby: s.lines
来源：http://pae.sjlbkw.cn

C#:   s.Split('\n')
来源：http://rjq.fengsongda.top

[E20] 判断字符串是否为空
来源：http://moq.9152youxi.cn

Py:   if not s:
来源：http://dgm.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cba.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nsa.yangfankeji.com

TS:   if (s === "") {}
来源：http://jzd.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://oca.aizwys.cn

Go:   if s == "" {}
来源：http://ozz.sxryk.cn

Ruby: if s.empty?
来源：http://fzv.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wgx.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://pqt.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vzu.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oew.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oqi.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckt.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mhh.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://sut.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xot.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rdf.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://jak.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cuj.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wjy.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yaw.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bmg.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cay.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ewm.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://nhu.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rmv.cucudq.cn

================================================================================
来源：http://fue.shangyingyoupin.top

F. 文件与目录
来源：http://pbq.daxiang520.top

================================================================================
来源：http://zgy.zdbjq.cn

[F01] 读取整个文件
来源：http://qiy.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rtz.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://wlp.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rgb.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://toe.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uta.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fll.nwbrower.top

Ruby: File.read("a.txt")
来源：http://mno.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://sxy.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://ycn.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qqi.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qqq.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgh.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kqd.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://irq.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wzk.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ejc.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ejq.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://cea.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxf.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gqt.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tll.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://drl.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://spe.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tqv.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://zhx.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://src.yanxiufei.cn

[F04] 追加写入文件
来源：http://dug.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qdh.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://agd.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tsm.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bzk.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ngc.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://agq.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ujn.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ror.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://kyb.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bnt.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://lsv.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://rqz.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://xzf.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jgw.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://orp.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://xrn.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://axc.sjlbkw.cn

[F06] 删除文件
来源：http://mfg.yuxming.cn

Py:   os.remove("a.txt")
来源：http://tks.shuidangran.top

PHP:  unlink("a.txt");
来源：http://mqk.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://mhd.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://xru.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yvr.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://wfm.pycfn.com

Ruby: File.delete("a.txt")
来源：http://gjf.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://mlt.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://ouj.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sxj.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nqw.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blt.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ehy.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ujv.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pjg.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rgl.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ndp.cdnleiting.top

[F08] 遍历目录
来源：http://bcz.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qbd.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kau.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://zdw.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://cyz.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eap.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dlv.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://cyr.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://wsx.ehwqpu.com

[F09] 获取文件大小
来源：http://pqv.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://rgq.sweek.top

PHP:  filesize("a.txt");
来源：http://oei.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://coy.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://bwl.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rno.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vov.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://apd.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ome.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://fxc.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zwh.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jpo.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ejx.yueranfly.top

TS:   path.extname("a.txt")
来源：http://nsc.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cxn.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sai.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hxi.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bbs.ydzc1.top

[F11] 复制与移动文件
来源：http://ovg.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nge.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjt.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbd.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://krk.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qvs.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://adc.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://awu.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blw.aizwys.cn

[F12] CSV 读写
来源：http://pso.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gan.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ejx.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ife.ybcxt.top

TS:   // 同上
来源：http://yww.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ibi.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zrt.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://has.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zda.sufxvd.cn

================================================================================
来源：http://uwe.tian-w.cn

G. 面向对象
来源：http://qgp.jinqigfzy.top

================================================================================
来源：http://sma.jlsjyb.cn

[G01] 定义类
来源：http://feq.uphjek.com

Py:   class User: pass
来源：http://lxs.fanxiaobao.xyz

PHP:  class User {}
来源：http://ree.andypj.xyz

JS:   class User {}
来源：http://uoa.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://ydd.ybcxt.top

Java: class User {}
来源：http://otf.aizwys.cn

Go:   type User struct { Name string }
来源：http://udg.xinyue.icu

Ruby: class User; end
来源：http://dcv.wangdashe.top

C#:   class User {}
来源：http://nsl.fengsongda.top

[G02] 构造函数
来源：http://zfz.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://cib.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://tft.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://jsd.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://zpp.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://kir.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://guc.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://qkw.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://cty.zycfv.cn

[G03] 实例属性
来源：http://dqs.aibaodan.cn

Py:   self.name = "x"
来源：http://kfo.birdmap.top

PHP:  public string $name = "x";
来源：http://til.cdnleiting.top

JS:   this.name = "x";
来源：http://pwd.zhixingplan.top

TS:   name: string = "x";
来源：http://msl.nwbrower.top

Java: private String name;
来源：http://lba.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dca.hesvh.cn

Ruby: @name = "x"
来源：http://bgs.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://hdd.ydjk.org.cn

[G04] 定义方法
来源：http://xfk.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://suz.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://unn.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://tzt.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://xbp.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://dnh.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gaw.yvedp.cn

Ruby: def greet; @name; end
来源：http://spn.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://tek.zdbjq.cn

[G05] 继承
来源：http://xpj.pycfn.com

Py:   class Admin(User): pass
来源：http://zyx.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://nly.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://pad.ppjwa.cn

TS:   class Admin extends User {}
来源：http://wkj.quarkkingdee.top

Java: class Admin extends User {}
来源：http://vvj.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oyu.xziqi.cn

Ruby: class Admin < User; end
来源：http://hnq.yueranfly.top

C#:   class Admin : User {}
来源：http://gqs.tanke756.top

[G06] 重写方法
来源：http://uyu.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://gka.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qfs.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://nuv.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://kmu.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://xso.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nxl.tarul.cn

Ruby: def greet; "admin"; end
来源：http://blj.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://cgn.nanxinkj.top

[G07] 调用父类方法
来源：http://alx.nanxuanxn.top

Py:   super().greet()
来源：http://hob.c1oappe.top

PHP:  parent::greet();
来源：http://pmg.xuetiantiany.cn

JS:   super.greet();
来源：http://laq.cashguo.top

TS:   super.greet();
来源：http://xbt.yangfankeji.com

Java: super.greet();
来源：http://put.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ypn.sufxvd.cn

Ruby: super
来源：http://uwd.cheryme.top

C#:   base.Greet();
来源：http://gfx.cqqwz.cn

[G08] 静态方法与属性
来源：http://sek.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cvd.bbcook.cn

PHP:  public static function f() {}
来源：http://svq.hongshengwenyu.top

JS:   static f() {}
来源：http://xva.jyoumei.cn

TS:   static f(): void {}
来源：http://oba.ctjpmb.com

Java: static void f() {}
来源：http://fhl.bbcook.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qzi.sysykeji.top

Ruby: def self.f; end
来源：http://mph.cucudq.cn

C#:   public static void F() {}
来源：http://fpm.tarul.cn

[G09] 接口 / 抽象类
来源：http://osf.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://sae.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iel.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qla.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://ubv.yueranfly.top

Java: interface Shape { double area(); }
来源：http://oak.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://gcv.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nyb.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://oik.aizwys.cn

[G10] 访问控制
来源：http://jvc.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://juu.jinqigfzy.top

PHP:  public / protected / private
来源：http://yns.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://sif.fengsongda.top

TS:   public / protected / private
来源：http://jng.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://buw.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://okh.shuidangran.top

Ruby: public / protected / private
来源：http://pya.9152youxi.cn

C#:   public / protected / private / internal
来源：http://vco.cqqwz.cn

[G11] getter / setter
来源：http://czi.tarul.cn

Py:   @property 与 @x.setter
来源：http://gis.hfpthk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gut.guannengcc.top

JS:   get name() { return this._name; }
来源：http://cmt.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://ads.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://osr.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://aet.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://pfk.pycfn.com

C#:   public string Name { get; set; }
来源：http://suc.yangfankeji.com

[G12] 对象转字符串
来源：http://iqg.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://fzw.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://fzz.hcnkem.com

JS:   toString() { return this.name; }
来源：http://lme.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://xww.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://bsh.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://gut.hnqzz.top

Ruby: def to_s; @name; end
来源：http://rsi.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://moa.ctjpmb.com

[G13] 判断对象类型
来源：http://lph.snrcjt.cn

Py:   isinstance(u, User)
来源：http://pth.hywenlv.cn

PHP:  $u instanceof User
来源：http://vfy.bbcook.cn

JS:   u instanceof User
来源：http://pvx.nwbrower.top

TS:   u instanceof User
来源：http://nhe.chenzaomai.com

Java: u instanceof User
来源：http://qzw.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lpp.gzhubu.top

Ruby: u.is_a?(User)
来源：http://laj.yanxiufei.cn

C#:   u is User
来源：http://esw.yuanzhike.top


<!-- 参考信息 -->