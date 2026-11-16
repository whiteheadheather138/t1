代发 wailian999

Ruby: s.lines
来源：http://pnj.chenlongwang.top

C#:   s.Split('\n')
来源：http://kfp.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://muu.fengsongda.top

Py:   if not s:
来源：http://tux.zhengqikj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mtq.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xtp.mhx1999.top

TS:   if (s === "") {}
来源：http://smh.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://qra.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://xre.ivvv.top

Ruby: if s.empty?
来源：http://euw.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vig.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://sga.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kfs.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ptj.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jib.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqc.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ywk.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://ejm.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fmm.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pke.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://akf.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mit.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yua.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aqy.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eyx.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dyh.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ckb.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://kup.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jrw.hnqzz.top

================================================================================
来源：http://phl.bbcook.cn

F. 文件与目录
来源：http://ofg.xziqi.cn

================================================================================
来源：http://ojx.sysykeji.top

[F01] 读取整个文件
来源：http://ees.xingfuxueyuan.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fie.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://xzo.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://woj.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wtd.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iqa.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pwl.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://hbr.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://iub.ydjk.org.cn

[F02] 逐行读取文件
来源：http://mzv.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ykr.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zcc.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nou.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xfx.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ugx.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fet.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rzs.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zwm.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://onh.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ubd.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hjm.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpt.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://inw.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sik.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ito.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://vjb.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pdy.yonumen.top

[F04] 追加写入文件
来源：http://lne.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bak.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mma.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bxl.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://flx.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://esq.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xtk.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iby.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lbp.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://bdr.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qzd.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://ugt.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://obp.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://uaq.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mgi.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fbt.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://ncr.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://sqf.hesvh.cn

[F06] 删除文件
来源：http://amv.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://kkv.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://fsn.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://mmc.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://wec.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jno.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://ybc.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://amy.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://wxw.wangdashe.top

[F07] 创建目录（含多级）
来源：http://yxr.cqqwz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ics.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ixe.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://php.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rlw.epnwcf.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sgi.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qpd.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zmx.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xnl.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://dgu.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ygn.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oan.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://dls.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://lux.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kkp.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://hpp.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://rqv.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://tlt.yueranfly.top

[F09] 获取文件大小
来源：http://oeg.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://vpw.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://dje.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://oif.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://twj.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://civ.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qyd.xuanzx.com

Ruby: File.size("a.txt")
来源：http://amv.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://qpa.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://tbi.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lwr.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://myq.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hdp.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://aaj.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vvy.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oxf.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yyu.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://orn.c1oappe.top

[F11] 复制与移动文件
来源：http://ucm.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hgk.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://evb.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hxx.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tdj.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fwk.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mvj.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nxa.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nzh.jinqigfzy.top

[F12] CSV 读写
来源：http://apy.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ynx.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://euo.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rek.shanyushiyangtech.top

TS:   // 同上
来源：http://tjr.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dow.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qbx.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xsm.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gng.gotoacloud.top

================================================================================
来源：http://kkd.hnxiangtu.top

G. 面向对象
来源：http://ghd.zhoulong.xyz

================================================================================
来源：http://tov.hywenlv.cn

[G01] 定义类
来源：http://yrl.xylfe.cn

Py:   class User: pass
来源：http://yxx.xziqi.cn

PHP:  class User {}
来源：http://kly.fktsv.cn

JS:   class User {}
来源：http://btc.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://olq.jlsjyb.cn

Java: class User {}
来源：http://yod.gzhubu.top

Go:   type User struct { Name string }
来源：http://bcn.chenzaomai.com

Ruby: class User; end
来源：http://fcs.tian-w.cn

C#:   class User {}
来源：http://avo.guannengcc.top

[G02] 构造函数
来源：http://iiz.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://dnr.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://rzf.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://aze.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://ucg.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://psz.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://omw.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://esx.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://xhi.svipenyu.cn

[G03] 实例属性
来源：http://bjy.jinqigufen.top

Py:   self.name = "x"
来源：http://qie.sweek.top

PHP:  public string $name = "x";
来源：http://ukl.hfpthk.cn

JS:   this.name = "x";
来源：http://hcn.dianchejie.cn

TS:   name: string = "x";
来源：http://zsr.iojbl.cn

Java: private String name;
来源：http://ofq.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olq.aibaodan.cn

Ruby: @name = "x"
来源：http://clu.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://mcb.chenlongwang.top

[G04] 定义方法
来源：http://crn.sweek.top

Py:   def greet(self): return self.name
来源：http://frw.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zur.316326.xyz

JS:   greet() { return this.name; }
来源：http://ccj.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://lex.haohaochexian.top

Java: String greet() { return name; }
来源：http://vba.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jul.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://cpk.birdmap.top

C#:   public string Greet() => Name;
来源：http://nmu.fanxiaobao.xyz

[G05] 继承
来源：http://ehu.gzhubu.top

Py:   class Admin(User): pass
来源：http://noz.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://hoo.jinqigufen.top

JS:   class Admin extends User {}
来源：http://mgt.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://uux.cdnleiting.top

Java: class Admin extends User {}
来源：http://aaw.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qkf.xylfe.cn

Ruby: class Admin < User; end
来源：http://cli.epnwcf.com

C#:   class Admin : User {}
来源：http://vtt.dashuyun.cn

[G06] 重写方法
来源：http://kkd.yongpay.top

Py:   def greet(self): return "admin"
来源：http://riy.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rwg.316326.xyz

JS:   greet() { return "admin"; }
来源：http://ack.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://sew.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://gxe.jinyuanbaomall.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oke.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://ruk.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://fnc.sysykeji.top

[G07] 调用父类方法
来源：http://gwl.vqdsnc.cn

Py:   super().greet()
来源：http://qiu.zhixingplan.top

PHP:  parent::greet();
来源：http://scj.zhengqikj.top

JS:   super.greet();
来源：http://aag.tian-w.cn

TS:   super.greet();
来源：http://mnw.nwbrower.top

Java: super.greet();
来源：http://prj.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lqy.sjlbkw.cn

Ruby: super
来源：http://zrc.yanxiufei.cn

C#:   base.Greet();
来源：http://qmf.zdbjq.cn

[G08] 静态方法与属性
来源：http://sbo.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tcf.yonumen.top

PHP:  public static function f() {}
来源：http://fxk.tianlin.xyz

JS:   static f() {}
来源：http://dse.shangyingyoupin.top

TS:   static f(): void {}
来源：http://zet.nanxuanxn.top

Java: static void f() {}
来源：http://sef.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://krs.bjfxy.top

Ruby: def self.f; end
来源：http://nzw.meibo888.top

C#:   public static void F() {}
来源：http://xmq.havefunace.top

[G09] 接口 / 抽象类
来源：http://ubq.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://ted.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ayd.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qtv.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://jie.mhx1999.top

Java: interface Shape { double area(); }
来源：http://csj.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://cqa.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qtk.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://dqy.yongpay.top

[G10] 访问控制
来源：http://urz.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://hcx.ybcxt.top

PHP:  public / protected / private
来源：http://ugj.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://rde.fktsv.cn

TS:   public / protected / private
来源：http://qwh.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://jrn.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yrt.yj20258888.top

Ruby: public / protected / private
来源：http://bdr.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://wcv.smart0.xyz

[G11] getter / setter
来源：http://dnj.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://bif.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pdc.ivvv.top

JS:   get name() { return this._name; }
来源：http://dnc.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://orr.cqqwz.cn

Java: public String getName() { return name; }
来源：http://shp.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hyi.0kj1m.cn

Ruby: attr_accessor :name
来源：http://agd.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://bwx.zhengqikj.top

[G12] 对象转字符串
来源：http://tdh.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://iqj.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tgw.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://rkq.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://bjc.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://ytc.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://sov.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://pnt.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://fjy.andypj.xyz

[G13] 判断对象类型
来源：http://gng.yvedp.cn

Py:   isinstance(u, User)
来源：http://qyr.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://wzn.yangfankeji.com

JS:   u instanceof User
来源：http://vhd.yueranfly.top

TS:   u instanceof User
来源：http://jsj.ydzc1.top

Java: u instanceof User
来源：http://xsd.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvi.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://mru.gotoacloud.top

C#:   u is User
来源：http://dev.iojbl.cn

[G14] 数据类 / record
来源：http://zbc.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vdo.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://qkd.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://acr.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://oxq.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://uaj.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://umt.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nzd.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://ilx.yvedp.cn

[G15] 枚举
来源：http://grd.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pql.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mjn.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vss.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fgc.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://axt.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://acp.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://ryf.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kex.meibo888.top

[G16] 对象转数组 / 字典
来源：http://jty.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lyx.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://tpd.yj20258.top

JS:   Object.entries(obj)
来源：http://vot.smart0.xyz

TS:   Object.entries(obj)
来源：http://cgn.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fvz.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aed.gogol.net.cn

Ruby: obj.instance_variables
来源：http://igs.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://hjs.guowangkeji.top

================================================================================
来源：http://ths.yj202588.top

H. 异常与错误处理
来源：http://ugv.52xcode.cn

================================================================================
来源：http://dgq.yvedp.cn

[H01] try / catch 基础
来源：http://wql.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gsj.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iou.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://epr.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pgz.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wzw.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://air.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zly.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://spf.hesvh.cn

[H02] finally / ensure 收尾
来源：http://zer.nwbrower.top


<!-- 参考信息 -->