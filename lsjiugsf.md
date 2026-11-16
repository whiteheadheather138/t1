代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bbz.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qmy.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfw.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://una.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cfr.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://zwz.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eco.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ssf.aizwys.cn

[E22] 字节长度与字符长度
来源：http://utx.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vby.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qmk.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fib.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tuh.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rgf.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ran.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://lmv.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fpx.yuanzhike.top

================================================================================
来源：http://zzt.c1oappe.top

F. 文件与目录
来源：http://ism.9152youxi.cn

================================================================================
来源：http://ycd.yj20258888.top

[F01] 读取整个文件
来源：http://zbu.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tsj.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://beh.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kdo.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nzc.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sfn.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dga.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://eda.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://mto.nwbrower.top

[F02] 逐行读取文件
来源：http://fhr.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ouw.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ynm.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ehx.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zbi.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ujl.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://twz.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ozf.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eqi.yongpay.top

[F03] 写入文件（覆盖）
来源：http://qxq.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eii.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yxk.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qhn.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://plx.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sby.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wlv.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://dag.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kqm.jlsjyb.cn

[F04] 追加写入文件
来源：http://jma.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://umv.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kvf.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vek.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eop.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fsw.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zoi.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://abl.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tnu.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://fkh.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hrd.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://wbm.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://ull.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://uwb.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kqk.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dhi.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://vkd.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://hop.guowangkeji.top

[F06] 删除文件
来源：http://vvx.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://ukc.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://nye.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lja.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://vqo.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xon.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://jtp.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://sui.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://wew.hesvh.cn

[F07] 创建目录（含多级）
来源：http://cox.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zuq.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xvn.tanke756.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://res.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uyg.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rgs.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cum.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rqb.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wrl.hammf.cn

[F08] 遍历目录
来源：http://lcn.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://weh.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fgo.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://egx.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://oso.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eys.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajc.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://nze.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://vre.cheryme.top

[F09] 获取文件大小
来源：http://ztj.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://lxw.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://yhz.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://ukh.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://xmk.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://edg.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sll.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://hsj.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://eph.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://rsn.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dwo.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ipt.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vpp.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://wkc.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mth.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fjj.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://env.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ifs.sufxvd.cn

[F11] 复制与移动文件
来源：http://yuy.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gfg.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aqr.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pjp.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aks.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bgt.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rmh.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lfd.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dhi.jianghu66.top

[F12] CSV 读写
来源：http://mad.jinqigufen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ede.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://inn.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ypi.xingfuxueyuan.xyz

TS:   // 同上
来源：http://bdv.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ztw.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://quu.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cnp.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hfd.cheryme.top

================================================================================
来源：http://dnd.vehdjk.com

G. 面向对象
来源：http://dvl.yj20258888.top

================================================================================
来源：http://jeg.tianlin.xyz

[G01] 定义类
来源：http://pbq.yj202588.top

Py:   class User: pass
来源：http://nwl.zhiwuduotai.top

PHP:  class User {}
来源：http://ycc.zhiwuduotai.top

JS:   class User {}
来源：http://txn.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://dua.fktsv.cn

Java: class User {}
来源：http://qjk.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://tex.wangshuangyany.cn

Ruby: class User; end
来源：http://sli.hongshengwenyu.top

C#:   class User {}
来源：http://uvf.fehbvm.com

[G02] 构造函数
来源：http://nbo.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://phg.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://iaw.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://icv.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://oeu.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://gcz.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tse.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://hsx.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://evu.redwolf501.top

[G03] 实例属性
来源：http://pdg.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://smq.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://obk.jinqigufen.top

JS:   this.name = "x";
来源：http://glr.tian-w.cn

TS:   name: string = "x";
来源：http://ahy.hesvh.cn

Java: private String name;
来源：http://syy.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cnf.jqgfzy.top

Ruby: @name = "x"
来源：http://gds.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://vyo.dianchejie.cn

[G04] 定义方法
来源：http://jms.sweek.top

Py:   def greet(self): return self.name
来源：http://dca.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pve.gzhubu.top

JS:   greet() { return this.name; }
来源：http://yjb.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://naw.haohaochexian.top

Java: String greet() { return name; }
来源：http://dbm.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qfb.jinqigufen.top

Ruby: def greet; @name; end
来源：http://mlr.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://rqx.hysaishi.cn

[G05] 继承
来源：http://ywo.yangfankeji.com

Py:   class Admin(User): pass
来源：http://fyt.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://tpv.gogol.net.cn

JS:   class Admin extends User {}
来源：http://qug.zdqjudy.top

TS:   class Admin extends User {}
来源：http://apv.haohaochexian.top

Java: class Admin extends User {}
来源：http://lop.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://odx.bjfxy.top

Ruby: class Admin < User; end
来源：http://sbt.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://mwh.cheryme.top

[G06] 重写方法
来源：http://alf.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://nxf.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bps.pycfn.com

JS:   greet() { return "admin"; }
来源：http://xcx.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://bye.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://tsy.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zjg.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://uug.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://kwr.yfazqb.com

[G07] 调用父类方法
来源：http://lih.sufxvd.cn

Py:   super().greet()
来源：http://wvw.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://qkb.dianchejie.cn

JS:   super.greet();
来源：http://rir.hammf.cn

TS:   super.greet();
来源：http://jth.haohaochexian.top

Java: super.greet();
来源：http://otx.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zkz.mhx1999.top

Ruby: super
来源：http://zwd.yuanzhike.top

C#:   base.Greet();
来源：http://zib.havefunace.top

[G08] 静态方法与属性
来源：http://tgy.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fxx.svipenyu.cn

PHP:  public static function f() {}
来源：http://hog.yfazqb.com

JS:   static f() {}
来源：http://npc.nwbrower.top

TS:   static f(): void {}
来源：http://wxy.cqqwz.cn

Java: static void f() {}
来源：http://roj.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sdj.zycfv.cn

Ruby: def self.f; end
来源：http://qlm.tian-w.cn

C#:   public static void F() {}
来源：http://msb.hnqzz.top

[G09] 接口 / 抽象类
来源：http://qhd.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://vzu.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hlp.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oay.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://rsb.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://ngu.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://ime.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nhk.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://idt.jianghu66.top

[G10] 访问控制
来源：http://kjj.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://vkr.ivvv.top

PHP:  public / protected / private
来源：http://dks.smart0.xyz

JS:   #private 字段；其余公开
来源：http://ern.nanxuanxn.top

TS:   public / protected / private
来源：http://vxv.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://nle.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vcb.vqdsnc.cn

Ruby: public / protected / private
来源：http://exq.jyoumei.cn

C#:   public / protected / private / internal
来源：http://pjz.tarul.cn

[G11] getter / setter
来源：http://njk.bbcook.cn

Py:   @property 与 @x.setter
来源：http://rqg.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://fpt.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://xxi.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://orj.daria6918.cn

Java: public String getName() { return name; }
来源：http://ltd.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://skd.316326.xyz

Ruby: attr_accessor :name
来源：http://jvr.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://vqp.birdmap.top

[G12] 对象转字符串
来源：http://ujb.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://hqu.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pix.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://fum.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://nks.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://ykl.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xhh.tarul.cn

Ruby: def to_s; @name; end
来源：http://khf.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://qtv.pengpengdd.cyou

[G13] 判断对象类型
来源：http://lbs.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://tky.ppjwa.cn

PHP:  $u instanceof User
来源：http://nqu.yfazqb.com

JS:   u instanceof User
来源：http://seu.chenlongwang.top

TS:   u instanceof User
来源：http://vgk.zhijiandao.cn

Java: u instanceof User
来源：http://vta.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xwl.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://ndf.shangyingyoupin.top

C#:   u is User
来源：http://rkg.zdbjq.cn

[G14] 数据类 / record
来源：http://vst.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jfq.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://pda.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://hrv.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://jwm.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://zsz.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://emn.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yob.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://chb.jyoumei.cn

[G15] 枚举
来源：http://itl.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qma.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xho.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lah.yvedp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gso.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://vxa.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jjv.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://pcf.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rsc.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://yqm.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fvf.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://vxn.aibaodan.cn

JS:   Object.entries(obj)
来源：http://zlq.ybcxt.top

TS:   Object.entries(obj)
来源：http://ran.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zbt.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lbq.9152youxi.cn

Ruby: obj.instance_variables
来源：http://xvl.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://qrb.ctjpmb.com

================================================================================
来源：http://eof.ywan-chungtsiang.top

H. 异常与错误处理
来源：http://rjz.hysaishi.cn

================================================================================
来源：http://jcc.shangyingyoupin.top

[H01] try / catch 基础
来源：http://ojs.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://not.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qmo.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ord.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bej.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vhk.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lby.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rom.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tve.xuanzx.com

[H02] finally / ensure 收尾
来源：http://tpz.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iau.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://taa.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ant.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cin.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://xmg.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gyu.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wlf.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://twg.jianghu66.top

[H03] 主动抛出异常
来源：http://zyi.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://qgr.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aht.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://qzp.jinqigufen.top


<!-- 参考信息 -->