代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rxc.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gdv.0kj1m.cn

Ruby: s.capitalize
来源：http://uet.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nyu.ivvv.top

[E18] 模板占位符替换
来源：http://pku.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://adz.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ndk.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qrn.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rzk.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://anc.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nqg.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vte.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://slf.sxryk.cn

[E19] 多行文本按行拆分
来源：http://sep.wangdashe.top

Py:   s.splitlines()
来源：http://vji.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://swe.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://weu.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://wah.yanxiufei.cn

Java: s.lines().toList()
来源：http://eef.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://xvb.guowangkeji.top

Ruby: s.lines
来源：http://luh.ivvv.top

C#:   s.Split('\n')
来源：http://wre.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://hkf.sxryk.cn

Py:   if not s:
来源：http://naf.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jej.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zzd.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://ktv.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://ueu.yj20258888.top

Go:   if s == "" {}
来源：http://uss.cashguo.top

Ruby: if s.empty?
来源：http://zan.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cph.yuxming.cn

[E21] 超长截断加省略号
来源：http://knq.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dwr.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cpn.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mae.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zpc.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ojc.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://njz.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qfc.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cra.cucudq.cn

[E22] 字节长度与字符长度
来源：http://meo.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://efi.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tcp.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wcc.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://czt.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uxz.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://smr.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://pri.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://san.hcnkem.com

================================================================================
来源：http://jcb.xinyue.icu

F. 文件与目录
来源：http://fms.fengsongda.top

================================================================================
来源：http://wkf.gzhubu.top

[F01] 读取整个文件
来源：http://weh.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ozf.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://qdt.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ams.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xse.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xkc.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lsg.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://gjo.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://wch.xuanzx.com

[F02] 逐行读取文件
来源：http://yao.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hjp.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://scj.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qwb.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aoc.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ley.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nhi.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vve.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ilc.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://aop.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rdg.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hef.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zti.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pui.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hdc.cashguo.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://apa.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://vnj.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lit.zhiwuduotai.top

[F04] 追加写入文件
来源：http://vwn.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sdz.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rcz.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wzp.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kew.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rvu.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bcr.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://npn.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nnx.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://nrv.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wfd.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://uur.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://exg.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://ckr.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fpg.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qzk.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://xkn.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://iuf.sysykeji.top

[F06] 删除文件
来源：http://dop.xuanzx.com

Py:   os.remove("a.txt")
来源：http://gko.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://aow.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://hzk.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://kaq.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mqy.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://elz.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://khv.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://qcb.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://itx.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://npg.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yzd.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eap.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://emc.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://utl.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjv.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tca.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qwx.tanke756.top

[F08] 遍历目录
来源：http://pbc.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://puj.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rhc.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://loe.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://vtq.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tiv.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cxf.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://qzp.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://csf.sweek.top

[F09] 获取文件大小
来源：http://alm.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://ymi.xuanzx.com

PHP:  filesize("a.txt");
来源：http://beu.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://ysr.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://arh.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://ekx.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nty.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://aph.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://jha.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://tpb.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gfx.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wjx.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://akt.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://xst.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kpq.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iwd.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vod.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kna.yvedp.cn

[F11] 复制与移动文件
来源：http://tqy.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lvl.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qsd.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kke.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gtn.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mgg.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ete.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pbk.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eqm.yueranfly.top

[F12] CSV 读写
来源：http://eaz.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://igw.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hvk.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vne.ydzc1.top

TS:   // 同上
来源：http://okc.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dir.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://drw.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hij.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://yax.zhongyouzk.top

================================================================================
来源：http://qzy.fengsongda.top

G. 面向对象
来源：http://hhl.birdmap.top

================================================================================
来源：http://xcd.fanxiaobao.xyz

[G01] 定义类
来源：http://gja.tianlin.xyz

Py:   class User: pass
来源：http://ezb.xziqi.cn

PHP:  class User {}
来源：http://cdv.jianghu66.top

JS:   class User {}
来源：http://nmb.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://upq.cashguo.top

Java: class User {}
来源：http://jhd.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://oqa.yangfankeji.com

Ruby: class User; end
来源：http://kpx.sysykeji.top

C#:   class User {}
来源：http://pdq.andypj.xyz

[G02] 构造函数
来源：http://xtu.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://hlp.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://ony.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://aom.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://qdz.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://jlh.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dtv.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://ppc.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://vrm.jqgfzy.top

[G03] 实例属性
来源：http://vym.gzhubu.top

Py:   self.name = "x"
来源：http://ppz.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://uqp.nanxuanxn.top

JS:   this.name = "x";
来源：http://gub.redwolf501.top

TS:   name: string = "x";
来源：http://dad.epnwcf.com

Java: private String name;
来源：http://ppz.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ufi.tarul.cn

Ruby: @name = "x"
来源：http://ixe.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://exm.hnxiangtu.top

[G04] 定义方法
来源：http://dcv.yfazqb.com

Py:   def greet(self): return self.name
来源：http://spz.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sup.yj20258.top

JS:   greet() { return this.name; }
来源：http://wnl.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://lxv.ppjwa.cn

Java: String greet() { return name; }
来源：http://mpg.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://atw.gogol.net.cn

Ruby: def greet; @name; end
来源：http://awb.bbcook.cn

C#:   public string Greet() => Name;
来源：http://efc.hfpthk.cn

[G05] 继承
来源：http://wsv.tarul.cn

Py:   class Admin(User): pass
来源：http://bkn.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://mjo.haohaochexian.top

JS:   class Admin extends User {}
来源：http://vuq.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://moo.xziqi.cn

Java: class Admin extends User {}
来源：http://ctp.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://epa.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://ytj.yvedp.cn

C#:   class Admin : User {}
来源：http://goh.fzhhl.top

[G06] 重写方法
来源：http://rjc.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://ryl.tian-w.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dwx.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://cwz.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://pgv.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://fkp.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://byv.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://aek.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://vlx.xziqi.cn

[G07] 调用父类方法
来源：http://dje.yvedp.cn

Py:   super().greet()
来源：http://gsb.cheryme.top

PHP:  parent::greet();
来源：http://dak.shzxlz.cn

JS:   super.greet();
来源：http://tdk.vehdjk.com

TS:   super.greet();
来源：http://fmb.cqqwz.cn

Java: super.greet();
来源：http://soq.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oot.guannengcc.top

Ruby: super
来源：http://lsz.xuetiantiany.cn

C#:   base.Greet();
来源：http://brz.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://cvu.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ewr.jqgfzy.top

PHP:  public static function f() {}
来源：http://dhy.zdqjudy.top

JS:   static f() {}
来源：http://gij.wangdashe.top

TS:   static f(): void {}
来源：http://qnp.guannengcc.top

Java: static void f() {}
来源：http://uya.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://unj.cqqwz.cn

Ruby: def self.f; end
来源：http://bir.tarul.cn

C#:   public static void F() {}
来源：http://buj.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://qsb.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://mnk.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://pnr.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lkq.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://uho.xuanzx.com

Java: interface Shape { double area(); }
来源：http://oty.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://nel.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lte.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://suj.cqqwz.cn

[G10] 访问控制
来源：http://ewb.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://apf.zhoulong.xyz

PHP:  public / protected / private
来源：http://djx.uphjek.com

JS:   #private 字段；其余公开
来源：http://eww.sysykeji.top

TS:   public / protected / private
来源：http://ddb.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://cpn.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://exa.daria6918.cn

Ruby: public / protected / private
来源：http://dta.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://wzo.epnwcf.com

[G11] getter / setter
来源：http://jve.xuanzx.com

Py:   @property 与 @x.setter
来源：http://xzg.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://lhu.yj20258888.top

JS:   get name() { return this._name; }
来源：http://mlb.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://mih.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://emj.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://nnz.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://rjv.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://fmy.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://syy.havefunace.top

Py:   def __str__(self): return self.name
来源：http://vxf.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aym.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://zzd.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://akt.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://ggu.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zyn.xuanzx.com

Ruby: def to_s; @name; end
来源：http://nib.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://pqv.0kj1m.cn

[G13] 判断对象类型
来源：http://cny.yongpay.top

Py:   isinstance(u, User)
来源：http://jbb.fktsv.cn

PHP:  $u instanceof User
来源：http://zqw.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://mvv.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://dut.ydjk.org.cn

Java: u instanceof User
来源：http://gmd.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://xue.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://ppc.gaohongyu789.top

C#:   u is User
来源：http://ska.zhijiandao.cn

[G14] 数据类 / record
来源：http://qij.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wgv.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://cex.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://hav.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://fea.redwolf501.top

Java: record User(String name, int age) {}
来源：http://jsp.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://wbb.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vgw.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://pqf.svipenyu.cn

[G15] 枚举
来源：http://lbk.dashuyun.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mca.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rtl.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fjn.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dlq.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://wmu.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gfk.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://pey.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://slm.gaohongyu789.top

[G16] 对象转数组 / 字典
来源：http://ihx.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dsu.hcnkem.com


<!-- 参考信息 -->