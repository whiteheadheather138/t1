代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lvf.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pzc.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nov.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eaa.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pkl.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://cft.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://euk.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yha.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://zgc.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sky.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://krq.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cnk.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jha.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cme.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ugh.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://qyw.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://diy.xingfuxueyuan.xyz

================================================================================
来源：http://fat.tian-w.cn

F. 文件与目录
来源：http://uvc.zhengqikj.top

================================================================================
来源：http://yqz.wangshuangyany.cn

[F01] 读取整个文件
来源：http://rnv.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://juk.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://ggv.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nex.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ayj.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ojl.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uuy.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://hnd.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://xhv.gaohongyu789.top

[F02] 逐行读取文件
来源：http://yiz.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pzt.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pbz.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nqm.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://evc.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://woz.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rvb.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://doz.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dgz.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://vff.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hyz.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nch.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqd.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ykt.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nlk.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://osi.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://rso.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lkm.ctjpmb.com

[F04] 追加写入文件
来源：http://meu.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jin.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lfg.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tax.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://trw.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mrr.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qhk.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fzt.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dqj.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://mqe.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dwm.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://egn.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://vwt.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://rkb.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iub.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kbi.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://eax.tarul.cn

C#:   File.Exists("a.txt")
来源：http://zkz.haohaochexian.top

[F06] 删除文件
来源：http://dmz.pycfn.com

Py:   os.remove("a.txt")
来源：http://ips.pycfn.com

PHP:  unlink("a.txt");
来源：http://goe.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://efj.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ktf.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jhm.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://xnj.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://kar.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://lku.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://kpy.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://afv.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mpy.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cgy.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pvd.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fvj.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://shc.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vbx.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zwb.quarkkingdee.top

[F08] 遍历目录
来源：http://fsa.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kei.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vzv.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://bjs.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://ybj.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zlq.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://znm.cucudq.cn

Ruby: Dir.children("dir")
来源：http://ohk.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://kvu.hnqzz.top

[F09] 获取文件大小
来源：http://lxa.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://syv.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://fax.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://eti.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://fkd.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nvt.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nqn.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://iac.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://hee.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://zga.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iss.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ies.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://soe.meibo888.top

TS:   path.extname("a.txt")
来源：http://klc.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lpb.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uuy.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xyz.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lzf.zycfv.cn

[F11] 复制与移动文件
来源：http://vfh.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qfd.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://azy.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://egf.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pum.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yds.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fel.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://grg.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://upc.tianlin.xyz

[F12] CSV 读写
来源：http://wli.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vwk.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://guv.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pyw.nanxinkj.top

TS:   // 同上
来源：http://yjl.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aqh.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rgg.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nfv.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://czh.c1oappe.top

================================================================================
来源：http://hgf.cheryme.top

G. 面向对象
来源：http://mfw.fehbvm.com

================================================================================
来源：http://ann.chenzaomai.com

[G01] 定义类
来源：http://nou.jiagoushi.top

Py:   class User: pass
来源：http://use.cashguo.top

PHP:  class User {}
来源：http://syh.fanxiaobao.xyz

JS:   class User {}
来源：http://asn.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://yyo.meibo888.top

Java: class User {}
来源：http://wmn.ctjpmb.com

Go:   type User struct { Name string }
来源：http://uqu.nwbrower.top

Ruby: class User; end
来源：http://igi.hcnkem.com

C#:   class User {}
来源：http://ikw.hnxiangtu.top

[G02] 构造函数
来源：http://tag.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://lkv.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://uco.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://sch.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://imd.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://pxx.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wmj.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://pqt.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://vzf.snrcjt.cn

[G03] 实例属性
来源：http://tpk.cucudq.cn

Py:   self.name = "x"
来源：http://ukz.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://thc.jiagoushi.top

JS:   this.name = "x";
来源：http://hme.iojbl.cn

TS:   name: string = "x";
来源：http://rve.dianchejie.cn

Java: private String name;
来源：http://lzx.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tts.ydjk.org.cn

Ruby: @name = "x"
来源：http://une.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://hxp.c1oappe.top

[G04] 定义方法
来源：http://vft.daria6918.cn

Py:   def greet(self): return self.name
来源：http://bik.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://usw.tarul.cn

JS:   greet() { return this.name; }
来源：http://yqt.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://noc.tian-w.cn

Java: String greet() { return name; }
来源：http://czq.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nzd.meibo888.top

Ruby: def greet; @name; end
来源：http://ibp.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://kxo.xingfuxueyuan.xyz

[G05] 继承
来源：http://umx.yangfankeji.com

Py:   class Admin(User): pass
来源：http://nhn.yj202588.top

PHP:  class Admin extends User {}
来源：http://wxz.chenlongwang.top

JS:   class Admin extends User {}
来源：http://oro.wangdashe.top

TS:   class Admin extends User {}
来源：http://ifg.jyoumei.cn

Java: class Admin extends User {}
来源：http://wgc.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hpy.zhengqikj.top

Ruby: class Admin < User; end
来源：http://xsa.yuanzhike.top

C#:   class Admin : User {}
来源：http://bfq.jqgfzy.top

[G06] 重写方法
来源：http://upt.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://nvq.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wvg.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://dwc.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://ynp.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://tjb.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lvh.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://hok.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://knt.yongpay.top

[G07] 调用父类方法
来源：http://kos.shzxlz.cn

Py:   super().greet()
来源：http://prl.ctjpmb.com

PHP:  parent::greet();
来源：http://sbc.zhaomingkeji.xyz

JS:   super.greet();
来源：http://yvx.zdbjq.cn

TS:   super.greet();
来源：http://edp.daria6918.cn

Java: super.greet();
来源：http://kap.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ktr.chenlongwang.top

Ruby: super
来源：http://wuz.pengpengdd.cyou

C#:   base.Greet();
来源：http://hxz.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://eyn.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://acy.cucudq.cn

PHP:  public static function f() {}
来源：http://mxe.iojbl.cn

JS:   static f() {}
来源：http://fyv.zhongyouzk.top

TS:   static f(): void {}
来源：http://exx.sufxvd.cn

Java: static void f() {}
来源：http://xkw.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://enr.ctjpmb.com

Ruby: def self.f; end
来源：http://zyp.shzxlz.cn

C#:   public static void F() {}
来源：http://wss.tarul.cn

[G09] 接口 / 抽象类
来源：http://ccf.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://obk.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ivt.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wim.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://nfb.fktsv.cn

Java: interface Shape { double area(); }
来源：http://zpi.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://qzj.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qgm.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://bke.fktsv.cn

[G10] 访问控制
来源：http://yau.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://lzd.316326.xyz

PHP:  public / protected / private
来源：http://zeg.hammf.cn

JS:   #private 字段；其余公开
来源：http://shc.cdnleiting.top

TS:   public / protected / private
来源：http://wof.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://sng.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wxv.yongpay.top

Ruby: public / protected / private
来源：http://zgh.sxryk.cn

C#:   public / protected / private / internal
来源：http://wsn.pycfn.com

[G11] getter / setter
来源：http://bqs.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://jqo.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://edz.ybcxt.top

JS:   get name() { return this._name; }
来源：http://jhp.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://iyi.aizwys.cn

Java: public String getName() { return name; }
来源：http://xqh.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://efg.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://ink.hcnkem.com

C#:   public string Name { get; set; }
来源：http://ubx.chenzaomai.com

[G12] 对象转字符串
来源：http://ecq.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://srb.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://siq.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://wns.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://rdp.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://lix.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://nmx.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://pzx.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://izd.yangfankeji.com

[G13] 判断对象类型
来源：http://vzc.hywenlv.cn

Py:   isinstance(u, User)
来源：http://otw.daxiang520.top

PHP:  $u instanceof User
来源：http://hjp.pycfn.com

JS:   u instanceof User
来源：http://uzq.hammf.cn

TS:   u instanceof User
来源：http://kmi.daria6918.cn

Java: u instanceof User
来源：http://pdo.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://uvr.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://oet.sweek.top

C#:   u is User
来源：http://koh.zhoulong.xyz

[G14] 数据类 / record
来源：http://hwr.hysaishi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cob.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://iuv.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://hui.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://xnq.guannengcc.top

Java: record User(String name, int age) {}
来源：http://hmw.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://det.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hss.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://fqj.gaohongyu789.top

[G15] 枚举
来源：http://mrn.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mmw.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lny.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mby.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fjc.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://ewa.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uyy.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://xov.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suq.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://xxc.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://enh.birdmap.top

PHP:  get_object_vars($obj);
来源：http://ywy.yuanzhike.top

JS:   Object.entries(obj)
来源：http://ogj.birdmap.top

TS:   Object.entries(obj)
来源：http://txx.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gar.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bmb.yangfankeji.com

Ruby: obj.instance_variables
来源：http://sle.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://aup.bjfxy.top

================================================================================
来源：http://sll.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://ixr.ybcxt.top

================================================================================
来源：http://zsn.pengpengdd.cyou

[H01] try / catch 基础
来源：http://ktq.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://upq.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lzw.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://byc.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fgk.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://knk.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oxe.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bqb.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://saj.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://xob.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://dtb.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://weh.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://njz.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://oru.cheryme.top

Java: try { f(); } finally { cleanup(); }
来源：http://jpj.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rou.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://nro.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cyy.zycfv.cn

[H03] 主动抛出异常
来源：http://wml.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://mzz.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ckg.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://bqz.sufxvd.cn


<!-- 参考信息 -->