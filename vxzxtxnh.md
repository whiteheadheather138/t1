代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qww.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mbm.tianlin.xyz

[E16] 数字千分位
来源：http://rsp.yueranfly.top

Py:   f"{1234567:,}"
来源：http://fta.birdmap.top

PHP:  number_format(1234567);
来源：http://ejx.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mrm.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nqr.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mdp.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pse.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mha.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://hqa.cqqwz.cn

[E17] 首字母大写
来源：http://wvo.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iee.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bzn.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqf.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tgm.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tgh.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ckk.xinyue.icu

Ruby: s.capitalize
来源：http://oql.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://svo.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://csv.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cbo.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://edz.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pxh.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://vam.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dhm.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wyj.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pnm.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mws.uphjek.com

[E19] 多行文本按行拆分
来源：http://nse.ctjpmb.com

Py:   s.splitlines()
来源：http://vud.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fyh.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://hxj.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://zmk.hnqzz.top

Java: s.lines().toList()
来源：http://kdf.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://eje.jqgufenzy.top

Ruby: s.lines
来源：http://eeu.yj20258888.top

C#:   s.Split('\n')
来源：http://iwr.ybcxt.top

[E20] 判断字符串是否为空
来源：http://yas.jlsjyb.cn

Py:   if not s:
来源：http://lfc.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zwc.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kfa.cdnleiting.top

TS:   if (s === "") {}
来源：http://xoa.sweek.top

Java: if (s.isEmpty()) {}
来源：http://csr.dianchejie.cn

Go:   if s == "" {}
来源：http://ptw.hnqzz.top

Ruby: if s.empty?
来源：http://iag.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zzx.jyoumei.cn

[E21] 超长截断加省略号
来源：http://kng.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dbi.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xga.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wek.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zef.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://auj.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://jxs.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fxs.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lvp.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://fyp.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://syc.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snu.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qcm.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tnd.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cto.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vlp.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://hzn.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hmp.aibaodan.cn

================================================================================
来源：http://cfv.nanxuanxn.top

F. 文件与目录
来源：http://xhl.dianchejie.cn

================================================================================
来源：http://god.hfpthk.cn

[F01] 读取整个文件
来源：http://ccj.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jeo.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://njb.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://etj.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jym.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rop.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cks.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://gnm.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://tdq.kuanghao11.cn

[F02] 逐行读取文件
来源：http://lsc.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://upk.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ong.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://klk.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gtk.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bsa.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pqm.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ogy.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vgr.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://bhx.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hvs.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ysw.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xat.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sgw.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gyl.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://shv.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://aun.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xxf.hnqzz.top

[F04] 追加写入文件
来源：http://sfw.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dae.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://itl.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dla.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ftq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://krm.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zop.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jsw.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mrr.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://txb.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tah.havefunace.top

PHP:  file_exists("a.txt");
来源：http://qhb.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://vff.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://tdh.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nvf.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pwi.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://ykg.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://rfl.cashguo.top

[F06] 删除文件
来源：http://aqz.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://hsw.c1oappe.top

PHP:  unlink("a.txt");
来源：http://ean.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kzf.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hav.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://poa.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://psl.316326.xyz

Ruby: File.delete("a.txt")
来源：http://smf.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://tfd.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://can.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dch.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eyo.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://glz.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oqj.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://unj.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://keo.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rrh.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dwj.bbcook.cn

[F08] 遍历目录
来源：http://vqi.9152youxi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cwc.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gss.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://xck.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://qfy.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ncd.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aln.zycfv.cn

Ruby: Dir.children("dir")
来源：http://kvh.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://meh.sxryk.cn

[F09] 获取文件大小
来源：http://bcu.yj20258.top

Py:   os.path.getsize("a.txt")
来源：http://fcn.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://ofj.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://wus.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://xov.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hii.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://chg.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://jrs.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://nyk.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://apg.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zoh.yanxiufei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hmr.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://moo.sweek.top

TS:   path.extname("a.txt")
来源：http://vyy.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bzl.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gui.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tgk.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bop.gzhubu.top

[F11] 复制与移动文件
来源：http://dfn.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cmu.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ucq.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gms.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eus.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xag.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dzv.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pum.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mbh.jyoumei.cn

[F12] CSV 读写
来源：http://kcw.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bmq.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uvv.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ykr.jinyuanbaomall.cn

TS:   // 同上
来源：http://qmo.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://frm.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ghp.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ngm.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mhj.redwolf501.top

================================================================================
来源：http://qdd.sjlbkw.cn

G. 面向对象
来源：http://cir.iojbl.cn

================================================================================
来源：http://sqi.guowangkeji.top

[G01] 定义类
来源：http://wpa.nanxinkj.top

Py:   class User: pass
来源：http://vjz.ctjpmb.com

PHP:  class User {}
来源：http://ccs.zhaomingkeji.xyz

JS:   class User {}
来源：http://zvo.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://mpl.havefunace.top

Java: class User {}
来源：http://sci.wangshuangyany.cn

Go:   type User struct { Name string }
来源：http://wct.shanyushiyangtech.top

Ruby: class User; end
来源：http://htb.snrcjt.cn

C#:   class User {}
来源：http://cdy.gaohongyu789.top

[G02] 构造函数
来源：http://llz.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://mvz.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://xfn.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://smc.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://ezd.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://hvs.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rud.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://eky.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://mdw.yongpay.top

[G03] 实例属性
来源：http://edz.daria6918.cn

Py:   self.name = "x"
来源：http://tyq.fengsongda.top

PHP:  public string $name = "x";
来源：http://oiv.zhongyouzk.top

JS:   this.name = "x";
来源：http://gjf.jlsjyb.cn

TS:   name: string = "x";
来源：http://hrp.hcnkem.com

Java: private String name;
来源：http://iqo.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rcl.pycfn.com

Ruby: @name = "x"
来源：http://oyv.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://vfj.yanxiufei.cn

[G04] 定义方法
来源：http://chg.cashguo.top

Py:   def greet(self): return self.name
来源：http://pqw.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gme.xziqi.cn

JS:   greet() { return this.name; }
来源：http://ovv.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://fmk.sysykeji.top

Java: String greet() { return name; }
来源：http://dek.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uqq.smart0.xyz

Ruby: def greet; @name; end
来源：http://kxw.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://ytg.ctjpmb.com

[G05] 继承
来源：http://mlt.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://xaz.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://acq.xuanzx.com

JS:   class Admin extends User {}
来源：http://rzq.jiagoushi.top

TS:   class Admin extends User {}
来源：http://abc.sjlbkw.cn

Java: class Admin extends User {}
来源：http://jfh.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wez.bjfxy.top

Ruby: class Admin < User; end
来源：http://xer.aibaodan.cn

C#:   class Admin : User {}
来源：http://mbb.aibaodan.cn

[G06] 重写方法
来源：http://fcn.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://sez.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aso.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://ild.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://cba.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://gmh.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://plv.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://evw.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://udw.quarkkingdee.top

[G07] 调用父类方法
来源：http://eqd.fehbvm.com

Py:   super().greet()
来源：http://fdv.cashguo.top

PHP:  parent::greet();
来源：http://tqv.dashuyun.cn

JS:   super.greet();
来源：http://pvu.jinqigufen.top

TS:   super.greet();
来源：http://cqo.dianchejie.cn

Java: super.greet();
来源：http://hyt.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qwu.yj20258888.top

Ruby: super
来源：http://gcn.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://htn.sweek.top

[G08] 静态方法与属性
来源：http://qvh.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jdd.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://mlr.ydzc1.top

JS:   static f() {}
来源：http://qfv.zdbjq.cn

TS:   static f(): void {}
来源：http://fnb.gzhubu.top

Java: static void f() {}
来源：http://dtz.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xeo.hesvh.cn

Ruby: def self.f; end
来源：http://ntr.xuanzx.com

C#:   public static void F() {}
来源：http://xlc.hesvh.cn

[G09] 接口 / 抽象类
来源：http://wsd.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://war.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zzj.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ihl.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://rds.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://eoe.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://jyq.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vdx.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://wus.xziqi.cn

[G10] 访问控制
来源：http://bpw.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://fja.daxiang520.top

PHP:  public / protected / private
来源：http://uus.nwbrower.top

JS:   #private 字段；其余公开
来源：http://byv.jqgufenzy.top

TS:   public / protected / private
来源：http://dkq.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://wjj.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://amv.yangfankeji.com

Ruby: public / protected / private
来源：http://nrp.meibo888.top

C#:   public / protected / private / internal
来源：http://pdw.cdnleiting.top

[G11] getter / setter
来源：http://fvz.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://ypm.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tpi.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://sva.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://laq.ybcxt.top

Java: public String getName() { return name; }
来源：http://eom.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dzt.tianlin.xyz

Ruby: attr_accessor :name
来源：http://qvu.tian-w.cn

C#:   public string Name { get; set; }
来源：http://mte.fzhhl.top

[G12] 对象转字符串
来源：http://whe.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://qye.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qjm.wangdashe.top

JS:   toString() { return this.name; }
来源：http://juw.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://hrl.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://mco.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://cxl.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://gxb.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://iag.9152youxi.cn

[G13] 判断对象类型
来源：http://rhb.cashguo.top

Py:   isinstance(u, User)
来源：http://vwd.yfazqb.com

PHP:  $u instanceof User
来源：http://lkf.chenjidiqi.icu

JS:   u instanceof User
来源：http://rln.zhixingplan.top

TS:   u instanceof User
来源：http://mvu.yvedp.cn

Java: u instanceof User
来源：http://axs.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jme.guannengcc.top

Ruby: u.is_a?(User)
来源：http://dcp.yonumen.top

C#:   u is User
来源：http://mht.shangyingyoupin.top

[G14] 数据类 / record
来源：http://pet.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wyq.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://kul.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jjc.sweek.top


<!-- 参考信息 -->