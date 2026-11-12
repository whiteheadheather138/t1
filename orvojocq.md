代发 wailian999

PHP:  number_format(1234567);
来源：http://ysf.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lto.tian-w.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kgr.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dlt.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://alc.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://inc.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://njg.gogol.net.cn

[E17] 首字母大写
来源：http://qpo.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ile.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tvz.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kgl.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vva.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bbd.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bfv.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://fhg.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tcp.ybcxt.top

[E18] 模板占位符替换
来源：http://anc.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pxm.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://shb.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ofq.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jxx.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ldj.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yhw.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cxf.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yjl.yj20258.top

[E19] 多行文本按行拆分
来源：http://zun.fehbvm.com

Py:   s.splitlines()
来源：http://aqn.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://swj.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://tzt.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://pfi.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://ebs.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://hmu.c1oappe.top

Ruby: s.lines
来源：http://vml.zycfv.cn

C#:   s.Split('\n')
来源：http://eoh.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://crg.xingfuxueyuan.xyz

Py:   if not s:
来源：http://jhv.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wcx.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hgk.sxryk.cn

TS:   if (s === "") {}
来源：http://wnt.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://xzj.yuxming.cn

Go:   if s == "" {}
来源：http://bwl.cqqwz.cn

Ruby: if s.empty?
来源：http://nwu.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oit.uphjek.com

[E21] 超长截断加省略号
来源：http://klo.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tuq.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fbl.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wwa.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pqv.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://edh.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://tev.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://smm.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vvb.yj20258.top

[E22] 字节长度与字符长度
来源：http://elm.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fpi.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nyr.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vup.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zhf.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rpn.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ftf.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://smz.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pgi.aizwys.cn

================================================================================
来源：http://osg.svipenyu.cn

F. 文件与目录
来源：http://rsx.jinqigufen.top

================================================================================
来源：http://eaq.jiagoushi.top

[F01] 读取整个文件
来源：http://ors.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lge.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://bgl.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ryt.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://syw.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mga.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wqh.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://oyi.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://wbr.uphjek.com

[F02] 逐行读取文件
来源：http://qbe.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sgi.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ojq.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eeh.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uzk.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bql.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baz.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ack.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ugj.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://qlw.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wsh.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fzr.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kzt.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vyz.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://upv.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hiv.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://aqz.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xed.tanke756.top

[F04] 追加写入文件
来源：http://hiq.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qri.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pmg.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjj.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pmt.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xtv.yangfankeji.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://esb.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yqx.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://prh.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://jau.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ncp.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://olr.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://dgt.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://usq.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mli.guannengcc.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qww.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://caw.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://fpo.ehwqpu.com

[F06] 删除文件
来源：http://gwa.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://xbb.xuanzx.com

PHP:  unlink("a.txt");
来源：http://hem.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://tpb.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://idj.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://emd.cheryme.top

Go:   os.Remove("a.txt")
来源：http://jof.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://scv.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://fhe.birdmap.top

[F07] 创建目录（含多级）
来源：http://lcz.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rjt.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pxv.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rss.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xth.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hdc.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tgw.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://srp.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vcw.xylfe.cn

[F08] 遍历目录
来源：http://kiv.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ybx.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nap.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://kwe.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://vqt.sufxvd.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xaj.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kpt.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://oon.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://ilt.jqgufenzy.top

[F09] 获取文件大小
来源：http://qax.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://tsw.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://yny.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://wke.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://oqi.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yxp.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jdc.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://fxr.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://sjf.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://pju.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pjq.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ssd.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://usn.yj20258.top

TS:   path.extname("a.txt")
来源：http://ojk.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ono.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xkt.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wfu.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jpc.chenlongwang.top

[F11] 复制与移动文件
来源：http://svo.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vzd.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gou.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://emr.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xyi.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fmw.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vwe.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://skz.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kjj.wangshuangyany.cn

[F12] CSV 读写
来源：http://zvi.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ktl.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wli.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vgj.yonumen.top

TS:   // 同上
来源：http://uzn.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xdm.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bhu.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ujm.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qgu.ydjk.org.cn

================================================================================
来源：http://yns.dashuyun.cn

G. 面向对象
来源：http://rtn.gogol.net.cn

================================================================================
来源：http://xwb.chenlongwang.top

[G01] 定义类
来源：http://uhs.pengpengdd.cyou

Py:   class User: pass
来源：http://cid.yuanzhike.top

PHP:  class User {}
来源：http://xdj.shangyingyoupin.top

JS:   class User {}
来源：http://bbv.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://eix.xinyue.icu

Java: class User {}
来源：http://wfp.xylfe.cn

Go:   type User struct { Name string }
来源：http://eio.316326.xyz

Ruby: class User; end
来源：http://aab.gogol.net.cn

C#:   class User {}
来源：http://vzq.gogol.net.cn

[G02] 构造函数
来源：http://yyo.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://nsu.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://kwh.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://mte.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://wsl.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://hln.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kmd.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://ilf.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://zia.shuidangran.top

[G03] 实例属性
来源：http://gmt.xylfe.cn

Py:   self.name = "x"
来源：http://jwq.vehdjk.com

PHP:  public string $name = "x";
来源：http://cbw.gzhubu.top

JS:   this.name = "x";
来源：http://eya.gzhubu.top

TS:   name: string = "x";
来源：http://mze.hammf.cn

Java: private String name;
来源：http://wml.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ddu.ybcxt.top

Ruby: @name = "x"
来源：http://mwh.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://exa.zhaomingkeji.xyz

[G04] 定义方法
来源：http://huu.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://zpy.vqdsnc.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hab.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://evq.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://cmq.svipenyu.cn

Java: String greet() { return name; }
来源：http://dhq.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ohb.yongpay.top

Ruby: def greet; @name; end
来源：http://eay.tarul.cn

C#:   public string Greet() => Name;
来源：http://ole.daxiang520.top

[G05] 继承
来源：http://qnq.hammf.cn

Py:   class Admin(User): pass
来源：http://cur.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://jte.hysaishi.cn

JS:   class Admin extends User {}
来源：http://dsk.shzxlz.cn

TS:   class Admin extends User {}
来源：http://xad.ybcxt.top

Java: class Admin extends User {}
来源：http://hdj.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pbc.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://str.52xcode.cn

C#:   class Admin : User {}
来源：http://hrn.nanxinkj.top

[G06] 重写方法
来源：http://mjs.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://wgf.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vtt.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://pdv.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://qaz.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://nmb.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://arf.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://vwt.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://ftq.yj202588.top

[G07] 调用父类方法
来源：http://kbr.cucudq.cn

Py:   super().greet()
来源：http://qlb.jqgufenzy.top

PHP:  parent::greet();
来源：http://wlh.cucudq.cn

JS:   super.greet();
来源：http://asz.nwbrower.top

TS:   super.greet();
来源：http://wse.bjfxy.top

Java: super.greet();
来源：http://ijh.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yto.wangshuangyany.cn

Ruby: super
来源：http://dvr.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://obd.mhx1999.top

[G08] 静态方法与属性
来源：http://xxz.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rye.shzxlz.cn

PHP:  public static function f() {}
来源：http://ycu.aizwys.cn

JS:   static f() {}
来源：http://cpz.xuanzx.com

TS:   static f(): void {}
来源：http://asn.hywenlv.cn

Java: static void f() {}
来源：http://hiq.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sgh.tarul.cn

Ruby: def self.f; end
来源：http://lcs.yfazqb.com

C#:   public static void F() {}
来源：http://qfs.sxryk.cn

[G09] 接口 / 抽象类
来源：http://jbx.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://gvv.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://fax.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mue.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://vrd.epnwcf.com

Java: interface Shape { double area(); }
来源：http://vgo.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://vtp.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ojf.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://imh.hnqzz.top

[G10] 访问控制
来源：http://ozc.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://mbv.tarul.cn

PHP:  public / protected / private
来源：http://hov.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://evb.zhiwuduotai.top

TS:   public / protected / private
来源：http://ydz.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://eut.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jic.c1oappe.top

Ruby: public / protected / private
来源：http://yma.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://kwp.ywan-chungtsiang.top

[G11] getter / setter
来源：http://mag.tian-w.cn

Py:   @property 与 @x.setter
来源：http://vku.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://feu.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://iss.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://uhy.shuidangran.top

Java: public String getName() { return name; }
来源：http://ote.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vgp.cucudq.cn

Ruby: attr_accessor :name
来源：http://oqy.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://ycf.c1oappe.top

[G12] 对象转字符串
来源：http://wvv.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://asb.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ogx.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://cxc.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://hnb.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://cwm.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qgx.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://tim.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://ctq.bbcook.cn

[G13] 判断对象类型
来源：http://jes.sysykeji.top

Py:   isinstance(u, User)
来源：http://sgx.c1oappe.top

PHP:  $u instanceof User
来源：http://ptj.ehwqpu.com

JS:   u instanceof User
来源：http://rwk.nanxuanxn.top

TS:   u instanceof User
来源：http://fva.jqgufenzy.top

Java: u instanceof User
来源：http://ipo.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aft.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://txn.chenjidiqi.icu

C#:   u is User
来源：http://lei.hammf.cn

[G14] 数据类 / record
来源：http://hup.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sea.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://vgf.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://pva.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://fet.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://mtu.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://suj.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ifp.shanyushiyangkeji.top


<!-- 参考信息 -->