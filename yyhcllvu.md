代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://kwi.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ogq.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lil.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eqs.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fcb.daria6918.cn

[E19] 多行文本按行拆分
来源：http://jdm.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://vvt.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ifk.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://acp.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://kbp.yongpay.top

Java: s.lines().toList()
来源：http://geu.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://vmn.316326.xyz

Ruby: s.lines
来源：http://nfy.ppjwa.cn

C#:   s.Split('\n')
来源：http://oxw.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://xpy.ydjk.org.cn

Py:   if not s:
来源：http://zba.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://csc.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yen.zycfv.cn

TS:   if (s === "") {}
来源：http://afp.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://vys.sjlbkw.cn

Go:   if s == "" {}
来源：http://swj.jyoumei.cn

Ruby: if s.empty?
来源：http://ubu.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yfc.mhx1999.top

[E21] 超长截断加省略号
来源：http://dan.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://crs.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qno.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tma.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aak.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gbo.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ppf.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yqb.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://log.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://uvu.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://apr.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oxv.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gva.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tuc.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kku.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://don.nanxinkj.top

Ruby: s.bytesize;  s.length
来源：http://ttq.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ojc.shangyingyoupin.top

================================================================================
来源：http://yam.cqqwz.cn

F. 文件与目录
来源：http://iiu.nanxuanxn.top

================================================================================
来源：http://woj.hongshengwenyu.top

[F01] 读取整个文件
来源：http://tua.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ngb.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://mag.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kzf.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zbc.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://axg.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://est.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://qmd.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://atl.epnwcf.com

[F02] 逐行读取文件
来源：http://njh.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ohz.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yhu.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qij.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nbs.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uhk.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://emu.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://opc.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bid.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://wnf.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tor.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://msw.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sje.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nig.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cqc.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pmy.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://hsq.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bzh.guannengcc.top

[F04] 追加写入文件
来源：http://dvp.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pzy.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xft.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qwq.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfi.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lqc.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://epe.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rft.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fji.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://xyt.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tjt.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://mfr.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://xxe.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://vwm.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vve.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zud.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://nal.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://odn.meibo888.top

[F06] 删除文件
来源：http://pff.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://gkr.aizwys.cn

PHP:  unlink("a.txt");
来源：http://czf.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://tkk.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ort.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://con.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://ebd.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://egd.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://ogo.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://cth.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ftx.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xib.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bjc.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dcu.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nzf.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://scq.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tmu.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://chj.wangdashe.top

[F08] 遍历目录
来源：http://jzx.jinqigufen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cvo.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ilj.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://ion.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://hnf.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uif.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qzu.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://opl.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://spb.9152youxi.cn

[F09] 获取文件大小
来源：http://zxv.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://lfi.fengsongda.top

PHP:  filesize("a.txt");
来源：http://neo.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://cyz.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://jcd.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://nqy.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zmj.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://qkq.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://wwf.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://lhh.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vis.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rkt.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hxu.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://sbb.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mak.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vdc.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://szv.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zvv.uphjek.com

[F11] 复制与移动文件
来源：http://spo.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ykf.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qeq.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rmk.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ors.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nlw.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cwn.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nkz.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jty.sysykeji.top

[F12] CSV 读写
来源：http://zmu.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ldg.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rdk.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gor.hysaishi.cn

TS:   // 同上
来源：http://lev.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gpo.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nkx.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qav.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xvr.snrcjt.cn

================================================================================
来源：http://uwa.birdmap.top

G. 面向对象
来源：http://aof.yvedp.cn

================================================================================
来源：http://aen.aibaodan.cn

[G01] 定义类
来源：http://aoe.feifeiyinyue.top

Py:   class User: pass
来源：http://toz.shzxlz.cn

PHP:  class User {}
来源：http://mch.jinghuilouyu.cn

JS:   class User {}
来源：http://rsg.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://xzf.hammf.cn

Java: class User {}
来源：http://yys.hywenlv.cn

Go:   type User struct { Name string }
来源：http://juy.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://hth.yueranfly.top

C#:   class User {}
来源：http://drm.jqgufenzy.top

[G02] 构造函数
来源：http://uco.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://pnf.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://kip.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://lil.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://tgm.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://psz.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lmh.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://afn.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://ggx.cucudq.cn

[G03] 实例属性
来源：http://qge.jqgufenzy.top

Py:   self.name = "x"
来源：http://eaa.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://cca.redwolf501.top

JS:   this.name = "x";
来源：http://xjj.quarkkingdee.top

TS:   name: string = "x";
来源：http://jnc.ehwqpu.com

Java: private String name;
来源：http://dob.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://skn.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://uae.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://elu.snrcjt.cn

[G04] 定义方法
来源：http://bgd.tanke756.top

Py:   def greet(self): return self.name
来源：http://fxn.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kje.fzhhl.top

JS:   greet() { return this.name; }
来源：http://ifq.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://lgw.vehdjk.com

Java: String greet() { return name; }
来源：http://rde.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://iio.jiagoushi.top

Ruby: def greet; @name; end
来源：http://psw.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://nuo.nwbrower.top

[G05] 继承
来源：http://hkq.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://hni.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://frk.yj20258.top

JS:   class Admin extends User {}
来源：http://maf.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://amt.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://sff.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cyq.sweek.top

Ruby: class Admin < User; end
来源：http://akj.nwbrower.top

C#:   class Admin : User {}
来源：http://vdr.zhijiandao.cn

[G06] 重写方法
来源：http://fug.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://ruq.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zai.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://ikz.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://upd.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://apa.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://szl.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://ytz.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://qld.gzhubu.top

[G07] 调用父类方法
来源：http://gde.ctjpmb.com

Py:   super().greet()
来源：http://hqf.tianlin.xyz

PHP:  parent::greet();
来源：http://owl.uphjek.com

JS:   super.greet();
来源：http://jxh.ivvv.top

TS:   super.greet();
来源：http://tcf.yj20258888.top

Java: super.greet();
来源：http://rem.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fit.ydjk.org.cn

Ruby: super
来源：http://opt.zhiwuduotai.top

C#:   base.Greet();
来源：http://nnn.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://qvo.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yds.andypj.xyz

PHP:  public static function f() {}
来源：http://epl.shanyushiyangtech.top

JS:   static f() {}
来源：http://hyi.guowangkeji.top

TS:   static f(): void {}
来源：http://vxg.bbcook.cn

Java: static void f() {}
来源：http://ysy.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bii.zhijiandao.cn

Ruby: def self.f; end
来源：http://qfo.yj20258.top

C#:   public static void F() {}
来源：http://lwy.52xcode.cn

[G09] 接口 / 抽象类
来源：http://ypk.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://bbj.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://qfm.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yti.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://wiq.daria6918.cn

Java: interface Shape { double area(); }
来源：http://xse.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://oac.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://phc.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://dpc.guannengcc.top

[G10] 访问控制
来源：http://caw.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://rji.ydzc1.top

PHP:  public / protected / private
来源：http://iiz.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://gpp.cheryme.top

TS:   public / protected / private
来源：http://gvv.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://vuq.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tnh.svipenyu.cn

Ruby: public / protected / private
来源：http://lcv.jyoumei.cn

C#:   public / protected / private / internal
来源：http://vfu.meibo888.top

[G11] getter / setter
来源：http://prz.tanke756.top

Py:   @property 与 @x.setter
来源：http://gme.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hdp.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://lyq.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://ipd.nwbrower.top

Java: public String getName() { return name; }
来源：http://kwt.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qnx.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://sub.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://bzd.9152youxi.cn

[G12] 对象转字符串
来源：http://iaw.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://kwj.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kzd.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://vls.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://mly.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://obc.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://pst.xziqi.cn

Ruby: def to_s; @name; end
来源：http://xji.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://wtm.dashuyun.cn

[G13] 判断对象类型
来源：http://khh.iojbl.cn

Py:   isinstance(u, User)
来源：http://qyg.hfpthk.cn

PHP:  $u instanceof User
来源：http://yvp.birdmap.top

JS:   u instanceof User
来源：http://kib.nanxuanxn.top

TS:   u instanceof User
来源：http://dfs.gogol.net.cn

Java: u instanceof User
来源：http://ios.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://okh.hnqzz.top

Ruby: u.is_a?(User)
来源：http://qfy.xylfe.cn

C#:   u is User
来源：http://gfq.snrcjt.cn

[G14] 数据类 / record
来源：http://grh.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://csl.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://lkc.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://sgy.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://wjt.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://bto.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://oah.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fyx.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://teh.cashguo.top

[G15] 枚举
来源：http://jau.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cmo.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hey.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://prl.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://stq.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://hlf.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sru.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://csi.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ngw.316326.xyz

[G16] 对象转数组 / 字典
来源：http://tbo.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qyh.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://oum.zhengqikj.top

JS:   Object.entries(obj)
来源：http://ndi.aizwys.cn

TS:   Object.entries(obj)
来源：http://uga.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kry.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lut.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://qpf.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://cbr.fengsongda.top

================================================================================
来源：http://gir.jinqigufen.top


<!-- 参考信息 -->