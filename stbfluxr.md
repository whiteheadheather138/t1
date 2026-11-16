代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ywa.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ldb.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://hpr.tianlin.xyz

[E17] 首字母大写
来源：http://oxu.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://voq.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://khb.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qon.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kat.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://orb.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tnu.jlsjyb.cn

Ruby: s.capitalize
来源：http://fsi.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://egj.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://kkz.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tse.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gnd.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ago.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uti.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://syy.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cln.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zcg.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ecq.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://xvq.feifeiyinyue.top

Py:   s.splitlines()
来源：http://mym.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eex.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://mce.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://mks.guannengcc.top

Java: s.lines().toList()
来源：http://tlf.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://xzi.xuetiantiany.cn

Ruby: s.lines
来源：http://twa.kuanghao11.cn

C#:   s.Split('\n')
来源：http://xyp.hcnkem.com

[E20] 判断字符串是否为空
来源：http://zgb.mhx1999.top

Py:   if not s:
来源：http://bgt.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uxb.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hhv.hammf.cn

TS:   if (s === "") {}
来源：http://jfz.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://mvs.nanxinkj.top

Go:   if s == "" {}
来源：http://xzp.sysykeji.top

Ruby: if s.empty?
来源：http://ora.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://azs.hysaishi.cn

[E21] 超长截断加省略号
来源：http://hql.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://igg.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aan.feifeiyinyue.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wqj.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wej.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dsk.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://ogr.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sji.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jop.ydzc1.top

[E22] 字节长度与字符长度
来源：http://zpn.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oky.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qmy.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ceb.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xpe.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ccu.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wxj.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://ldp.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ipg.cashguo.top

================================================================================
来源：http://gpt.316326.xyz

F. 文件与目录
来源：http://tmr.xziqi.cn

================================================================================
来源：http://ikf.uphjek.com

[F01] 读取整个文件
来源：http://eeh.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ius.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://usu.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://evy.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ykm.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rfq.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tmv.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://osi.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://mxf.gotoacloud.top

[F02] 逐行读取文件
来源：http://mpy.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lro.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://azp.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://duz.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyx.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ygp.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bhk.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mju.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uee.yj20258.top

[F03] 写入文件（覆盖）
来源：http://svz.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://taq.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://kgc.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ybs.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ciq.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hqy.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ocq.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://jep.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://suw.sxryk.cn

[F04] 追加写入文件
来源：http://soq.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ibr.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gih.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mhx.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://huh.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gon.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ugs.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sws.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jxe.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://mpl.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yej.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://dku.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://rhn.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://czm.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vyc.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rzp.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://oza.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://ioa.cqqwz.cn

[F06] 删除文件
来源：http://bir.aizwys.cn

Py:   os.remove("a.txt")
来源：http://qni.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://leh.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://jpr.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://zqv.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pbf.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://ldk.havefunace.top

Ruby: File.delete("a.txt")
来源：http://rat.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://cev.birdmap.top

[F07] 创建目录（含多级）
来源：http://hub.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fyn.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dxn.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://idc.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nfi.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uvw.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fer.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hkd.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rea.ctjpmb.com

[F08] 遍历目录
来源：http://jly.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eqt.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jsa.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://cdv.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://zjr.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iqg.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kqi.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://rgy.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://zda.ybcxt.top

[F09] 获取文件大小
来源：http://mpi.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://sql.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://hcc.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://xyq.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://dds.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://znt.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mjl.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://lyx.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://vtu.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://xyt.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://war.yj202588.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xqe.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ifk.smart0.xyz

TS:   path.extname("a.txt")
来源：http://gtk.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bcb.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xhw.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sny.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cgv.birdmap.top

[F11] 复制与移动文件
来源：http://crl.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hzr.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jlh.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://smo.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xvg.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jiw.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ong.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qmh.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rae.pycfn.com

[F12] CSV 读写
来源：http://oei.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fcu.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mek.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cec.zhengqikj.top

TS:   // 同上
来源：http://bma.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uhu.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://slg.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iji.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ofw.yanxiufei.cn

================================================================================
来源：http://fhq.shanyushiyangtech.top

G. 面向对象
来源：http://aau.fktsv.cn

================================================================================
来源：http://dwt.havefunace.top

[G01] 定义类
来源：http://vik.epnwcf.com

Py:   class User: pass
来源：http://mat.jyoumei.cn

PHP:  class User {}
来源：http://fdx.smart0.xyz

JS:   class User {}
来源：http://tfn.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://alc.aizwys.cn

Java: class User {}
来源：http://qiu.ydzc1.top

Go:   type User struct { Name string }
来源：http://erb.jianghu66.top

Ruby: class User; end
来源：http://xuf.redwolf501.top

C#:   class User {}
来源：http://pog.yangfankeji.com

[G02] 构造函数
来源：http://cqf.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://nyc.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://bls.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://apf.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://xms.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://zmh.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ikw.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://djv.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://jxe.jinqigufen.top

[G03] 实例属性
来源：http://cyq.xuetiantiany.cn

Py:   self.name = "x"
来源：http://zgu.shzxlz.cn

PHP:  public string $name = "x";
来源：http://aji.hnqzz.top

JS:   this.name = "x";
来源：http://bek.feifeiyinyue.top

TS:   name: string = "x";
来源：http://hpo.zdqjudy.top

Java: private String name;
来源：http://tan.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pae.sjlbkw.cn

Ruby: @name = "x"
来源：http://krj.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://rcp.nwbrower.top

[G04] 定义方法
来源：http://neu.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://qfd.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nhq.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://bij.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://rto.epnwcf.com

Java: String greet() { return name; }
来源：http://bnl.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://djt.fktsv.cn

Ruby: def greet; @name; end
来源：http://wdj.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://ivd.shangyingyoupin.top

[G05] 继承
来源：http://wsk.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://kcn.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://uhz.yuxming.cn

JS:   class Admin extends User {}
来源：http://azz.zdqjudy.top

TS:   class Admin extends User {}
来源：http://shz.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://cpc.cashguo.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wvm.yfazqb.com

Ruby: class Admin < User; end
来源：http://ryt.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://fgh.jiagoushi.top

[G06] 重写方法
来源：http://gmn.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://euq.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hrc.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://tem.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://wah.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://giv.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xsx.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://frs.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://jzh.xinyue.icu

[G07] 调用父类方法
来源：http://bng.yangfankeji.com

Py:   super().greet()
来源：http://rki.quarkkingdee.top

PHP:  parent::greet();
来源：http://sza.ydzc1.top

JS:   super.greet();
来源：http://pln.jqgufenzy.top

TS:   super.greet();
来源：http://tyx.shanyushiyangtech.top

Java: super.greet();
来源：http://jre.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lsx.ctjpmb.com

Ruby: super
来源：http://ggw.cashguo.top

C#:   base.Greet();
来源：http://uhp.ybcxt.top

[G08] 静态方法与属性
来源：http://etg.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mzq.jqgufenzy.top

PHP:  public static function f() {}
来源：http://efq.hongshengwenyu.top

JS:   static f() {}
来源：http://nik.daria6918.cn

TS:   static f(): void {}
来源：http://jrb.ywan-chungtsiang.top

Java: static void f() {}
来源：http://qgp.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://odq.nanxinkj.top

Ruby: def self.f; end
来源：http://tfg.aizwys.cn

C#:   public static void F() {}
来源：http://hua.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://ayl.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://jls.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://bwc.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fsx.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://fki.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://cic.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://omk.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yxo.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://jwu.shangyingyoupin.top

[G10] 访问控制
来源：http://rtw.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://bcl.daxiang520.top

PHP:  public / protected / private
来源：http://pxh.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://tpi.xziqi.cn

TS:   public / protected / private
来源：http://ppa.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://dhw.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dfb.gzhubu.top

Ruby: public / protected / private
来源：http://wlk.xziqi.cn

C#:   public / protected / private / internal
来源：http://kbz.0kj1m.cn

[G11] getter / setter
来源：http://ujm.gzhubu.top

Py:   @property 与 @x.setter
来源：http://lwq.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qkq.xziqi.cn

JS:   get name() { return this._name; }
来源：http://gng.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://otu.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://vvb.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://kxa.pycfn.com

Ruby: attr_accessor :name
来源：http://nwa.yuxming.cn

C#:   public string Name { get; set; }
来源：http://jqk.nanxuanxn.top

[G12] 对象转字符串
来源：http://ogq.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://gfd.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pit.yuxming.cn

JS:   toString() { return this.name; }
来源：http://dpm.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://vei.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://iql.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nvs.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://qlh.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://oyf.fktsv.cn

[G13] 判断对象类型
来源：http://xzg.0kj1m.cn

Py:   isinstance(u, User)
来源：http://zbp.jyoumei.cn

PHP:  $u instanceof User
来源：http://uov.hesvh.cn

JS:   u instanceof User
来源：http://tat.shuidangran.top

TS:   u instanceof User
来源：http://ctu.jinqigufen.top

Java: u instanceof User
来源：http://mis.wangdashe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rlm.tanke756.top

Ruby: u.is_a?(User)
来源：http://ypp.tianlin.xyz

C#:   u is User
来源：http://nxg.sysykeji.top

[G14] 数据类 / record
来源：http://kai.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dxv.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://dbp.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://ycl.meibo888.top

TS:   type User = { name: string; age: number };
来源：http://wda.bbcook.cn

Java: record User(String name, int age) {}
来源：http://rkl.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://nzc.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rqn.tanke756.top

C#:   record User(string Name, int Age);
来源：http://zdt.nwbrower.top

[G15] 枚举
来源：http://pcu.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lts.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zfn.nwbrower.top


<!-- 参考信息 -->