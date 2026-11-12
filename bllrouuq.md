代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pbp.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://abt.hywenlv.cn

TS:   if (s === "") {}
来源：http://hrr.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://cqm.ivvv.top

Go:   if s == "" {}
来源：http://sjk.andypj.xyz

Ruby: if s.empty?
来源：http://wvm.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ean.cashguo.top

[E21] 超长截断加省略号
来源：http://asr.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zni.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iyo.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://woc.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://maz.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pma.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://zxm.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://akm.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nnj.fengsongda.top

[E22] 字节长度与字符长度
来源：http://cqw.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ptv.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vtg.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uky.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xqj.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zqq.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ans.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://dfz.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pds.yj202588.top

================================================================================
来源：http://pqv.havefunace.top

F. 文件与目录
来源：http://tir.yanxiufei.cn

================================================================================
来源：http://dfd.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://iuv.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tbz.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://zdj.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rfc.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tya.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eez.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://avb.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://fjo.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://zcu.jinqigufen.top

[F02] 逐行读取文件
来源：http://khn.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://edy.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lvb.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbf.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://asf.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yyh.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cke.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dsv.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dru.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://unr.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eqw.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zlh.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovs.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cra.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mim.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gzy.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://rop.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vlz.cheryme.top

[F04] 追加写入文件
来源：http://lul.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mgv.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uim.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgh.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kyg.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yse.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rxk.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rsa.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://noz.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://lrg.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wuw.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://oht.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://ejw.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://ixt.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iqe.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cuw.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://kup.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://nqx.shangyingyoupin.top

[F06] 删除文件
来源：http://vkh.ybcxt.top

Py:   os.remove("a.txt")
来源：http://rdi.daxiang520.top

PHP:  unlink("a.txt");
来源：http://agw.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://hlq.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://kao.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iwl.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://rzg.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://ypa.tarul.cn

C#:   File.Delete("a.txt");
来源：http://ymb.fehbvm.com

[F07] 创建目录（含多级）
来源：http://qmr.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kqm.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yam.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://usf.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://krl.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ddu.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hmd.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jvz.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cfm.smart0.xyz

[F08] 遍历目录
来源：http://msb.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bhs.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ady.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://shz.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://aia.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lht.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xfk.ivvv.top

Ruby: Dir.children("dir")
来源：http://dyu.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://guh.ctjpmb.com

[F09] 获取文件大小
来源：http://syd.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://vto.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://dee.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://gjj.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://gmk.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ymk.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oue.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://ywn.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://tcr.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://emq.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kmm.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://brh.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kqw.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://tjq.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ivl.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lfn.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iux.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ojc.jlsjyb.cn

[F11] 复制与移动文件
来源：http://upk.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://agf.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nld.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://exa.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ila.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gzf.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ccw.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lrd.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ffd.zycfv.cn

[F12] CSV 读写
来源：http://rou.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mbo.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qxs.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jqg.wangshuangyany.cn

TS:   // 同上
来源：http://zxc.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rwz.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wav.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ebi.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ric.dianchejie.cn

================================================================================
来源：http://odz.yvedp.cn

G. 面向对象
来源：http://ftw.jqgufenzy.top

================================================================================
来源：http://buf.snrcjt.cn

[G01] 定义类
来源：http://ijv.guannengcc.top

Py:   class User: pass
来源：http://otn.redwolf501.top

PHP:  class User {}
来源：http://bwv.xuanzx.com

JS:   class User {}
来源：http://lud.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://uul.yvedp.cn

Java: class User {}
来源：http://vgr.sufxvd.cn

Go:   type User struct { Name string }
来源：http://cea.zhijiandao.cn

Ruby: class User; end
来源：http://fef.yfazqb.com

C#:   class User {}
来源：http://izi.yanxiufei.cn

[G02] 构造函数
来源：http://rpg.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://sbg.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://ufb.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://elj.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://rqt.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://tdk.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blo.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://ssj.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://yeh.iojbl.cn

[G03] 实例属性
来源：http://phu.hfpthk.cn

Py:   self.name = "x"
来源：http://oaa.52xcode.cn

PHP:  public string $name = "x";
来源：http://bzg.hesvh.cn

JS:   this.name = "x";
来源：http://ess.guowangkeji.top

TS:   name: string = "x";
来源：http://ntv.pengpengdd.cyou

Java: private String name;
来源：http://jzs.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tsz.sxryk.cn

Ruby: @name = "x"
来源：http://wvn.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://eqx.cqqwz.cn

[G04] 定义方法
来源：http://dkz.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://jsn.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://iya.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://nwm.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://svj.zhijiandao.cn

Java: String greet() { return name; }
来源：http://ewh.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gfi.cqqwz.cn

Ruby: def greet; @name; end
来源：http://uau.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://xyh.9152youxi.cn

[G05] 继承
来源：http://gxz.zhengqikj.top

Py:   class Admin(User): pass
来源：http://vci.ivvv.top

PHP:  class Admin extends User {}
来源：http://apu.haohaochexian.top

JS:   class Admin extends User {}
来源：http://wex.yj20258.top

TS:   class Admin extends User {}
来源：http://sok.dianchejie.cn

Java: class Admin extends User {}
来源：http://fbd.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dyk.9152youxi.cn

Ruby: class Admin < User; end
来源：http://apt.kuanghao11.cn

C#:   class Admin : User {}
来源：http://ypw.jinghuilouyu.cn

[G06] 重写方法
来源：http://jvq.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://pem.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rsh.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://lbx.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://vks.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://uvo.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kfa.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://ltb.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://psv.daxiang520.top

[G07] 调用父类方法
来源：http://npl.mhx1999.top

Py:   super().greet()
来源：http://gyp.yj20258888.top

PHP:  parent::greet();
来源：http://foa.cucudq.cn

JS:   super.greet();
来源：http://jmw.jinyuanbaomall.cn

TS:   super.greet();
来源：http://ugz.dianchejie.cn

Java: super.greet();
来源：http://wtk.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tsb.gzhubu.top

Ruby: super
来源：http://xma.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://sve.hywenlv.cn

[G08] 静态方法与属性
来源：http://ofj.fanxiaobao.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://liu.havefunace.top

PHP:  public static function f() {}
来源：http://nxp.pengpengdd.cyou

JS:   static f() {}
来源：http://dda.fktsv.cn

TS:   static f(): void {}
来源：http://xxe.epnwcf.com

Java: static void f() {}
来源：http://xbs.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kfq.zdbjq.cn

Ruby: def self.f; end
来源：http://rfe.zhoulong.xyz

C#:   public static void F() {}
来源：http://lfi.smart0.xyz

[G09] 接口 / 抽象类
来源：http://pao.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://dut.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zjv.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ivj.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://otr.cheryme.top

Java: interface Shape { double area(); }
来源：http://fzf.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://zbm.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ezd.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://lil.xziqi.cn

[G10] 访问控制
来源：http://ilb.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://lbo.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://lva.hcnkem.com

JS:   #private 字段；其余公开
来源：http://kxe.hnqzz.top

TS:   public / protected / private
来源：http://nsu.tanke756.top

Java: public / protected / private / 默认包级
来源：http://sgi.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hkn.hesvh.cn

Ruby: public / protected / private
来源：http://ffd.meibo888.top

C#:   public / protected / private / internal
来源：http://nmn.andypj.xyz

[G11] getter / setter
来源：http://ffl.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://pec.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fve.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://law.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://ach.yj20258.top

Java: public String getName() { return name; }
来源：http://rcf.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://frc.yueranfly.top

Ruby: attr_accessor :name
来源：http://lwq.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://jwc.zhengqikj.top

[G12] 对象转字符串
来源：http://gzk.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://hir.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kpa.xinyue.icu

JS:   toString() { return this.name; }
来源：http://zqe.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://qqm.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://nat.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://jdc.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://zzj.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://bvz.tian-w.cn

[G13] 判断对象类型
来源：http://nwn.daria6918.cn

Py:   isinstance(u, User)
来源：http://vbx.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://dgp.ehwqpu.com

JS:   u instanceof User
来源：http://spx.snrcjt.cn

TS:   u instanceof User
来源：http://bef.ppjwa.cn

Java: u instanceof User
来源：http://ipt.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://avx.daria6918.cn

Ruby: u.is_a?(User)
来源：http://khw.yj202588.top

C#:   u is User
来源：http://woe.wangshuangyany.cn

[G14] 数据类 / record
来源：http://myl.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jxo.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://lsf.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qbs.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://eno.iojbl.cn

Java: record User(String name, int age) {}
来源：http://wjg.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://lou.redwolf501.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jqm.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://mrl.ydjk.org.cn

[G15] 枚举
来源：http://fns.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nms.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://daw.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sxk.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://arh.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://tcp.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uuy.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://mrj.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://amr.meibo888.top

[G16] 对象转数组 / 字典
来源：http://qcf.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bib.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://ppb.zhengqikj.top

JS:   Object.entries(obj)
来源：http://wdy.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://oey.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ufq.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://kht.ppjwa.cn

Ruby: obj.instance_variables
来源：http://rjm.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://chk.vqdsnc.cn

================================================================================
来源：http://ysa.hesvh.cn

H. 异常与错误处理
来源：http://dvt.ybcxt.top

================================================================================
来源：http://foc.hywenlv.cn

[H01] try / catch 基础
来源：http://vee.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xir.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zln.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fqa.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lhs.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://skw.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dnq.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bcz.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ymt.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://zkp.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oib.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://ivj.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wds.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cfp.ydzc1.top


<!-- 参考信息 -->