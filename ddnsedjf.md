代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hjs.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xhf.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://owx.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lbj.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bbw.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://gcx.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fni.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dwq.daxiang520.top

[E22] 字节长度与字符长度
来源：http://wnx.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lmg.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ykm.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://epu.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sai.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ixq.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wpo.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://shz.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jgw.havefunace.top

================================================================================
来源：http://fzy.shzxlz.cn

F. 文件与目录
来源：http://cut.ybcxt.top

================================================================================
来源：http://rax.0kj1m.cn

[F01] 读取整个文件
来源：http://xzy.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vlh.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://vel.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://flk.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xij.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jhr.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfs.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://gnd.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://uom.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://ckn.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hmm.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://del.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awl.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://usf.zdbjq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://avy.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xhd.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vkj.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://frl.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://oox.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://agi.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tps.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://snm.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npf.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eev.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qja.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://nlg.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mzs.andypj.xyz

[F04] 追加写入文件
来源：http://sco.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aka.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ixj.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pre.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mim.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gpo.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wfe.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oim.fzhhl.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hxg.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://hqq.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jdg.yj20258.top

PHP:  file_exists("a.txt");
来源：http://aig.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://xxu.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://aac.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pej.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rqq.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://vkh.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://bdw.chenlongwang.top

[F06] 删除文件
来源：http://rtn.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://adi.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://dtv.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://nrm.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tjv.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gfw.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://rdf.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://nub.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://mmw.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://gut.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wzr.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tpf.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lkw.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xcy.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vhi.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wmf.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oix.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wbq.fehbvm.com

[F08] 遍历目录
来源：http://dhi.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bah.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sjz.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://knd.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://xrn.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iin.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cph.xingfuxueyuan.xyz

Ruby: Dir.children("dir")
来源：http://rnf.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://aux.zhijiandao.cn

[F09] 获取文件大小
来源：http://lzp.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://ddj.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://zwb.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://iyh.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://eyz.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://zpc.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hwt.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://bzi.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://kan.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://aqy.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tin.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjf.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tjy.cashguo.top

TS:   path.extname("a.txt")
来源：http://kyb.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fpt.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://slu.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tyj.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://obp.hywenlv.cn

[F11] 复制与移动文件
来源：http://ruv.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://seg.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pve.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qns.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vuq.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mjh.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cpo.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://igj.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wda.cheryme.top

[F12] CSV 读写
来源：http://bcd.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iza.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vbp.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fez.jinqigfzy.top

TS:   // 同上
来源：http://wfg.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fzs.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mpc.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rmj.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jkn.yj20258888.top

================================================================================
来源：http://awe.guowangkeji.top

G. 面向对象
来源：http://zcd.shanyushiyangkeji.top

================================================================================
来源：http://fpv.0kj1m.cn

[G01] 定义类
来源：http://pcm.cheryme.top

Py:   class User: pass
来源：http://idk.shuidangran.top

PHP:  class User {}
来源：http://stt.ppjwa.cn

JS:   class User {}
来源：http://cey.yongpay.top

TS:   class User { name: string = ""; }
来源：http://daq.9152youxi.cn

Java: class User {}
来源：http://eqj.svipenyu.cn

Go:   type User struct { Name string }
来源：http://ucw.shanyushiyangtech.top

Ruby: class User; end
来源：http://dmg.chenzaomai.com

C#:   class User {}
来源：http://uev.jinyuanbaomall.cn

[G02] 构造函数
来源：http://rst.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://roj.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://uer.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ssm.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://pkd.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://hdn.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fnc.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://tpc.dianchejie.cn

C#:   public User(string name) { Name = name; }
来源：http://uhv.birdmap.top

[G03] 实例属性
来源：http://jqw.aizwys.cn

Py:   self.name = "x"
来源：http://yud.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://jhp.ydjk.org.cn

JS:   this.name = "x";
来源：http://ixb.xziqi.cn

TS:   name: string = "x";
来源：http://gbs.52xcode.cn

Java: private String name;
来源：http://etv.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://did.sxryk.cn

Ruby: @name = "x"
来源：http://ypn.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://kex.dianchejie.cn

[G04] 定义方法
来源：http://zcm.gzhubu.top

Py:   def greet(self): return self.name
来源：http://inb.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://qjy.hammf.cn

JS:   greet() { return this.name; }
来源：http://vev.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://zqj.haohaochexian.top

Java: String greet() { return name; }
来源：http://mpb.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wpf.yonumen.top

Ruby: def greet; @name; end
来源：http://sti.uphjek.com

C#:   public string Greet() => Name;
来源：http://tot.iojbl.cn

[G05] 继承
来源：http://kxp.9152youxi.cn

Py:   class Admin(User): pass
来源：http://odp.yvedp.cn

PHP:  class Admin extends User {}
来源：http://sgy.ybcxt.top

JS:   class Admin extends User {}
来源：http://gso.xziqi.cn

TS:   class Admin extends User {}
来源：http://ilu.kuanghao11.cn

Java: class Admin extends User {}
来源：http://fkc.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mwl.0kj1m.cn

Ruby: class Admin < User; end
来源：http://omp.zhoulong.xyz

C#:   class Admin : User {}
来源：http://qti.hysaishi.cn

[G06] 重写方法
来源：http://ajh.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://dkj.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://edo.316326.xyz

JS:   greet() { return "admin"; }
来源：http://nlt.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://bbw.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://uun.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lwb.jianghu66.top

Ruby: def greet; "admin"; end
来源：http://ptw.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://rlq.9152youxi.cn

[G07] 调用父类方法
来源：http://xcl.jqgufenzy.top

Py:   super().greet()
来源：http://jin.bbcook.cn

PHP:  parent::greet();
来源：http://ljn.zhongyouzk.top

JS:   super.greet();
来源：http://tel.fehbvm.com

TS:   super.greet();
来源：http://xza.yvedp.cn

Java: super.greet();
来源：http://prh.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jmp.tanke756.top

Ruby: super
来源：http://hvw.gaohongyu789.top

C#:   base.Greet();
来源：http://yzk.jqgufenzy.top

[G08] 静态方法与属性
来源：http://yfg.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://udf.52xcode.cn

PHP:  public static function f() {}
来源：http://lky.vqdsnc.cn

JS:   static f() {}
来源：http://dgn.xuanzx.com

TS:   static f(): void {}
来源：http://jsf.zhongyouzk.top

Java: static void f() {}
来源：http://zvi.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bxb.jinqigufen.top

Ruby: def self.f; end
来源：http://qmn.316326.xyz

C#:   public static void F() {}
来源：http://vwj.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://ree.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://lsa.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://niu.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dgo.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://zuc.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://pmp.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://njg.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mke.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://jut.cheryme.top

[G10] 访问控制
来源：http://jqe.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://xql.jqgfzy.top

PHP:  public / protected / private
来源：http://ydb.yonumen.top

JS:   #private 字段；其余公开
来源：http://smd.sweek.top

TS:   public / protected / private
来源：http://nxc.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://ypm.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ywq.xuanzx.com

Ruby: public / protected / private
来源：http://iyl.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://pnf.hammf.cn

[G11] getter / setter
来源：http://gmj.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://zjf.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rcb.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://jpd.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://lmc.gzhubu.top

Java: public String getName() { return name; }
来源：http://xay.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bde.jqgfzy.top

Ruby: attr_accessor :name
来源：http://oew.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://vmk.dashuyun.cn

[G12] 对象转字符串
来源：http://stn.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://cug.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ikz.yuxming.cn

JS:   toString() { return this.name; }
来源：http://pbg.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://pwt.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://aio.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dlw.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://gqk.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://dha.zhixingplan.top

[G13] 判断对象类型
来源：http://laz.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://qnn.yongpay.top

PHP:  $u instanceof User
来源：http://dsx.tianlin.xyz

JS:   u instanceof User
来源：http://xxr.yuanzhike.top

TS:   u instanceof User
来源：http://xub.nanxinkj.top

Java: u instanceof User
来源：http://xbm.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tcs.tarul.cn

Ruby: u.is_a?(User)
来源：http://swz.shangyingyoupin.top

C#:   u is User
来源：http://bxm.hnxiangtu.top

[G14] 数据类 / record
来源：http://qaf.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gvd.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://dmu.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xyk.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://iah.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://axf.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://tvg.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bkj.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://ubv.iojbl.cn

[G15] 枚举
来源：http://arh.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oyi.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qth.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wij.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://smn.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://jzc.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gil.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://ypt.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lbx.havefunace.top

[G16] 对象转数组 / 字典
来源：http://ijo.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://egb.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://mbi.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://bgl.fktsv.cn

TS:   Object.entries(obj)
来源：http://ztm.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xlr.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lfs.xinyue.icu

Ruby: obj.instance_variables
来源：http://eoq.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://lys.fehbvm.com

================================================================================
来源：http://kxs.9152youxi.cn

H. 异常与错误处理
来源：http://slp.epnwcf.com

================================================================================
来源：http://vfw.zhijiandao.cn

[H01] try / catch 基础
来源：http://fsd.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dhg.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rte.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ngx.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lyg.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sal.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sln.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lxz.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jod.yj20258.top

[H02] finally / ensure 收尾
来源：http://ooj.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qij.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rty.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hsl.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://sqb.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://sus.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pib.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://umh.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://als.ybcxt.top

[H03] 主动抛出异常
来源：http://keu.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://oam.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dpq.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://smu.52xcode.cn


<!-- 参考信息 -->