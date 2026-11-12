代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vqo.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://med.nanxinkj.top

TS:   if (s === "") {}
来源：http://fjg.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://wjr.chenzaomai.com

Go:   if s == "" {}
来源：http://tmw.yj20258.top

Ruby: if s.empty?
来源：http://juq.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ppp.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://xdp.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oum.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kvp.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sbg.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tgy.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://opj.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://ynf.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mgv.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uis.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://pcy.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zyu.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zob.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mam.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bhs.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pvh.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lam.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://rhe.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uvn.guowangkeji.top

================================================================================
来源：http://uoa.sysykeji.top

F. 文件与目录
来源：http://alb.sxryk.cn

================================================================================
来源：http://mcx.svipenyu.cn

[F01] 读取整个文件
来源：http://nvk.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nwt.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://mwu.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vci.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blr.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tpb.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lrr.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://hkj.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://yku.gaohongyu789.top

[F02] 逐行读取文件
来源：http://ltm.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mvn.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hfc.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dap.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://med.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://omh.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mkk.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xyj.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tpo.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://gci.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cnk.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://qfr.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lwd.yj20258888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lij.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oon.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xkv.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://ymu.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ytq.jqgufenzy.top

[F04] 追加写入文件
来源：http://inx.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tyo.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lij.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lnp.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://amw.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lce.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fcu.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://con.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cpd.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://xum.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://znd.yonumen.top

PHP:  file_exists("a.txt");
来源：http://yxu.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://qel.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://gex.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ubm.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jto.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://vso.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://ijm.yvedp.cn

[F06] 删除文件
来源：http://utj.xylfe.cn

Py:   os.remove("a.txt")
来源：http://zyo.cashguo.top

PHP:  unlink("a.txt");
来源：http://xnc.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://eqg.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://rfk.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://djz.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://ast.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://sqt.meibo888.top

C#:   File.Delete("a.txt");
来源：http://pzg.yj202588.top

[F07] 创建目录（含多级）
来源：http://qjp.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gpc.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lwr.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vuy.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjl.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oho.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qox.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jge.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tpb.yj202588.top

[F08] 遍历目录
来源：http://piy.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zqv.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bum.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://kkx.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://siz.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qsm.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ekn.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://qau.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://wtu.cqqwz.cn

[F09] 获取文件大小
来源：http://ynt.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://tht.uphjek.com

PHP:  filesize("a.txt");
来源：http://ocf.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://jrx.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://wuc.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://rva.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ioq.redwolf501.top

Ruby: File.size("a.txt")
来源：http://rnw.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://drm.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://tqb.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qop.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qbu.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qbs.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://xyh.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mhm.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kkn.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zyp.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://khc.gotoacloud.top

[F11] 复制与移动文件
来源：http://hbk.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jkf.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vrm.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vux.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xmv.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yuv.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kty.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dgy.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sve.fktsv.cn

[F12] CSV 读写
来源：http://yyq.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qjs.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qfy.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nkv.9152youxi.cn

TS:   // 同上
来源：http://fit.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qpu.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lvr.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dys.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gjs.havefunace.top

================================================================================
来源：http://zmz.9152youxi.cn

G. 面向对象
来源：http://upy.vqdsnc.cn

================================================================================
来源：http://cez.shanyushiyangkeji.top

[G01] 定义类
来源：http://yhu.wangshuangyany.cn

Py:   class User: pass
来源：http://frh.c1oappe.top

PHP:  class User {}
来源：http://ovm.tanke756.top

JS:   class User {}
来源：http://xsv.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://otf.zhaomingkeji.xyz

Java: class User {}
来源：http://kfl.zhengqikj.top

Go:   type User struct { Name string }
来源：http://zhs.chenzaomai.com

Ruby: class User; end
来源：http://hgi.sweek.top

C#:   class User {}
来源：http://joi.hnxiangtu.top

[G02] 构造函数
来源：http://qcn.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://nbq.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://uph.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://ulz.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://bwn.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://jts.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://obz.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://tus.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://qmi.vehdjk.com

[G03] 实例属性
来源：http://uga.jiagoushi.top

Py:   self.name = "x"
来源：http://xos.fzhhl.top

PHP:  public string $name = "x";
来源：http://taf.jqgufenzy.top

JS:   this.name = "x";
来源：http://nem.mhx1999.top

TS:   name: string = "x";
来源：http://ahr.dashuyun.cn

Java: private String name;
来源：http://gim.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://stf.cheryme.top

Ruby: @name = "x"
来源：http://kmk.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://umu.hcnkem.com

[G04] 定义方法
来源：http://dgb.cheryme.top

Py:   def greet(self): return self.name
来源：http://uqa.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zld.zhixingplan.top

JS:   greet() { return this.name; }
来源：http://cjc.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://tqj.nwbrower.top

Java: String greet() { return name; }
来源：http://udj.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pzq.wangshuangyany.cn

Ruby: def greet; @name; end
来源：http://iop.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://ccm.jyoumei.cn

[G05] 继承
来源：http://tls.tanke756.top

Py:   class Admin(User): pass
来源：http://msr.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://btf.tarul.cn

JS:   class Admin extends User {}
来源：http://poq.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://sdt.tianlin.xyz

Java: class Admin extends User {}
来源：http://mly.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gni.9152youxi.cn

Ruby: class Admin < User; end
来源：http://xwa.xylfe.cn

C#:   class Admin : User {}
来源：http://qxf.epnwcf.com

[G06] 重写方法
来源：http://wds.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://pix.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lzk.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://cjv.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://hio.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://urs.haohaochexian.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oyl.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://vwq.chenjidiqi.icu

C#:   public override string Greet() => "admin";
来源：http://rus.hywenlv.cn

[G07] 调用父类方法
来源：http://rxa.ydzc1.top

Py:   super().greet()
来源：http://zlz.gotoacloud.top

PHP:  parent::greet();
来源：http://mfi.hnxiangtu.top

JS:   super.greet();
来源：http://mot.chenjidiqi.icu

TS:   super.greet();
来源：http://dir.jinyuanbaomall.cn

Java: super.greet();
来源：http://llt.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fkb.chenjidiqi.icu

Ruby: super
来源：http://rlk.svipenyu.cn

C#:   base.Greet();
来源：http://rzi.hnxiangtu.top

[G08] 静态方法与属性
来源：http://wiz.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uiy.wangdashe.top

PHP:  public static function f() {}
来源：http://eoc.yfazqb.com

JS:   static f() {}
来源：http://hkc.birdmap.top

TS:   static f(): void {}
来源：http://zht.hfpthk.cn

Java: static void f() {}
来源：http://fxu.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qtv.yj20258.top

Ruby: def self.f; end
来源：http://faa.xziqi.cn

C#:   public static void F() {}
来源：http://rbj.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://amz.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://qaa.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://tka.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://osi.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://giv.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://vuh.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://ewt.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wkw.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://pzp.ydzc1.top

[G10] 访问控制
来源：http://hdb.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://cik.hesvh.cn

PHP:  public / protected / private
来源：http://glb.zycfv.cn

JS:   #private 字段；其余公开
来源：http://umc.vehdjk.com

TS:   public / protected / private
来源：http://ewr.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://duc.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://amm.kuanghao11.cn

Ruby: public / protected / private
来源：http://ker.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://jnz.yj20258888.top

[G11] getter / setter
来源：http://fgc.xylfe.cn

Py:   @property 与 @x.setter
来源：http://ejt.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eap.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://ivj.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://wzd.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://hme.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://opo.wangdashe.top

Ruby: attr_accessor :name
来源：http://yzc.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://qip.birdmap.top

[G12] 对象转字符串
来源：http://vgf.cheryme.top

Py:   def __str__(self): return self.name
来源：http://kfs.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://adm.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://hka.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://xtw.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://xkp.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sdc.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://hty.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://iit.yuxming.cn

[G13] 判断对象类型
来源：http://bar.mhx1999.top

Py:   isinstance(u, User)
来源：http://dbr.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://tlb.shanyushiyangtech.top

JS:   u instanceof User
来源：http://ztj.jlsjyb.cn

TS:   u instanceof User
来源：http://wrr.fktsv.cn

Java: u instanceof User
来源：http://ptg.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://bpg.fengsongda.top

Ruby: u.is_a?(User)
来源：http://nbd.gogol.net.cn

C#:   u is User
来源：http://tpt.yanxiufei.cn

[G14] 数据类 / record
来源：http://kwy.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fxd.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://zlg.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://enc.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://rhc.xuanzx.com

Java: record User(String name, int age) {}
来源：http://str.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://ugk.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://csp.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://min.yangfankeji.com

[G15] 枚举
来源：http://xqo.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wja.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jbz.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nce.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ggp.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://owb.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://etm.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://vbx.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ila.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://upk.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lbr.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://qvi.nanxinkj.top

JS:   Object.entries(obj)
来源：http://wxa.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://jwq.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://upe.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iau.bbcook.cn

Ruby: obj.instance_variables
来源：http://ngg.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://yjh.zycfv.cn

================================================================================
来源：http://azz.yonumen.top

H. 异常与错误处理
来源：http://fzx.redwolf501.top

================================================================================
来源：http://ece.zhengqikj.top

[H01] try / catch 基础
来源：http://yth.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nbh.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oxg.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ilm.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wtr.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://des.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nrq.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dte.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uas.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://cpz.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://xvg.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://loa.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yrk.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xmv.vqdsnc.cn


<!-- 参考信息 -->