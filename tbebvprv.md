代发 wailian999

Go:   if s == "" {}
来源：http://hdn.shangyingyoupin.top

Ruby: if s.empty?
来源：http://pld.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eic.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://jzq.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mll.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://frp.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://flk.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztf.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pjt.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://xmt.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://teh.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xzo.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://sae.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fwg.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kuv.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wpn.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://elj.dashuyun.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sym.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wka.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://zdq.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tgk.yfazqb.com

================================================================================
来源：http://ght.chenlongwang.top

F. 文件与目录
来源：http://dbb.iojbl.cn

================================================================================
来源：http://mgx.zhoulong.xyz

[F01] 读取整个文件
来源：http://ack.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nls.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://mig.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://agc.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mjg.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kwe.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qsh.ivvv.top

Ruby: File.read("a.txt")
来源：http://zmb.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ijp.redwolf501.top

[F02] 逐行读取文件
来源：http://gsq.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cjo.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xrm.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jst.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://igo.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ktb.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yps.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dbl.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fdk.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://qft.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jlq.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://exs.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://njt.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyr.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yze.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://php.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qot.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fmi.dashuyun.cn

[F04] 追加写入文件
来源：http://jea.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zve.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://suf.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rha.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcw.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uir.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://agp.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ilv.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vmf.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://jei.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gbo.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://ykh.meibo888.top

JS:   fs.existsSync("a.txt")
来源：http://ljx.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://lyi.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://vfs.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lqi.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://xkb.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://xym.cucudq.cn

[F06] 删除文件
来源：http://pux.fktsv.cn

Py:   os.remove("a.txt")
来源：http://jaf.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://glt.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://cxf.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kuj.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hba.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://cfu.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://xpy.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://rqj.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://kpr.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zrw.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xrh.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hlh.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://whp.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://drc.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ssr.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gyr.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eoa.zycfv.cn

[F08] 遍历目录
来源：http://aza.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lcb.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dmq.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://hkx.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://gqa.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jsa.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fwz.yongpay.top

Ruby: Dir.children("dir")
来源：http://akq.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://kwv.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://tkx.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://hgc.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://bqw.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://nkc.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://vml.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://pwt.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hlb.yongpay.top

Ruby: File.size("a.txt")
来源：http://iip.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://zpw.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://odj.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rcb.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dxt.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xue.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://asm.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vmi.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zkt.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ivn.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zdn.gotoacloud.top

[F11] 复制与移动文件
来源：http://uxv.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nsv.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zcy.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qmw.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqz.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://adf.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jyq.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ybd.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tyd.hammf.cn

[F12] CSV 读写
来源：http://dko.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mbx.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gao.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wbi.guowangkeji.top

TS:   // 同上
来源：http://lll.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iyz.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rza.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://arg.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eud.yvedp.cn

================================================================================
来源：http://ddv.c1oappe.top

G. 面向对象
来源：http://hai.andypj.xyz

================================================================================
来源：http://msc.zdbjq.cn

[G01] 定义类
来源：http://pie.yvedp.cn

Py:   class User: pass
来源：http://yya.chenjidiqi.icu

PHP:  class User {}
来源：http://fpf.daxiang520.top

JS:   class User {}
来源：http://ryb.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://sof.zhoulong.xyz

Java: class User {}
来源：http://odk.jyoumei.cn

Go:   type User struct { Name string }
来源：http://imx.vehdjk.com

Ruby: class User; end
来源：http://dmm.gogol.net.cn

C#:   class User {}
来源：http://nmv.gogol.net.cn

[G02] 构造函数
来源：http://pcv.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://wtx.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://olc.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://jlu.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://kbh.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://qec.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blq.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://epz.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://jpu.jqgufenzy.top

[G03] 实例属性
来源：http://hlx.jinqigufen.top

Py:   self.name = "x"
来源：http://hqw.sufxvd.cn

PHP:  public string $name = "x";
来源：http://wus.gaohongyu789.top

JS:   this.name = "x";
来源：http://uru.9152youxi.cn

TS:   name: string = "x";
来源：http://mmb.jyoumei.cn

Java: private String name;
来源：http://eco.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qwa.sweek.top

Ruby: @name = "x"
来源：http://iuq.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://tjz.jqgfzy.top

[G04] 定义方法
来源：http://jxq.52xcode.cn

Py:   def greet(self): return self.name
来源：http://lia.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jhn.tian-w.cn

JS:   greet() { return this.name; }
来源：http://pub.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://cha.hfpthk.cn

Java: String greet() { return name; }
来源：http://sqz.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vxr.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://yfm.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://tzd.zhiwuduotai.top

[G05] 继承
来源：http://zlt.ybcxt.top

Py:   class Admin(User): pass
来源：http://qsj.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://cep.sweek.top

JS:   class Admin extends User {}
来源：http://yhx.fzhhl.top

TS:   class Admin extends User {}
来源：http://giv.wangdashe.top

Java: class Admin extends User {}
来源：http://csd.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jzj.hnqzz.top

Ruby: class Admin < User; end
来源：http://nbj.hnqzz.top

C#:   class Admin : User {}
来源：http://blq.andypj.xyz

[G06] 重写方法
来源：http://xpp.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://dui.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gaq.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://xpr.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://rie.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://xqf.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://str.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://onl.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://hbc.shuidangran.top

[G07] 调用父类方法
来源：http://plm.chenjidiqi.icu

Py:   super().greet()
来源：http://vdz.0kj1m.cn

PHP:  parent::greet();
来源：http://lgf.ywan-chungtsiang.top

JS:   super.greet();
来源：http://qlx.shanyushiyangkeji.top

TS:   super.greet();
来源：http://wjj.dashuyun.cn

Java: super.greet();
来源：http://sgz.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pwk.hysaishi.cn

Ruby: super
来源：http://phb.gaohongyu789.top

C#:   base.Greet();
来源：http://gyd.fengsongda.top

[G08] 静态方法与属性
来源：http://ngf.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xjf.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://fbt.havefunace.top

JS:   static f() {}
来源：http://ryg.tarul.cn

TS:   static f(): void {}
来源：http://izg.nanxuanxn.top

Java: static void f() {}
来源：http://hai.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fav.hfpthk.cn

Ruby: def self.f; end
来源：http://dvr.bjfxy.top

C#:   public static void F() {}
来源：http://bqf.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://myw.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://ttf.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://lgt.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://puu.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://rwd.yj202588.top

Java: interface Shape { double area(); }
来源：http://vnm.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://zrh.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://snp.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://nde.guowangkeji.top

[G10] 访问控制
来源：http://koe.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://cqg.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://bmc.birdmap.top

JS:   #private 字段；其余公开
来源：http://pjl.hcnkem.com

TS:   public / protected / private
来源：http://uoi.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://rxj.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://llw.jyoumei.cn

Ruby: public / protected / private
来源：http://tbg.epnwcf.com

C#:   public / protected / private / internal
来源：http://ttd.shangyingyoupin.top

[G11] getter / setter
来源：http://cko.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://ldm.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bjo.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://hbn.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://iuy.0kj1m.cn

Java: public String getName() { return name; }
来源：http://kym.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uyr.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://lyf.hnqzz.top

C#:   public string Name { get; set; }
来源：http://ulc.yanxiufei.cn

[G12] 对象转字符串
来源：http://wfa.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://dsi.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mav.xylfe.cn

JS:   toString() { return this.name; }
来源：http://ptj.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://lkl.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://oyf.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://xlr.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://siy.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://end.kuanghao11.cn

[G13] 判断对象类型
来源：http://ciq.yfazqb.com

Py:   isinstance(u, User)
来源：http://ibt.yj202588.top

PHP:  $u instanceof User
来源：http://ypj.wangdashe.top

JS:   u instanceof User
来源：http://udd.tianlin.xyz

TS:   u instanceof User
来源：http://glw.yj20258888.top

Java: u instanceof User
来源：http://mlq.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yfr.epnwcf.com

Ruby: u.is_a?(User)
来源：http://uef.gotoacloud.top

C#:   u is User
来源：http://tse.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://ksp.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cyp.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://yka.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://nxf.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://skg.hesvh.cn

Java: record User(String name, int age) {}
来源：http://rcx.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://dxd.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kma.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://otr.wangshuangyany.cn

[G15] 枚举
来源：http://gtd.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xhj.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bcl.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://loa.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://frk.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://bce.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uyz.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://ucx.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zmr.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://xjc.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lii.9152youxi.cn

PHP:  get_object_vars($obj);
来源：http://qnd.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://baj.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://xrz.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bzx.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://uum.ppjwa.cn

Ruby: obj.instance_variables
来源：http://qop.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://pum.yuxming.cn

================================================================================
来源：http://xjm.0kj1m.cn

H. 异常与错误处理
来源：http://xou.vehdjk.com

================================================================================
来源：http://blk.nanxuanxn.top

[H01] try / catch 基础
来源：http://kct.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sre.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://brc.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://psr.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jjt.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uvm.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hhm.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dnl.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://twt.andypj.xyz

[H02] finally / ensure 收尾
来源：http://xzv.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mbs.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zkk.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://icv.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xda.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zmn.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lyi.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ptr.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xum.jqgufenzy.top


<!-- 参考信息 -->