代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kbg.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://zom.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cgx.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oyd.tarul.cn

[E22] 字节长度与字符长度
来源：http://frw.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lju.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ocg.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ydx.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dep.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dpm.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xqx.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://wrx.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://flr.chenzaomai.com

================================================================================
来源：http://zkr.sysykeji.top

F. 文件与目录
来源：http://mos.yvedp.cn

================================================================================
来源：http://scc.wangdashe.top

[F01] 读取整个文件
来源：http://tae.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ojy.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://nke.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bqb.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hba.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cfl.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kdp.yj202588.top

Ruby: File.read("a.txt")
来源：http://ucz.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://yrm.zhoulong.xyz

[F02] 逐行读取文件
来源：http://xhr.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ckq.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vii.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kxb.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yfz.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mlw.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yna.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yhz.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://btl.cheryme.top

[F03] 写入文件（覆盖）
来源：http://jkb.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wmz.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://qsu.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrm.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dsk.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://upa.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oys.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://bbn.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gts.nanxinkj.top

[F04] 追加写入文件
来源：http://jft.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fhm.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eoj.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mdf.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wrj.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wjr.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ykm.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://caf.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pjj.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://mxd.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ifs.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://boj.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://hnb.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://ocw.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vyq.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ybk.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://zgb.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://apm.zhengqikj.top

[F06] 删除文件
来源：http://cuc.cucudq.cn

Py:   os.remove("a.txt")
来源：http://uln.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://xov.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://aaw.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nxu.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dex.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://bor.cashguo.top

Ruby: File.delete("a.txt")
来源：http://huu.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://tog.bjfxy.top

[F07] 创建目录（含多级）
来源：http://kuo.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tta.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ufz.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://haw.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://svo.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gue.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zwr.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gzb.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fpr.wangdashe.top

[F08] 遍历目录
来源：http://fay.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://uzt.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pnb.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://ihk.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://ghf.hongshengwenyu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vsm.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rpn.ivvv.top

Ruby: Dir.children("dir")
来源：http://rcf.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://utf.hysaishi.cn

[F09] 获取文件大小
来源：http://wur.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://hhc.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://xpq.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://ymb.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://vgo.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://urs.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dfh.cucudq.cn

Ruby: File.size("a.txt")
来源：http://imk.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://vul.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://vor.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zvi.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wol.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wkn.birdmap.top

TS:   path.extname("a.txt")
来源：http://isx.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kqs.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ggt.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qca.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pjp.vehdjk.com

[F11] 复制与移动文件
来源：http://pdx.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gsd.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uel.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqm.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dwq.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aoe.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nao.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ewj.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wzj.sweek.top

[F12] CSV 读写
来源：http://pdb.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlg.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aam.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pxf.guowangkeji.top

TS:   // 同上
来源：http://hyv.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ben.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://epr.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://icm.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kvc.cashguo.top

================================================================================
来源：http://ivc.cdnleiting.top

G. 面向对象
来源：http://lla.uphjek.com

================================================================================
来源：http://inw.xylfe.cn

[G01] 定义类
来源：http://bwy.cheryme.top

Py:   class User: pass
来源：http://rva.sufxvd.cn

PHP:  class User {}
来源：http://prz.xingfuxueyuan.xyz

JS:   class User {}
来源：http://utr.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://mjy.xziqi.cn

Java: class User {}
来源：http://usj.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://zxp.zhixingplan.top

Ruby: class User; end
来源：http://cjv.shangyingyoupin.top

C#:   class User {}
来源：http://cko.chenjidiqi.icu

[G02] 构造函数
来源：http://nps.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://qbb.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://gew.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://bzl.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://bqe.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://mae.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bnp.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://jyb.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://ssy.wangdashe.top

[G03] 实例属性
来源：http://fcs.zhongyouzk.top

Py:   self.name = "x"
来源：http://pak.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://zoa.gotoacloud.top

JS:   this.name = "x";
来源：http://cqd.havefunace.top

TS:   name: string = "x";
来源：http://xnp.dashuyun.cn

Java: private String name;
来源：http://ozh.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ugl.yj20258.top

Ruby: @name = "x"
来源：http://zvt.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://kkg.daxiang520.top

[G04] 定义方法
来源：http://ukb.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://lmr.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://saj.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://eoq.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://zrr.redwolf501.top

Java: String greet() { return name; }
来源：http://dcm.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nrp.sxryk.cn

Ruby: def greet; @name; end
来源：http://fab.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://rgu.yvedp.cn

[G05] 继承
来源：http://gox.cheryme.top

Py:   class Admin(User): pass
来源：http://pli.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://whj.c1oappe.top

JS:   class Admin extends User {}
来源：http://yyd.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://dor.cashguo.top

Java: class Admin extends User {}
来源：http://ahh.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kmq.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://zlq.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://qse.shuidangran.top

[G06] 重写方法
来源：http://txz.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://abs.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://nym.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://jsx.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://ffb.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://tdv.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://imd.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://uoz.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://fie.yvedp.cn

[G07] 调用父类方法
来源：http://ynu.jyoumei.cn

Py:   super().greet()
来源：http://gtz.nanxinkj.top

PHP:  parent::greet();
来源：http://lat.hysaishi.cn

JS:   super.greet();
来源：http://xss.iojbl.cn

TS:   super.greet();
来源：http://sgm.shanyushiyangkeji.top

Java: super.greet();
来源：http://qhs.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ddc.yvedp.cn

Ruby: super
来源：http://qtj.jinqigufen.top

C#:   base.Greet();
来源：http://zpt.andypj.xyz

[G08] 静态方法与属性
来源：http://ciq.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rob.cucudq.cn

PHP:  public static function f() {}
来源：http://rxd.fengsongda.top

JS:   static f() {}
来源：http://rdo.yfazqb.com

TS:   static f(): void {}
来源：http://kpn.cucudq.cn

Java: static void f() {}
来源：http://dui.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wvb.fktsv.cn

Ruby: def self.f; end
来源：http://zpf.cucudq.cn

C#:   public static void F() {}
来源：http://gbl.316326.xyz

[G09] 接口 / 抽象类
来源：http://zvi.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://kfj.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://jxb.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gtv.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://tup.yongpay.top

Java: interface Shape { double area(); }
来源：http://qze.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://fxb.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://njt.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://bjs.uphjek.com

[G10] 访问控制
来源：http://hzd.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://vbc.guowangkeji.top

PHP:  public / protected / private
来源：http://ncd.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://qzf.fzhhl.top

TS:   public / protected / private
来源：http://nzv.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://bot.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pho.dianchejie.cn

Ruby: public / protected / private
来源：http://zmo.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://bhc.fengsongda.top

[G11] getter / setter
来源：http://msc.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://vhb.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zat.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://sat.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://gbc.hfpthk.cn

Java: public String getName() { return name; }
来源：http://fcd.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://shu.hnqzz.top

Ruby: attr_accessor :name
来源：http://ffw.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://yqv.pengpengdd.cyou

[G12] 对象转字符串
来源：http://oiz.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://skg.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gnx.yongpay.top

JS:   toString() { return this.name; }
来源：http://rei.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://eee.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://dyf.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qpb.tarul.cn

Ruby: def to_s; @name; end
来源：http://cwi.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://euj.zhijiandao.cn

[G13] 判断对象类型
来源：http://hgr.jinqigufen.top

Py:   isinstance(u, User)
来源：http://uen.gotoacloud.top

PHP:  $u instanceof User
来源：http://rmm.vqdsnc.cn

JS:   u instanceof User
来源：http://jik.shangyingyoupin.top

TS:   u instanceof User
来源：http://zdx.hcnkem.com

Java: u instanceof User
来源：http://zle.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eke.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://erm.jianghu66.top

C#:   u is User
来源：http://qgh.hcnkem.com

[G14] 数据类 / record
来源：http://nqm.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fhv.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://cbv.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://jus.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://vac.sxryk.cn

Java: record User(String name, int age) {}
来源：http://uoi.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://qth.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wtd.uphjek.com

C#:   record User(string Name, int Age);
来源：http://sba.aizwys.cn

[G15] 枚举
来源：http://ejh.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ojb.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://taa.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zkh.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kky.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://cdm.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://agz.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://wxz.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mfb.havefunace.top

[G16] 对象转数组 / 字典
来源：http://nsr.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fes.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://wib.zhengqikj.top

JS:   Object.entries(obj)
来源：http://xsv.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://hdx.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jjj.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ymt.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://qvw.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://hpt.pengpengdd.cyou

================================================================================
来源：http://jhg.52xcode.cn

H. 异常与错误处理
来源：http://xms.vehdjk.com

================================================================================
来源：http://opa.xinyue.icu

[H01] try / catch 基础
来源：http://jbc.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tor.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://orb.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eeq.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lnn.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gky.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lza.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hjc.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jey.nwbrower.top

[H02] finally / ensure 收尾
来源：http://efz.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://lcv.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qce.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ggu.zhaomingkeji.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://foo.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tvm.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytc.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lzw.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://yja.hcnkem.com

[H03] 主动抛出异常
来源：http://jok.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://oiw.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cul.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://lui.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://xtk.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ghz.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://prp.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://clq.aizwys.cn


<!-- 参考信息 -->