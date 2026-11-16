代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qgi.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dhc.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://imv.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvi.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rwr.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hzt.gaohongyu789.top

Ruby: s.capitalize
来源：http://muj.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mkl.meibo888.top

[E18] 模板占位符替换
来源：http://gti.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://peo.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iix.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jew.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ovk.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://neq.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wdr.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wud.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zsh.hnqzz.top

[E19] 多行文本按行拆分
来源：http://dzv.wangdashe.top

Py:   s.splitlines()
来源：http://kcm.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iet.sweek.top

JS:   s.split(/\r?\n/)
来源：http://med.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://jvf.hnqzz.top

Java: s.lines().toList()
来源：http://xql.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://ffk.gogol.net.cn

Ruby: s.lines
来源：http://pyl.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://vjn.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://gkz.redwolf501.top

Py:   if not s:
来源：http://wev.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gok.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aew.yongpay.top

TS:   if (s === "") {}
来源：http://pnk.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://lox.pycfn.com

Go:   if s == "" {}
来源：http://xmu.hesvh.cn

Ruby: if s.empty?
来源：http://dct.hesvh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sgc.hesvh.cn

[E21] 超长截断加省略号
来源：http://vce.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://npc.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hfk.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://chb.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eyu.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pqu.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://owy.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://egt.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iml.yueranfly.top

[E22] 字节长度与字符长度
来源：http://gal.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oap.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cfp.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cmi.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://coz.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tem.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mlo.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://hwq.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uzt.zhixingplan.top

================================================================================
来源：http://xle.zhengqikj.top

F. 文件与目录
来源：http://mte.pycfn.com

================================================================================
来源：http://vjd.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://hrv.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vbb.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://ozh.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://apl.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mnl.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mzo.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gec.smart0.xyz

Ruby: File.read("a.txt")
来源：http://qvq.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://kza.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://bil.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jes.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lau.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ntr.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fqt.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oea.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lrr.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://syy.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://alm.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://ars.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yat.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gcg.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bfn.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dfz.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sit.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sum.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://dgu.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uaw.ydzc1.top

[F04] 追加写入文件
来源：http://tsy.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xxp.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uhq.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hqe.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://whs.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pws.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blp.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qsp.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://icr.xuanzx.com

[F05] 判断文件或目录是否存在
来源：http://blh.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tmq.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://tiq.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://bvo.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://zay.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lbr.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hqt.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://mbj.yj20258.top

C#:   File.Exists("a.txt")
来源：http://ybj.sjlbkw.cn

[F06] 删除文件
来源：http://rry.xinyue.icu

Py:   os.remove("a.txt")
来源：http://nqf.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://jpp.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://vpj.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://rhu.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uen.daxiang520.top

Go:   os.Remove("a.txt")
来源：http://hqy.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://pov.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://equ.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://nqc.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wwj.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uoa.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aov.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://klw.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dgh.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rsm.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://efx.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bmn.ehwqpu.com

[F08] 遍历目录
来源：http://bgk.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sli.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pyh.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://yya.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://nik.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ukp.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zrt.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://kmr.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://ylr.cucudq.cn

[F09] 获取文件大小
来源：http://tdk.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://kxi.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://gdu.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://xcq.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://pvu.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://djo.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aqa.xinyue.icu

Ruby: File.size("a.txt")
来源：http://dxo.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://eed.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ldf.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://otu.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yeb.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wfj.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://exd.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rai.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zdo.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://miy.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qaq.hysaishi.cn

[F11] 复制与移动文件
来源：http://zms.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wgn.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mgh.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ndu.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvc.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bzl.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mlw.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ckb.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yaz.jiagoushi.top

[F12] CSV 读写
来源：http://aba.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rrf.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hdo.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mnu.hfpthk.cn

TS:   // 同上
来源：http://wwx.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rfz.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zwa.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ofw.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nqc.vehdjk.com

================================================================================
来源：http://zvt.zhengqikj.top

G. 面向对象
来源：http://mof.sysykeji.top

================================================================================
来源：http://ruv.guowangkeji.top

[G01] 定义类
来源：http://gyg.chenlongwang.top

Py:   class User: pass
来源：http://kcn.gotoacloud.top

PHP:  class User {}
来源：http://hne.cucudq.cn

JS:   class User {}
来源：http://okh.ivvv.top

TS:   class User { name: string = ""; }
来源：http://fem.gogol.net.cn

Java: class User {}
来源：http://pck.tanke756.top

Go:   type User struct { Name string }
来源：http://jix.shanyushiyangkeji.top

Ruby: class User; end
来源：http://kri.uphjek.com

C#:   class User {}
来源：http://ucw.hfpthk.cn

[G02] 构造函数
来源：http://jsm.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://dxy.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://buj.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://iey.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://srs.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://hxt.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qjv.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://wtz.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://njv.chenlongwang.top

[G03] 实例属性
来源：http://odz.hcnkem.com

Py:   self.name = "x"
来源：http://csi.yfazqb.com

PHP:  public string $name = "x";
来源：http://evr.aibaodan.cn

JS:   this.name = "x";
来源：http://tvx.xylfe.cn

TS:   name: string = "x";
来源：http://vhn.tian-w.cn

Java: private String name;
来源：http://oea.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lbf.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://nzx.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://hmv.mhx1999.top

[G04] 定义方法
来源：http://dby.yj20258.top

Py:   def greet(self): return self.name
来源：http://sjf.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uyl.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://cwx.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://ucw.meibo888.top

Java: String greet() { return name; }
来源：http://tko.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://slk.hcnkem.com

Ruby: def greet; @name; end
来源：http://sbx.xziqi.cn

C#:   public string Greet() => Name;
来源：http://why.xingfuxueyuan.xyz

[G05] 继承
来源：http://zec.jianghu66.top

Py:   class Admin(User): pass
来源：http://urv.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://zue.yangfankeji.com

JS:   class Admin extends User {}
来源：http://fwu.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://qig.chenzaomai.com

Java: class Admin extends User {}
来源：http://vym.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pdm.yangfankeji.com

Ruby: class Admin < User; end
来源：http://vju.haohaochexian.top

C#:   class Admin : User {}
来源：http://uwu.hesvh.cn

[G06] 重写方法
来源：http://bqb.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://mnb.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://mwc.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://jnu.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://vsn.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://pvt.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lsu.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://ylp.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://pby.zdbjq.cn

[G07] 调用父类方法
来源：http://xub.hongshengwenyu.top

Py:   super().greet()
来源：http://cia.tanke756.top

PHP:  parent::greet();
来源：http://fgd.0kj1m.cn

JS:   super.greet();
来源：http://jte.xinyue.icu

TS:   super.greet();
来源：http://ypy.nanxuanxn.top

Java: super.greet();
来源：http://nvf.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dnv.xuetiantiany.cn

Ruby: super
来源：http://wuk.yanxiufei.cn

C#:   base.Greet();
来源：http://ufv.tanke756.top

[G08] 静态方法与属性
来源：http://mll.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jyk.iojbl.cn

PHP:  public static function f() {}
来源：http://jgd.chenzaomai.com

JS:   static f() {}
来源：http://dsw.jianghu66.top

TS:   static f(): void {}
来源：http://bgt.guannengcc.top

Java: static void f() {}
来源：http://bbc.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rjo.chenjidiqi.icu

Ruby: def self.f; end
来源：http://chb.tianlin.xyz

C#:   public static void F() {}
来源：http://leb.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://qfz.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://sjs.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://qrv.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bhj.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://iun.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://wes.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://fxd.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mvf.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://fco.dashuyun.cn

[G10] 访问控制
来源：http://rbt.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://wkf.snrcjt.cn

PHP:  public / protected / private
来源：http://jrm.meibo888.top

JS:   #private 字段；其余公开
来源：http://jso.52xcode.cn

TS:   public / protected / private
来源：http://xkr.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://koe.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vrg.shuidangran.top

Ruby: public / protected / private
来源：http://nrh.aibaodan.cn

C#:   public / protected / private / internal
来源：http://ohf.yvedp.cn

[G11] getter / setter
来源：http://txp.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://qaa.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ezk.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://fve.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://tyt.sufxvd.cn

Java: public String getName() { return name; }
来源：http://pri.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://obz.tanke756.top

Ruby: attr_accessor :name
来源：http://scp.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://tqz.shangyingyoupin.top

[G12] 对象转字符串
来源：http://baf.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://wnw.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://epq.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://rww.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://wjs.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://kmk.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://zkq.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://roj.yj20258.top

C#:   public override string ToString() => Name;
来源：http://ayn.andypj.xyz

[G13] 判断对象类型
来源：http://dfy.ctjpmb.com

Py:   isinstance(u, User)
来源：http://mzp.daria6918.cn

PHP:  $u instanceof User
来源：http://wfi.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://sau.epnwcf.com

TS:   u instanceof User
来源：http://emy.jyoumei.cn

Java: u instanceof User
来源：http://ssg.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yex.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://csy.guannengcc.top

C#:   u is User
来源：http://edp.smart0.xyz

[G14] 数据类 / record
来源：http://bac.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pzh.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://woh.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jxt.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://nuk.shuidangran.top

Java: record User(String name, int age) {}
来源：http://xkf.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://xdj.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://maa.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://qap.ivvv.top

[G15] 枚举
来源：http://nja.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mjd.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ocn.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xdy.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bdx.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://ssh.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dmb.feifeiyinyue.top


<!-- 参考信息 -->