代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zhh.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qwd.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://phl.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://quw.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zmf.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wko.jlsjyb.cn

[E16] 数字千分位
来源：http://yiu.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://clg.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://mhw.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://kqk.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ial.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fas.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://acs.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://izg.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://ivk.chenlongwang.top

[E17] 首字母大写
来源：http://yvq.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kua.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kok.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://efc.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vhq.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vku.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qes.zdqjudy.top

Ruby: s.capitalize
来源：http://dhb.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://arm.gotoacloud.top

[E18] 模板占位符替换
来源：http://jfv.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tyw.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bth.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hgh.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zbj.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xmi.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cis.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ocn.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ihm.hnqzz.top

[E19] 多行文本按行拆分
来源：http://bqh.svipenyu.cn

Py:   s.splitlines()
来源：http://raf.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zur.sweek.top

JS:   s.split(/\r?\n/)
来源：http://inj.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://bsx.hnxiangtu.top

Java: s.lines().toList()
来源：http://hid.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://ant.yangfankeji.com

Ruby: s.lines
来源：http://vgk.gotoacloud.top

C#:   s.Split('\n')
来源：http://hep.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://cfl.gogol.net.cn

Py:   if not s:
来源：http://uku.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pwc.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vfh.chenzaomai.com

TS:   if (s === "") {}
来源：http://zrm.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://hwt.ehwqpu.com

Go:   if s == "" {}
来源：http://zwc.svipenyu.cn

Ruby: if s.empty?
来源：http://lfc.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uhj.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://bkz.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://faa.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://obq.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qah.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qne.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://muq.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://puv.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mri.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://owb.wangdashe.top

[E22] 字节长度与字符长度
来源：http://mfl.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zbq.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fmd.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fao.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zew.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ejy.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ikh.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://bcb.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fca.jiagoushi.top

================================================================================
来源：http://kzn.yuxming.cn

F. 文件与目录
来源：http://dgr.dashuyun.cn

================================================================================
来源：http://unn.pengpengdd.cyou

[F01] 读取整个文件
来源：http://gwk.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cum.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://roy.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iem.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rlt.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hyp.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xcv.ivvv.top

Ruby: File.read("a.txt")
来源：http://isl.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://cqj.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://vrn.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yqx.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xqa.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fhd.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jhv.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aec.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ueg.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ema.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fkb.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://abv.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://snk.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://whz.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cot.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rse.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rfv.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://msl.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://vpl.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qih.yanxiufei.cn

[F04] 追加写入文件
来源：http://nzq.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bcf.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rnz.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jcp.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ypi.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qiz.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eqs.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vkt.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tmx.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://nte.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://abn.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://ycd.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://whu.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://ewp.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wfo.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://clk.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://gva.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://osm.hywenlv.cn

[F06] 删除文件
来源：http://qja.c1oappe.top

Py:   os.remove("a.txt")
来源：http://xcm.sxryk.cn

PHP:  unlink("a.txt");
来源：http://kjp.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zoc.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://bxt.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://csk.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://afn.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://jva.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://met.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://qac.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://biu.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qno.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fxp.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aza.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cqb.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hnj.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kyo.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wuw.hysaishi.cn

[F08] 遍历目录
来源：http://gtb.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ywa.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pdt.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://mlr.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://pdj.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tos.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rzt.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://thz.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://lco.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://ack.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://hlw.yueranfly.top

PHP:  filesize("a.txt");
来源：http://sod.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://sbo.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://bhu.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://nov.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://okw.smart0.xyz

Ruby: File.size("a.txt")
来源：http://pmd.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://zlr.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://gwl.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mak.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjl.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uqh.xinyue.icu

TS:   path.extname("a.txt")
来源：http://ijd.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qgn.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wfr.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://izd.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://klt.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://izq.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oih.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ggo.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqr.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqz.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pvd.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://khd.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wvz.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zpg.svipenyu.cn

[F12] CSV 读写
来源：http://xvd.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://via.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dbb.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lcf.0kj1m.cn

TS:   // 同上
来源：http://jmx.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ixz.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eue.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ode.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xbx.tianlin.xyz

================================================================================
来源：http://cab.jinqigufen.top

G. 面向对象
来源：http://drh.yonumen.top

================================================================================
来源：http://viv.yueranfly.top

[G01] 定义类
来源：http://geb.c1oappe.top

Py:   class User: pass
来源：http://hnm.fengsongda.top

PHP:  class User {}
来源：http://wng.52xcode.cn

JS:   class User {}
来源：http://bvc.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://izd.hysaishi.cn

Java: class User {}
来源：http://xrb.9152youxi.cn

Go:   type User struct { Name string }
来源：http://ess.hysaishi.cn

Ruby: class User; end
来源：http://kqe.dashuyun.cn

C#:   class User {}
来源：http://gep.shzxlz.cn

[G02] 构造函数
来源：http://tfq.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://ufq.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://nih.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://ndy.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://kkl.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://vhj.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vyg.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://hcg.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://pyp.gotoacloud.top

[G03] 实例属性
来源：http://utb.haohaochexian.top

Py:   self.name = "x"
来源：http://dfm.meibo888.top

PHP:  public string $name = "x";
来源：http://xez.sxryk.cn

JS:   this.name = "x";
来源：http://kps.xuanzx.com

TS:   name: string = "x";
来源：http://uwe.fengsongda.top

Java: private String name;
来源：http://crd.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vbb.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://mcy.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://tfs.cqqwz.cn

[G04] 定义方法
来源：http://brv.yueranfly.top

Py:   def greet(self): return self.name
来源：http://jtk.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://quv.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://phe.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://fua.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://qgb.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jkj.fktsv.cn

Ruby: def greet; @name; end
来源：http://msj.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://jsu.nanxuanxn.top

[G05] 继承
来源：http://cop.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://agb.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://tmu.svipenyu.cn

JS:   class Admin extends User {}
来源：http://tvu.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://are.tian-w.cn

Java: class Admin extends User {}
来源：http://yxq.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aai.svipenyu.cn

Ruby: class Admin < User; end
来源：http://ghj.xinyue.icu

C#:   class Admin : User {}
来源：http://wsg.yj202588.top

[G06] 重写方法
来源：http://yrw.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://xja.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wgs.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://wfl.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://amf.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://qbb.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dzj.yj20258.top

Ruby: def greet; "admin"; end
来源：http://aue.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://kbs.vehdjk.com

[G07] 调用父类方法
来源：http://yvt.fehbvm.com

Py:   super().greet()
来源：http://zjy.yj20258888.top

PHP:  parent::greet();
来源：http://pln.jinghuilouyu.cn

JS:   super.greet();
来源：http://xrq.jqgufenzy.top

TS:   super.greet();
来源：http://geg.jyoumei.cn

Java: super.greet();
来源：http://sbs.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://njn.jinghuilouyu.cn

Ruby: super
来源：http://qgt.zhongyouzk.top

C#:   base.Greet();
来源：http://vku.haohaochexian.top

[G08] 静态方法与属性
来源：http://yzx.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wtq.bjfxy.top

PHP:  public static function f() {}
来源：http://xye.yj202588.top

JS:   static f() {}
来源：http://bpd.vqdsnc.cn

TS:   static f(): void {}
来源：http://nmh.gzhubu.top

Java: static void f() {}
来源：http://obm.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jwf.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://yks.cdnleiting.top

C#:   public static void F() {}
来源：http://hsu.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://kir.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://jrh.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://esr.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wgk.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://gzn.birdmap.top

Java: interface Shape { double area(); }
来源：http://kdb.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://upk.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nwe.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://abp.hcnkem.com

[G10] 访问控制
来源：http://klg.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://mbt.aizwys.cn

PHP:  public / protected / private
来源：http://ldn.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://xdg.ctjpmb.com

TS:   public / protected / private
来源：http://brm.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://gfm.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://slw.hcnkem.com

Ruby: public / protected / private
来源：http://gnc.hcnkem.com

C#:   public / protected / private / internal
来源：http://xfs.chenjidiqi.icu

[G11] getter / setter
来源：http://snv.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://wct.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://esg.cucudq.cn

JS:   get name() { return this._name; }
来源：http://gbz.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://qvc.cucudq.cn

Java: public String getName() { return name; }
来源：http://hug.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://bmd.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://bhi.cheryme.top

C#:   public string Name { get; set; }
来源：http://vvt.feifeiyinyue.top

[G12] 对象转字符串
来源：http://hgo.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://oca.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://emr.guannengcc.top

JS:   toString() { return this.name; }
来源：http://pml.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://gsi.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://nvj.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xeg.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://ukd.birdmap.top

C#:   public override string ToString() => Name;
来源：http://thp.nanxinkj.top

[G13] 判断对象类型
来源：http://ojb.xylfe.cn

Py:   isinstance(u, User)
来源：http://lbu.sjlbkw.cn

PHP:  $u instanceof User
来源：http://tbg.yongpay.top

JS:   u instanceof User
来源：http://ntk.chenzaomai.com

TS:   u instanceof User
来源：http://tfy.aibaodan.cn

Java: u instanceof User
来源：http://nag.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xig.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://rbb.vqdsnc.cn

C#:   u is User
来源：http://jea.pengpengdd.cyou


<!-- 参考信息 -->