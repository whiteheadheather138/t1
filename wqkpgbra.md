代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vkh.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kal.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dnw.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mab.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xxa.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://whb.havefunace.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://umz.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gmc.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://zzr.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://inc.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ngi.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pzq.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iyb.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wsz.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eqp.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://snt.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pdg.sufxvd.cn

================================================================================
来源：http://bkc.hammf.cn

F. 文件与目录
来源：http://yzw.xziqi.cn

================================================================================
来源：http://ebo.chenzaomai.com

[F01] 读取整个文件
来源：http://opn.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hza.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://ypp.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fef.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ovv.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rng.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jqp.fktsv.cn

Ruby: File.read("a.txt")
来源：http://gkw.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://dld.zdqjudy.top

[F02] 逐行读取文件
来源：http://tgo.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jgj.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tnj.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpz.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akh.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jvh.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ldr.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sqc.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ihz.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://hpn.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fnj.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bek.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwt.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uql.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bui.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ybi.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://hfr.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lor.shangyingyoupin.top

[F04] 追加写入文件
来源：http://cib.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bfg.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jwe.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://psk.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aqw.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cue.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lki.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sbq.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qlv.xuanzx.com

[F05] 判断文件或目录是否存在
来源：http://agr.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ekr.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://blx.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://jep.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://kjx.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://eyk.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rvc.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://jzz.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://pzp.zycfv.cn

[F06] 删除文件
来源：http://jke.ydzc1.top

Py:   os.remove("a.txt")
来源：http://zkk.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://bpu.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://pmr.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://yru.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fip.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://uny.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://eue.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://qsp.hnqzz.top

[F07] 创建目录（含多级）
来源：http://qtd.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lcj.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ruf.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nbj.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lsk.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rrl.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tov.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://krm.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zup.zhoulong.xyz

[F08] 遍历目录
来源：http://lar.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nna.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bzx.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://geo.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://iui.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vxj.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qgc.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://spo.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://zhl.wangshuangyany.cn

[F09] 获取文件大小
来源：http://bvu.jianghu66.top

Py:   os.path.getsize("a.txt")
来源：http://ptf.guannengcc.top

PHP:  filesize("a.txt");
来源：http://cjy.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://ixe.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://afb.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eyp.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gcn.bjfxy.top

Ruby: File.size("a.txt")
来源：http://kxq.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://dwa.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://lwo.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ukx.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zxg.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cjn.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://dcz.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rjp.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tyt.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ubo.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ogd.yfazqb.com

[F11] 复制与移动文件
来源：http://lsk.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cbx.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wvz.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwz.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qst.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pkh.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dzx.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mof.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qct.hnqzz.top

[F12] CSV 读写
来源：http://slb.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xwh.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://inp.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sha.smart0.xyz

TS:   // 同上
来源：http://klj.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oxm.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fne.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fcj.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zbh.feifeiyinyue.top

================================================================================
来源：http://vqx.fengsongda.top

G. 面向对象
来源：http://nei.kuanghao11.cn

================================================================================
来源：http://ump.zhiwuduotai.top

[G01] 定义类
来源：http://epk.yuanzhike.top

Py:   class User: pass
来源：http://aoe.hammf.cn

PHP:  class User {}
来源：http://zeb.fengsongda.top

JS:   class User {}
来源：http://jfz.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://ieq.xingfuxueyuan.xyz

Java: class User {}
来源：http://mod.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://zfu.tian-w.cn

Ruby: class User; end
来源：http://qpa.sjlbkw.cn

C#:   class User {}
来源：http://jve.zhijiandao.cn

[G02] 构造函数
来源：http://umf.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://wsz.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://uqa.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://npj.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://lbr.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://sdc.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ukd.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://had.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://lnz.nanxinkj.top

[G03] 实例属性
来源：http://esd.9152youxi.cn

Py:   self.name = "x"
来源：http://eve.316326.xyz

PHP:  public string $name = "x";
来源：http://otu.ydzc1.top

JS:   this.name = "x";
来源：http://dyh.zycfv.cn

TS:   name: string = "x";
来源：http://oad.aibaodan.cn

Java: private String name;
来源：http://gib.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cfh.tianlin.xyz

Ruby: @name = "x"
来源：http://sab.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://ffs.nwbrower.top

[G04] 定义方法
来源：http://smq.wangdashe.top

Py:   def greet(self): return self.name
来源：http://nnu.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ngt.xylfe.cn

JS:   greet() { return this.name; }
来源：http://pgr.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://oni.andypj.xyz

Java: String greet() { return name; }
来源：http://eel.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://aqy.sxryk.cn

Ruby: def greet; @name; end
来源：http://aps.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://txc.fanxiaobao.xyz

[G05] 继承
来源：http://vkq.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://xjo.xylfe.cn

PHP:  class Admin extends User {}
来源：http://hqt.iojbl.cn

JS:   class Admin extends User {}
来源：http://kgy.yvedp.cn

TS:   class Admin extends User {}
来源：http://wcy.tian-w.cn

Java: class Admin extends User {}
来源：http://btc.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://osj.xziqi.cn

Ruby: class Admin < User; end
来源：http://ugm.52xcode.cn

C#:   class Admin : User {}
来源：http://kze.jianghu66.top

[G06] 重写方法
来源：http://dbg.chenzaomai.com

Py:   def greet(self): return "admin"
来源：http://tlq.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://mti.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://huz.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://vay.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://pcq.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://csr.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://vua.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://ypc.ehwqpu.com

[G07] 调用父类方法
来源：http://gvo.xylfe.cn

Py:   super().greet()
来源：http://oru.zhixingplan.top

PHP:  parent::greet();
来源：http://ewn.epnwcf.com

JS:   super.greet();
来源：http://sag.9152youxi.cn

TS:   super.greet();
来源：http://azx.fanxiaobao.xyz

Java: super.greet();
来源：http://zfn.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zyc.yj20258.top

Ruby: super
来源：http://ueq.aizwys.cn

C#:   base.Greet();
来源：http://qea.mhx1999.top

[G08] 静态方法与属性
来源：http://dmk.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qqd.ppjwa.cn

PHP:  public static function f() {}
来源：http://qho.tianlin.xyz

JS:   static f() {}
来源：http://yvw.zhixingplan.top

TS:   static f(): void {}
来源：http://rtt.zhixingplan.top

Java: static void f() {}
来源：http://imi.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://efd.feifeiyinyue.top

Ruby: def self.f; end
来源：http://nvm.daria6918.cn

C#:   public static void F() {}
来源：http://nid.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://muz.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://tbx.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://bpx.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ybz.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://jmd.xziqi.cn

Java: interface Shape { double area(); }
来源：http://nce.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://dno.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://phj.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://eat.wangshuangyany.cn

[G10] 访问控制
来源：http://vqt.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://kam.guowangkeji.top

PHP:  public / protected / private
来源：http://huc.fengsongda.top

JS:   #private 字段；其余公开
来源：http://oiy.fktsv.cn

TS:   public / protected / private
来源：http://hmk.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://jbk.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://egi.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://qlp.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://qtk.jinqigfzy.top

[G11] getter / setter
来源：http://uud.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://mdn.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://weh.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://lss.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://orr.wangdashe.top

Java: public String getName() { return name; }
来源：http://axc.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vqm.dashuyun.cn

Ruby: attr_accessor :name
来源：http://dii.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://knc.redwolf501.top

[G12] 对象转字符串
来源：http://tcg.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://xkl.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://kch.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://nit.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://lck.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://kcc.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://emq.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://zmz.cashguo.top

C#:   public override string ToString() => Name;
来源：http://zmm.sysykeji.top

[G13] 判断对象类型
来源：http://ods.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://dcg.sxryk.cn

PHP:  $u instanceof User
来源：http://lmb.ehwqpu.com

JS:   u instanceof User
来源：http://izc.shuidangran.top

TS:   u instanceof User
来源：http://mbt.nwbrower.top

Java: u instanceof User
来源：http://ndb.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vym.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://hlx.gzhubu.top

C#:   u is User
来源：http://tti.aizwys.cn

[G14] 数据类 / record
来源：http://rhj.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://imy.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://xbe.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://ufe.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://smx.meibo888.top

Java: record User(String name, int age) {}
来源：http://daf.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://pdd.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tyv.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://bvv.tianlin.xyz

[G15] 枚举
来源：http://tzh.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ezr.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kro.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fjr.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jpo.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://fdv.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lww.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://mtw.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suv.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://npq.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fcq.cheryme.top

PHP:  get_object_vars($obj);
来源：http://vcz.ctjpmb.com

JS:   Object.entries(obj)
来源：http://bkc.chenlongwang.top

TS:   Object.entries(obj)
来源：http://vni.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://msi.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nah.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://kjd.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://xmz.xuanzx.com

================================================================================
来源：http://clk.uphjek.com

H. 异常与错误处理
来源：http://ivq.gogol.net.cn

================================================================================
来源：http://ouk.svipenyu.cn

[H01] try / catch 基础
来源：http://zbx.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zvd.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eed.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://teb.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rfj.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jru.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://itn.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://azd.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zfa.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://jrt.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://pff.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://shb.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://eck.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tdf.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://mvv.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xic.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yek.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fkh.9152youxi.cn

[H03] 主动抛出异常
来源：http://ofd.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://iyo.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bpd.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://ghd.cucudq.cn


<!-- 参考信息 -->