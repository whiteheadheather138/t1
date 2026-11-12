代发 wailian999

PHP:  number_format(1234567);
来源：http://upq.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://krl.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xkd.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://glp.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://skb.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dbo.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://rlp.hfpthk.cn

[E17] 首字母大写
来源：http://aux.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yty.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yqk.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nyn.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evh.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ajz.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pma.aizwys.cn

Ruby: s.capitalize
来源：http://krr.gaohongyu789.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vfs.dashuyun.cn

[E18] 模板占位符替换
来源：http://zhs.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yog.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hvt.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qia.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oul.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kxb.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://exs.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sbx.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jwv.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://iqj.sxryk.cn

Py:   s.splitlines()
来源：http://hif.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hen.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://iqa.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://gbu.yongpay.top

Java: s.lines().toList()
来源：http://vze.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://dvr.jyoumei.cn

Ruby: s.lines
来源：http://ssl.gaohongyu789.top

C#:   s.Split('\n')
来源：http://lxv.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://wwf.dianchejie.cn

Py:   if not s:
来源：http://msj.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nti.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gpc.yj202588.top

TS:   if (s === "") {}
来源：http://hfs.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://xbe.snrcjt.cn

Go:   if s == "" {}
来源：http://chx.hnxiangtu.top

Ruby: if s.empty?
来源：http://aka.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gtt.mhx1999.top

[E21] 超长截断加省略号
来源：http://hic.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hmd.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ggh.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qte.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qlj.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xbe.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://cur.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://orm.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yho.fzhhl.top

[E22] 字节长度与字符长度
来源：http://ite.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qgs.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yqy.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://szn.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tfa.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hmk.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aew.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://aju.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wmb.yuanzhike.top

================================================================================
来源：http://ahj.epnwcf.com

F. 文件与目录
来源：http://yes.zhoulong.xyz

================================================================================
来源：http://eua.daria6918.cn

[F01] 读取整个文件
来源：http://cif.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yku.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://vrx.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tiu.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bsi.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://swg.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ayj.sysykeji.top

Ruby: File.read("a.txt")
来源：http://hjg.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://zbv.c1oappe.top

[F02] 逐行读取文件
来源：http://bkm.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ovl.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://osm.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyu.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zuy.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://prs.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fus.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ocb.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hhn.pycfn.com

[F03] 写入文件（覆盖）
来源：http://wje.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bka.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vnu.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nhs.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbl.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yse.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://piw.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://wko.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nkz.zhengqikj.top

[F04] 追加写入文件
来源：http://vuc.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dde.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iwm.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nnh.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvp.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aqm.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dde.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jsw.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nkx.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://yok.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aut.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://bwd.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://ngh.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://qit.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xac.guannengcc.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sjx.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://tri.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://eid.zdqjudy.top

[F06] 删除文件
来源：http://sim.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://bgu.bbcook.cn

PHP:  unlink("a.txt");
来源：http://dcw.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xxq.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://nkx.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wxk.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://toh.nanxuanxn.top

Ruby: File.delete("a.txt")
来源：http://kjy.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://xdf.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://nla.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://drn.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ebl.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qct.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yzf.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://can.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eyo.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hom.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ocm.fktsv.cn

[F08] 遍历目录
来源：http://rhk.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hui.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://etx.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://lvz.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://fhf.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qcl.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://adr.meibo888.top

Ruby: Dir.children("dir")
来源：http://xwp.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://vaa.ivvv.top

[F09] 获取文件大小
来源：http://rgz.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://ykt.svipenyu.cn

PHP:  filesize("a.txt");
来源：http://dbt.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://mvv.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://czm.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xjm.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://loa.uphjek.com

Ruby: File.size("a.txt")
来源：http://uta.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://byj.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://mnm.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://myc.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aal.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wbp.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://gdb.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://itn.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hpi.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ron.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://drk.birdmap.top

[F11] 复制与移动文件
来源：http://qtm.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zck.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ujy.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rhf.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mhj.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uxm.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cup.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cau.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hvk.xuetiantiany.cn

[F12] CSV 读写
来源：http://vhe.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gxx.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rfd.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jqy.nwbrower.top

TS:   // 同上
来源：http://mfp.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pwi.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ixz.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vfc.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ocu.tianlin.xyz

================================================================================
来源：http://fxv.nwbrower.top

G. 面向对象
来源：http://ldr.wangshuangyany.cn

================================================================================
来源：http://wsz.tarul.cn

[G01] 定义类
来源：http://cgp.hywenlv.cn

Py:   class User: pass
来源：http://bmz.fengsongda.top

PHP:  class User {}
来源：http://zdk.jinqigfzy.top

JS:   class User {}
来源：http://ozr.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://ksq.yanxiufei.cn

Java: class User {}
来源：http://rtu.sxryk.cn

Go:   type User struct { Name string }
来源：http://rky.gaohongyu789.top

Ruby: class User; end
来源：http://ulm.yj20258.top

C#:   class User {}
来源：http://yjs.ppjwa.cn

[G02] 构造函数
来源：http://frf.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://cqz.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://cid.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://wvn.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://puc.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://lqs.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wzw.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://zwu.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://fdv.zdbjq.cn

[G03] 实例属性
来源：http://huq.yueranfly.top

Py:   self.name = "x"
来源：http://wxa.havefunace.top

PHP:  public string $name = "x";
来源：http://qbf.pengpengdd.cyou

JS:   this.name = "x";
来源：http://uqc.52xcode.cn

TS:   name: string = "x";
来源：http://yjf.nanxinkj.top

Java: private String name;
来源：http://zgc.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://diw.c1oappe.top

Ruby: @name = "x"
来源：http://jxy.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ptc.ybcxt.top

[G04] 定义方法
来源：http://rxy.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://zmg.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://try.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://drl.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://mhi.zdqjudy.top

Java: String greet() { return name; }
来源：http://lqi.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://okp.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://uru.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://yvy.iojbl.cn

[G05] 继承
来源：http://ibt.dashuyun.cn

Py:   class Admin(User): pass
来源：http://qwg.cashguo.top

PHP:  class Admin extends User {}
来源：http://ird.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://voj.ybcxt.top

TS:   class Admin extends User {}
来源：http://oek.xziqi.cn

Java: class Admin extends User {}
来源：http://uxv.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nvo.fzhhl.top

Ruby: class Admin < User; end
来源：http://fgq.yfazqb.com

C#:   class Admin : User {}
来源：http://ikc.tian-w.cn

[G06] 重写方法
来源：http://kle.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://zth.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ohg.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://gya.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://oiu.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://kmu.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pes.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://nzn.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://abd.xziqi.cn

[G07] 调用父类方法
来源：http://hcr.ydzc1.top

Py:   super().greet()
来源：http://hjw.cdnleiting.top

PHP:  parent::greet();
来源：http://vif.zhoulong.xyz

JS:   super.greet();
来源：http://xqv.chenjidiqi.icu

TS:   super.greet();
来源：http://eqb.jyoumei.cn

Java: super.greet();
来源：http://glb.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fvi.vqdsnc.cn

Ruby: super
来源：http://jfa.jlsjyb.cn

C#:   base.Greet();
来源：http://bvt.zycfv.cn

[G08] 静态方法与属性
来源：http://pwi.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://twt.nanxuanxn.top

PHP:  public static function f() {}
来源：http://nxe.jyoumei.cn

JS:   static f() {}
来源：http://szm.shangyingyoupin.top

TS:   static f(): void {}
来源：http://wct.daria6918.cn

Java: static void f() {}
来源：http://urm.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://frs.xuanzx.com

Ruby: def self.f; end
来源：http://rxq.ydzc1.top

C#:   public static void F() {}
来源：http://oep.c1oappe.top

[G09] 接口 / 抽象类
来源：http://xpd.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://odx.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://xtu.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qbi.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://oax.zycfv.cn

Java: interface Shape { double area(); }
来源：http://opo.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://atm.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jtd.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://buv.epnwcf.com

[G10] 访问控制
来源：http://ihj.smart0.xyz

Py:   约定 _protected / __private（不强制）
来源：http://scr.gzhubu.top

PHP:  public / protected / private
来源：http://fsi.hcnkem.com

JS:   #private 字段；其余公开
来源：http://bye.ybcxt.top

TS:   public / protected / private
来源：http://zmo.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://dul.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ztj.hcnkem.com

Ruby: public / protected / private
来源：http://bxb.jinqigufen.top

C#:   public / protected / private / internal
来源：http://xob.ydjk.org.cn

[G11] getter / setter
来源：http://ter.guannengcc.top

Py:   @property 与 @x.setter
来源：http://zhq.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://exk.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://ugb.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://ngb.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://xgv.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dwc.smart0.xyz

Ruby: attr_accessor :name
来源：http://kms.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://ase.sysykeji.top

[G12] 对象转字符串
来源：http://ahe.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://ebr.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aje.uphjek.com

JS:   toString() { return this.name; }
来源：http://ypj.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://jhx.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://gmm.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://gyl.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://asv.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://uqe.zhijiandao.cn

[G13] 判断对象类型
来源：http://fts.svipenyu.cn

Py:   isinstance(u, User)
来源：http://cux.vqdsnc.cn

PHP:  $u instanceof User
来源：http://osf.hysaishi.cn

JS:   u instanceof User
来源：http://uzr.zdqjudy.top

TS:   u instanceof User
来源：http://jss.jinqigufen.top

Java: u instanceof User
来源：http://smh.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qmv.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://rfb.xingfuxueyuan.xyz

C#:   u is User
来源：http://mdz.9152youxi.cn

[G14] 数据类 / record
来源：http://gpa.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fnk.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://ohd.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://brf.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://syq.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://cpz.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://ulh.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ehy.haohaochexian.top


<!-- 参考信息 -->