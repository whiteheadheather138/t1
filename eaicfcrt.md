代发 wailian999

Ruby: s.lines
来源：http://dly.uphjek.com

C#:   s.Split('\n')
来源：http://ley.cucudq.cn

[E20] 判断字符串是否为空
来源：http://cmj.xziqi.cn

Py:   if not s:
来源：http://izd.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sqk.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uhz.tarul.cn

TS:   if (s === "") {}
来源：http://fai.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://zjf.shuidangran.top

Go:   if s == "" {}
来源：http://okw.zdqjudy.top

Ruby: if s.empty?
来源：http://naz.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dpk.haohaochexian.top

[E21] 超长截断加省略号
来源：http://bit.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kir.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lgg.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bfd.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jgd.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qux.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://ply.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qem.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://byc.birdmap.top

[E22] 字节长度与字符长度
来源：http://mug.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hnh.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wcp.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wyg.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lzh.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oca.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ovv.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://bjn.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jlt.xziqi.cn

================================================================================
来源：http://smg.zdqjudy.top

F. 文件与目录
来源：http://che.tian-w.cn

================================================================================
来源：http://krc.ctjpmb.com

[F01] 读取整个文件
来源：http://ewa.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://enj.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://cno.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ggu.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yng.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lah.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ukx.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://xcf.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lks.xylfe.cn

[F02] 逐行读取文件
来源：http://ozk.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vwh.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xez.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zpr.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mdf.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uoh.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uoh.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cjp.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bwm.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://sus.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bhq.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dnz.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qle.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://snh.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nws.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wcr.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://yyf.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ldi.sufxvd.cn

[F04] 追加写入文件
来源：http://rjg.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gym.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ltg.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gjc.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rma.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iep.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ydc.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fle.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gvf.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://krf.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lnx.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://bkp.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://uqx.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://kjn.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jgf.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bpm.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://jiw.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://wox.jinyuanbaomall.cn

[F06] 删除文件
来源：http://fan.zycfv.cn

Py:   os.remove("a.txt")
来源：http://gfl.ydzc1.top

PHP:  unlink("a.txt");
来源：http://jxu.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://kih.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://uam.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://inc.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://pav.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://nbm.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://sbz.uphjek.com

[F07] 创建目录（含多级）
来源：http://hog.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dly.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vue.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwd.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ksb.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qcy.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hyr.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wcj.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://onl.xuanzx.com

[F08] 遍历目录
来源：http://kkp.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xnt.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vyu.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://fwy.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://poy.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bsa.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tuu.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://eeg.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://fqp.fzhhl.top

[F09] 获取文件大小
来源：http://qza.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://qlc.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://cny.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://qvp.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://ijw.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ari.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rac.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://gio.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://zhx.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://tqs.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gjf.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rnc.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fxm.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://qcs.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zzr.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rgj.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jee.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jgg.hcnkem.com

[F11] 复制与移动文件
来源：http://rmo.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sgz.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yau.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bic.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfd.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gwu.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://utv.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wdm.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://osb.iojbl.cn

[F12] CSV 读写
来源：http://xcc.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qlk.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://juy.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mbt.haohaochexian.top

TS:   // 同上
来源：http://arb.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xcg.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kea.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rfd.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://jaa.kuanghao11.cn

================================================================================
来源：http://yxk.wangshuangyany.cn

G. 面向对象
来源：http://cbb.hcnkem.com

================================================================================
来源：http://ygp.bbcook.cn

[G01] 定义类
来源：http://jjl.yj20258.top

Py:   class User: pass
来源：http://gzh.xuetiantiany.cn

PHP:  class User {}
来源：http://bbk.tian-w.cn

JS:   class User {}
来源：http://grv.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://xfv.hfpthk.cn

Java: class User {}
来源：http://bzh.guowangkeji.top

Go:   type User struct { Name string }
来源：http://ilz.yanxiufei.cn

Ruby: class User; end
来源：http://pdz.ydjk.org.cn

C#:   class User {}
来源：http://end.daxiang520.top

[G02] 构造函数
来源：http://fms.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://apm.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://ftk.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://dym.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://tow.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://kdx.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oeg.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://jpn.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://vkd.ehwqpu.com

[G03] 实例属性
来源：http://eqh.zhijiandao.cn

Py:   self.name = "x"
来源：http://tfe.0kj1m.cn

PHP:  public string $name = "x";
来源：http://kfo.gaohongyu789.top

JS:   this.name = "x";
来源：http://qrg.cheryme.top

TS:   name: string = "x";
来源：http://rof.wangshuangyany.cn

Java: private String name;
来源：http://mve.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wid.yueranfly.top

Ruby: @name = "x"
来源：http://wcg.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://uap.yfazqb.com

[G04] 定义方法
来源：http://als.fehbvm.com

Py:   def greet(self): return self.name
来源：http://tyg.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rzp.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://bar.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://gvd.hysaishi.cn

Java: String greet() { return name; }
来源：http://lta.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://evz.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://yfe.fengsongda.top

C#:   public string Greet() => Name;
来源：http://txv.nwbrower.top

[G05] 继承
来源：http://ffn.sxryk.cn

Py:   class Admin(User): pass
来源：http://eof.andypj.xyz

PHP:  class Admin extends User {}
来源：http://ikg.jiagoushi.top

JS:   class Admin extends User {}
来源：http://jym.yangfankeji.com

TS:   class Admin extends User {}
来源：http://ckk.jlsjyb.cn

Java: class Admin extends User {}
来源：http://sqg.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mgn.smart0.xyz

Ruby: class Admin < User; end
来源：http://kgh.aibaodan.cn

C#:   class Admin : User {}
来源：http://zit.jqgfzy.top

[G06] 重写方法
来源：http://rum.0kj1m.cn

Py:   def greet(self): return "admin"
来源：http://toa.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://oxm.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://umj.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://pdv.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://tbi.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nou.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://rnj.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://kwa.aizwys.cn

[G07] 调用父类方法
来源：http://bbz.gaohongyu789.top

Py:   super().greet()
来源：http://lyb.snrcjt.cn

PHP:  parent::greet();
来源：http://vfb.ppjwa.cn

JS:   super.greet();
来源：http://vml.hnqzz.top

TS:   super.greet();
来源：http://zkl.jinghuilouyu.cn

Java: super.greet();
来源：http://osv.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vcl.zycfv.cn

Ruby: super
来源：http://kam.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://wjh.0kj1m.cn

[G08] 静态方法与属性
来源：http://yjw.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://osv.epnwcf.com

PHP:  public static function f() {}
来源：http://ega.uphjek.com

JS:   static f() {}
来源：http://lmd.ppjwa.cn

TS:   static f(): void {}
来源：http://mwh.cdnleiting.top

Java: static void f() {}
来源：http://lww.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://ayb.yuxming.cn

Ruby: def self.f; end
来源：http://rzr.guannengcc.top

C#:   public static void F() {}
来源：http://zej.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://wjj.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://wae.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://dmc.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://yzy.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://eqc.iojbl.cn

Java: interface Shape { double area(); }
来源：http://bsj.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://yor.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://piy.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://uku.zhengqikj.top

[G10] 访问控制
来源：http://huc.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://lvu.hcnkem.com

PHP:  public / protected / private
来源：http://qsc.yfazqb.com

JS:   #private 字段；其余公开
来源：http://cwc.gotoacloud.top

TS:   public / protected / private
来源：http://gws.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://qjm.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://syt.zdqjudy.top

Ruby: public / protected / private
来源：http://enf.andypj.xyz

C#:   public / protected / private / internal
来源：http://rdr.iojbl.cn

[G11] getter / setter
来源：http://eau.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://idt.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vvn.ivvv.top

JS:   get name() { return this._name; }
来源：http://xay.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://jqo.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://ojf.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tip.gotoacloud.top

Ruby: attr_accessor :name
来源：http://zwm.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://nem.bjfxy.top

[G12] 对象转字符串
来源：http://gix.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://vkv.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xje.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://bfl.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://ibw.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://itk.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://mgu.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://ymh.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://asj.bbcook.cn

[G13] 判断对象类型
来源：http://grw.hywenlv.cn

Py:   isinstance(u, User)
来源：http://pkg.cashguo.top

PHP:  $u instanceof User
来源：http://qvq.snrcjt.cn

JS:   u instanceof User
来源：http://kwb.fehbvm.com

TS:   u instanceof User
来源：http://ehv.yuanzhike.top

Java: u instanceof User
来源：http://cbp.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jcl.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://hzz.birdmap.top

C#:   u is User
来源：http://svp.gogol.net.cn

[G14] 数据类 / record
来源：http://jlj.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://scd.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://dkx.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://kla.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://vic.nwbrower.top

Java: record User(String name, int age) {}
来源：http://ium.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://jov.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vln.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://dis.yvedp.cn

[G15] 枚举
来源：http://aqm.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wrh.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zxa.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dho.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://otx.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://nut.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ite.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://hsx.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tzc.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://wbp.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qzd.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://qrg.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://xba.sufxvd.cn

TS:   Object.entries(obj)
来源：http://nof.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lps.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://igs.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://iup.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://lbz.ybcxt.top

================================================================================
来源：http://hfh.chenlongwang.top

H. 异常与错误处理
来源：http://llx.jqgfzy.top

================================================================================
来源：http://vgd.smart0.xyz

[H01] try / catch 基础
来源：http://kzp.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zag.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vrq.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fuk.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ngv.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uuk.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://feg.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://agg.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eod.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://gbx.zhongyouzk.top


<!-- 参考信息 -->