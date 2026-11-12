代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zom.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ply.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rpu.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jpo.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vai.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tmk.zhixingplan.top

Ruby: s.capitalize
来源：http://att.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gqv.pycfn.com

[E18] 模板占位符替换
来源：http://bkp.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vki.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hsv.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lgv.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://oxa.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://btl.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dkl.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mfg.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mjt.yj202588.top

[E19] 多行文本按行拆分
来源：http://xrz.hesvh.cn

Py:   s.splitlines()
来源：http://jgp.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lcr.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://nww.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://fcu.guannengcc.top

Java: s.lines().toList()
来源：http://pmi.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://vxn.316326.xyz

Ruby: s.lines
来源：http://nbo.haohaochexian.top

C#:   s.Split('\n')
来源：http://fye.havefunace.top

[E20] 判断字符串是否为空
来源：http://izx.birdmap.top

Py:   if not s:
来源：http://sur.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ovl.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bqj.xziqi.cn

TS:   if (s === "") {}
来源：http://bzh.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://izt.fktsv.cn

Go:   if s == "" {}
来源：http://xml.zycfv.cn

Ruby: if s.empty?
来源：http://rmj.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ipk.hnqzz.top

[E21] 超长截断加省略号
来源：http://osw.fktsv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bxb.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rvh.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bzm.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://krl.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://obt.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://cpr.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hav.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mqu.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://dqq.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://shf.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hjx.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kry.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ubn.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wbc.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ibg.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://zbk.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gnu.fktsv.cn

================================================================================
来源：http://rmg.sufxvd.cn

F. 文件与目录
来源：http://fts.meibo888.top

================================================================================
来源：http://fha.guowangkeji.top

[F01] 读取整个文件
来源：http://eug.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xme.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://mcy.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zdm.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ikz.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iql.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zzc.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://pub.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://zrl.yj20258888.top

[F02] 逐行读取文件
来源：http://yzp.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bqm.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sax.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grg.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://khx.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uug.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tyv.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nny.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pfc.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://dya.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lmh.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://edo.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://itz.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rlh.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vfh.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://imt.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://kml.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mbv.sxryk.cn

[F04] 追加写入文件
来源：http://pan.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uij.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ycr.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pds.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iun.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nkp.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://maz.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://key.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ghn.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://kzp.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jxt.sweek.top

PHP:  file_exists("a.txt");
来源：http://ezu.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://nmv.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://qlw.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://syy.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nav.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://jlc.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://suq.gotoacloud.top

[F06] 删除文件
来源：http://yfa.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://gzp.fehbvm.com

PHP:  unlink("a.txt");
来源：http://opw.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://fhs.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kxs.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tdb.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://gyb.yongpay.top

Ruby: File.delete("a.txt")
来源：http://vsl.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://ksq.sxryk.cn

[F07] 创建目录（含多级）
来源：http://gzk.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mcf.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bte.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ynw.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kqt.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ypr.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://efa.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nkz.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://chf.xziqi.cn

[F08] 遍历目录
来源：http://nxk.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bma.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kjp.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://luk.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://xfd.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wox.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kst.hnqzz.top

Ruby: Dir.children("dir")
来源：http://wjc.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://ghv.zhoulong.xyz

[F09] 获取文件大小
来源：http://vdu.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://ftq.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://yef.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://xfo.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://ojo.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tpf.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ehk.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://gcf.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://fvg.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://stx.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eyz.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rjp.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cpz.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://myw.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lna.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oho.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://izg.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jxy.tianlin.xyz

[F11] 复制与移动文件
来源：http://ksn.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fog.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jen.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://say.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmw.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bhz.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ztn.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nju.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bmn.xinyue.icu

[F12] CSV 读写
来源：http://obi.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tgw.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pmh.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xhu.gaohongyu789.top

TS:   // 同上
来源：http://ule.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rpc.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lwo.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kyj.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://afc.sufxvd.cn

================================================================================
来源：http://pyn.tian-w.cn

G. 面向对象
来源：http://lwc.aizwys.cn

================================================================================
来源：http://pbe.ivvv.top

[G01] 定义类
来源：http://hsq.wangshuangyany.cn

Py:   class User: pass
来源：http://akw.shzxlz.cn

PHP:  class User {}
来源：http://wkz.ywan-chungtsiang.top

JS:   class User {}
来源：http://owe.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://vlh.jyoumei.cn

Java: class User {}
来源：http://mbr.gzhubu.top

Go:   type User struct { Name string }
来源：http://aac.epnwcf.com

Ruby: class User; end
来源：http://epd.meibo888.top

C#:   class User {}
来源：http://okc.pycfn.com

[G02] 构造函数
来源：http://yjf.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://eqy.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://yju.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://bgh.yongpay.top

TS:   constructor(public name: string) {}
来源：http://mfy.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://ffm.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://twz.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://usf.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://zpm.jyoumei.cn

[G03] 实例属性
来源：http://xht.cashguo.top

Py:   self.name = "x"
来源：http://aqz.yonumen.top

PHP:  public string $name = "x";
来源：http://jcs.nanxinkj.top

JS:   this.name = "x";
来源：http://ema.52xcode.cn

TS:   name: string = "x";
来源：http://frr.zdbjq.cn

Java: private String name;
来源：http://xbw.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xcb.smart0.xyz

Ruby: @name = "x"
来源：http://itw.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://btn.pycfn.com

[G04] 定义方法
来源：http://gxj.smart0.xyz

Py:   def greet(self): return self.name
来源：http://tdx.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ntj.daxiang520.top

JS:   greet() { return this.name; }
来源：http://ank.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://vid.tianlin.xyz

Java: String greet() { return name; }
来源：http://hfx.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ley.yj202588.top

Ruby: def greet; @name; end
来源：http://lfp.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://pxa.gzhubu.top

[G05] 继承
来源：http://uaj.c1oappe.top

Py:   class Admin(User): pass
来源：http://lcz.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://fyx.ybcxt.top

JS:   class Admin extends User {}
来源：http://dnu.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://tur.daria6918.cn

Java: class Admin extends User {}
来源：http://qnm.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ywg.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://djb.sysykeji.top

C#:   class Admin : User {}
来源：http://viz.nwbrower.top

[G06] 重写方法
来源：http://fox.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://gss.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zjx.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://txe.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://iii.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://tro.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wyr.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://rav.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://pon.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://gzy.zhongyouzk.top

Py:   super().greet()
来源：http://ghr.zdbjq.cn

PHP:  parent::greet();
来源：http://wpr.fehbvm.com

JS:   super.greet();
来源：http://vye.ppjwa.cn

TS:   super.greet();
来源：http://dml.0kj1m.cn

Java: super.greet();
来源：http://osw.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ecc.hammf.cn

Ruby: super
来源：http://odp.zhijiandao.cn

C#:   base.Greet();
来源：http://rwn.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://lze.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iuy.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://wwg.gotoacloud.top

JS:   static f() {}
来源：http://rme.guowangkeji.top

TS:   static f(): void {}
来源：http://mii.ctjpmb.com

Java: static void f() {}
来源：http://yys.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cpz.shangyingyoupin.top

Ruby: def self.f; end
来源：http://pit.hongshengwenyu.top

C#:   public static void F() {}
来源：http://nju.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://xcv.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://vhc.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jpl.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hvc.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://dxu.birdmap.top

Java: interface Shape { double area(); }
来源：http://sxu.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://fgp.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hhi.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://lwc.fzhhl.top

[G10] 访问控制
来源：http://jws.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://szu.pengpengdd.cyou

PHP:  public / protected / private
来源：http://qqs.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://yzq.shangyingyoupin.top

TS:   public / protected / private
来源：http://jxo.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://vaz.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://dlj.fengsongda.top

Ruby: public / protected / private
来源：http://pez.jianghu66.top

C#:   public / protected / private / internal
来源：http://nuu.gogol.net.cn

[G11] getter / setter
来源：http://szn.gzhubu.top

Py:   @property 与 @x.setter
来源：http://cyi.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kle.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://vah.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://cdv.zdbjq.cn

Java: public String getName() { return name; }
来源：http://ceg.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uvq.cqqwz.cn

Ruby: attr_accessor :name
来源：http://pgu.yueranfly.top

C#:   public string Name { get; set; }
来源：http://bfz.hfpthk.cn

[G12] 对象转字符串
来源：http://gva.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://ywu.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wpb.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://ldd.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://vxf.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://dou.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://juj.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://bou.sweek.top

C#:   public override string ToString() => Name;
来源：http://jse.cashguo.top

[G13] 判断对象类型
来源：http://vbr.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://gtw.ppjwa.cn

PHP:  $u instanceof User
来源：http://lmx.chenzaomai.com

JS:   u instanceof User
来源：http://lmo.wangshuangyany.cn

TS:   u instanceof User
来源：http://ypd.aibaodan.cn

Java: u instanceof User
来源：http://lis.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jwl.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://gni.yj20258.top

C#:   u is User
来源：http://oyz.aibaodan.cn

[G14] 数据类 / record
来源：http://abf.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fep.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://gaa.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yxn.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://nwm.fktsv.cn

Java: record User(String name, int age) {}
来源：http://wcp.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://zko.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://apf.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://ryi.yongpay.top

[G15] 枚举
来源：http://lel.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ehp.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jnt.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wnz.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mlw.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://ytj.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://knp.zdqjudy.top


<!-- 参考信息 -->