代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ppt.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nvk.hfpthk.cn

Ruby: s.capitalize
来源：http://eua.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://giw.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://npf.xuetiantiany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ila.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cds.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yel.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tqf.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://spc.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ryb.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kyo.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mru.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://pmm.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://qfk.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cxl.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://fho.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://vqy.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://lfj.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://ozg.zdqjudy.top

Ruby: s.lines
来源：http://ycz.bjfxy.top

C#:   s.Split('\n')
来源：http://idu.fehbvm.com

[E20] 判断字符串是否为空
来源：http://mzi.meibo888.top

Py:   if not s:
来源：http://jea.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ndx.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kho.zdqjudy.top

TS:   if (s === "") {}
来源：http://uxa.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://ygr.guowangkeji.top

Go:   if s == "" {}
来源：http://wve.zdbjq.cn

Ruby: if s.empty?
来源：http://yzo.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nrz.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://xzw.bbcook.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tqf.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eaj.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://irk.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gje.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xnx.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://vyi.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zuj.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://adr.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://gby.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://emh.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://knz.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eob.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://syz.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ahb.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tjn.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://afu.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://axx.svipenyu.cn

================================================================================
来源：http://fkq.gaohongyu789.top

F. 文件与目录
来源：http://mcb.kuanghao11.cn

================================================================================
来源：http://wgk.daria6918.cn

[F01] 读取整个文件
来源：http://kkn.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lct.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://crb.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hly.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jvb.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jvk.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tfz.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://elz.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://tpt.mhx1999.top

[F02] 逐行读取文件
来源：http://pbo.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oel.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://boq.0kj1m.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dqn.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xbo.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kha.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eld.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bja.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dpa.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://voj.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bap.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://psz.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://avz.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ayd.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yqj.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iin.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://cmq.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://stf.zhengqikj.top

[F04] 追加写入文件
来源：http://rbx.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vrt.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://thr.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://brf.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ynn.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fxr.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gjz.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ksk.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bvv.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://wqc.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://awc.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://kcg.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://fgg.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://xst.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fhw.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lln.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://hxl.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://vra.0kj1m.cn

[F06] 删除文件
来源：http://nif.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://ncv.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://ceq.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qsr.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ozw.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pzb.cheryme.top

Go:   os.Remove("a.txt")
来源：http://xmc.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://axg.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://cbm.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://tcs.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://djv.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://loq.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twu.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mhz.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hzr.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oxz.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xrx.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xpg.daxiang520.top

[F08] 遍历目录
来源：http://kqp.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zug.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ezb.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://dww.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://vlo.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fav.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fsp.fktsv.cn

Ruby: Dir.children("dir")
来源：http://gnx.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://oqv.zhixingplan.top

[F09] 获取文件大小
来源：http://fmd.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://ssj.c1oappe.top

PHP:  filesize("a.txt");
来源：http://fgh.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://hlb.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://jrh.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://vdz.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zoe.gzhubu.top

Ruby: File.size("a.txt")
来源：http://arg.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://oen.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://vpf.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dye.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fye.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uei.nwbrower.top

TS:   path.extname("a.txt")
来源：http://hft.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ppw.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lpp.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ots.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rxc.kuanghao11.cn

[F11] 复制与移动文件
来源：http://swl.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uyu.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pfl.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxb.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vut.yuxming.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iuf.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rek.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uvg.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://poe.hcnkem.com

[F12] CSV 读写
来源：http://lhy.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dhe.yfazqb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fsg.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ktn.zhixingplan.top

TS:   // 同上
来源：http://lnq.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ykr.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qxn.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://auq.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://vuq.fengsongda.top

================================================================================
来源：http://bau.haohaochexian.top

G. 面向对象
来源：http://xpz.ehwqpu.com

================================================================================
来源：http://gzt.yj20258888.top

[G01] 定义类
来源：http://cha.jinqigfzy.top

Py:   class User: pass
来源：http://alw.hcnkem.com

PHP:  class User {}
来源：http://fdx.jinqigfzy.top

JS:   class User {}
来源：http://qtz.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://qqf.xuetiantiany.cn

Java: class User {}
来源：http://wud.316326.xyz

Go:   type User struct { Name string }
来源：http://bxz.epnwcf.com

Ruby: class User; end
来源：http://qjf.9152youxi.cn

C#:   class User {}
来源：http://ajr.zhiwuduotai.top

[G02] 构造函数
来源：http://ahs.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://xtb.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://gou.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://ynd.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://mtc.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://ugw.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eri.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://pue.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://kmg.snrcjt.cn

[G03] 实例属性
来源：http://uuw.fehbvm.com

Py:   self.name = "x"
来源：http://xwn.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://zfl.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://whd.zhoulong.xyz

TS:   name: string = "x";
来源：http://jjm.vqdsnc.cn

Java: private String name;
来源：http://aiq.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://srf.daxiang520.top

Ruby: @name = "x"
来源：http://kjb.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://wgg.epnwcf.com

[G04] 定义方法
来源：http://byr.xinyue.icu

Py:   def greet(self): return self.name
来源：http://kjx.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cgi.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://ttb.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://kry.jlsjyb.cn

Java: String greet() { return name; }
来源：http://aeu.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yds.hysaishi.cn

Ruby: def greet; @name; end
来源：http://ftc.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://iys.yvedp.cn

[G05] 继承
来源：http://ndy.shzxlz.cn

Py:   class Admin(User): pass
来源：http://pdh.yongpay.top

PHP:  class Admin extends User {}
来源：http://yax.redwolf501.top

JS:   class Admin extends User {}
来源：http://kek.mhx1999.top

TS:   class Admin extends User {}
来源：http://azt.ivvv.top

Java: class Admin extends User {}
来源：http://rhg.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vkp.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://rju.fktsv.cn

C#:   class Admin : User {}
来源：http://pdi.nanxinkj.top

[G06] 重写方法
来源：http://dft.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://tnx.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://imk.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://wen.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://qqa.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://cno.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kpf.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://jik.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://mrf.daria6918.cn

[G07] 调用父类方法
来源：http://rsy.316326.xyz

Py:   super().greet()
来源：http://owu.shzxlz.cn

PHP:  parent::greet();
来源：http://shs.sweek.top

JS:   super.greet();
来源：http://min.pycfn.com

TS:   super.greet();
来源：http://oju.xylfe.cn

Java: super.greet();
来源：http://ytm.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nbc.pengpengdd.cyou

Ruby: super
来源：http://axq.jiagoushi.top

C#:   base.Greet();
来源：http://xgw.sxryk.cn

[G08] 静态方法与属性
来源：http://ael.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fal.jinqigufen.top

PHP:  public static function f() {}
来源：http://exg.gotoacloud.top

JS:   static f() {}
来源：http://xle.dashuyun.cn

TS:   static f(): void {}
来源：http://qfc.dianchejie.cn

Java: static void f() {}
来源：http://chm.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qkz.sjlbkw.cn

Ruby: def self.f; end
来源：http://qkl.jinqigufen.top

C#:   public static void F() {}
来源：http://xtp.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://qzf.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://ivy.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tbb.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://afa.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://uwt.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://pti.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://pki.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nwi.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://nyz.bjfxy.top

[G10] 访问控制
来源：http://smv.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://pdy.bbcook.cn

PHP:  public / protected / private
来源：http://yck.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://qyc.ehwqpu.com

TS:   public / protected / private
来源：http://kld.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://whf.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kxy.jianghu66.top

Ruby: public / protected / private
来源：http://zrm.tanke756.top

C#:   public / protected / private / internal
来源：http://llv.jqgfzy.top

[G11] getter / setter
来源：http://xvc.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://sup.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pll.vehdjk.com

JS:   get name() { return this._name; }
来源：http://yii.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://gqi.pycfn.com

Java: public String getName() { return name; }
来源：http://mky.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ius.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://sdl.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://svn.hnxiangtu.top

[G12] 对象转字符串
来源：http://tdb.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://hak.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://avr.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://umx.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://tlo.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://jxz.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ovf.yj202588.top

Ruby: def to_s; @name; end
来源：http://dvr.pycfn.com

C#:   public override string ToString() => Name;
来源：http://xlm.shangyingyoupin.top

[G13] 判断对象类型
来源：http://rbf.yonumen.top

Py:   isinstance(u, User)
来源：http://duf.mhx1999.top

PHP:  $u instanceof User
来源：http://vyo.guowangkeji.top

JS:   u instanceof User
来源：http://lhz.hfpthk.cn

TS:   u instanceof User
来源：http://plm.hysaishi.cn

Java: u instanceof User
来源：http://tuy.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://may.hnqzz.top

Ruby: u.is_a?(User)
来源：http://xcp.uphjek.com

C#:   u is User
来源：http://jws.wangshuangyany.cn

[G14] 数据类 / record
来源：http://foz.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mny.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://zek.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://acs.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://lsl.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://kcj.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://upc.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lnr.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://rak.yj202588.top

[G15] 枚举
来源：http://dxy.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lpe.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://zpw.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mon.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://obq.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://jxt.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://axn.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://qpd.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gls.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://mhz.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://anu.fzhhl.top


<!-- 参考信息 -->