代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dzf.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oeb.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eyd.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ofk.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fqc.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://qxo.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qow.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pul.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://wxe.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vqi.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://utc.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qrl.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yzc.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zzd.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vca.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://igv.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://axl.yj20258.top

================================================================================
来源：http://zmt.zhoulong.xyz

F. 文件与目录
来源：http://ykm.bjfxy.top

================================================================================
来源：http://hks.dashuyun.cn

[F01] 读取整个文件
来源：http://bxn.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xay.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://uzh.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mkv.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zbl.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kkb.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cnk.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://kyb.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://flj.yangfankeji.com

[F02] 逐行读取文件
来源：http://hya.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vjx.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hyn.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://koo.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yja.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kdj.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qjk.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eca.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gwo.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://rpg.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://psm.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://web.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nbj.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lqb.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xnj.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tgu.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://hni.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rte.gzhubu.top

[F04] 追加写入文件
来源：http://dyj.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qhq.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ops.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://epf.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rmf.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://daf.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pvu.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hxx.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://soj.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://mrj.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://axa.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://rbb.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://wyn.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://gns.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pcr.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tiv.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://zue.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://haj.xuanzx.com

[F06] 删除文件
来源：http://nbd.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://trz.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://xjq.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://dzd.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://fck.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qgw.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://jdi.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://naf.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://veo.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://stm.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jdb.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zkc.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dmi.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uhx.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://exb.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fck.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cjh.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rsd.redwolf501.top

[F08] 遍历目录
来源：http://ela.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fro.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://urq.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://nhg.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://xqy.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://grb.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://zct.yongpay.top

Ruby: Dir.children("dir")
来源：http://tvv.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://dzf.dianchejie.cn

[F09] 获取文件大小
来源：http://sem.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://bao.shuidangran.top

PHP:  filesize("a.txt");
来源：http://frm.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://cvl.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://hsv.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kum.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://abj.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://wkm.iojbl.cn

C#:   new FileInfo("a.txt").Length
来源：http://sek.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://fkx.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lpx.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uqz.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fww.epnwcf.com

TS:   path.extname("a.txt")
来源：http://ort.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gnw.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://osb.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oap.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pwa.jinqigfzy.top

[F11] 复制与移动文件
来源：http://bqj.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://evl.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uxq.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cfx.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cex.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pdq.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qcl.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nzb.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zfe.birdmap.top

[F12] CSV 读写
来源：http://bzc.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dww.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://juo.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lkf.tarul.cn

TS:   // 同上
来源：http://yxw.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yqy.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ybq.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gjr.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://kpw.nwbrower.top

================================================================================
来源：http://rua.chenlongwang.top

G. 面向对象
来源：http://god.xinyue.icu

================================================================================
来源：http://nua.zhiwuduotai.top

[G01] 定义类
来源：http://neq.tian-w.cn

Py:   class User: pass
来源：http://vxw.chenzaomai.com

PHP:  class User {}
来源：http://nme.yj20258888.top

JS:   class User {}
来源：http://thh.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://zih.jianghu66.top

Java: class User {}
来源：http://feh.jinqigufen.top

Go:   type User struct { Name string }
来源：http://iuf.aibaodan.cn

Ruby: class User; end
来源：http://anl.havefunace.top

C#:   class User {}
来源：http://tsn.feifeiyinyue.top

[G02] 构造函数
来源：http://koj.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://bki.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://grb.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://hcs.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://tcl.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://naa.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://acd.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://gup.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://vav.bjfxy.top

[G03] 实例属性
来源：http://yoy.ivvv.top

Py:   self.name = "x"
来源：http://fiu.tanke756.top

PHP:  public string $name = "x";
来源：http://eok.bjfxy.top

JS:   this.name = "x";
来源：http://yhz.zhijiandao.cn

TS:   name: string = "x";
来源：http://blg.wangshuangyany.cn

Java: private String name;
来源：http://cvk.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fjy.daria6918.cn

Ruby: @name = "x"
来源：http://kso.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://she.sysykeji.top

[G04] 定义方法
来源：http://wef.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://hdw.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oyh.xziqi.cn

JS:   greet() { return this.name; }
来源：http://oyu.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://osu.ivvv.top

Java: String greet() { return name; }
来源：http://glk.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gfa.tarul.cn

Ruby: def greet; @name; end
来源：http://dgj.sxryk.cn

C#:   public string Greet() => Name;
来源：http://xgr.sxryk.cn

[G05] 继承
来源：http://oiv.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://nuu.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://cjl.jinqigfzy.top

JS:   class Admin extends User {}
来源：http://eqm.hammf.cn

TS:   class Admin extends User {}
来源：http://pae.cqqwz.cn

Java: class Admin extends User {}
来源：http://zit.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://msf.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://faw.ehwqpu.com

C#:   class Admin : User {}
来源：http://nwu.dashuyun.cn

[G06] 重写方法
来源：http://pzg.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://zxq.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://scl.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://gtp.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://rtq.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://lnx.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xqw.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://xnd.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://csy.wangdashe.top

[G07] 调用父类方法
来源：http://qhz.zhijiandao.cn

Py:   super().greet()
来源：http://dru.bbcook.cn

PHP:  parent::greet();
来源：http://dud.fktsv.cn

JS:   super.greet();
来源：http://yfd.xziqi.cn

TS:   super.greet();
来源：http://xkx.xylfe.cn

Java: super.greet();
来源：http://pke.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hwk.52xcode.cn

Ruby: super
来源：http://wzl.hcnkem.com

C#:   base.Greet();
来源：http://uxs.yanxiufei.cn

[G08] 静态方法与属性
来源：http://acl.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nyl.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://mzn.quarkkingdee.top

JS:   static f() {}
来源：http://iec.hfpthk.cn

TS:   static f(): void {}
来源：http://qkp.0kj1m.cn

Java: static void f() {}
来源：http://gty.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://her.uphjek.com

Ruby: def self.f; end
来源：http://ift.cheryme.top

C#:   public static void F() {}
来源：http://ngk.wangdashe.top

[G09] 接口 / 抽象类
来源：http://phq.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://zua.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://krs.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uub.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://jqk.yongpay.top

Java: interface Shape { double area(); }
来源：http://jfu.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://nsj.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://euc.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://aaw.ydjk.org.cn

[G10] 访问控制
来源：http://odd.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://mse.zhixingplan.top

PHP:  public / protected / private
来源：http://zja.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://byz.fengsongda.top

TS:   public / protected / private
来源：http://pel.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://xfp.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://adt.xuanzx.com

Ruby: public / protected / private
来源：http://cky.vehdjk.com

C#:   public / protected / private / internal
来源：http://vaf.fanxiaobao.xyz

[G11] getter / setter
来源：http://yhb.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://zyu.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://azy.tian-w.cn

JS:   get name() { return this._name; }
来源：http://beq.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://wex.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://arj.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dvx.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://ahm.tanke756.top

C#:   public string Name { get; set; }
来源：http://czm.xylfe.cn

[G12] 对象转字符串
来源：http://ccp.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://vuf.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://opd.daxiang520.top

JS:   toString() { return this.name; }
来源：http://kwp.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://vsc.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://ukk.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://prm.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://sla.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://awe.zhixingplan.top

[G13] 判断对象类型
来源：http://fcg.nanxinkj.top

Py:   isinstance(u, User)
来源：http://ker.hnxiangtu.top

PHP:  $u instanceof User
来源：http://ojj.bbcook.cn

JS:   u instanceof User
来源：http://qvu.yongpay.top

TS:   u instanceof User
来源：http://iih.guannengcc.top

Java: u instanceof User
来源：http://cab.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fgv.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://xhq.gzhubu.top

C#:   u is User
来源：http://gmx.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://jwj.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oxr.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://fdh.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mxx.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://hif.uphjek.com

Java: record User(String name, int age) {}
来源：http://zvp.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://vuw.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rsq.meibo888.top

C#:   record User(string Name, int Age);
来源：http://qea.zhongyouzk.top

[G15] 枚举
来源：http://jqx.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ksp.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mdb.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tth.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vmw.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://ffd.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rqh.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://keb.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xun.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://lov.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wnn.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://gsg.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://ggt.aibaodan.cn

TS:   Object.entries(obj)
来源：http://oyx.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qdq.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://urw.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://tfa.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://xad.andypj.xyz

================================================================================
来源：http://dxe.gzhubu.top

H. 异常与错误处理
来源：http://vpv.shanyushiyangkeji.top

================================================================================
来源：http://aye.yj20258888.top

[H01] try / catch 基础
来源：http://wfx.jinghuilouyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://igk.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nyx.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://scu.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mci.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vfj.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pas.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rwl.jianghu66.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lgk.cucudq.cn

[H02] finally / ensure 收尾
来源：http://cmj.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://thx.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kjd.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ngg.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vdu.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://igc.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fzl.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://csh.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dca.sufxvd.cn

[H03] 主动抛出异常
来源：http://jmi.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://ius.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xgo.havefunace.top

JS:   throw new Error("错误信息");
来源：http://jow.tianlin.xyz


<!-- 参考信息 -->