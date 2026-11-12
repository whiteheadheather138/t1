代发 wailian999

Ruby: s.lines
来源：http://rvc.yueranfly.top

C#:   s.Split('\n')
来源：http://rqx.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://umw.quarkkingdee.top

Py:   if not s:
来源：http://tnn.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jvz.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ubl.cdnleiting.top

TS:   if (s === "") {}
来源：http://jak.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://tgq.zycfv.cn

Go:   if s == "" {}
来源：http://evg.gotoacloud.top

Ruby: if s.empty?
来源：http://nsc.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ahm.gotoacloud.top

[E21] 超长截断加省略号
来源：http://wvw.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xky.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://umy.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lkb.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbq.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ubc.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://cxf.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://adx.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://isb.ybcxt.top

[E22] 字节长度与字符长度
来源：http://mbj.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wab.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xqh.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://itg.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qek.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xou.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fru.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://tqf.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vls.52xcode.cn

================================================================================
来源：http://upf.hnqzz.top

F. 文件与目录
来源：http://mak.yangfankeji.com

================================================================================
来源：http://inb.guowangkeji.top

[F01] 读取整个文件
来源：http://col.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ixg.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://chz.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xac.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://grf.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bcu.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pek.bbcook.cn

Ruby: File.read("a.txt")
来源：http://fez.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://eow.meibo888.top

[F02] 逐行读取文件
来源：http://syh.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ctv.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://diy.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dli.ywan-chungtsiang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ojr.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dqo.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sag.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kik.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nfo.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://dol.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jrb.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hnh.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hxc.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jaq.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vht.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jmr.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://epw.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://czg.c1oappe.top

[F04] 追加写入文件
来源：http://mzx.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yai.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mun.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xua.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lay.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xlv.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fgg.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://elk.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uyk.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://qus.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://udn.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://fzz.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://mhf.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://aqi.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jli.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lut.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://xbq.yj202588.top

C#:   File.Exists("a.txt")
来源：http://zrq.fktsv.cn

[F06] 删除文件
来源：http://snh.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://wsh.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://eew.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ljj.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hpd.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ghi.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://zqt.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://aou.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://xoh.sxryk.cn

[F07] 创建目录（含多级）
来源：http://ueu.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fby.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lgu.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qez.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hvl.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eyb.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uyk.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xwk.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wlj.nanxinkj.top

[F08] 遍历目录
来源：http://vlg.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://cdo.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ibj.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://jpq.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://rsd.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dnx.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://roj.yj20258.top

Ruby: Dir.children("dir")
来源：http://gnu.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://qag.yanxiufei.cn

[F09] 获取文件大小
来源：http://nsc.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://epo.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://uvm.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://hbh.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://arq.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://mnt.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iev.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://fpj.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://tto.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://qsa.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ccy.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qoq.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aih.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://cxo.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pvm.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jpi.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://acx.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bcg.shuidangran.top

[F11] 复制与移动文件
来源：http://mec.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nme.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jay.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://srt.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hbb.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ier.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uox.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://orc.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fzw.chenjidiqi.icu

[F12] CSV 读写
来源：http://ayn.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mhj.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ayw.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xde.quarkkingdee.top

TS:   // 同上
来源：http://uof.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wur.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zyu.jinghuilouyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lzs.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rzz.xingfuxueyuan.xyz

================================================================================
来源：http://qzm.shanyushiyangtech.top

G. 面向对象
来源：http://deg.zdbjq.cn

================================================================================
来源：http://mbs.fzhhl.top

[G01] 定义类
来源：http://fcn.yonumen.top

Py:   class User: pass
来源：http://jhf.zhoulong.xyz

PHP:  class User {}
来源：http://bsa.pengpengdd.cyou

JS:   class User {}
来源：http://xpi.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://usc.0kj1m.cn

Java: class User {}
来源：http://ytf.xinyue.icu

Go:   type User struct { Name string }
来源：http://jdi.shanyushiyangtech.top

Ruby: class User; end
来源：http://jdt.mhx1999.top

C#:   class User {}
来源：http://tga.yj20258888.top

[G02] 构造函数
来源：http://mpb.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://zuq.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://jrv.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://oqp.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://qnu.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://jvn.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hjb.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://vro.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://twl.xuanzx.com

[G03] 实例属性
来源：http://tst.jyoumei.cn

Py:   self.name = "x"
来源：http://fxn.jinqigufen.top

PHP:  public string $name = "x";
来源：http://afu.jianghu66.top

JS:   this.name = "x";
来源：http://hxe.chenzaomai.com

TS:   name: string = "x";
来源：http://dpq.hongshengwenyu.top

Java: private String name;
来源：http://rio.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lnj.yueranfly.top

Ruby: @name = "x"
来源：http://jcl.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://var.yfazqb.com

[G04] 定义方法
来源：http://npn.bjfxy.top

Py:   def greet(self): return self.name
来源：http://vvn.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ccg.ywan-chungtsiang.top

JS:   greet() { return this.name; }
来源：http://xao.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://uuz.dashuyun.cn

Java: String greet() { return name; }
来源：http://eyn.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zyr.dianchejie.cn

Ruby: def greet; @name; end
来源：http://dvr.redwolf501.top

C#:   public string Greet() => Name;
来源：http://dca.pengpengdd.cyou

[G05] 继承
来源：http://ttg.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://utt.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://rst.havefunace.top

JS:   class Admin extends User {}
来源：http://lxj.yangfankeji.com

TS:   class Admin extends User {}
来源：http://vik.shuidangran.top

Java: class Admin extends User {}
来源：http://fps.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yxq.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://jei.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://hbm.hcnkem.com

[G06] 重写方法
来源：http://nyp.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://qli.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://drs.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://wxx.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://dhe.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://fxe.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qam.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://qiu.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://jtg.yj20258888.top

[G07] 调用父类方法
来源：http://ydu.yj20258.top

Py:   super().greet()
来源：http://twi.svipenyu.cn

PHP:  parent::greet();
来源：http://phn.wangdashe.top

JS:   super.greet();
来源：http://equ.daxiang520.top

TS:   super.greet();
来源：http://kio.cucudq.cn

Java: super.greet();
来源：http://ukr.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oof.fktsv.cn

Ruby: super
来源：http://cyv.fzhhl.top

C#:   base.Greet();
来源：http://owb.yanxiufei.cn

[G08] 静态方法与属性
来源：http://cld.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xtk.chenlongwang.top

PHP:  public static function f() {}
来源：http://zzy.zhongyouzk.top

JS:   static f() {}
来源：http://qss.yuanzhike.top

TS:   static f(): void {}
来源：http://xej.ehwqpu.com

Java: static void f() {}
来源：http://gkk.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fnt.bjfxy.top

Ruby: def self.f; end
来源：http://oht.cdnleiting.top

C#:   public static void F() {}
来源：http://mlj.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://zoa.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://rdw.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qba.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ihk.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://cqc.bbcook.cn

Java: interface Shape { double area(); }
来源：http://mfd.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://lqo.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xug.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://fby.xuetiantiany.cn

[G10] 访问控制
来源：http://yrq.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://kqf.zhoulong.xyz

PHP:  public / protected / private
来源：http://thl.andypj.xyz

JS:   #private 字段；其余公开
来源：http://zaa.ehwqpu.com

TS:   public / protected / private
来源：http://tos.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://cvy.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nmj.daxiang520.top

Ruby: public / protected / private
来源：http://vrk.ehwqpu.com

C#:   public / protected / private / internal
来源：http://ktp.sjlbkw.cn

[G11] getter / setter
来源：http://tew.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://vop.shangyingyoupin.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ufo.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://sgu.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://gop.shzxlz.cn

Java: public String getName() { return name; }
来源：http://xvh.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kee.c1oappe.top

Ruby: attr_accessor :name
来源：http://fci.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://cfg.c1oappe.top

[G12] 对象转字符串
来源：http://wdf.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://qgg.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://war.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://uci.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://bon.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://evq.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uhv.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://vjj.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://htk.jinqigufen.top

[G13] 判断对象类型
来源：http://usk.mhx1999.top

Py:   isinstance(u, User)
来源：http://ltu.jqgufenzy.top

PHP:  $u instanceof User
来源：http://ocm.vqdsnc.cn

JS:   u instanceof User
来源：http://ezs.yanxiufei.cn

TS:   u instanceof User
来源：http://pwr.quarkkingdee.top

Java: u instanceof User
来源：http://oue.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ahg.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://pex.cqqwz.cn

C#:   u is User
来源：http://owf.0kj1m.cn

[G14] 数据类 / record
来源：http://kvs.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sqg.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://nff.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://uku.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://bfu.yj20258.top

Java: record User(String name, int age) {}
来源：http://hns.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://onq.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hxl.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://gmj.dashuyun.cn

[G15] 枚举
来源：http://ism.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uts.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dkk.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oci.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yrn.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://ked.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://arx.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://urv.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://imo.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://bkw.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oki.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://ggi.hysaishi.cn

JS:   Object.entries(obj)
来源：http://ldc.gotoacloud.top

TS:   Object.entries(obj)
来源：http://ojy.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hjd.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yrl.0kj1m.cn

Ruby: obj.instance_variables
来源：http://rwb.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://rvc.jqgfzy.top

================================================================================
来源：http://xkf.sxryk.cn

H. 异常与错误处理
来源：http://mci.dashuyun.cn

================================================================================
来源：http://rjb.zhoulong.xyz

[H01] try / catch 基础
来源：http://doi.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wno.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://joe.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sii.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ixf.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cvq.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qfi.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ibv.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ykc.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://zva.yanxiufei.cn


<!-- 参考信息 -->