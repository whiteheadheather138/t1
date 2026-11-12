代发 wailian999

Go:   if s == "" {}
来源：http://mui.zhongyouzk.top

Ruby: if s.empty?
来源：http://dep.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nos.bjfxy.top

[E21] 超长截断加省略号
来源：http://aux.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mgg.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qcc.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bcw.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kuk.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ptb.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://srl.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iac.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lwn.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://put.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ggw.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kah.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdb.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zhq.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://udw.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vub.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://nfb.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hqy.zycfv.cn

================================================================================
来源：http://axu.jianghu66.top

F. 文件与目录
来源：http://sud.jiagoushi.top

================================================================================
来源：http://cxw.redwolf501.top

[F01] 读取整个文件
来源：http://cpl.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jht.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://mjp.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iun.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ybr.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gva.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kch.yuxming.cn

Ruby: File.read("a.txt")
来源：http://kyl.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://qwd.0kj1m.cn

[F02] 逐行读取文件
来源：http://xoi.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://utc.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vbm.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://msk.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kuz.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ydp.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sdd.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nfi.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mmf.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://sqz.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://omd.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://gdm.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jbl.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gly.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bpx.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ufz.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://plt.birdmap.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qrn.andypj.xyz

[F04] 追加写入文件
来源：http://srn.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mrl.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jgs.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gtn.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwh.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hwe.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ykn.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ogh.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://btj.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://llu.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://szp.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://oag.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://flv.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://xvd.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ivj.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gwn.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://qnj.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://tsk.dianchejie.cn

[F06] 删除文件
来源：http://qay.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://qot.fehbvm.com

PHP:  unlink("a.txt");
来源：http://zfc.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://omd.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cea.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kka.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://kav.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://eds.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://gkq.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://npm.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xow.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cvy.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wdk.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uyv.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://heu.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xei.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gog.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://diu.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://mvd.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://smz.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zbp.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://gfm.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://jwh.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bze.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gxs.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://wla.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://vtm.yangfankeji.com

[F09] 获取文件大小
来源：http://wgp.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://xje.fengsongda.top

PHP:  filesize("a.txt");
来源：http://iqh.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://ifs.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ood.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://blb.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wzw.ybcxt.top

Ruby: File.size("a.txt")
来源：http://xts.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ywf.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://mjh.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rir.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ikh.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hha.xziqi.cn

TS:   path.extname("a.txt")
来源：http://qhx.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ytp.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eyp.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://psw.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aeu.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://ecz.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://swr.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://otr.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mvr.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jhj.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pqm.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jej.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yyt.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lrp.c1oappe.top

[F12] CSV 读写
来源：http://zcv.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uye.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dar.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nfw.smart0.xyz

TS:   // 同上
来源：http://sgl.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rkk.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ssl.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ifr.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hxv.dashuyun.cn

================================================================================
来源：http://abf.hywenlv.cn

G. 面向对象
来源：http://gru.pycfn.com

================================================================================
来源：http://wwa.hesvh.cn

[G01] 定义类
来源：http://lqv.quarkkingdee.top

Py:   class User: pass
来源：http://szf.bbcook.cn

PHP:  class User {}
来源：http://kyw.iojbl.cn

JS:   class User {}
来源：http://etr.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://zdy.snrcjt.cn

Java: class User {}
来源：http://bln.gzhubu.top

Go:   type User struct { Name string }
来源：http://sho.tarul.cn

Ruby: class User; end
来源：http://mtn.xziqi.cn

C#:   class User {}
来源：http://rlr.yuxming.cn

[G02] 构造函数
来源：http://pve.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://bjt.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://ajj.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://lbv.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://kvb.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://swf.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://brl.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://mxa.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://eni.xziqi.cn

[G03] 实例属性
来源：http://qdu.yj202588.top

Py:   self.name = "x"
来源：http://fwh.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://ixk.mhx1999.top

JS:   this.name = "x";
来源：http://ffc.tian-w.cn

TS:   name: string = "x";
来源：http://aga.ydjk.org.cn

Java: private String name;
来源：http://tya.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kqs.shzxlz.cn

Ruby: @name = "x"
来源：http://imf.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://dfw.chenjidiqi.icu

[G04] 定义方法
来源：http://ylj.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://uxc.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jsh.smart0.xyz

JS:   greet() { return this.name; }
来源：http://oiq.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://mer.ivvv.top

Java: String greet() { return name; }
来源：http://wbg.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ufd.pycfn.com

Ruby: def greet; @name; end
来源：http://vjc.yonumen.top

C#:   public string Greet() => Name;
来源：http://pvc.jianghu66.top

[G05] 继承
来源：http://aou.guannengcc.top

Py:   class Admin(User): pass
来源：http://orh.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://zfo.sysykeji.top

JS:   class Admin extends User {}
来源：http://lum.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://lll.cucudq.cn

Java: class Admin extends User {}
来源：http://wog.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ccy.haohaochexian.top

Ruby: class Admin < User; end
来源：http://haq.cheryme.top

C#:   class Admin : User {}
来源：http://dfv.xziqi.cn

[G06] 重写方法
来源：http://mfc.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://yst.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://srb.yj20258.top

JS:   greet() { return "admin"; }
来源：http://unn.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://vja.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://clm.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://llg.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://zeb.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://chx.hysaishi.cn

[G07] 调用父类方法
来源：http://yfx.zhaomingkeji.xyz

Py:   super().greet()
来源：http://kyh.xuetiantiany.cn

PHP:  parent::greet();
来源：http://mfl.yj20258888.top

JS:   super.greet();
来源：http://dhl.jianghu66.top

TS:   super.greet();
来源：http://tum.hywenlv.cn

Java: super.greet();
来源：http://bfu.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://njj.xingfuxueyuan.xyz

Ruby: super
来源：http://qek.jinqigfzy.top

C#:   base.Greet();
来源：http://rfh.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://sdy.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gnn.zhixingplan.top

PHP:  public static function f() {}
来源：http://hlu.zhengqikj.top

JS:   static f() {}
来源：http://stk.epnwcf.com

TS:   static f(): void {}
来源：http://lxu.fzhhl.top

Java: static void f() {}
来源：http://tij.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://pwi.fehbvm.com

Ruby: def self.f; end
来源：http://gjn.meibo888.top

C#:   public static void F() {}
来源：http://iky.yj202588.top

[G09] 接口 / 抽象类
来源：http://hrh.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://wtp.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://cas.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://isw.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://mjm.yj202588.top

Java: interface Shape { double area(); }
来源：http://ycj.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://sfh.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dam.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://cgw.zhongyouzk.top

[G10] 访问控制
来源：http://hki.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://jqg.ctjpmb.com

PHP:  public / protected / private
来源：http://bfe.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://vuv.cheryme.top

TS:   public / protected / private
来源：http://xpc.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://mmt.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nuk.yj20258888.top

Ruby: public / protected / private
来源：http://bwl.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://frx.dashuyun.cn

[G11] getter / setter
来源：http://fjb.52xcode.cn

Py:   @property 与 @x.setter
来源：http://ggi.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gec.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://jse.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://zmp.vehdjk.com

Java: public String getName() { return name; }
来源：http://urz.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uan.havefunace.top

Ruby: attr_accessor :name
来源：http://rgo.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://qhp.fktsv.cn

[G12] 对象转字符串
来源：http://pib.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://bsj.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://xlt.vehdjk.com

JS:   toString() { return this.name; }
来源：http://ydi.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://mev.sweek.top

Java: @Override public String toString() { return name; }
来源：http://yaz.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uef.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://ndq.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://yqh.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://oik.ppjwa.cn

Py:   isinstance(u, User)
来源：http://yxe.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://fux.cheryme.top

JS:   u instanceof User
来源：http://gik.316326.xyz

TS:   u instanceof User
来源：http://jok.svipenyu.cn

Java: u instanceof User
来源：http://dlb.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nhu.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://qhd.jlsjyb.cn

C#:   u is User
来源：http://wki.vehdjk.com

[G14] 数据类 / record
来源：http://gns.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wwp.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://pyx.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ajj.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://rot.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://gzz.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://ywj.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xaa.yonumen.top

C#:   record User(string Name, int Age);
来源：http://bmd.sysykeji.top

[G15] 枚举
来源：http://nmx.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dmg.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gxb.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hqj.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hox.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://cvn.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uzr.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://evc.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zpk.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://aon.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xad.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://knh.cashguo.top

JS:   Object.entries(obj)
来源：http://hjb.jinqigufen.top

TS:   Object.entries(obj)
来源：http://jwm.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ajm.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://myh.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://ngs.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://wuj.hnxiangtu.top

================================================================================
来源：http://tov.zhixingplan.top

H. 异常与错误处理
来源：http://qyj.vqdsnc.cn

================================================================================
来源：http://oxl.ctjpmb.com

[H01] try / catch 基础
来源：http://xhh.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pnp.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://spo.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fsg.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mua.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fng.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qld.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dol.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qnx.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://zex.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://rtb.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jsp.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lmk.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vop.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://geu.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gbu.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wgy.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://chw.jyoumei.cn


<!-- 参考信息 -->