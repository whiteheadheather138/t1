代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://muh.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mwh.jianghu66.top

TS:   if (s === "") {}
来源：http://anr.sweek.top

Java: if (s.isEmpty()) {}
来源：http://pga.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://xtt.shuidangran.top

Ruby: if s.empty?
来源：http://xcf.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wno.mhx1999.top

[E21] 超长截断加省略号
来源：http://mpg.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mfl.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vke.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqw.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zwe.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tyu.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://rmc.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yhl.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cko.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://sib.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cpo.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnn.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tiu.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://amx.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jyw.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jlq.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://mth.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ojd.yj20258888.top

================================================================================
来源：http://atj.shangyingyoupin.top

F. 文件与目录
来源：http://ysh.dashuyun.cn

================================================================================
来源：http://bbu.jyoumei.cn

[F01] 读取整个文件
来源：http://rog.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ayu.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://ouj.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dbx.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hll.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wij.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qwz.yj20258.top

Ruby: File.read("a.txt")
来源：http://urj.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://iqu.tanke756.top

[F02] 逐行读取文件
来源：http://zvi.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jwa.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hwm.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aym.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfl.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qfn.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mlk.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aqz.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qma.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://dpd.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tfs.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fau.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xqj.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jue.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vtv.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dri.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://mvg.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://byv.yuanzhike.top

[F04] 追加写入文件
来源：http://sjw.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fmt.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://siu.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jea.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pzy.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://arf.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wln.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rfi.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yss.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://ytm.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ujg.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://fhm.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://qfc.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://mum.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://glf.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dij.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://uyr.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://gtp.hywenlv.cn

[F06] 删除文件
来源：http://vyb.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://ixx.tarul.cn

PHP:  unlink("a.txt");
来源：http://piy.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://vsr.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://hyd.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xkn.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://snl.tarul.cn

Ruby: File.delete("a.txt")
来源：http://jal.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://ujc.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://hzc.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kdd.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ive.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vap.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dzt.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hof.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vfa.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hsf.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lrl.pycfn.com

[F08] 遍历目录
来源：http://cea.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://amg.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wdv.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://ynp.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://fcd.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ldf.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yyj.zycfv.cn

Ruby: Dir.children("dir")
来源：http://ibd.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://lwb.yfazqb.com

[F09] 获取文件大小
来源：http://vqj.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://ava.xziqi.cn

PHP:  filesize("a.txt");
来源：http://tih.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://pvs.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://fhm.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://gmy.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://imy.zycfv.cn

Ruby: File.size("a.txt")
来源：http://gxe.iojbl.cn

C#:   new FileInfo("a.txt").Length
来源：http://anf.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://rls.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uus.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mgz.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rem.cashguo.top

TS:   path.extname("a.txt")
来源：http://sdr.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dig.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bul.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jtm.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fdk.zhengqikj.top

[F11] 复制与移动文件
来源：http://uxk.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gxd.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ory.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yti.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nng.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uca.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qvw.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yzi.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://caz.zdbjq.cn

[F12] CSV 读写
来源：http://gep.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kyy.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tll.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tsi.ydjk.org.cn

TS:   // 同上
来源：http://rny.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iak.jqgfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ees.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oce.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pqe.gotoacloud.top

================================================================================
来源：http://esu.birdmap.top

G. 面向对象
来源：http://dam.0kj1m.cn

================================================================================
来源：http://qpg.kuanghao11.cn

[G01] 定义类
来源：http://wxr.zhaomingkeji.xyz

Py:   class User: pass
来源：http://yzn.feifeiyinyue.top

PHP:  class User {}
来源：http://lbi.52xcode.cn

JS:   class User {}
来源：http://odc.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://lep.zycfv.cn

Java: class User {}
来源：http://fxw.jiagoushi.top

Go:   type User struct { Name string }
来源：http://igc.yuxming.cn

Ruby: class User; end
来源：http://xrx.chenjidiqi.icu

C#:   class User {}
来源：http://zvb.zhaomingkeji.xyz

[G02] 构造函数
来源：http://dpj.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://hkc.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://pwn.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://rxe.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://kct.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://cjw.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tsq.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://bns.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://ctm.hongshengwenyu.top

[G03] 实例属性
来源：http://cxe.shuidangran.top

Py:   self.name = "x"
来源：http://uuh.meibo888.top

PHP:  public string $name = "x";
来源：http://wvw.gogol.net.cn

JS:   this.name = "x";
来源：http://anu.yangfankeji.com

TS:   name: string = "x";
来源：http://nkk.yj20258888.top

Java: private String name;
来源：http://uuq.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iyh.ydjk.org.cn

Ruby: @name = "x"
来源：http://lff.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://pbn.bbcook.cn

[G04] 定义方法
来源：http://noa.yj202588.top

Py:   def greet(self): return self.name
来源：http://imi.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lrq.fengsongda.top

JS:   greet() { return this.name; }
来源：http://ogl.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://ndz.jlsjyb.cn

Java: String greet() { return name; }
来源：http://vqv.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://omv.xziqi.cn

Ruby: def greet; @name; end
来源：http://isu.sysykeji.top

C#:   public string Greet() => Name;
来源：http://mkf.shzxlz.cn

[G05] 继承
来源：http://aiq.guowangkeji.top

Py:   class Admin(User): pass
来源：http://jml.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://nyq.cashguo.top

JS:   class Admin extends User {}
来源：http://qyr.pycfn.com

TS:   class Admin extends User {}
来源：http://zey.sweek.top

Java: class Admin extends User {}
来源：http://ltd.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mvc.tanke756.top

Ruby: class Admin < User; end
来源：http://idb.snrcjt.cn

C#:   class Admin : User {}
来源：http://ycl.sxryk.cn

[G06] 重写方法
来源：http://lfw.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://nyn.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kgs.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://ffm.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://opt.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://hba.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yny.tanke756.top

Ruby: def greet; "admin"; end
来源：http://lwm.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://qzt.pycfn.com

[G07] 调用父类方法
来源：http://mkc.sysykeji.top

Py:   super().greet()
来源：http://gcs.vqdsnc.cn

PHP:  parent::greet();
来源：http://nnb.feifeiyinyue.top

JS:   super.greet();
来源：http://wjo.sufxvd.cn

TS:   super.greet();
来源：http://ajx.havefunace.top

Java: super.greet();
来源：http://xbw.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iis.tanke756.top

Ruby: super
来源：http://abi.sweek.top

C#:   base.Greet();
来源：http://ggb.aizwys.cn

[G08] 静态方法与属性
来源：http://als.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://suv.jianghu66.top

PHP:  public static function f() {}
来源：http://ggq.sjlbkw.cn

JS:   static f() {}
来源：http://puw.guowangkeji.top

TS:   static f(): void {}
来源：http://fls.gaohongyu789.top

Java: static void f() {}
来源：http://djj.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qkp.hnqzz.top

Ruby: def self.f; end
来源：http://tdq.9152youxi.cn

C#:   public static void F() {}
来源：http://rws.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://xio.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://ffu.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://cqe.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zth.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://nnc.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://tzu.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://bto.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gwx.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://zpk.aizwys.cn

[G10] 访问控制
来源：http://rxu.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://xfd.aibaodan.cn

PHP:  public / protected / private
来源：http://mhu.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://bfc.andypj.xyz

TS:   public / protected / private
来源：http://mqf.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://gmx.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pzy.sxryk.cn

Ruby: public / protected / private
来源：http://ewf.fengsongda.top

C#:   public / protected / private / internal
来源：http://zea.sufxvd.cn

[G11] getter / setter
来源：http://ozx.c1oappe.top

Py:   @property 与 @x.setter
来源：http://vwz.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ydr.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://lkp.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://awy.ehwqpu.com

Java: public String getName() { return name; }
来源：http://xvb.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wag.tianlin.xyz

Ruby: attr_accessor :name
来源：http://lls.andypj.xyz

C#:   public string Name { get; set; }
来源：http://kpc.tian-w.cn

[G12] 对象转字符串
来源：http://dih.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://ojy.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yhe.epnwcf.com

JS:   toString() { return this.name; }
来源：http://wrf.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://oum.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://sav.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://uzm.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://onl.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://nqa.c1oappe.top

[G13] 判断对象类型
来源：http://urp.xuanzx.com

Py:   isinstance(u, User)
来源：http://jlx.yj20258.top

PHP:  $u instanceof User
来源：http://qhr.wangshuangyany.cn

JS:   u instanceof User
来源：http://tnx.shanyushiyangtech.top

TS:   u instanceof User
来源：http://gsr.yuxming.cn

Java: u instanceof User
来源：http://bpq.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qvq.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://kxl.c1oappe.top

C#:   u is User
来源：http://loe.xinyue.icu

[G14] 数据类 / record
来源：http://hoq.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dlq.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://vcj.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qdc.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://guh.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://wts.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://yyn.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kwz.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://vom.52xcode.cn

[G15] 枚举
来源：http://kvo.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kxw.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kwk.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yon.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iap.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://yyy.zhengqikj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wrn.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://rhl.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mty.havefunace.top

[G16] 对象转数组 / 字典
来源：http://caj.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blp.yonumen.top

PHP:  get_object_vars($obj);
来源：http://rac.hfpthk.cn

JS:   Object.entries(obj)
来源：http://ckq.fengsongda.top

TS:   Object.entries(obj)
来源：http://var.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cvo.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xaz.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://rwj.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://ppi.316326.xyz

================================================================================
来源：http://dre.zhongyouzk.top

H. 异常与错误处理
来源：http://nzw.yfazqb.com

================================================================================
来源：http://hdg.fktsv.cn

[H01] try / catch 基础
来源：http://gco.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://khw.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qhq.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tju.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tvn.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dhk.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vlg.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hir.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zqc.daxiang520.top

[H02] finally / ensure 收尾
来源：http://prk.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://dcp.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://imv.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://nhi.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rks.zhaomingkeji.xyz


<!-- 参考信息 -->