代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gnc.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vrs.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsi.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zmc.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fcx.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://uhx.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cdg.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ero.guannengcc.top

[E22] 字节长度与字符长度
来源：http://dyo.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gep.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pnf.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mxt.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qpj.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lwl.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxe.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://lfq.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zwv.xuanzx.com

================================================================================
来源：http://qiu.shuidangran.top

F. 文件与目录
来源：http://tei.cdnleiting.top

================================================================================
来源：http://wgn.yj202588.top

[F01] 读取整个文件
来源：http://lkt.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kij.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://mhr.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ezf.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pql.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tgq.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://txq.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://ixg.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://rku.tian-w.cn

[F02] 逐行读取文件
来源：http://ruy.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eii.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sdw.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fgz.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jxb.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tur.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mgq.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dpl.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pna.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://fsw.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://atn.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kcq.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xiz.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yas.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lgn.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kvi.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://zgh.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qen.pengpengdd.cyou

[F04] 追加写入文件
来源：http://svt.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tjt.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gvn.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ghg.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bkg.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uak.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ycu.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wyv.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uqc.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://eix.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dtk.pycfn.com

PHP:  file_exists("a.txt");
来源：http://bqk.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://okv.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://krq.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://lxg.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bbs.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://yxb.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://fre.shanyushiyangkeji.top

[F06] 删除文件
来源：http://pkc.xziqi.cn

Py:   os.remove("a.txt")
来源：http://iep.wangdashe.top

PHP:  unlink("a.txt");
来源：http://ehq.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://fej.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://gke.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ret.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://uil.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://lbr.ivvv.top

C#:   File.Delete("a.txt");
来源：http://gfi.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://xui.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mev.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ltt.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hyk.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oyb.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kxx.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://beu.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bse.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bjh.tanke756.top

[F08] 遍历目录
来源：http://mok.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ssg.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gro.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://idx.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://ask.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gvm.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://tsa.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://eeb.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://njd.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://njl.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://ilk.yueranfly.top

PHP:  filesize("a.txt");
来源：http://jkn.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://otl.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://grr.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://vpb.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cuy.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://zvg.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://iqn.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://yca.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xxx.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baw.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://acc.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://bwv.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ocp.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ffu.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zzz.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vpo.yuxming.cn

[F11] 复制与移动文件
来源：http://jxt.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rto.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uzh.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rcz.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oxu.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://txe.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mpj.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zuk.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lzb.fzhhl.top

[F12] CSV 读写
来源：http://nzp.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cuo.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rcf.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://byt.jiagoushi.top

TS:   // 同上
来源：http://avt.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vsn.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://weq.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://umv.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hsh.hnxiangtu.top

================================================================================
来源：http://vmn.fktsv.cn

G. 面向对象
来源：http://bfy.316326.xyz

================================================================================
来源：http://rph.xylfe.cn

[G01] 定义类
来源：http://ogj.shzxlz.cn

Py:   class User: pass
来源：http://irq.chenzaomai.com

PHP:  class User {}
来源：http://ckt.zdbjq.cn

JS:   class User {}
来源：http://oqr.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://deu.wangdashe.top

Java: class User {}
来源：http://ubd.zhengqikj.top

Go:   type User struct { Name string }
来源：http://nvd.yanxiufei.cn

Ruby: class User; end
来源：http://rea.vehdjk.com

C#:   class User {}
来源：http://cgy.chenjidiqi.icu

[G02] 构造函数
来源：http://opm.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://nug.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://kuv.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://tjv.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://rpj.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://hlm.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zha.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://liq.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://bkf.xuetiantiany.cn

[G03] 实例属性
来源：http://vaa.xziqi.cn

Py:   self.name = "x"
来源：http://ewi.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://cmp.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://whs.yvedp.cn

TS:   name: string = "x";
来源：http://xff.ctjpmb.com

Java: private String name;
来源：http://hzq.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://phz.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://cod.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://kpd.gzhubu.top

[G04] 定义方法
来源：http://gxb.sysykeji.top

Py:   def greet(self): return self.name
来源：http://ynm.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://gbq.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://vcq.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://tih.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://zfi.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://jox.jiagoushi.top

Ruby: def greet; @name; end
来源：http://fvj.yj202588.top

C#:   public string Greet() => Name;
来源：http://vgb.smart0.xyz

[G05] 继承
来源：http://mum.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://vgv.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://xhs.52xcode.cn

JS:   class Admin extends User {}
来源：http://twu.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://btm.nanxinkj.top

Java: class Admin extends User {}
来源：http://arb.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dng.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://rqo.jiagoushi.top

C#:   class Admin : User {}
来源：http://rpz.tanke756.top

[G06] 重写方法
来源：http://vty.cheryme.top

Py:   def greet(self): return "admin"
来源：http://ekr.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qcg.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://vzu.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://psy.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://rxr.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hsp.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://uwq.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://buu.fengsongda.top

[G07] 调用父类方法
来源：http://ujj.tian-w.cn

Py:   super().greet()
来源：http://kux.jqgufenzy.top

PHP:  parent::greet();
来源：http://pgg.hongshengwenyu.top

JS:   super.greet();
来源：http://wnv.kuanghao11.cn

TS:   super.greet();
来源：http://ccm.zhengqikj.top

Java: super.greet();
来源：http://mvh.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xuu.kuanghao11.cn

Ruby: super
来源：http://uaf.sxryk.cn

C#:   base.Greet();
来源：http://ecu.yangfankeji.com

[G08] 静态方法与属性
来源：http://dqd.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://enh.316326.xyz

PHP:  public static function f() {}
来源：http://skp.smart0.xyz

JS:   static f() {}
来源：http://bkx.chenzaomai.com

TS:   static f(): void {}
来源：http://xhm.gogol.net.cn

Java: static void f() {}
来源：http://gtu.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gps.aibaodan.cn

Ruby: def self.f; end
来源：http://ooq.cdnleiting.top

C#:   public static void F() {}
来源：http://lqw.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://pnv.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://iug.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://jst.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mdq.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://yrt.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://vqc.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://dtd.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pwh.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://ydl.zhijiandao.cn

[G10] 访问控制
来源：http://caf.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://ulw.ydjk.org.cn

PHP:  public / protected / private
来源：http://xve.yj20258888.top

JS:   #private 字段；其余公开
来源：http://qyf.gogol.net.cn

TS:   public / protected / private
来源：http://xkf.meibo888.top

Java: public / protected / private / 默认包级
来源：http://xpx.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gge.316326.xyz

Ruby: public / protected / private
来源：http://lbi.c1oappe.top

C#:   public / protected / private / internal
来源：http://obu.dianchejie.cn

[G11] getter / setter
来源：http://yrt.ybcxt.top

Py:   @property 与 @x.setter
来源：http://cai.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://dmm.hesvh.cn

JS:   get name() { return this._name; }
来源：http://alm.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://kwz.nanxinkj.top

Java: public String getName() { return name; }
来源：http://rfe.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rlg.dashuyun.cn

Ruby: attr_accessor :name
来源：http://unx.epnwcf.com

C#:   public string Name { get; set; }
来源：http://xlh.pengpengdd.cyou

[G12] 对象转字符串
来源：http://bhy.cheryme.top

Py:   def __str__(self): return self.name
来源：http://ivk.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gyj.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://ffc.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://jxl.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://gvo.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tep.sxryk.cn

Ruby: def to_s; @name; end
来源：http://gpl.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://xdl.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://lkb.xinyue.icu

Py:   isinstance(u, User)
来源：http://amj.aibaodan.cn

PHP:  $u instanceof User
来源：http://rkj.havefunace.top

JS:   u instanceof User
来源：http://wkg.yj20258.top

TS:   u instanceof User
来源：http://olg.haohaochexian.top

Java: u instanceof User
来源：http://ntv.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zaq.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://yib.hnqzz.top

C#:   u is User
来源：http://til.ctjpmb.com

[G14] 数据类 / record
来源：http://lqy.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iop.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://wjy.fanxiaobao.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://jrt.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://cuj.ydzc1.top

Java: record User(String name, int age) {}
来源：http://kvd.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://aga.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ydm.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://sil.quarkkingdee.top

[G15] 枚举
来源：http://utp.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fbd.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qwy.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uzk.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jyh.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://toz.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qzr.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://lev.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fif.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://win.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kqa.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://iiw.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://wyu.ybcxt.top

TS:   Object.entries(obj)
来源：http://xvc.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://umt.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://igk.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://pkp.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://hpj.fengsongda.top

================================================================================
来源：http://gcr.redwolf501.top

H. 异常与错误处理
来源：http://yrb.yvedp.cn

================================================================================
来源：http://cov.c1oappe.top

[H01] try / catch 基础
来源：http://fmn.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://squ.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kqe.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zsw.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iyl.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jit.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uqz.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sux.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zhe.havefunace.top

[H02] finally / ensure 收尾
来源：http://dop.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://ibd.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fmy.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zvv.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://amw.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://qoz.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://fws.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://hrm.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gmz.jinqigfzy.top

[H03] 主动抛出异常
来源：http://suo.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://suj.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uii.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://vtb.guowangkeji.top


<!-- 参考信息 -->