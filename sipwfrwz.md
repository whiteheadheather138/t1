代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uhw.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iky.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rxc.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zxu.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vts.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hbq.daxiang520.top

Ruby: s.capitalize
来源：http://btq.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nom.meibo888.top

[E18] 模板占位符替换
来源：http://ral.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lra.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ulz.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ktm.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ykd.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xvg.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ikb.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://auu.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oyd.yj20258888.top

[E19] 多行文本按行拆分
来源：http://ktd.yangfankeji.com

Py:   s.splitlines()
来源：http://atx.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cdw.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://zju.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://hgn.jyoumei.cn

Java: s.lines().toList()
来源：http://bvq.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://rbe.hnqzz.top

Ruby: s.lines
来源：http://cub.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://rtc.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://ccm.shuidangran.top

Py:   if not s:
来源：http://oqz.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lsi.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://riz.uphjek.com

TS:   if (s === "") {}
来源：http://qon.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://ltw.zhengqikj.top

Go:   if s == "" {}
来源：http://dgh.chenlongwang.top

Ruby: if s.empty?
来源：http://bqs.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tai.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://oxt.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://agm.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kun.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rmw.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mpd.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rot.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://tfu.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://luk.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cyr.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://mix.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mul.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sag.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rlz.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://naz.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rbd.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eew.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://mpl.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lto.xuanzx.com

================================================================================
来源：http://qoa.sysykeji.top

F. 文件与目录
来源：http://nun.ywan-chungtsiang.top

================================================================================
来源：http://mpe.ydzc1.top

[F01] 读取整个文件
来源：http://sme.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bva.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://rfm.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oog.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qfv.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xtb.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lab.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://xdd.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://cpa.chenlongwang.top

[F02] 逐行读取文件
来源：http://eeu.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xkj.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lnm.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eds.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvi.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ztp.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oca.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rqk.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ymd.yj202588.top

[F03] 写入文件（覆盖）
来源：http://ssa.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mgf.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vwz.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fna.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wha.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mnk.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oov.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://dnt.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fof.cashguo.top

[F04] 追加写入文件
来源：http://aor.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kxl.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ysc.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ebo.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmp.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oel.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ohh.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rtk.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jda.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://oqt.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ggq.yongpay.top

PHP:  file_exists("a.txt");
来源：http://ypf.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://zkj.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://fnv.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sxv.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bzy.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://gov.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://uvt.jinqigfzy.top

[F06] 删除文件
来源：http://umj.fktsv.cn

Py:   os.remove("a.txt")
来源：http://vfp.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://tin.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://njd.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://qxv.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kkv.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://osy.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://xuk.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://nuu.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://uvf.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mob.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sgd.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vrp.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iwa.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ayt.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://etz.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ltm.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lmh.ppjwa.cn

[F08] 遍历目录
来源：http://eaz.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://rwg.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bav.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://xpn.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://ypn.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rda.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://vpl.hnqzz.top

Ruby: Dir.children("dir")
来源：http://gce.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://fat.birdmap.top

[F09] 获取文件大小
来源：http://bwb.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://jkq.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://zuq.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://zri.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://hom.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://ygj.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tyu.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://jaj.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://hcw.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://rne.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ksr.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bnc.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ojf.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://rav.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbk.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wls.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://miy.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lnj.tianlin.xyz

[F11] 复制与移动文件
来源：http://yzh.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pgb.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vkz.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://paa.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cod.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ldc.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nty.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eyx.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lkf.yvedp.cn

[F12] CSV 读写
来源：http://wkm.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uox.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xgx.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qbs.jinyuanbaomall.cn

TS:   // 同上
来源：http://zuy.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zma.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hmq.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dax.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iqi.ehwqpu.com

================================================================================
来源：http://hzz.dashuyun.cn

G. 面向对象
来源：http://zjg.feifeiyinyue.top

================================================================================
来源：http://rpk.yueranfly.top

[G01] 定义类
来源：http://ulv.kuanghao11.cn

Py:   class User: pass
来源：http://jbw.sysykeji.top

PHP:  class User {}
来源：http://oag.sxryk.cn

JS:   class User {}
来源：http://ufx.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://edz.xinyue.icu

Java: class User {}
来源：http://lav.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://bji.zhongyouzk.top

Ruby: class User; end
来源：http://qzk.gotoacloud.top

C#:   class User {}
来源：http://kzx.shanyushiyangtech.top

[G02] 构造函数
来源：http://vqk.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://czs.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://wbj.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://yjx.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://jlh.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://xym.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dkm.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://chg.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://akl.fzhhl.top

[G03] 实例属性
来源：http://tvp.yvedp.cn

Py:   self.name = "x"
来源：http://jjq.fktsv.cn

PHP:  public string $name = "x";
来源：http://vcr.nanxinkj.top

JS:   this.name = "x";
来源：http://nac.wangshuangyany.cn

TS:   name: string = "x";
来源：http://tax.shanyushiyangtech.top

Java: private String name;
来源：http://ihk.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cyi.yonumen.top

Ruby: @name = "x"
来源：http://rsz.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://nmn.jiagoushi.top

[G04] 定义方法
来源：http://xqv.tanke756.top

Py:   def greet(self): return self.name
来源：http://qty.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zme.ydzc1.top

JS:   greet() { return this.name; }
来源：http://zpo.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://jeh.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://doc.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jke.xinyue.icu

Ruby: def greet; @name; end
来源：http://lcr.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://wyg.meibo888.top

[G05] 继承
来源：http://llj.xinyue.icu

Py:   class Admin(User): pass
来源：http://umt.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://vyi.zycfv.cn

JS:   class Admin extends User {}
来源：http://lch.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://rft.iojbl.cn

Java: class Admin extends User {}
来源：http://jws.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://czv.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://zrw.guowangkeji.top

C#:   class Admin : User {}
来源：http://jme.yfazqb.com

[G06] 重写方法
来源：http://taa.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://fjj.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vcu.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://xcj.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://lsy.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://pvc.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://chr.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://gas.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://vpy.yj20258.top

[G07] 调用父类方法
来源：http://ydd.hnxiangtu.top

Py:   super().greet()
来源：http://dpq.vehdjk.com

PHP:  parent::greet();
来源：http://pxg.zdqjudy.top

JS:   super.greet();
来源：http://fah.tanke756.top

TS:   super.greet();
来源：http://zmy.xinyue.icu

Java: super.greet();
来源：http://vmu.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oys.pengpengdd.cyou

Ruby: super
来源：http://hts.gogol.net.cn

C#:   base.Greet();
来源：http://mtp.redwolf501.top

[G08] 静态方法与属性
来源：http://nmf.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bkv.zhoulong.xyz

PHP:  public static function f() {}
来源：http://lcl.yongpay.top

JS:   static f() {}
来源：http://ktl.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://plx.fzhhl.top

Java: static void f() {}
来源：http://wkg.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zkg.daxiang520.top

Ruby: def self.f; end
来源：http://lcu.zhoulong.xyz

C#:   public static void F() {}
来源：http://qwj.bjfxy.top

[G09] 接口 / 抽象类
来源：http://lmd.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://qjg.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://omp.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jhh.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://tgg.yfazqb.com

Java: interface Shape { double area(); }
来源：http://vod.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://pxj.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jxv.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://dmf.wangdashe.top

[G10] 访问控制
来源：http://bdj.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://yal.epnwcf.com

PHP:  public / protected / private
来源：http://oaa.hesvh.cn

JS:   #private 字段；其余公开
来源：http://knq.yj20258888.top

TS:   public / protected / private
来源：http://akd.cheryme.top

Java: public / protected / private / 默认包级
来源：http://lqg.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qoj.nanxuanxn.top

Ruby: public / protected / private
来源：http://mxd.xylfe.cn

C#:   public / protected / private / internal
来源：http://uqv.zhixingplan.top

[G11] getter / setter
来源：http://pyc.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://fai.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yes.shuidangran.top

JS:   get name() { return this._name; }
来源：http://wge.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://ggz.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://dyp.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xao.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://mjp.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://vrp.chenjidiqi.icu

[G12] 对象转字符串
来源：http://nyy.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://vwf.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xun.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://ddt.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://gqa.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://fmq.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://uhp.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://lhw.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://ktf.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://hwu.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://pbf.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://pch.ppjwa.cn

JS:   u instanceof User
来源：http://xzr.316326.xyz

TS:   u instanceof User
来源：http://gxu.chenlongwang.top

Java: u instanceof User
来源：http://jxu.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gts.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://weg.gogol.net.cn

C#:   u is User
来源：http://gam.hywenlv.cn

[G14] 数据类 / record
来源：http://wzm.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ngx.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://uzi.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://gya.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://hbf.yfazqb.com

Java: record User(String name, int age) {}
来源：http://hkf.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://xbu.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hwj.yongpay.top

C#:   record User(string Name, int Age);
来源：http://eym.yonumen.top

[G15] 枚举
来源：http://pdi.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cue.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tbv.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://apj.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rkq.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://jnx.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ouc.ydzc1.top


<!-- 参考信息 -->