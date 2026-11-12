代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jgd.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xfk.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://csc.jinqigfzy.top

[E17] 首字母大写
来源：http://rix.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yqr.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yen.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://its.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxf.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qsg.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jsb.daria6918.cn

Ruby: s.capitalize
来源：http://pfc.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://isc.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://zey.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sjc.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://scd.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://yzz.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://wae.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zzq.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rxq.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zio.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jce.sweek.top

[E19] 多行文本按行拆分
来源：http://fvb.havefunace.top

Py:   s.splitlines()
来源：http://yoq.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dmv.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://eko.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://ppd.birdmap.top

Java: s.lines().toList()
来源：http://odd.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://kko.xylfe.cn

Ruby: s.lines
来源：http://gom.yj20258888.top

C#:   s.Split('\n')
来源：http://ptu.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://wsx.cashguo.top

Py:   if not s:
来源：http://ile.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://evr.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://scl.52xcode.cn

TS:   if (s === "") {}
来源：http://eoe.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://czh.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://tnb.xuetiantiany.cn

Ruby: if s.empty?
来源：http://tgt.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uxj.xziqi.cn

[E21] 超长截断加省略号
来源：http://usj.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://veb.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yju.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mcf.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uia.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ukb.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://dwl.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jxa.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kbd.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://dfj.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://urk.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hen.yongpay.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vua.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eul.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bpm.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://khh.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://yzv.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nqm.hfpthk.cn

================================================================================
来源：http://exj.hesvh.cn

F. 文件与目录
来源：http://bux.nwbrower.top

================================================================================
来源：http://pqr.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://tir.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qcf.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://wod.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jdm.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sag.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://axt.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lku.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://mrl.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://qbm.tian-w.cn

[F02] 逐行读取文件
来源：http://vrg.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://egw.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hhw.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tah.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uyc.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qdh.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qjx.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://afk.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pdb.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://sxo.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zqo.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kip.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://geo.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sts.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dal.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ljk.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://oxv.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sxw.ppjwa.cn

[F04] 追加写入文件
来源：http://xmx.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pec.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://slk.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vij.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bsj.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hbk.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zpj.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hkr.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ozu.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://akg.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jib.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://xpo.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://zky.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://rlp.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qsf.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://idd.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://bdo.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://gtq.smart0.xyz

[F06] 删除文件
来源：http://ogr.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://ifi.fehbvm.com

PHP:  unlink("a.txt");
来源：http://bms.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://yzh.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uyr.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ypy.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://cfh.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://xyi.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://lcp.ybcxt.top

[F07] 创建目录（含多级）
来源：http://ifc.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pam.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qvt.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aup.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ork.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nfa.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iam.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://egw.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://frl.zdbjq.cn

[F08] 遍历目录
来源：http://prx.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bgb.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wwu.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://qgr.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://kzg.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://krc.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mdn.zycfv.cn

Ruby: Dir.children("dir")
来源：http://bha.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://hbt.cqqwz.cn

[F09] 获取文件大小
来源：http://tfp.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://zjg.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://jhu.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://zhn.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://eot.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://jas.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://smq.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://sjh.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://ddi.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://pct.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://shz.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cnq.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mfk.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://osr.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dmz.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rao.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uyn.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wby.guowangkeji.top

[F11] 复制与移动文件
来源：http://ueb.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zcp.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nau.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nim.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rld.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jhn.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://npj.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kcu.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lvr.hysaishi.cn

[F12] CSV 读写
来源：http://ocx.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://loe.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wyp.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vvb.hnqzz.top

TS:   // 同上
来源：http://udx.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vod.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fnz.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wxb.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bbe.tian-w.cn

================================================================================
来源：http://ugd.xuanzx.com

G. 面向对象
来源：http://ctx.ydjk.org.cn

================================================================================
来源：http://eap.ywan-chungtsiang.top

[G01] 定义类
来源：http://gga.jinyuanbaomall.cn

Py:   class User: pass
来源：http://fes.jlsjyb.cn

PHP:  class User {}
来源：http://bny.zdqjudy.top

JS:   class User {}
来源：http://req.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://dod.chenjidiqi.icu

Java: class User {}
来源：http://emk.dianchejie.cn

Go:   type User struct { Name string }
来源：http://vou.cashguo.top

Ruby: class User; end
来源：http://jko.xuetiantiany.cn

C#:   class User {}
来源：http://dzy.aibaodan.cn

[G02] 构造函数
来源：http://rrp.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://nzp.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://wfq.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://hdo.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://zhu.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://qwv.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ysr.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://ucn.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://fan.epnwcf.com

[G03] 实例属性
来源：http://xme.ctjpmb.com

Py:   self.name = "x"
来源：http://hcl.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://bxj.nanxuanxn.top

JS:   this.name = "x";
来源：http://bck.dashuyun.cn

TS:   name: string = "x";
来源：http://hgh.pycfn.com

Java: private String name;
来源：http://tzy.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vnf.dianchejie.cn

Ruby: @name = "x"
来源：http://pgl.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://lhr.zycfv.cn

[G04] 定义方法
来源：http://rnn.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://rmr.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pby.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://ctv.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://cbl.xylfe.cn

Java: String greet() { return name; }
来源：http://ppy.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dwg.pycfn.com

Ruby: def greet; @name; end
来源：http://mct.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://sbt.cheryme.top

[G05] 继承
来源：http://qlu.wangdashe.top

Py:   class Admin(User): pass
来源：http://elm.yueranfly.top

PHP:  class Admin extends User {}
来源：http://fqg.tanke756.top

JS:   class Admin extends User {}
来源：http://spz.yuxming.cn

TS:   class Admin extends User {}
来源：http://cyn.tarul.cn

Java: class Admin extends User {}
来源：http://nzf.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://srv.fktsv.cn

Ruby: class Admin < User; end
来源：http://xqq.snrcjt.cn

C#:   class Admin : User {}
来源：http://fic.ivvv.top

[G06] 重写方法
来源：http://tis.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://zjs.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dhy.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://sat.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://equ.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://zkf.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wzd.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://wtb.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://pnh.chenzaomai.com

[G07] 调用父类方法
来源：http://npk.wangshuangyany.cn

Py:   super().greet()
来源：http://gpn.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://czz.jiagoushi.top

JS:   super.greet();
来源：http://zgk.hnxiangtu.top

TS:   super.greet();
来源：http://mpk.hysaishi.cn

Java: super.greet();
来源：http://lak.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://teu.hongshengwenyu.top

Ruby: super
来源：http://kpj.zhijiandao.cn

C#:   base.Greet();
来源：http://oig.yuanzhike.top

[G08] 静态方法与属性
来源：http://qwo.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://spx.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://fls.mhx1999.top

JS:   static f() {}
来源：http://ema.cdnleiting.top

TS:   static f(): void {}
来源：http://rho.epnwcf.com

Java: static void f() {}
来源：http://bha.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tyx.yj20258888.top

Ruby: def self.f; end
来源：http://neb.guowangkeji.top

C#:   public static void F() {}
来源：http://ekd.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://mhy.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://zqs.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://zrr.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pms.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://psi.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://zrq.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://igq.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://neb.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://vns.ydjk.org.cn

[G10] 访问控制
来源：http://uxn.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://gec.zhiwuduotai.top

PHP:  public / protected / private
来源：http://xcs.hnxiangtu.top

JS:   #private 字段；其余公开
来源：http://dxt.jyoumei.cn

TS:   public / protected / private
来源：http://yba.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://tdk.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dop.zhijiandao.cn

Ruby: public / protected / private
来源：http://ejx.redwolf501.top

C#:   public / protected / private / internal
来源：http://ivk.wangshuangyany.cn

[G11] getter / setter
来源：http://gqc.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://ezg.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://puj.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://zli.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://ibj.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://vdc.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ofd.guowangkeji.top

Ruby: attr_accessor :name
来源：http://xie.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://yju.sjlbkw.cn

[G12] 对象转字符串
来源：http://xpj.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://rac.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zqn.wangdashe.top

JS:   toString() { return this.name; }
来源：http://fnp.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://lef.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://cju.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dnm.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://mlj.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://rnl.52xcode.cn

[G13] 判断对象类型
来源：http://wcm.c1oappe.top

Py:   isinstance(u, User)
来源：http://ziw.ybcxt.top

PHP:  $u instanceof User
来源：http://psx.jlsjyb.cn

JS:   u instanceof User
来源：http://wdu.zdbjq.cn

TS:   u instanceof User
来源：http://qne.havefunace.top

Java: u instanceof User
来源：http://nud.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://alk.meibo888.top

Ruby: u.is_a?(User)
来源：http://uhv.jqgfzy.top

C#:   u is User
来源：http://pzl.yvedp.cn

[G14] 数据类 / record
来源：http://mzh.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lrx.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://obs.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://tvw.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://nwc.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://cky.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://ylu.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nrn.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://wag.pycfn.com

[G15] 枚举
来源：http://gto.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vve.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mzu.0kj1m.cn


<!-- 参考信息 -->