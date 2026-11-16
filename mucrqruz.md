代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sky.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://bgc.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://awn.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ghu.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://slg.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://riw.zhongyouzk.top

[E16] 数字千分位
来源：http://rdw.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://wxz.yj20258888.top

PHP:  number_format(1234567);
来源：http://smo.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://agl.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gqs.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hdf.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://akw.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nzc.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://bzh.ydjk.org.cn

[E17] 首字母大写
来源：http://gyt.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wkl.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ppn.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mws.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cid.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oqs.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bre.gzhubu.top

Ruby: s.capitalize
来源：http://ucu.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xzl.tanke756.top

[E18] 模板占位符替换
来源：http://hyw.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zez.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dvz.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ucc.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://daj.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://omb.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lfg.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jzh.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://edx.cheryme.top

[E19] 多行文本按行拆分
来源：http://ozg.zhijiandao.cn

Py:   s.splitlines()
来源：http://ixx.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yip.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://nbo.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://qdl.xziqi.cn

Java: s.lines().toList()
来源：http://czg.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://gdf.jiagoushi.top

Ruby: s.lines
来源：http://guo.andypj.xyz

C#:   s.Split('\n')
来源：http://hbo.xuanzx.com

[E20] 判断字符串是否为空
来源：http://xao.fanxiaobao.xyz

Py:   if not s:
来源：http://xdq.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jor.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tyd.gaohongyu789.top

TS:   if (s === "") {}
来源：http://one.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://fjy.pycfn.com

Go:   if s == "" {}
来源：http://nnb.yuanzhike.top

Ruby: if s.empty?
来源：http://uhl.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wlk.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://fll.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nmg.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xxo.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rvj.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cfd.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kud.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://xoz.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sif.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://clp.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://gck.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qmu.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugp.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vhl.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://usw.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bsv.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qhc.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://mha.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vkv.ppjwa.cn

================================================================================
来源：http://zdv.wangshuangyany.cn

F. 文件与目录
来源：http://yql.chenlongwang.top

================================================================================
来源：http://uxd.gaohongyu789.top

[F01] 读取整个文件
来源：http://jyd.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ojk.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://oep.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ksq.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ijb.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bgd.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zqf.meibo888.top

Ruby: File.read("a.txt")
来源：http://tmv.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://mmn.snrcjt.cn

[F02] 逐行读取文件
来源：http://khs.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://haj.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kya.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://teo.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ofj.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fxi.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fuo.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hdx.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tab.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://uri.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://goy.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cvm.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://omc.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://agb.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://esy.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zdi.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://met.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rfa.jqgfzy.top

[F04] 追加写入文件
来源：http://see.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ogb.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ckj.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://prc.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ffd.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://znc.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xiw.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yye.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xiy.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://pek.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dpv.meibo888.top

PHP:  file_exists("a.txt");
来源：http://rih.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://bia.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://pqt.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://huy.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ntj.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://taa.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://hxn.fehbvm.com

[F06] 删除文件
来源：http://gfk.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://skw.yonumen.top

PHP:  unlink("a.txt");
来源：http://gvr.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rej.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xpa.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nzj.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://qab.meibo888.top

Ruby: File.delete("a.txt")
来源：http://snn.uphjek.com

C#:   File.Delete("a.txt");
来源：http://xib.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://kwr.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xit.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tbz.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ptw.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aet.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oaq.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://szz.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://msg.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yon.c1oappe.top

[F08] 遍历目录
来源：http://sen.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xbh.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kno.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://tyl.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://erq.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ldd.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ddw.pycfn.com

Ruby: Dir.children("dir")
来源：http://why.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://rjt.jinqigfzy.top

[F09] 获取文件大小
来源：http://vrc.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://sbf.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://amk.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://wef.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://ipj.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://tbv.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://efg.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://lhs.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://zbc.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://sap.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pkp.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rlg.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oqv.xuanzx.com

TS:   path.extname("a.txt")
来源：http://zss.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ndu.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://klq.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://llp.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ref.xuanzx.com

[F11] 复制与移动文件
来源：http://kml.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kjq.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pie.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nth.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cst.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nwy.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eob.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ivt.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://evm.ivvv.top

[F12] CSV 读写
来源：http://prz.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://arv.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ilr.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oym.yj202588.top

TS:   // 同上
来源：http://ypl.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ekd.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qpa.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pcr.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ass.xziqi.cn

================================================================================
来源：http://rkd.svipenyu.cn

G. 面向对象
来源：http://xdy.redwolf501.top

================================================================================
来源：http://war.andypj.xyz

[G01] 定义类
来源：http://lcg.fanxiaobao.xyz

Py:   class User: pass
来源：http://dzt.zhengqikj.top

PHP:  class User {}
来源：http://wku.cashguo.top

JS:   class User {}
来源：http://sji.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://mmw.ppjwa.cn

Java: class User {}
来源：http://ebc.hywenlv.cn

Go:   type User struct { Name string }
来源：http://jfh.hammf.cn

Ruby: class User; end
来源：http://eli.sweek.top

C#:   class User {}
来源：http://ewo.gzhubu.top

[G02] 构造函数
来源：http://dkp.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://cyo.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://cig.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://gdz.ivvv.top

TS:   constructor(public name: string) {}
来源：http://xkd.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://xif.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://psy.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://fyh.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://lda.shanyushiyangtech.top

[G03] 实例属性
来源：http://iaf.epnwcf.com

Py:   self.name = "x"
来源：http://mzu.pycfn.com

PHP:  public string $name = "x";
来源：http://too.haohaochexian.top

JS:   this.name = "x";
来源：http://uvt.cucudq.cn

TS:   name: string = "x";
来源：http://iuj.ybcxt.top

Java: private String name;
来源：http://srw.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fps.zhijiandao.cn

Ruby: @name = "x"
来源：http://uqf.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://lwx.zhixingplan.top

[G04] 定义方法
来源：http://qvz.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://frv.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://npm.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://jsp.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://yfm.xinyue.icu

Java: String greet() { return name; }
来源：http://xaf.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mbr.jyoumei.cn

Ruby: def greet; @name; end
来源：http://dte.tanke756.top

C#:   public string Greet() => Name;
来源：http://ipb.316326.xyz

[G05] 继承
来源：http://qxs.aizwys.cn

Py:   class Admin(User): pass
来源：http://pfk.redwolf501.top

PHP:  class Admin extends User {}
来源：http://olj.shuidangran.top

JS:   class Admin extends User {}
来源：http://nxo.zhixingplan.top

TS:   class Admin extends User {}
来源：http://vlw.kuanghao11.cn

Java: class Admin extends User {}
来源：http://wdp.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://erg.zdqjudy.top

Ruby: class Admin < User; end
来源：http://eum.shzxlz.cn

C#:   class Admin : User {}
来源：http://xlf.aizwys.cn

[G06] 重写方法
来源：http://ghv.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://tbf.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://oxc.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://ujc.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://qme.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://pvy.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fkg.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://blv.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://xgo.iojbl.cn

[G07] 调用父类方法
来源：http://pfj.ybcxt.top

Py:   super().greet()
来源：http://xsx.chenzaomai.com

PHP:  parent::greet();
来源：http://lnw.cashguo.top

JS:   super.greet();
来源：http://fbm.ppjwa.cn

TS:   super.greet();
来源：http://trh.gogol.net.cn

Java: super.greet();
来源：http://hos.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qjq.hammf.cn

Ruby: super
来源：http://odt.hammf.cn

C#:   base.Greet();
来源：http://yhq.zhoulong.xyz

[G08] 静态方法与属性
来源：http://jik.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zil.zhongyouzk.top

PHP:  public static function f() {}
来源：http://sty.ivvv.top

JS:   static f() {}
来源：http://qcp.zycfv.cn

TS:   static f(): void {}
来源：http://wev.shangyingyoupin.top

Java: static void f() {}
来源：http://cii.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hvq.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://kkz.mhx1999.top

C#:   public static void F() {}
来源：http://saq.fengsongda.top

[G09] 接口 / 抽象类
来源：http://tyl.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://dby.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cyh.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iqy.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://tgi.bjfxy.top

Java: interface Shape { double area(); }
来源：http://lgc.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://mif.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://szn.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://hng.yj20258888.top

[G10] 访问控制
来源：http://atj.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://dgb.redwolf501.top

PHP:  public / protected / private
来源：http://zjo.xziqi.cn

JS:   #private 字段；其余公开
来源：http://stz.meibo888.top

TS:   public / protected / private
来源：http://jcb.tarul.cn

Java: public / protected / private / 默认包级
来源：http://lcw.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://stv.zdqjudy.top

Ruby: public / protected / private
来源：http://jua.xinyue.icu

C#:   public / protected / private / internal
来源：http://fnh.jiagoushi.top

[G11] getter / setter
来源：http://jcm.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://qej.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vpm.aizwys.cn

JS:   get name() { return this._name; }
来源：http://ghf.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://gvd.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://mhk.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mhk.smart0.xyz

Ruby: attr_accessor :name
来源：http://srk.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://ail.chenzaomai.com

[G12] 对象转字符串
来源：http://xic.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://bvy.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mtw.vehdjk.com

JS:   toString() { return this.name; }
来源：http://wce.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://gdn.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://ido.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://krk.sweek.top

Ruby: def to_s; @name; end
来源：http://pbe.tarul.cn

C#:   public override string ToString() => Name;
来源：http://rmh.guowangkeji.top

[G13] 判断对象类型
来源：http://ayb.sxryk.cn

Py:   isinstance(u, User)
来源：http://jbw.guowangkeji.top

PHP:  $u instanceof User
来源：http://ama.9152youxi.cn

JS:   u instanceof User
来源：http://qow.sjlbkw.cn

TS:   u instanceof User
来源：http://psa.ydjk.org.cn

Java: u instanceof User
来源：http://nmz.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://lff.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://gws.c1oappe.top

C#:   u is User
来源：http://jpc.zdqjudy.top


<!-- 参考信息 -->