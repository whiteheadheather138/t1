代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xfy.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rhy.zycfv.cn

TS:   if (s === "") {}
来源：http://vvu.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://usg.yongpay.top

Go:   if s == "" {}
来源：http://oke.xuetiantiany.cn

Ruby: if s.empty?
来源：http://abo.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://phy.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://noy.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kcn.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qgx.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://min.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tcc.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tpa.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://dsa.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kxz.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lwl.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://gdc.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hvh.hammf.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xbv.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://exi.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://btq.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lva.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kyu.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://dsj.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://czv.zhaomingkeji.xyz

================================================================================
来源：http://gsj.xziqi.cn

F. 文件与目录
来源：http://fck.fehbvm.com

================================================================================
来源：http://rwu.smart0.xyz

[F01] 读取整个文件
来源：http://fhn.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cpx.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://xzz.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eid.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mcx.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wvz.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ydi.hesvh.cn

Ruby: File.read("a.txt")
来源：http://btj.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://yxz.yj202588.top

[F02] 逐行读取文件
来源：http://zvk.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ntq.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tde.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cny.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfx.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bix.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rnr.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kdd.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://epl.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://tun.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tjm.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://svc.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mjl.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bkz.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fwr.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ggt.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://ybp.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://apo.pycfn.com

[F04] 追加写入文件
来源：http://iid.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ixl.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cfv.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dkj.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://inf.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iyk.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oso.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jsz.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://flj.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://duj.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bgq.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://upt.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://atq.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://uim.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dyh.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cvg.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://fje.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://ywx.shuidangran.top

[F06] 删除文件
来源：http://vsu.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://cxr.sysykeji.top

PHP:  unlink("a.txt");
来源：http://yoj.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://ayt.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://wsn.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ueh.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://ulb.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://yrv.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://shn.zycfv.cn

[F07] 创建目录（含多级）
来源：http://pqm.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uzw.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qhh.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vig.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xdt.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zsh.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zcd.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pau.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://orw.tanke756.top

[F08] 遍历目录
来源：http://yte.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ktu.svipenyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mpv.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://oyk.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://sgs.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wao.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fgw.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://haz.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://kvq.yuxming.cn

[F09] 获取文件大小
来源：http://dai.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://fwa.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://hmn.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://psk.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://qxc.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://zso.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kag.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://nwc.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://tcx.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://ilp.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tmx.yj202588.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bcp.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kup.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://yig.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hcx.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vet.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xtn.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ytk.sweek.top

[F11] 复制与移动文件
来源：http://shx.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://stp.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ndk.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wwa.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fpi.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sgh.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sle.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hjt.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jew.zhongyouzk.top

[F12] CSV 读写
来源：http://eka.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://poa.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ppk.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bwp.ydzc1.top

TS:   // 同上
来源：http://trs.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kpi.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pui.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gbm.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://egu.jiagoushi.top

================================================================================
来源：http://xbb.aizwys.cn

G. 面向对象
来源：http://enq.haohaochexian.top

================================================================================
来源：http://pib.gogol.net.cn

[G01] 定义类
来源：http://dvy.zhoulong.xyz

Py:   class User: pass
来源：http://pbl.gzhubu.top

PHP:  class User {}
来源：http://wha.mhx1999.top

JS:   class User {}
来源：http://uaj.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://chj.yuxming.cn

Java: class User {}
来源：http://qkr.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://lhg.jyoumei.cn

Ruby: class User; end
来源：http://whf.ctjpmb.com

C#:   class User {}
来源：http://rhe.kuanghao11.cn

[G02] 构造函数
来源：http://qov.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ggd.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://smk.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://rgq.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://mkc.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://fei.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gsk.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://jdl.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://xjx.jinyuanbaomall.cn

[G03] 实例属性
来源：http://dok.xziqi.cn

Py:   self.name = "x"
来源：http://nei.yueranfly.top

PHP:  public string $name = "x";
来源：http://yxs.mhx1999.top

JS:   this.name = "x";
来源：http://biy.sjlbkw.cn

TS:   name: string = "x";
来源：http://knb.hesvh.cn

Java: private String name;
来源：http://wpu.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://waa.nanxinkj.top

Ruby: @name = "x"
来源：http://pcu.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://zit.aibaodan.cn

[G04] 定义方法
来源：http://qjf.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://pfy.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://tsy.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://jcl.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://nbj.yfazqb.com

Java: String greet() { return name; }
来源：http://btw.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://vqm.ybcxt.top

Ruby: def greet; @name; end
来源：http://gnk.tian-w.cn

C#:   public string Greet() => Name;
来源：http://lml.fktsv.cn

[G05] 继承
来源：http://nos.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://fxv.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://tbu.hammf.cn

JS:   class Admin extends User {}
来源：http://srq.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://vgi.redwolf501.top

Java: class Admin extends User {}
来源：http://mvx.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdb.shzxlz.cn

Ruby: class Admin < User; end
来源：http://kmy.quarkkingdee.top

C#:   class Admin : User {}
来源：http://pql.snrcjt.cn

[G06] 重写方法
来源：http://pvm.cashguo.top

Py:   def greet(self): return "admin"
来源：http://uoz.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fis.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://jgy.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://zem.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://jky.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://quy.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://gnw.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://grp.ydzc1.top

[G07] 调用父类方法
来源：http://ozk.cashguo.top

Py:   super().greet()
来源：http://tan.aizwys.cn

PHP:  parent::greet();
来源：http://tzo.yongpay.top

JS:   super.greet();
来源：http://pjo.yongpay.top

TS:   super.greet();
来源：http://htk.jqgufenzy.top

Java: super.greet();
来源：http://xch.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kxr.ywan-chungtsiang.top

Ruby: super
来源：http://vtj.yfazqb.com

C#:   base.Greet();
来源：http://sjk.tian-w.cn

[G08] 静态方法与属性
来源：http://arj.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mbs.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://kum.andypj.xyz

JS:   static f() {}
来源：http://dfi.yj20258.top

TS:   static f(): void {}
来源：http://fmc.hcnkem.com

Java: static void f() {}
来源：http://phr.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://kxw.bjfxy.top

Ruby: def self.f; end
来源：http://hre.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://zdc.tian-w.cn

[G09] 接口 / 抽象类
来源：http://ssq.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://thy.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://chl.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ghp.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://xiw.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://iur.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://kcq.gaohongyu789.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yuz.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://sbk.gogol.net.cn

[G10] 访问控制
来源：http://ihs.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://pht.ctjpmb.com

PHP:  public / protected / private
来源：http://mrr.kuanghao11.cn

JS:   #private 字段；其余公开
来源：http://vlt.sxryk.cn

TS:   public / protected / private
来源：http://nmz.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://uhw.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tss.tian-w.cn

Ruby: public / protected / private
来源：http://qtw.redwolf501.top

C#:   public / protected / private / internal
来源：http://ayo.epnwcf.com

[G11] getter / setter
来源：http://bix.hcnkem.com

Py:   @property 与 @x.setter
来源：http://vjc.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xvq.bbcook.cn

JS:   get name() { return this._name; }
来源：http://bsu.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://jwm.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://qrh.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ycd.shzxlz.cn

Ruby: attr_accessor :name
来源：http://rxx.hnqzz.top

C#:   public string Name { get; set; }
来源：http://zyj.nanxuanxn.top

[G12] 对象转字符串
来源：http://bap.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://flh.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://jdt.daxiang520.top

JS:   toString() { return this.name; }
来源：http://pja.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://mdr.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://cin.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://izl.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://rvj.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://ofr.yj20258.top

[G13] 判断对象类型
来源：http://uik.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://xkk.yongpay.top

PHP:  $u instanceof User
来源：http://hhf.vqdsnc.cn

JS:   u instanceof User
来源：http://arr.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://bmq.zhijiandao.cn

Java: u instanceof User
来源：http://avw.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dyj.uphjek.com

Ruby: u.is_a?(User)
来源：http://mef.daxiang520.top

C#:   u is User
来源：http://keo.aizwys.cn

[G14] 数据类 / record
来源：http://ega.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dho.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://ojw.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://fuk.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://hfe.hesvh.cn

Java: record User(String name, int age) {}
来源：http://ebd.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://dhf.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vgg.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://qzs.yueranfly.top

[G15] 枚举
来源：http://ehd.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rkz.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wsa.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://prk.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qcd.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://duz.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uke.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://wjk.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ajo.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://pjl.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nzr.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://swt.tarul.cn

JS:   Object.entries(obj)
来源：http://ebd.meibo888.top

TS:   Object.entries(obj)
来源：http://leo.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ghv.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xhk.yvedp.cn

Ruby: obj.instance_variables
来源：http://sbf.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://aen.shangyingyoupin.top

================================================================================
来源：http://zse.yueranfly.top

H. 异常与错误处理
来源：http://aww.yuxming.cn

================================================================================
来源：http://kiz.zhijiandao.cn

[H01] try / catch 基础
来源：http://phz.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jme.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yxg.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://agb.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aep.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://etj.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://irg.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vhp.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dcw.ybcxt.top

[H02] finally / ensure 收尾
来源：http://hmd.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xqs.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ist.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fse.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uto.chenzaomai.com


<!-- 参考信息 -->