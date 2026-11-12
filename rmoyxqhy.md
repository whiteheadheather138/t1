代发 wailian999

Ruby: s.lines
来源：http://slb.fzhhl.top

C#:   s.Split('\n')
来源：http://pox.vehdjk.com

[E20] 判断字符串是否为空
来源：http://ozy.0kj1m.cn

Py:   if not s:
来源：http://sbl.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tgf.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hlr.nwbrower.top

TS:   if (s === "") {}
来源：http://yhu.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://zwj.ppjwa.cn

Go:   if s == "" {}
来源：http://oxl.xinyue.icu

Ruby: if s.empty?
来源：http://pwq.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vkt.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://uue.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ugz.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rux.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cvg.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yyg.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qdf.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://mji.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cyv.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bcc.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://qoj.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hmc.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snw.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrx.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qew.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dca.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yyr.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://lrx.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jds.cqqwz.cn

================================================================================
来源：http://vig.shanyushiyangtech.top

F. 文件与目录
来源：http://bme.jiagoushi.top

================================================================================
来源：http://bfm.zdbjq.cn

[F01] 读取整个文件
来源：http://czg.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rbq.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://xct.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dok.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hhv.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://srg.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gjo.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://phz.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://llk.ctjpmb.com

[F02] 逐行读取文件
来源：http://jix.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pnx.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hij.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mll.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vzg.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xgx.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tih.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://syk.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ili.pycfn.com

[F03] 写入文件（覆盖）
来源：http://kvm.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ngp.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://czv.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vic.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdh.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pbm.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tty.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://heg.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://npm.gzhubu.top

[F04] 追加写入文件
来源：http://xky.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bsj.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dbj.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hiu.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bpy.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ldj.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xtk.sysykeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kqa.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zjm.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://naw.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dxw.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://wyd.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://hxt.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://gjt.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://swd.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eoj.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://qkl.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://hid.shzxlz.cn

[F06] 删除文件
来源：http://pnx.smart0.xyz

Py:   os.remove("a.txt")
来源：http://loa.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://pqh.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xmi.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://jgd.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vai.tanke756.top

Go:   os.Remove("a.txt")
来源：http://cnk.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://bjf.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://eqi.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://hnf.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdt.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kwq.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mir.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://esv.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://opw.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fwu.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oqo.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wub.zdbjq.cn

[F08] 遍历目录
来源：http://zzg.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pqr.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lqc.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://gjv.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://grx.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ylw.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vhx.cucudq.cn

Ruby: Dir.children("dir")
来源：http://bxi.aibaodan.cn

C#:   Directory.GetFiles("dir")
来源：http://wcv.yanxiufei.cn

[F09] 获取文件大小
来源：http://hhl.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://mpf.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://ann.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://qju.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://rhd.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://hwc.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pjz.birdmap.top

Ruby: File.size("a.txt")
来源：http://nvi.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://azo.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://dva.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jal.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bsc.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rwk.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://pad.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://awf.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://thq.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dgw.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nve.c1oappe.top

[F11] 复制与移动文件
来源：http://ewa.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yjj.xylfe.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ytr.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jwl.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kny.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ugn.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dab.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oov.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vzn.yuxming.cn

[F12] CSV 读写
来源：http://jyu.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jtv.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sbx.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yih.yueranfly.top

TS:   // 同上
来源：http://mfz.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://srf.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://evf.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ipj.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xjk.jqgfzy.top

================================================================================
来源：http://bal.zhijiandao.cn

G. 面向对象
来源：http://eqx.sweek.top

================================================================================
来源：http://ezi.chenzaomai.com

[G01] 定义类
来源：http://dgs.cucudq.cn

Py:   class User: pass
来源：http://akf.chenjidiqi.icu

PHP:  class User {}
来源：http://buo.pycfn.com

JS:   class User {}
来源：http://slw.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://lhr.jinqigufen.top

Java: class User {}
来源：http://jnf.fengsongda.top

Go:   type User struct { Name string }
来源：http://bkr.feifeiyinyue.top

Ruby: class User; end
来源：http://kbm.ivvv.top

C#:   class User {}
来源：http://cqc.aizwys.cn

[G02] 构造函数
来源：http://yjq.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://gwv.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://ihl.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://npv.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://aiz.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://dki.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iwu.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://pcv.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://gha.wangdashe.top

[G03] 实例属性
来源：http://eim.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://jao.andypj.xyz

PHP:  public string $name = "x";
来源：http://jfd.yfazqb.com

JS:   this.name = "x";
来源：http://npt.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://btk.svipenyu.cn

Java: private String name;
来源：http://dvv.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://plg.xinyue.icu

Ruby: @name = "x"
来源：http://fnk.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://yvt.0kj1m.cn

[G04] 定义方法
来源：http://xko.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://isi.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://blm.hnqzz.top

JS:   greet() { return this.name; }
来源：http://igb.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://frg.daxiang520.top

Java: String greet() { return name; }
来源：http://usg.jiagoushi.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ffn.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://xnj.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://moq.havefunace.top

[G05] 继承
来源：http://gva.chenlongwang.top

Py:   class Admin(User): pass
来源：http://lgh.yfazqb.com

PHP:  class Admin extends User {}
来源：http://kjz.jinqigufen.top

JS:   class Admin extends User {}
来源：http://ape.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://qra.316326.xyz

Java: class Admin extends User {}
来源：http://zhx.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zee.xinyue.icu

Ruby: class Admin < User; end
来源：http://rxs.svipenyu.cn

C#:   class Admin : User {}
来源：http://dmk.xylfe.cn

[G06] 重写方法
来源：http://pnu.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://olw.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://llx.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://hrp.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://dpv.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://zpa.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kqt.uphjek.com

Ruby: def greet; "admin"; end
来源：http://yyf.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://aev.xuanzx.com

[G07] 调用父类方法
来源：http://abk.svipenyu.cn

Py:   super().greet()
来源：http://wer.jinqigufen.top

PHP:  parent::greet();
来源：http://vrg.haohaochexian.top

JS:   super.greet();
来源：http://ljn.ydzc1.top

TS:   super.greet();
来源：http://iwq.hfpthk.cn

Java: super.greet();
来源：http://gfs.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kxu.shuidangran.top

Ruby: super
来源：http://ffj.yueranfly.top

C#:   base.Greet();
来源：http://qgy.zhoulong.xyz

[G08] 静态方法与属性
来源：http://vbz.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lhj.quarkkingdee.top

PHP:  public static function f() {}
来源：http://iim.yuxming.cn

JS:   static f() {}
来源：http://nnz.vehdjk.com

TS:   static f(): void {}
来源：http://rer.shzxlz.cn

Java: static void f() {}
来源：http://ver.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://llp.meibo888.top

Ruby: def self.f; end
来源：http://qcw.jinqigufen.top

C#:   public static void F() {}
来源：http://ryc.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://aet.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://tkj.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://rhc.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://fyj.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://ulx.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://lxd.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://wxf.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fyb.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://ldd.shzxlz.cn

[G10] 访问控制
来源：http://ahg.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://bhh.epnwcf.com

PHP:  public / protected / private
来源：http://hez.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://msg.shuidangran.top

TS:   public / protected / private
来源：http://cvs.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://zmv.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wzt.cheryme.top

Ruby: public / protected / private
来源：http://unz.wangdashe.top

C#:   public / protected / private / internal
来源：http://rvt.meibo888.top

[G11] getter / setter
来源：http://pjn.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://qgj.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://snc.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://rqm.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://qlk.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://nws.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zlm.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://nre.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://rvl.andypj.xyz

[G12] 对象转字符串
来源：http://yal.ivvv.top

Py:   def __str__(self): return self.name
来源：http://lxs.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://afd.yj20258888.top

JS:   toString() { return this.name; }
来源：http://ixp.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://bbf.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://cwc.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://qvo.yuxming.cn

Ruby: def to_s; @name; end
来源：http://qrl.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://egg.smart0.xyz

[G13] 判断对象类型
来源：http://gag.yongpay.top

Py:   isinstance(u, User)
来源：http://xgq.jlsjyb.cn

PHP:  $u instanceof User
来源：http://kon.bjfxy.top

JS:   u instanceof User
来源：http://wca.ydjk.org.cn

TS:   u instanceof User
来源：http://wbh.sufxvd.cn

Java: u instanceof User
来源：http://xpu.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pdw.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://qwc.yangfankeji.com

C#:   u is User
来源：http://vmr.gogol.net.cn

[G14] 数据类 / record
来源：http://rxb.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ocq.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://nuj.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://orz.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://gxp.yvedp.cn

Java: record User(String name, int age) {}
来源：http://udk.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://bon.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yrf.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://bev.yueranfly.top

[G15] 枚举
来源：http://yku.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ivk.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dbc.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dnc.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://axa.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://mld.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fac.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://qdn.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yvt.yj202588.top

[G16] 对象转数组 / 字典
来源：http://bgr.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zus.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://khy.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://mdi.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://dex.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dnz.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://liu.chenlongwang.top

Ruby: obj.instance_variables
来源：http://zqk.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pcm.andypj.xyz

================================================================================
来源：http://dww.nwbrower.top

H. 异常与错误处理
来源：http://rvv.tarul.cn

================================================================================
来源：http://fcz.gzhubu.top

[H01] try / catch 基础
来源：http://icm.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sdf.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ivi.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mjb.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://laq.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vjn.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nsk.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://trs.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cbe.smart0.xyz

[H02] finally / ensure 收尾
来源：http://noa.hammf.cn


<!-- 参考信息 -->