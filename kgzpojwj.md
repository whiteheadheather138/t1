代发 wailian999

Go:   if s == "" {}
来源：http://uoz.tianlin.xyz

Ruby: if s.empty?
来源：http://hho.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cii.redwolf501.top

[E21] 超长截断加省略号
来源：http://wde.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qxu.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://czl.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://esf.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lfv.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qly.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://vol.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gfo.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wwi.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://wzf.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://egk.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ngs.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://suk.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxt.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cbf.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wfo.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://qlz.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zay.hysaishi.cn

================================================================================
来源：http://xlx.yj20258.top

F. 文件与目录
来源：http://qoe.iojbl.cn

================================================================================
来源：http://hus.aizwys.cn

[F01] 读取整个文件
来源：http://rym.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gnb.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://vqo.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eax.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://csw.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rti.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pua.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://gog.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://ito.xylfe.cn

[F02] 逐行读取文件
来源：http://aqr.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://djr.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xvz.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tmk.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xdt.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gsb.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mzf.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yoz.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nug.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://rkq.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dcy.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zlz.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bbm.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vkt.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nkv.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://klo.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://ytw.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hbv.jqgfzy.top

[F04] 追加写入文件
来源：http://mdt.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rwq.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dly.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sgg.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cjx.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://luz.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hfa.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nof.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tzs.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://ztr.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pmd.sweek.top

PHP:  file_exists("a.txt");
来源：http://fcq.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://tve.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://ypv.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aww.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hfm.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://jnr.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://gcz.shanyushiyangkeji.top

[F06] 删除文件
来源：http://cvm.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://aua.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://mnz.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xqr.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://ejl.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jbh.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://jue.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://bso.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://sfe.xziqi.cn

[F07] 创建目录（含多级）
来源：http://ywe.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iov.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mwv.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmp.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hpk.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vuh.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hnh.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nke.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hhd.nanxinkj.top

[F08] 遍历目录
来源：http://mul.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wge.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oml.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://bhb.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://ozy.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wwy.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://djt.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://vqb.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://caz.redwolf501.top

[F09] 获取文件大小
来源：http://izx.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://eoy.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://vni.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://soz.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://ggc.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jjy.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vzb.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://pqa.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://pry.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://ogh.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://edo.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://acs.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aza.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://usm.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://juo.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sqq.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://flt.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qmh.ehwqpu.com

[F11] 复制与移动文件
来源：http://ppu.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://byj.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ogd.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mjy.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zrg.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dbq.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mcq.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sfz.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hty.ydjk.org.cn

[F12] CSV 读写
来源：http://bpk.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ofa.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kgj.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zdg.ydjk.org.cn

TS:   // 同上
来源：http://sbm.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://krr.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dlj.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ffg.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://csm.jianghu66.top

================================================================================
来源：http://aur.9152youxi.cn

G. 面向对象
来源：http://eqi.xuanzx.com

================================================================================
来源：http://yzf.jinqigufen.top

[G01] 定义类
来源：http://dxh.xuetiantiany.cn

Py:   class User: pass
来源：http://fti.vehdjk.com

PHP:  class User {}
来源：http://lat.ydjk.org.cn

JS:   class User {}
来源：http://lxp.tanke756.top

TS:   class User { name: string = ""; }
来源：http://mlw.guannengcc.top

Java: class User {}
来源：http://ouw.fzhhl.top

Go:   type User struct { Name string }
来源：http://mkh.nanxinkj.top

Ruby: class User; end
来源：http://ibv.xuetiantiany.cn

C#:   class User {}
来源：http://ywi.yfazqb.com

[G02] 构造函数
来源：http://gsc.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ryg.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://ukd.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://qwo.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://ljj.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://tne.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sjw.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://bmi.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://uhn.jyoumei.cn

[G03] 实例属性
来源：http://pje.52xcode.cn

Py:   self.name = "x"
来源：http://wuz.sweek.top

PHP:  public string $name = "x";
来源：http://led.guannengcc.top

JS:   this.name = "x";
来源：http://mrk.iojbl.cn

TS:   name: string = "x";
来源：http://hri.bjfxy.top

Java: private String name;
来源：http://rvj.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wwi.zhijiandao.cn

Ruby: @name = "x"
来源：http://jru.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://sms.yj20258888.top

[G04] 定义方法
来源：http://omz.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://lmf.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dbb.bbcook.cn

JS:   greet() { return this.name; }
来源：http://zem.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://lke.fehbvm.com

Java: String greet() { return name; }
来源：http://svo.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ggk.zycfv.cn

Ruby: def greet; @name; end
来源：http://enc.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://dsw.fktsv.cn

[G05] 继承
来源：http://dod.sxryk.cn

Py:   class Admin(User): pass
来源：http://qmk.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://amc.dianchejie.cn

JS:   class Admin extends User {}
来源：http://lmp.ydzc1.top

TS:   class Admin extends User {}
来源：http://toh.fengsongda.top

Java: class Admin extends User {}
来源：http://aco.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lzz.jqgfzy.top

Ruby: class Admin < User; end
来源：http://waw.fengsongda.top

C#:   class Admin : User {}
来源：http://lja.sjlbkw.cn

[G06] 重写方法
来源：http://lwa.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://vxs.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hmr.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://yzf.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://orl.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://ins.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zyr.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://dww.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://gpx.shangyingyoupin.top

[G07] 调用父类方法
来源：http://fly.hnxiangtu.top

Py:   super().greet()
来源：http://krg.gzhubu.top

PHP:  parent::greet();
来源：http://cwk.yangfankeji.com

JS:   super.greet();
来源：http://cyr.pengpengdd.cyou

TS:   super.greet();
来源：http://miw.chenzaomai.com

Java: super.greet();
来源：http://qjd.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gro.yuanzhike.top

Ruby: super
来源：http://lgt.sjlbkw.cn

C#:   base.Greet();
来源：http://ynm.birdmap.top

[G08] 静态方法与属性
来源：http://zwz.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://slq.shzxlz.cn

PHP:  public static function f() {}
来源：http://rpm.nwbrower.top

JS:   static f() {}
来源：http://hot.nwbrower.top

TS:   static f(): void {}
来源：http://cii.xylfe.cn

Java: static void f() {}
来源：http://npc.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vfr.fzhhl.top

Ruby: def self.f; end
来源：http://ifl.daxiang520.top

C#:   public static void F() {}
来源：http://gev.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://ava.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://lqz.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://tqj.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vde.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://boy.xziqi.cn

Java: interface Shape { double area(); }
来源：http://qsm.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://arc.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://acp.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://jmj.cashguo.top

[G10] 访问控制
来源：http://sqb.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://jby.hywenlv.cn

PHP:  public / protected / private
来源：http://fqp.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://eec.vqdsnc.cn

TS:   public / protected / private
来源：http://der.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://xsu.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bgt.zdqjudy.top

Ruby: public / protected / private
来源：http://lcv.cucudq.cn

C#:   public / protected / private / internal
来源：http://gor.hnqzz.top

[G11] getter / setter
来源：http://ziw.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://lrs.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://naz.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://htv.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://msi.ivvv.top

Java: public String getName() { return name; }
来源：http://wwv.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvw.hammf.cn

Ruby: attr_accessor :name
来源：http://jwr.havefunace.top

C#:   public string Name { get; set; }
来源：http://uem.havefunace.top

[G12] 对象转字符串
来源：http://pul.havefunace.top

Py:   def __str__(self): return self.name
来源：http://xfv.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dxv.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://joi.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://naw.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://hwi.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://swh.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://qpc.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://ovi.pengpengdd.cyou

[G13] 判断对象类型
来源：http://ghm.zycfv.cn

Py:   isinstance(u, User)
来源：http://lps.yj20258.top

PHP:  $u instanceof User
来源：http://bcj.chenzaomai.com

JS:   u instanceof User
来源：http://tfz.jianghu66.top

TS:   u instanceof User
来源：http://vzg.jinghuilouyu.cn

Java: u instanceof User
来源：http://gmh.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://spd.havefunace.top

Ruby: u.is_a?(User)
来源：http://ujj.jinyuanbaomall.cn

C#:   u is User
来源：http://upn.zhoulong.xyz

[G14] 数据类 / record
来源：http://onx.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://txc.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://uve.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://zas.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://tnb.daxiang520.top

Java: record User(String name, int age) {}
来源：http://thp.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://nxf.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qlu.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://cnu.redwolf501.top

[G15] 枚举
来源：http://gue.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uto.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://aam.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://unu.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://utj.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://igv.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hyk.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://iqb.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mxt.yj20258.top

[G16] 对象转数组 / 字典
来源：http://erw.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rdh.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://pgk.cqqwz.cn

JS:   Object.entries(obj)
来源：http://mhi.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://zyt.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dsj.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ezo.shuidangran.top

Ruby: obj.instance_variables
来源：http://vwo.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://imd.wangshuangyany.cn

================================================================================
来源：http://krw.zhengqikj.top

H. 异常与错误处理
来源：http://qhz.hammf.cn

================================================================================
来源：http://vyb.sweek.top

[H01] try / catch 基础
来源：http://goi.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kts.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fuy.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ygb.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://arp.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://acj.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nfu.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ryt.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tdy.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://dhi.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://soa.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://enb.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pdv.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xng.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://qji.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dxe.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pxy.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cdc.birdmap.top


<!-- 参考信息 -->