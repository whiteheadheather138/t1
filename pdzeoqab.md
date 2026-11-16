代发 wailian999

[E18] 模板占位符替换
来源：http://ure.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gkp.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qtc.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dbw.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qti.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mdk.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mnj.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ehd.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gsn.xinyue.icu

[E19] 多行文本按行拆分
来源：http://vqx.cheryme.top

Py:   s.splitlines()
来源：http://mvp.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mus.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://vta.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://nuk.sysykeji.top

Java: s.lines().toList()
来源：http://wst.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://iic.316326.xyz

Ruby: s.lines
来源：http://tnu.vqdsnc.cn

C#:   s.Split('\n')
来源：http://agc.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://bnq.epnwcf.com

Py:   if not s:
来源：http://xuh.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qff.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dnm.cdnleiting.top

TS:   if (s === "") {}
来源：http://nni.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://goi.hfpthk.cn

Go:   if s == "" {}
来源：http://uym.yonumen.top

Ruby: if s.empty?
来源：http://vwz.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tek.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://oin.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ixa.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oei.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jle.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://men.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ceh.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://xrk.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yer.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lds.52xcode.cn

[E22] 字节长度与字符长度
来源：http://adt.xuetiantiany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hzm.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rpr.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qby.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mlm.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yxk.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sdf.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://alp.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://acn.zhaomingkeji.xyz

================================================================================
来源：http://acv.redwolf501.top

F. 文件与目录
来源：http://vlv.hcnkem.com

================================================================================
来源：http://wbz.epnwcf.com

[F01] 读取整个文件
来源：http://nlx.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hqc.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://pkf.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wgp.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vvf.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pvo.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uyn.xylfe.cn

Ruby: File.read("a.txt")
来源：http://lve.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://ats.hnxiangtu.top

[F02] 逐行读取文件
来源：http://ilv.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mbt.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ftm.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aea.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xxo.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jep.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wjz.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zdt.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://krz.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://aeo.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xrl.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dkj.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yea.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sjk.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nox.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://geg.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://vhu.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zkh.ybcxt.top

[F04] 追加写入文件
来源：http://mvt.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rmd.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mog.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jgo.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xoo.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://unw.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://unk.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rgl.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kht.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://jsp.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rqc.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://uvl.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://tqy.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://sol.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://upy.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://otj.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://ght.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://ihq.9152youxi.cn

[F06] 删除文件
来源：http://gds.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://xop.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://beq.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://mgi.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://izx.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yzd.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://ans.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://lkx.yj202588.top

C#:   File.Delete("a.txt");
来源：http://mug.fengsongda.top

[F07] 创建目录（含多级）
来源：http://poe.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pjy.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rti.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhv.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yge.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ldt.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gar.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://llb.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zlr.shanyushiyangtech.top

[F08] 遍历目录
来源：http://awx.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://jzq.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dnr.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://ykt.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://kiz.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tmq.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cel.guannengcc.top

Ruby: Dir.children("dir")
来源：http://gwb.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://xrj.yonumen.top

[F09] 获取文件大小
来源：http://wpx.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://ntb.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://pdo.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://oel.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://uww.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ssg.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xhy.havefunace.top

Ruby: File.size("a.txt")
来源：http://tng.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://hlm.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://gqm.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hlw.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ary.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uyl.pycfn.com

TS:   path.extname("a.txt")
来源：http://ocf.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://azo.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vmf.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gci.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oxp.9152youxi.cn

[F11] 复制与移动文件
来源：http://kbw.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pbm.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hyr.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hsj.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ibq.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uja.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xqd.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bvc.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dcw.kuanghao11.cn

[F12] CSV 读写
来源：http://vdk.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yvy.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eir.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://juu.nwbrower.top

TS:   // 同上
来源：http://hdt.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xao.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hmb.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dkz.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qhb.fanxiaobao.xyz

================================================================================
来源：http://efo.yonumen.top

G. 面向对象
来源：http://yht.shanyushiyangkeji.top

================================================================================
来源：http://ejd.ctjpmb.com

[G01] 定义类
来源：http://ssi.gzhubu.top

Py:   class User: pass
来源：http://ehg.zdbjq.cn

PHP:  class User {}
来源：http://hha.pengpengdd.cyou

JS:   class User {}
来源：http://axs.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://yys.fzhhl.top

Java: class User {}
来源：http://ewk.tian-w.cn

Go:   type User struct { Name string }
来源：http://mot.tianlin.xyz

Ruby: class User; end
来源：http://ous.zdqjudy.top

C#:   class User {}
来源：http://pmv.fktsv.cn

[G02] 构造函数
来源：http://stt.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://jex.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://yla.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://hts.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://qem.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://dvp.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fpn.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://xje.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://qiw.nanxinkj.top

[G03] 实例属性
来源：http://kim.yonumen.top

Py:   self.name = "x"
来源：http://wgv.316326.xyz

PHP:  public string $name = "x";
来源：http://bgb.xuetiantiany.cn

JS:   this.name = "x";
来源：http://neo.kuanghao11.cn

TS:   name: string = "x";
来源：http://jyo.hysaishi.cn

Java: private String name;
来源：http://zbw.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zeu.316326.xyz

Ruby: @name = "x"
来源：http://lpk.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://qdr.iojbl.cn

[G04] 定义方法
来源：http://jli.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://azw.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ofc.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://nql.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://vrg.hywenlv.cn

Java: String greet() { return name; }
来源：http://vvp.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jut.bbcook.cn

Ruby: def greet; @name; end
来源：http://pxj.hammf.cn

C#:   public string Greet() => Name;
来源：http://lkj.zhiwuduotai.top

[G05] 继承
来源：http://ecz.316326.xyz

Py:   class Admin(User): pass
来源：http://cqp.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://lbu.hesvh.cn

JS:   class Admin extends User {}
来源：http://qtu.316326.xyz

TS:   class Admin extends User {}
来源：http://jjo.tanke756.top

Java: class Admin extends User {}
来源：http://ndv.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ppb.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://sgi.hfpthk.cn

C#:   class Admin : User {}
来源：http://std.jianghu66.top

[G06] 重写方法
来源：http://pgl.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://bbw.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bup.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://fjy.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://dqz.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://fxw.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eli.hammf.cn

Ruby: def greet; "admin"; end
来源：http://zde.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://kre.xziqi.cn

[G07] 调用父类方法
来源：http://xif.iojbl.cn

Py:   super().greet()
来源：http://hxo.yj20258888.top

PHP:  parent::greet();
来源：http://cor.yanxiufei.cn

JS:   super.greet();
来源：http://bki.shanyushiyangkeji.top

TS:   super.greet();
来源：http://csa.snrcjt.cn

Java: super.greet();
来源：http://mzy.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://phb.guowangkeji.top

Ruby: super
来源：http://kla.hnqzz.top

C#:   base.Greet();
来源：http://nhf.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://gcl.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fjf.jlsjyb.cn

PHP:  public static function f() {}
来源：http://hri.sxryk.cn

JS:   static f() {}
来源：http://syf.guowangkeji.top

TS:   static f(): void {}
来源：http://rdy.shuidangran.top

Java: static void f() {}
来源：http://ocx.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bvv.vqdsnc.cn

Ruby: def self.f; end
来源：http://lnr.zhengqikj.top

C#:   public static void F() {}
来源：http://cuc.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://yro.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://ruq.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://zbz.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ieo.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://pys.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://rqo.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://eof.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wvr.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://npx.316326.xyz

[G10] 访问控制
来源：http://jbb.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://qup.wangdashe.top

PHP:  public / protected / private
来源：http://abb.c1oappe.top

JS:   #private 字段；其余公开
来源：http://npd.fktsv.cn

TS:   public / protected / private
来源：http://bke.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://toq.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gzb.yanxiufei.cn

Ruby: public / protected / private
来源：http://qdf.zycfv.cn

C#:   public / protected / private / internal
来源：http://btj.chenjidiqi.icu

[G11] getter / setter
来源：http://dvs.bjfxy.top

Py:   @property 与 @x.setter
来源：http://ueb.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xqb.fehbvm.com

JS:   get name() { return this._name; }
来源：http://toy.sufxvd.cn

TS:   get name(): string { return this._name; }
来源：http://cjr.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://jqa.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://qhv.redwolf501.top

Ruby: attr_accessor :name
来源：http://rfs.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://fof.snrcjt.cn

[G12] 对象转字符串
来源：http://peq.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://dqu.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rdd.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://lko.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://soo.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://fyo.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vzu.hcnkem.com

Ruby: def to_s; @name; end
来源：http://nyz.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://xfh.zhoulong.xyz

[G13] 判断对象类型
来源：http://prq.jqgfzy.top

Py:   isinstance(u, User)
来源：http://biz.xuanzx.com

PHP:  $u instanceof User
来源：http://ayk.ctjpmb.com

JS:   u instanceof User
来源：http://ued.cdnleiting.top

TS:   u instanceof User
来源：http://rmx.zhoulong.xyz

Java: u instanceof User
来源：http://gye.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qbv.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://nde.shangyingyoupin.top

C#:   u is User
来源：http://cqz.dashuyun.cn

[G14] 数据类 / record
来源：http://xgl.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ftt.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://zrv.ivvv.top

JS:   // 无内置：普通类或对象字面量
来源：http://ift.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://lcm.guannengcc.top

Java: record User(String name, int age) {}
来源：http://vtm.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://krc.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mna.uphjek.com

C#:   record User(string Name, int Age);
来源：http://upv.vqdsnc.cn

[G15] 枚举
来源：http://bpy.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hbt.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dbd.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yiq.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uqa.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://sgo.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gbk.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://zci.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pax.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://vtb.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aee.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://ybv.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://xgg.nwbrower.top

TS:   Object.entries(obj)
来源：http://bop.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pss.hcnkem.com


<!-- 参考信息 -->