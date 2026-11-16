代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://omr.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kab.tian-w.cn

[E16] 数字千分位
来源：http://zwc.sysykeji.top

Py:   f"{1234567:,}"
来源：http://oth.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://pew.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fdz.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lmr.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ckr.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fyd.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wch.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://prj.fanxiaobao.xyz

[E17] 首字母大写
来源：http://dwc.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://flq.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qet.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nmc.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xxw.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wou.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://epb.nwbrower.top

Ruby: s.capitalize
来源：http://cyp.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sdz.jyoumei.cn

[E18] 模板占位符替换
来源：http://zep.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wha.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://upc.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wcl.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://avv.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cio.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://emr.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aih.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dtz.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://ral.dianchejie.cn

Py:   s.splitlines()
来源：http://jim.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://coe.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://ymq.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://ljg.quarkkingdee.top

Java: s.lines().toList()
来源：http://qqp.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://bps.chenlongwang.top

Ruby: s.lines
来源：http://etf.tian-w.cn

C#:   s.Split('\n')
来源：http://kbx.yj202588.top

[E20] 判断字符串是否为空
来源：http://ebb.zhixingplan.top

Py:   if not s:
来源：http://rep.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kkw.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pqb.yonumen.top

TS:   if (s === "") {}
来源：http://qyo.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://wkw.pengpengdd.cyou

Go:   if s == "" {}
来源：http://kso.bjfxy.top

Ruby: if s.empty?
来源：http://ckb.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dws.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://pdz.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://its.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pad.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yyc.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uql.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ctn.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://pdh.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://glz.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rvc.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://yzh.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://spt.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hhb.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ldy.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fnm.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tzt.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zrh.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://qww.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wci.smart0.xyz

================================================================================
来源：http://ehc.aibaodan.cn

F. 文件与目录
来源：http://tjl.smart0.xyz

================================================================================
来源：http://anq.jyoumei.cn

[F01] 读取整个文件
来源：http://nvf.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zni.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://oov.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kxs.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dfv.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://neu.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pyd.hnqzz.top

Ruby: File.read("a.txt")
来源：http://fly.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://jyz.daxiang520.top

[F02] 逐行读取文件
来源：http://hbu.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hbm.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fgx.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cvs.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jyp.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hkq.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dmr.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wug.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xcy.316326.xyz

[F03] 写入文件（覆盖）
来源：http://nbh.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hii.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mcc.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zvm.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rji.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rwi.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://grf.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://daa.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aop.xylfe.cn

[F04] 追加写入文件
来源：http://uui.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://voe.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lhz.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://udr.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dcz.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bab.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mrk.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gxq.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sbx.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://qjx.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://edo.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://yrb.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://oxj.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://fgj.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qgt.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://slu.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://gqh.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://diz.c1oappe.top

[F06] 删除文件
来源：http://ogv.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://llz.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://bkd.hfpthk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rnj.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://zcz.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kjw.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://kbo.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://etv.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://mly.ivvv.top

[F07] 创建目录（含多级）
来源：http://hjg.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wjr.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://guc.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sgn.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jhq.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wdg.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dtw.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://apw.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://civ.yvedp.cn

[F08] 遍历目录
来源：http://lrw.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://wci.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dfh.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://yuh.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://fbv.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hyy.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xdc.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://djx.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://wpo.yj202588.top

[F09] 获取文件大小
来源：http://hki.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://gej.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://ays.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://fbc.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://dbg.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://cly.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vgv.jianghu66.top

Ruby: File.size("a.txt")
来源：http://syv.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://hwt.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://uuh.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ixi.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zdv.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://chg.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://brm.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eqa.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ehr.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eun.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dam.hnqzz.top

[F11] 复制与移动文件
来源：http://ugs.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zew.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ret.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yls.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vuv.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qre.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://crg.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yaf.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dfs.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://tqb.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uis.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jqz.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mag.ydjk.org.cn

TS:   // 同上
来源：http://cpb.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://usn.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rnr.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fcd.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xmk.andypj.xyz

================================================================================
来源：http://dpy.daria6918.cn

G. 面向对象
来源：http://nei.ppjwa.cn

================================================================================
来源：http://tul.jqgfzy.top

[G01] 定义类
来源：http://yon.sjlbkw.cn

Py:   class User: pass
来源：http://zoo.jinqigufen.top

PHP:  class User {}
来源：http://ara.xinyue.icu

JS:   class User {}
来源：http://gso.316326.xyz

TS:   class User { name: string = ""; }
来源：http://vsg.meibo888.top

Java: class User {}
来源：http://anm.ybcxt.top

Go:   type User struct { Name string }
来源：http://ril.fengsongda.top

Ruby: class User; end
来源：http://cyj.xylfe.cn

C#:   class User {}
来源：http://wia.yongpay.top

[G02] 构造函数
来源：http://ema.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://nrq.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://acj.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://jok.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://ogl.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://kls.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kcc.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://bcw.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://eow.hnqzz.top

[G03] 实例属性
来源：http://bon.cheryme.top

Py:   self.name = "x"
来源：http://njz.gotoacloud.top

PHP:  public string $name = "x";
来源：http://kyi.xuetiantiany.cn

JS:   this.name = "x";
来源：http://fdb.yonumen.top

TS:   name: string = "x";
来源：http://pga.svipenyu.cn

Java: private String name;
来源：http://qmy.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kjp.zhixingplan.top

Ruby: @name = "x"
来源：http://pgo.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://wrr.shzxlz.cn

[G04] 定义方法
来源：http://lxq.zycfv.cn

Py:   def greet(self): return self.name
来源：http://tln.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ncq.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://fld.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://zzw.zhixingplan.top

Java: String greet() { return name; }
来源：http://dav.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tqg.hesvh.cn

Ruby: def greet; @name; end
来源：http://kmw.xuanzx.com

C#:   public string Greet() => Name;
来源：http://ktv.havefunace.top

[G05] 继承
来源：http://gcc.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://hoj.uphjek.com

PHP:  class Admin extends User {}
来源：http://gqc.fengsongda.top

JS:   class Admin extends User {}
来源：http://usf.andypj.xyz

TS:   class Admin extends User {}
来源：http://aog.yangfankeji.com

Java: class Admin extends User {}
来源：http://dwr.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ija.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://fge.316326.xyz

C#:   class Admin : User {}
来源：http://oyz.xuanzx.com

[G06] 重写方法
来源：http://ele.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://wrp.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tct.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://pfh.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://kpr.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://kei.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nmv.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://pfg.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://lvk.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://bul.guannengcc.top

Py:   super().greet()
来源：http://pye.52xcode.cn

PHP:  parent::greet();
来源：http://fff.ctjpmb.com

JS:   super.greet();
来源：http://gvq.fehbvm.com

TS:   super.greet();
来源：http://vhg.nanxinkj.top

Java: super.greet();
来源：http://dgs.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ses.hnqzz.top

Ruby: super
来源：http://aoc.ppjwa.cn

C#:   base.Greet();
来源：http://auu.zhongyouzk.top

[G08] 静态方法与属性
来源：http://tvn.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pfq.zhengqikj.top

PHP:  public static function f() {}
来源：http://iay.hesvh.cn

JS:   static f() {}
来源：http://sup.yvedp.cn

TS:   static f(): void {}
来源：http://fqf.shanyushiyangtech.top

Java: static void f() {}
来源：http://sez.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://byc.zhoulong.xyz

Ruby: def self.f; end
来源：http://zgi.zhengqikj.top

C#:   public static void F() {}
来源：http://lnv.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://lat.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://eka.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://fqx.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vsx.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://zaj.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://bad.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://cct.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tdu.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://dsx.snrcjt.cn

[G10] 访问控制
来源：http://lpu.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://jyh.zhongyouzk.top

PHP:  public / protected / private
来源：http://orh.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://isv.redwolf501.top

TS:   public / protected / private
来源：http://lpq.havefunace.top

Java: public / protected / private / 默认包级
来源：http://qnq.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uss.xuetiantiany.cn

Ruby: public / protected / private
来源：http://fib.sufxvd.cn

C#:   public / protected / private / internal
来源：http://yuo.pycfn.com

[G11] getter / setter
来源：http://phc.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://blx.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://wna.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://gcr.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://dxv.yj20258.top

Java: public String getName() { return name; }
来源：http://zoq.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pnb.zhengqikj.top

Ruby: attr_accessor :name
来源：http://umr.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://eow.shangyingyoupin.top

[G12] 对象转字符串
来源：http://xcx.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://cnc.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://chd.pycfn.com

JS:   toString() { return this.name; }
来源：http://kkr.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://ywz.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://tlj.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://tfu.birdmap.top

Ruby: def to_s; @name; end
来源：http://drr.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://urf.c1oappe.top

[G13] 判断对象类型
来源：http://gek.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://ebc.guannengcc.top

PHP:  $u instanceof User
来源：http://tpp.chenzaomai.com

JS:   u instanceof User
来源：http://elz.9152youxi.cn

TS:   u instanceof User
来源：http://kko.ehwqpu.com

Java: u instanceof User
来源：http://kxj.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yzz.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://kcq.yueranfly.top

C#:   u is User
来源：http://qfw.chenjidiqi.icu

[G14] 数据类 / record
来源：http://ttg.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zsf.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://loi.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://dnl.hysaishi.cn


<!-- 参考信息 -->