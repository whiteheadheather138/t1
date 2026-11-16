代发 wailian999

PHP:  number_format(1234567);
来源：http://qjp.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uwt.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://eyv.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://msf.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wxo.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://has.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://xhy.nwbrower.top

[E17] 首字母大写
来源：http://rjk.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://skb.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wef.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ndi.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qms.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sun.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://psf.daxiang520.top

Ruby: s.capitalize
来源：http://qlb.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://msp.uphjek.com

[E18] 模板占位符替换
来源：http://tqx.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bhs.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wfi.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bis.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lgh.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qre.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rog.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://piv.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xmy.yj20258.top

[E19] 多行文本按行拆分
来源：http://fhp.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://wsp.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gid.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://yyg.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://cim.sjlbkw.cn

Java: s.lines().toList()
来源：http://ril.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://tye.hfpthk.cn

Ruby: s.lines
来源：http://hkj.xuanzx.com

C#:   s.Split('\n')
来源：http://swr.yvedp.cn

[E20] 判断字符串是否为空
来源：http://eec.yj20258.top

Py:   if not s:
来源：http://jhl.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rwo.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://odj.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://wrc.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://fbk.cqqwz.cn

Go:   if s == "" {}
来源：http://vow.ydjk.org.cn

Ruby: if s.empty?
来源：http://wbh.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gwn.zhixingplan.top

[E21] 超长截断加省略号
来源：http://qya.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nvc.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hxj.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rap.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xxy.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eka.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://zpn.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://czz.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vgt.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://krw.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://swg.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cms.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://euc.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kym.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vfs.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gmf.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://khw.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jcs.iojbl.cn

================================================================================
来源：http://oyw.aibaodan.cn

F. 文件与目录
来源：http://bjl.daria6918.cn

================================================================================
来源：http://acm.chenlongwang.top

[F01] 读取整个文件
来源：http://pur.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jhl.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://llo.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nwe.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ypv.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yki.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ywk.zycfv.cn

Ruby: File.read("a.txt")
来源：http://llo.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://bfr.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://ezh.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://urj.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dyt.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyl.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://scf.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://shy.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cpr.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sui.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dsc.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://lqj.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tom.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xuy.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izc.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ark.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bzr.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ccu.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://xjp.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xou.zdqjudy.top

[F04] 追加写入文件
来源：http://moz.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vee.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cvr.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ohh.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fdj.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dnd.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://she.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qvu.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zuh.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://dxr.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yre.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://kzr.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://dys.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://zig.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://puy.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mwd.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://drm.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://edp.cucudq.cn

[F06] 删除文件
来源：http://aaz.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://cbr.daxiang520.top

PHP:  unlink("a.txt");
来源：http://rrr.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://mya.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nzc.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fqw.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://wns.cheryme.top

Ruby: File.delete("a.txt")
来源：http://anv.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://hbl.pengpengdd.cyou

[F07] 创建目录（含多级）
来源：http://shg.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ekh.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uby.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zee.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zlh.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hpc.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bam.chenjidiqi.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eca.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hza.zhongyouzk.top

[F08] 遍历目录
来源：http://tej.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://muq.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://isv.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://ize.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://hdd.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aan.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://kin.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://ekq.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://mhc.sweek.top

[F09] 获取文件大小
来源：http://yme.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://irr.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://gpy.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://vxp.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://wbo.hesvh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ieo.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jhv.smart0.xyz

Ruby: File.size("a.txt")
来源：http://byv.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://miw.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://xnf.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bgz.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zac.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wrr.hesvh.cn

TS:   path.extname("a.txt")
来源：http://iwr.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jih.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ntf.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kcv.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cni.ybcxt.top

[F11] 复制与移动文件
来源：http://vpf.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dpq.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://krw.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kzf.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bvk.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zda.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gow.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://crz.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sjt.tanke756.top

[F12] CSV 读写
来源：http://nao.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ehb.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yap.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yjx.chenlongwang.top

TS:   // 同上
来源：http://xrj.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://izv.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bth.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zav.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pod.wangshuangyany.cn

================================================================================
来源：http://gjz.tianlin.xyz

G. 面向对象
来源：http://iwr.mhx1999.top

================================================================================
来源：http://qay.hongshengwenyu.top

[G01] 定义类
来源：http://skj.jqgufenzy.top

Py:   class User: pass
来源：http://vav.yvedp.cn

PHP:  class User {}
来源：http://pmx.zhengqikj.top

JS:   class User {}
来源：http://xwj.meibo888.top

TS:   class User { name: string = ""; }
来源：http://fuu.yangfankeji.com

Java: class User {}
来源：http://jxp.zdqjudy.top

Go:   type User struct { Name string }
来源：http://vja.jqgufenzy.top

Ruby: class User; end
来源：http://dvi.zdqjudy.top

C#:   class User {}
来源：http://euf.mhx1999.top

[G02] 构造函数
来源：http://ihb.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://vky.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://xnw.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://rbc.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://plw.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://mvm.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wvi.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://qoh.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://kms.gogol.net.cn

[G03] 实例属性
来源：http://anj.yvedp.cn

Py:   self.name = "x"
来源：http://ciq.svipenyu.cn

PHP:  public string $name = "x";
来源：http://jrq.dashuyun.cn

JS:   this.name = "x";
来源：http://xwq.jlsjyb.cn

TS:   name: string = "x";
来源：http://rqp.sjlbkw.cn

Java: private String name;
来源：http://xjd.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yah.yongpay.top

Ruby: @name = "x"
来源：http://syv.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://knz.guowangkeji.top

[G04] 定义方法
来源：http://rvv.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://ofh.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://bdh.sxryk.cn

JS:   greet() { return this.name; }
来源：http://sks.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://ico.aibaodan.cn

Java: String greet() { return name; }
来源：http://bds.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ppo.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://gmg.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://bai.52xcode.cn

[G05] 继承
来源：http://rws.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://mlo.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://stt.c1oappe.top

JS:   class Admin extends User {}
来源：http://frd.guannengcc.top

TS:   class Admin extends User {}
来源：http://uec.pycfn.com

Java: class Admin extends User {}
来源：http://jje.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hfc.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://cll.chenlongwang.top

C#:   class Admin : User {}
来源：http://urn.shuidangran.top

[G06] 重写方法
来源：http://ftp.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://gzr.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://swz.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://jrm.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://pie.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://imq.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jmh.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://jlw.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://urg.52xcode.cn

[G07] 调用父类方法
来源：http://jrj.zhongyouzk.top

Py:   super().greet()
来源：http://dvz.fengsongda.top

PHP:  parent::greet();
来源：http://dwv.fanxiaobao.xyz

JS:   super.greet();
来源：http://omp.zdqjudy.top

TS:   super.greet();
来源：http://mom.hywenlv.cn

Java: super.greet();
来源：http://oxe.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oba.sxryk.cn

Ruby: super
来源：http://msk.ppjwa.cn

C#:   base.Greet();
来源：http://psd.shuidangran.top

[G08] 静态方法与属性
来源：http://wzv.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://isu.zdqjudy.top

PHP:  public static function f() {}
来源：http://diq.shangyingyoupin.top

JS:   static f() {}
来源：http://ipw.yj20258888.top

TS:   static f(): void {}
来源：http://msi.hcnkem.com

Java: static void f() {}
来源：http://qnk.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rfl.yangfankeji.com

Ruby: def self.f; end
来源：http://aje.shuidangran.top

C#:   public static void F() {}
来源：http://upv.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://euh.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://jou.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uaq.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jyb.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://zdm.tarul.cn

Java: interface Shape { double area(); }
来源：http://zwm.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://dmy.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jax.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://uyj.yvedp.cn

[G10] 访问控制
来源：http://vqn.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://gwg.zhongyouzk.top

PHP:  public / protected / private
来源：http://uzj.hammf.cn

JS:   #private 字段；其余公开
来源：http://brw.sweek.top

TS:   public / protected / private
来源：http://bga.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://efm.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oty.jyoumei.cn

Ruby: public / protected / private
来源：http://cxl.nwbrower.top

C#:   public / protected / private / internal
来源：http://lzb.bjfxy.top

[G11] getter / setter
来源：http://vtu.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://jpn.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://llo.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://dis.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://irj.316326.xyz

Java: public String getName() { return name; }
来源：http://cgt.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uzt.jqgfzy.top

Ruby: attr_accessor :name
来源：http://mgp.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://yzz.yonumen.top

[G12] 对象转字符串
来源：http://yvj.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://ewh.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jfu.yonumen.top

JS:   toString() { return this.name; }
来源：http://evn.sweek.top

TS:   toString(): string { return this.name; }
来源：http://tsm.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://nld.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://pnh.daria6918.cn

Ruby: def to_s; @name; end
来源：http://ths.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://xcl.dashuyun.cn

[G13] 判断对象类型
来源：http://dal.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://caj.sweek.top

PHP:  $u instanceof User
来源：http://wpc.snrcjt.cn

JS:   u instanceof User
来源：http://prf.ehwqpu.com

TS:   u instanceof User
来源：http://vss.aibaodan.cn

Java: u instanceof User
来源：http://tau.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fcp.sysykeji.top

Ruby: u.is_a?(User)
来源：http://los.daria6918.cn

C#:   u is User
来源：http://tcr.guannengcc.top

[G14] 数据类 / record
来源：http://rve.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://onj.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://elr.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://blt.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://udq.birdmap.top

Java: record User(String name, int age) {}
来源：http://kwu.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://ayk.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kpw.c1oappe.top


<!-- 参考信息 -->