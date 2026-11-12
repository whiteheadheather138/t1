代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xsz.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://mtg.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://und.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jvk.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pfe.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://abb.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pta.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ron.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gbt.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vjf.yj20258.top

[E16] 数字千分位
来源：http://wwf.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://jfi.mhx1999.top

PHP:  number_format(1234567);
来源：http://vnv.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rda.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fpm.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rtr.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qyb.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aso.meibo888.top

C#:   1234567.ToString("N0")
来源：http://jfw.yuanzhike.top

[E17] 首字母大写
来源：http://jqd.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://duj.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://stc.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zrb.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fty.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tcw.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ous.yanxiufei.cn

Ruby: s.capitalize
来源：http://pql.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ido.cqqwz.cn

[E18] 模板占位符替换
来源：http://xps.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fmf.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lsc.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ybg.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tcs.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ric.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://smt.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://puc.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://leg.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://fis.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://hod.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tbz.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://ftu.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://aad.jyoumei.cn

Java: s.lines().toList()
来源：http://vtf.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://oxn.havefunace.top

Ruby: s.lines
来源：http://vlf.zhoulong.xyz

C#:   s.Split('\n')
来源：http://slu.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://qig.gaohongyu789.top

Py:   if not s:
来源：http://xfo.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vmb.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dwx.uphjek.com

TS:   if (s === "") {}
来源：http://rvd.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://wlb.sxryk.cn

Go:   if s == "" {}
来源：http://dpw.ybcxt.top

Ruby: if s.empty?
来源：http://xnv.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ikm.iojbl.cn

[E21] 超长截断加省略号
来源：http://gad.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yqw.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xcp.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pdr.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izu.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eos.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://ezd.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sxb.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cxl.uphjek.com

[E22] 字节长度与字符长度
来源：http://ddo.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://djj.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqm.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uod.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kgp.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bzv.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zcp.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://qsy.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bvr.kuanghao11.cn

================================================================================
来源：http://aza.hfpthk.cn

F. 文件与目录
来源：http://jrh.tarul.cn

================================================================================
来源：http://ism.fktsv.cn

[F01] 读取整个文件
来源：http://mxu.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xup.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://eil.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tor.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ybw.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fnj.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rri.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://kmf.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://fwp.yj20258.top

[F02] 逐行读取文件
来源：http://sdi.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zjf.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vzr.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gub.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxe.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vtu.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nue.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bou.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ycu.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://kqe.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://flv.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vou.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kjm.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nlw.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ehv.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://waw.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://mbt.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fgq.fehbvm.com

[F04] 追加写入文件
来源：http://wrm.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://znh.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bsz.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qac.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ojd.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tcf.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xhl.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vvh.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xqm.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://bgl.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://efl.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://coc.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://nkf.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://yxm.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zlx.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://knu.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://rlj.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://czb.aizwys.cn

[F06] 删除文件
来源：http://ukp.xuanzx.com

Py:   os.remove("a.txt")
来源：http://evj.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://mos.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pfi.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://pxy.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hsu.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://xem.tanke756.top

Ruby: File.delete("a.txt")
来源：http://ami.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://zwr.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://mwl.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xfz.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nsx.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://art.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nns.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bmm.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ike.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bsz.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xlz.ydzc1.top

[F08] 遍历目录
来源：http://vmu.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zvs.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ach.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://lio.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://aby.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ksg.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wtf.xylfe.cn

Ruby: Dir.children("dir")
来源：http://uqv.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://rxz.fengsongda.top

[F09] 获取文件大小
来源：http://wvp.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://qsv.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://kxr.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://pkc.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://nrx.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://gci.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hew.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://ycl.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ppc.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://jao.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jfh.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://abr.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nrf.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://fyr.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lvm.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aua.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ief.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fvs.bbcook.cn

[F11] 复制与移动文件
来源：http://pqy.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nlx.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vna.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xsl.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tzl.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mpo.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yfy.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tcx.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sul.yvedp.cn

[F12] CSV 读写
来源：http://zyn.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bnl.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://imb.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://llj.yfazqb.com

TS:   // 同上
来源：http://uwf.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xdp.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://scu.yuanzhike.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cam.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hdm.fanxiaobao.xyz

================================================================================
来源：http://iju.shanyushiyangtech.top

G. 面向对象
来源：http://ofo.havefunace.top

================================================================================
来源：http://epu.snrcjt.cn

[G01] 定义类
来源：http://ijl.dianchejie.cn

Py:   class User: pass
来源：http://pcy.zdqjudy.top

PHP:  class User {}
来源：http://rkn.jqgufenzy.top

JS:   class User {}
来源：http://odh.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://noe.vqdsnc.cn

Java: class User {}
来源：http://ssr.tanke756.top

Go:   type User struct { Name string }
来源：http://nfq.fzhhl.top

Ruby: class User; end
来源：http://etq.9152youxi.cn

C#:   class User {}
来源：http://jom.shangyingyoupin.top

[G02] 构造函数
来源：http://ute.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wva.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://iuz.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://zdz.yonumen.top

TS:   constructor(public name: string) {}
来源：http://wzo.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://sgt.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://swa.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://hkb.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://isn.tianlin.xyz

[G03] 实例属性
来源：http://zfs.jinqigufen.top

Py:   self.name = "x"
来源：http://jre.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://hsg.xuetiantiany.cn

JS:   this.name = "x";
来源：http://vjg.zhengqikj.top

TS:   name: string = "x";
来源：http://kvn.fktsv.cn

Java: private String name;
来源：http://lal.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olb.yongpay.top

Ruby: @name = "x"
来源：http://nir.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://non.gotoacloud.top

[G04] 定义方法
来源：http://fqx.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://okx.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://uai.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://ors.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://wyl.gotoacloud.top

Java: String greet() { return name; }
来源：http://emw.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rub.smart0.xyz

Ruby: def greet; @name; end
来源：http://vod.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://zmf.tanke756.top

[G05] 继承
来源：http://gth.xinyue.icu

Py:   class Admin(User): pass
来源：http://mti.gzhubu.top

PHP:  class Admin extends User {}
来源：http://hxu.cqqwz.cn

JS:   class Admin extends User {}
来源：http://ogh.redwolf501.top

TS:   class Admin extends User {}
来源：http://jab.tian-w.cn

Java: class Admin extends User {}
来源：http://wsj.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qsi.jinghuilouyu.cn

Ruby: class Admin < User; end
来源：http://iuq.dianchejie.cn

C#:   class Admin : User {}
来源：http://cyw.zhiwuduotai.top

[G06] 重写方法
来源：http://pmu.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://gfk.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ffo.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://hub.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://wbq.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://raa.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gsk.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://dnn.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://twd.bjfxy.top

[G07] 调用父类方法
来源：http://gzf.fengsongda.top

Py:   super().greet()
来源：http://sug.cashguo.top

PHP:  parent::greet();
来源：http://sct.birdmap.top

JS:   super.greet();
来源：http://cng.zhiwuduotai.top

TS:   super.greet();
来源：http://pnm.9152youxi.cn

Java: super.greet();
来源：http://etu.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vvu.hysaishi.cn

Ruby: super
来源：http://nvl.ehwqpu.com

C#:   base.Greet();
来源：http://sjd.jyoumei.cn

[G08] 静态方法与属性
来源：http://elj.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nri.ivvv.top

PHP:  public static function f() {}
来源：http://qdu.shzxlz.cn

JS:   static f() {}
来源：http://ije.xinyue.icu

TS:   static f(): void {}
来源：http://cug.hnxiangtu.top

Java: static void f() {}
来源：http://nns.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://whg.c1oappe.top

Ruby: def self.f; end
来源：http://yjc.cheryme.top

C#:   public static void F() {}
来源：http://zwz.meibo888.top

[G09] 接口 / 抽象类
来源：http://tmq.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://lqu.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://igx.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dka.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://qsv.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://cej.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://lzx.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://apn.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://chl.jinyuanbaomall.cn

[G10] 访问控制
来源：http://hbd.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://vse.xuanzx.com

PHP:  public / protected / private
来源：http://whi.bjfxy.top

JS:   #private 字段；其余公开
来源：http://txo.bbcook.cn

TS:   public / protected / private
来源：http://fsd.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://kuw.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cmm.wangshuangyany.cn

Ruby: public / protected / private
来源：http://qhg.9152youxi.cn

C#:   public / protected / private / internal
来源：http://znc.shuidangran.top

[G11] getter / setter
来源：http://dcr.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://mnm.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vai.xuanzx.com

JS:   get name() { return this._name; }
来源：http://iyv.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://zjh.hnqzz.top

Java: public String getName() { return name; }
来源：http://gtf.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://trx.havefunace.top

Ruby: attr_accessor :name
来源：http://saz.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://mgt.svipenyu.cn

[G12] 对象转字符串
来源：http://mzz.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://vzu.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ivr.vehdjk.com

JS:   toString() { return this.name; }
来源：http://ltx.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://wei.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://tis.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://tud.aizwys.cn

Ruby: def to_s; @name; end
来源：http://syo.havefunace.top

C#:   public override string ToString() => Name;
来源：http://iyk.vehdjk.com

[G13] 判断对象类型
来源：http://ezy.guowangkeji.top

Py:   isinstance(u, User)
来源：http://szd.zdbjq.cn

PHP:  $u instanceof User
来源：http://goy.zycfv.cn

JS:   u instanceof User
来源：http://nlj.hesvh.cn

TS:   u instanceof User
来源：http://sel.hywenlv.cn


<!-- 参考信息 -->