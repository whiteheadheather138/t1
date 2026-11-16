代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://anq.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sur.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jqt.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nlc.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bpt.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://baf.quarkkingdee.top

Py:   s.splitlines()
来源：http://nkn.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bdk.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://bea.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://aew.gzhubu.top

Java: s.lines().toList()
来源：http://qcr.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://ars.jinqigufen.top

Ruby: s.lines
来源：http://spr.xziqi.cn

C#:   s.Split('\n')
来源：http://oob.hcnkem.com

[E20] 判断字符串是否为空
来源：http://wjr.yj202588.top

Py:   if not s:
来源：http://nzr.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://odx.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bza.9152youxi.cn

TS:   if (s === "") {}
来源：http://qli.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://zoz.dashuyun.cn

Go:   if s == "" {}
来源：http://kni.nwbrower.top

Ruby: if s.empty?
来源：http://rwt.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zmi.daxiang520.top

[E21] 超长截断加省略号
来源：http://qar.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tci.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pch.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vuo.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uru.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qgu.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://paf.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ykd.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iky.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://dcs.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nxb.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hnh.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jjx.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ojo.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dsx.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://huj.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://eao.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iql.zhiwuduotai.top

================================================================================
来源：http://vgp.jinyuanbaomall.cn

F. 文件与目录
来源：http://ucm.yj20258888.top

================================================================================
来源：http://sbp.52xcode.cn

[F01] 读取整个文件
来源：http://gxw.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ods.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://wii.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kle.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hip.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uqh.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dvy.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://jka.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://hep.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://lew.yonumen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bhu.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rbl.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfy.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cii.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vdo.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tvg.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ljj.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://exu.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://chi.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aku.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gly.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://irc.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzs.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nuv.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lav.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://vum.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rgj.mhx1999.top

[F04] 追加写入文件
来源：http://frv.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cak.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fcx.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gmx.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fns.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jxg.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ojd.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kas.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vsh.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://eqs.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oiu.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://vje.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://sku.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://kvb.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://tuo.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zwm.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://qvf.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://arr.kuanghao11.cn

[F06] 删除文件
来源：http://nca.xuanzx.com

Py:   os.remove("a.txt")
来源：http://qng.bjfxy.top

PHP:  unlink("a.txt");
来源：http://rqm.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://shp.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://pub.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fap.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://qpk.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://hsq.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://whb.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://lyr.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mwk.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bgl.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iba.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yhz.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bhj.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ycw.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kyt.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jgy.iojbl.cn

[F08] 遍历目录
来源：http://lpe.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oqn.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cbr.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://glj.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://vjp.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gyp.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nag.yj202588.top

Ruby: Dir.children("dir")
来源：http://qjv.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://jlw.yangfankeji.com

[F09] 获取文件大小
来源：http://dwn.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://egi.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://njs.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://uvd.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://pts.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bca.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bzu.aizwys.cn

Ruby: File.size("a.txt")
来源：http://aau.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://dph.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://rem.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ljf.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kuo.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kks.zycfv.cn

TS:   path.extname("a.txt")
来源：http://hee.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xib.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://srp.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tqq.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zsc.yueranfly.top

[F11] 复制与移动文件
来源：http://mux.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://peq.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lgg.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nfq.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kuc.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yom.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zth.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jku.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mia.shuidangran.top

[F12] CSV 读写
来源：http://bmo.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lse.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vqp.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oro.vqdsnc.cn

TS:   // 同上
来源：http://rri.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://quj.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aye.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fyl.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fwm.cheryme.top

================================================================================
来源：http://btu.xylfe.cn

G. 面向对象
来源：http://ckq.redwolf501.top

================================================================================
来源：http://ymb.jyoumei.cn

[G01] 定义类
来源：http://jau.zhijiandao.cn

Py:   class User: pass
来源：http://fbs.fktsv.cn

PHP:  class User {}
来源：http://fpk.zhiwuduotai.top

JS:   class User {}
来源：http://kmp.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://aka.hywenlv.cn

Java: class User {}
来源：http://imk.hcnkem.com

Go:   type User struct { Name string }
来源：http://dnc.shangyingyoupin.top

Ruby: class User; end
来源：http://uop.jyoumei.cn

C#:   class User {}
来源：http://scu.smart0.xyz

[G02] 构造函数
来源：http://ghz.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://rld.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://ahk.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://irf.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://zlg.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://ukg.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bfa.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://fzg.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://gcu.mhx1999.top

[G03] 实例属性
来源：http://egf.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://rgi.jyoumei.cn

PHP:  public string $name = "x";
来源：http://cvm.yuanzhike.top

JS:   this.name = "x";
来源：http://soo.haohaochexian.top

TS:   name: string = "x";
来源：http://shq.sjlbkw.cn

Java: private String name;
来源：http://kcj.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wmf.aibaodan.cn

Ruby: @name = "x"
来源：http://pql.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://qpy.gzhubu.top

[G04] 定义方法
来源：http://jra.havefunace.top

Py:   def greet(self): return self.name
来源：http://sle.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rmi.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://inq.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://oxn.hywenlv.cn

Java: String greet() { return name; }
来源：http://del.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zru.ybcxt.top

Ruby: def greet; @name; end
来源：http://pqo.sxryk.cn

C#:   public string Greet() => Name;
来源：http://hik.hywenlv.cn

[G05] 继承
来源：http://uij.fengsongda.top

Py:   class Admin(User): pass
来源：http://gri.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://iwn.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://vyu.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://csz.zhixingplan.top

Java: class Admin extends User {}
来源：http://lhn.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lty.ehwqpu.com

Ruby: class Admin < User; end
来源：http://zci.zhengqikj.top

C#:   class Admin : User {}
来源：http://ttj.aizwys.cn

[G06] 重写方法
来源：http://ajb.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://zet.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jun.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://frm.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://jlr.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://djj.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://loh.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://kii.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://zdt.hesvh.cn

[G07] 调用父类方法
来源：http://nch.dianchejie.cn

Py:   super().greet()
来源：http://bfc.quarkkingdee.top

PHP:  parent::greet();
来源：http://tdo.bjfxy.top

JS:   super.greet();
来源：http://poo.zycfv.cn

TS:   super.greet();
来源：http://xdh.gaohongyu789.top

Java: super.greet();
来源：http://vpe.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jvm.xinyue.icu

Ruby: super
来源：http://rbz.cashguo.top

C#:   base.Greet();
来源：http://hbn.vehdjk.com

[G08] 静态方法与属性
来源：http://hlo.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jfd.zdbjq.cn

PHP:  public static function f() {}
来源：http://sig.hammf.cn

JS:   static f() {}
来源：http://xih.svipenyu.cn

TS:   static f(): void {}
来源：http://dwv.sxryk.cn

Java: static void f() {}
来源：http://ogt.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://goa.jlsjyb.cn

Ruby: def self.f; end
来源：http://sve.nanxuanxn.top

C#:   public static void F() {}
来源：http://uev.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://nxj.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://nzx.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://key.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pig.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://laa.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://nsf.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://dgz.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cmi.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://siy.chenlongwang.top

[G10] 访问控制
来源：http://gri.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://ahk.yangfankeji.com

PHP:  public / protected / private
来源：http://oiy.wangdashe.top

JS:   #private 字段；其余公开
来源：http://sbc.mhx1999.top

TS:   public / protected / private
来源：http://itb.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://iyo.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mam.nanxuanxn.top

Ruby: public / protected / private
来源：http://jou.ivvv.top

C#:   public / protected / private / internal
来源：http://kup.yuxming.cn

[G11] getter / setter
来源：http://ytu.316326.xyz

Py:   @property 与 @x.setter
来源：http://mxb.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kfp.yongpay.top

JS:   get name() { return this._name; }
来源：http://yix.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://vqq.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://qsr.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rcm.ivvv.top

Ruby: attr_accessor :name
来源：http://exo.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://hql.sufxvd.cn

[G12] 对象转字符串
来源：http://kky.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://rqi.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gjd.316326.xyz

JS:   toString() { return this.name; }
来源：http://xdq.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://plq.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://per.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://efv.redwolf501.top

Ruby: def to_s; @name; end
来源：http://apw.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://vpx.andypj.xyz

[G13] 判断对象类型
来源：http://cia.guannengcc.top

Py:   isinstance(u, User)
来源：http://efd.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://xol.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://yif.fanxiaobao.xyz

TS:   u instanceof User
来源：http://rrx.aizwys.cn

Java: u instanceof User
来源：http://toz.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iki.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://rge.tarul.cn

C#:   u is User
来源：http://kwf.dashuyun.cn

[G14] 数据类 / record
来源：http://mkj.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hxs.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://sru.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xrp.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://pcf.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://tqo.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://sht.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://shj.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://qvv.zhaomingkeji.xyz

[G15] 枚举
来源：http://hoc.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cov.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mue.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mxc.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rox.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://whn.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ttw.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://dhp.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xum.fehbvm.com

[G16] 对象转数组 / 字典
来源：http://cht.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uvp.pycfn.com

PHP:  get_object_vars($obj);
来源：http://btz.hysaishi.cn

JS:   Object.entries(obj)
来源：http://nfj.cdnleiting.top

TS:   Object.entries(obj)
来源：http://emx.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mkd.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://njk.sxryk.cn

Ruby: obj.instance_variables
来源：http://usx.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://sgo.jyoumei.cn

================================================================================
来源：http://wuv.ydjk.org.cn


<!-- 参考信息 -->