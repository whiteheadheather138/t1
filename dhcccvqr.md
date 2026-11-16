代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yoo.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yoo.sjlbkw.cn

Ruby: s.capitalize
来源：http://wkj.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://exw.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://rpr.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bcr.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kuf.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gmm.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vjk.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qhq.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kip.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tgf.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yzf.mhx1999.top

[E19] 多行文本按行拆分
来源：http://slx.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://wdb.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xju.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://dpp.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://yly.0kj1m.cn

Java: s.lines().toList()
来源：http://wye.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://spv.gotoacloud.top

Ruby: s.lines
来源：http://ift.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://pvw.yuxming.cn

[E20] 判断字符串是否为空
来源：http://cfm.wangdashe.top

Py:   if not s:
来源：http://thn.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hxg.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://esv.kuanghao11.cn

TS:   if (s === "") {}
来源：http://pun.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://svk.cucudq.cn

Go:   if s == "" {}
来源：http://wpx.zhiwuduotai.top

Ruby: if s.empty?
来源：http://dkt.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ukc.fehbvm.com

[E21] 超长截断加省略号
来源：http://pbn.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hnx.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lge.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lmg.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gpx.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rbq.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://noj.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://itc.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tvk.cucudq.cn

[E22] 字节长度与字符长度
来源：http://fpo.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://boa.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ize.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cwp.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xkt.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xxa.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ctn.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://tci.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ufj.epnwcf.com

================================================================================
来源：http://puh.yongpay.top

F. 文件与目录
来源：http://pro.wangdashe.top

================================================================================
来源：http://wpj.zhongyouzk.top

[F01] 读取整个文件
来源：http://lba.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mma.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://fyb.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yti.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ycm.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rys.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lyx.fktsv.cn

Ruby: File.read("a.txt")
来源：http://bqd.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://nqt.daria6918.cn

[F02] 逐行读取文件
来源：http://vps.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://akg.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rwg.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sur.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dqy.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jad.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://crm.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yyp.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ytn.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://guu.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lhd.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vjb.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uci.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zms.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cfq.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lor.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://wdc.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tge.zhongyouzk.top

[F04] 追加写入文件
来源：http://oah.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rqu.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://khg.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rnw.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://luk.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ycb.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ees.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lsh.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uwd.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://bop.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lpa.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://irb.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://nsk.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://kfb.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gdq.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://upn.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://yrf.yj202588.top

C#:   File.Exists("a.txt")
来源：http://zbc.jqgfzy.top

[F06] 删除文件
来源：http://dwh.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://xjp.cheryme.top

PHP:  unlink("a.txt");
来源：http://mjm.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://nfv.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://cdr.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lbh.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://ose.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://nco.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://wgq.daxiang520.top

[F07] 创建目录（含多级）
来源：http://pht.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dfq.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://teb.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dvb.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkc.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zjw.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vsd.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ahr.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dtj.jiagoushi.top

[F08] 遍历目录
来源：http://hyn.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://von.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rlf.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://jai.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://ucu.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sma.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uvp.ybcxt.top

Ruby: Dir.children("dir")
来源：http://xkg.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://hgf.guowangkeji.top

[F09] 获取文件大小
来源：http://chu.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://nca.daria6918.cn

PHP:  filesize("a.txt");
来源：http://ktg.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://hvh.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://uxa.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rqv.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gje.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://skn.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://hpz.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://cct.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uxd.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qsr.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xqi.daxiang520.top

TS:   path.extname("a.txt")
来源：http://eve.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vvq.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://njb.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://otz.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yka.fktsv.cn

[F11] 复制与移动文件
来源：http://hbu.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ngi.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://avk.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wkc.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yzb.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aat.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zrf.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://stj.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iwc.sweek.top

[F12] CSV 读写
来源：http://fea.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yya.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cfe.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nlt.sweek.top

TS:   // 同上
来源：http://wcv.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ykv.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pbw.jinghuilouyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rua.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tsj.svipenyu.cn

================================================================================
来源：http://rur.mhx1999.top

G. 面向对象
来源：http://cgs.nwbrower.top

================================================================================
来源：http://rca.yvedp.cn

[G01] 定义类
来源：http://dqu.jlsjyb.cn

Py:   class User: pass
来源：http://ccn.ppjwa.cn

PHP:  class User {}
来源：http://vgy.52xcode.cn

JS:   class User {}
来源：http://prn.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://fya.zhoulong.xyz

Java: class User {}
来源：http://eer.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://pdm.andypj.xyz

Ruby: class User; end
来源：http://iyy.zycfv.cn

C#:   class User {}
来源：http://ysm.fehbvm.com

[G02] 构造函数
来源：http://fim.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://ubg.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://pxc.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://jfo.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://rse.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://ruc.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fva.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://mkr.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://wwd.jyoumei.cn

[G03] 实例属性
来源：http://lbz.aizwys.cn

Py:   self.name = "x"
来源：http://dbb.gogol.net.cn

PHP:  public string $name = "x";
来源：http://zem.nwbrower.top

JS:   this.name = "x";
来源：http://jzp.shuidangran.top

TS:   name: string = "x";
来源：http://ftj.52xcode.cn

Java: private String name;
来源：http://man.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fin.ybcxt.top

Ruby: @name = "x"
来源：http://mzp.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://wqa.zhongyouzk.top

[G04] 定义方法
来源：http://cwe.hcnkem.com

Py:   def greet(self): return self.name
来源：http://loy.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://odd.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://qji.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://ovr.hcnkem.com

Java: String greet() { return name; }
来源：http://qyo.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iig.hammf.cn

Ruby: def greet; @name; end
来源：http://una.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://aci.dianchejie.cn

[G05] 继承
来源：http://mjs.yueranfly.top

Py:   class Admin(User): pass
来源：http://fau.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://bcs.gotoacloud.top

JS:   class Admin extends User {}
来源：http://nlf.smart0.xyz

TS:   class Admin extends User {}
来源：http://vql.smart0.xyz

Java: class Admin extends User {}
来源：http://rjb.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gli.yangfankeji.com

Ruby: class Admin < User; end
来源：http://jko.daria6918.cn

C#:   class Admin : User {}
来源：http://chv.gaohongyu789.top

[G06] 重写方法
来源：http://zhy.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://yzw.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kqn.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://csq.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://ioe.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://btt.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://goz.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://yel.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://dsn.ydjk.org.cn

[G07] 调用父类方法
来源：http://usz.iojbl.cn

Py:   super().greet()
来源：http://mku.hywenlv.cn

PHP:  parent::greet();
来源：http://jgv.jyoumei.cn

JS:   super.greet();
来源：http://qnb.fktsv.cn

TS:   super.greet();
来源：http://tmm.hammf.cn

Java: super.greet();
来源：http://djk.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hav.xinyue.icu

Ruby: super
来源：http://nqf.c1oappe.top

C#:   base.Greet();
来源：http://eee.yj20258.top

[G08] 静态方法与属性
来源：http://gyp.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cpx.epnwcf.com

PHP:  public static function f() {}
来源：http://uek.tanke756.top

JS:   static f() {}
来源：http://clo.jqgfzy.top

TS:   static f(): void {}
来源：http://jyp.jianghu66.top

Java: static void f() {}
来源：http://qim.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jqz.dianchejie.cn

Ruby: def self.f; end
来源：http://ueh.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://pwo.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://jyr.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://fjn.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ppn.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cqz.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://oyb.cheryme.top

Java: interface Shape { double area(); }
来源：http://sqp.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://nau.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cii.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://bqz.ydjk.org.cn

[G10] 访问控制
来源：http://agm.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://anb.yj20258888.top

PHP:  public / protected / private
来源：http://kyu.epnwcf.com

JS:   #private 字段；其余公开
来源：http://aoq.yvedp.cn

TS:   public / protected / private
来源：http://ugw.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://bjt.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dhl.sufxvd.cn

Ruby: public / protected / private
来源：http://jgg.tarul.cn

C#:   public / protected / private / internal
来源：http://xcx.zhixingplan.top

[G11] getter / setter
来源：http://uyd.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://qoc.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://otk.havefunace.top

JS:   get name() { return this._name; }
来源：http://elu.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://tpg.zdbjq.cn

Java: public String getName() { return name; }
来源：http://weg.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lse.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://quk.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://pgg.ydjk.org.cn

[G12] 对象转字符串
来源：http://dcw.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://usr.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://byc.jianghu66.top

JS:   toString() { return this.name; }
来源：http://zli.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://wlx.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://jhb.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://bir.wangdashe.top

Ruby: def to_s; @name; end
来源：http://grh.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://ukj.fehbvm.com

[G13] 判断对象类型
来源：http://pzg.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://jra.dashuyun.cn

PHP:  $u instanceof User
来源：http://pjp.fengsongda.top

JS:   u instanceof User
来源：http://njv.yangfankeji.com

TS:   u instanceof User
来源：http://ifv.shanyushiyangkeji.top

Java: u instanceof User
来源：http://nrr.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvb.havefunace.top

Ruby: u.is_a?(User)
来源：http://fgq.yueranfly.top

C#:   u is User
来源：http://jxi.shuidangran.top

[G14] 数据类 / record
来源：http://dag.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nnj.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://fwy.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://ndy.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://lfi.birdmap.top

Java: record User(String name, int age) {}
来源：http://oqq.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://vuu.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://frk.tarul.cn

C#:   record User(string Name, int Age);
来源：http://ebn.sjlbkw.cn

[G15] 枚举
来源：http://mli.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://roq.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jnj.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vsx.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iaw.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://cie.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://doy.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://gjp.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zia.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://sjw.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sua.pengpengdd.cyou


<!-- 参考信息 -->