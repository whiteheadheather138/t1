代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://arc.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ifi.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://saq.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uew.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rkp.yj202588.top

[E19] 多行文本按行拆分
来源：http://bkh.xuanzx.com

Py:   s.splitlines()
来源：http://vhg.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://txw.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://cwp.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://bot.wangdashe.top

Java: s.lines().toList()
来源：http://xon.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://qvm.yj20258.top

Ruby: s.lines
来源：http://byd.zhijiandao.cn

C#:   s.Split('\n')
来源：http://yen.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://pfs.yuxming.cn

Py:   if not s:
来源：http://yng.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wjl.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://orz.hnqzz.top

TS:   if (s === "") {}
来源：http://ond.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://kxm.xylfe.cn

Go:   if s == "" {}
来源：http://das.cucudq.cn

Ruby: if s.empty?
来源：http://yiu.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://meh.tianlin.xyz

[E21] 超长截断加省略号
来源：http://acw.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nnb.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lbs.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wrx.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wrl.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xjl.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://eca.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tzl.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jmv.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://kre.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ljb.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://caj.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fci.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qfz.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fgq.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://afs.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://fdl.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kro.jyoumei.cn

================================================================================
来源：http://pxs.tarul.cn

F. 文件与目录
来源：http://wmq.snrcjt.cn

================================================================================
来源：http://xrr.fktsv.cn

[F01] 读取整个文件
来源：http://nnu.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://smd.c1oappe.top

PHP:  file_get_contents("a.txt");
来源：http://wac.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bod.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tlc.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rta.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://los.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://dfa.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://awj.redwolf501.top

[F02] 逐行读取文件
来源：http://mwd.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ckm.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zil.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcz.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pbt.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xzx.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kdx.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hgb.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qml.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://rkc.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rdl.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://jkz.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://coq.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fah.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zmp.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gmb.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://fxu.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jwd.hnqzz.top

[F04] 追加写入文件
来源：http://jcu.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wvd.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ynd.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cut.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nlc.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xpu.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dqr.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xsy.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://spk.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://wfw.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iyv.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://kxc.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://oms.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://lxe.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tnw.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hfs.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://fow.quarkkingdee.top

C#:   File.Exists("a.txt")
来源：http://fmu.yj20258.top

[F06] 删除文件
来源：http://dmg.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://wba.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://abs.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ulz.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://gcn.redwolf501.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zod.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://mqs.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://dqm.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://ybh.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://krn.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ocg.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fyh.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zge.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yij.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jzy.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dkd.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://twv.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://inq.dashuyun.cn

[F08] 遍历目录
来源：http://ohk.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vmo.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wgg.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://blx.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://czj.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oaw.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://hiq.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://nyo.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://orx.hywenlv.cn

[F09] 获取文件大小
来源：http://uic.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://cuv.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://ojs.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://ebq.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://rgw.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://owk.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fyd.316326.xyz

Ruby: File.size("a.txt")
来源：http://pla.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://ghy.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://nkk.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yft.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jgp.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lgg.tian-w.cn

TS:   path.extname("a.txt")
来源：http://bod.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qzo.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wmz.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fxc.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jtl.nwbrower.top

[F11] 复制与移动文件
来源：http://hzf.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fnz.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ejq.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ttc.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymj.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wld.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vlm.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uap.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://whv.ehwqpu.com

[F12] CSV 读写
来源：http://vpu.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pjq.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://daq.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://thd.hongshengwenyu.top

TS:   // 同上
来源：http://qjx.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tdv.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://loi.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ngk.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zon.jiagoushi.top

================================================================================
来源：http://szb.feifeiyinyue.top

G. 面向对象
来源：http://ngi.aibaodan.cn

================================================================================
来源：http://mmi.yangfankeji.com

[G01] 定义类
来源：http://kkm.yvedp.cn

Py:   class User: pass
来源：http://jxc.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://lpl.shanyushiyangkeji.top

JS:   class User {}
来源：http://efn.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://suw.birdmap.top

Java: class User {}
来源：http://yoe.nanxinkj.top

Go:   type User struct { Name string }
来源：http://hif.316326.xyz

Ruby: class User; end
来源：http://kve.xuanzx.com

C#:   class User {}
来源：http://kyr.jqgufenzy.top

[G02] 构造函数
来源：http://tmf.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zns.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://fqv.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://tbg.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://zcb.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://nfm.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xcm.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://thd.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://ywk.bbcook.cn

[G03] 实例属性
来源：http://vub.sjlbkw.cn

Py:   self.name = "x"
来源：http://six.gogol.net.cn

PHP:  public string $name = "x";
来源：http://gpm.zdbjq.cn

JS:   this.name = "x";
来源：http://nxj.sweek.top

TS:   name: string = "x";
来源：http://rka.jinqigfzy.top

Java: private String name;
来源：http://bzy.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bpx.jinqigufen.top

Ruby: @name = "x"
来源：http://zep.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://fwd.svipenyu.cn

[G04] 定义方法
来源：http://oqu.ivvv.top

Py:   def greet(self): return self.name
来源：http://ybu.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://tua.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://knr.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://jbl.svipenyu.cn

Java: String greet() { return name; }
来源：http://wqx.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://acn.aibaodan.cn

Ruby: def greet; @name; end
来源：http://eih.birdmap.top

C#:   public string Greet() => Name;
来源：http://gbi.feifeiyinyue.top

[G05] 继承
来源：http://xsr.ehwqpu.com

Py:   class Admin(User): pass
来源：http://nvb.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://snt.hnqzz.top

JS:   class Admin extends User {}
来源：http://fft.yangfankeji.com

TS:   class Admin extends User {}
来源：http://pto.jinqigfzy.top

Java: class Admin extends User {}
来源：http://dcu.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ybc.cashguo.top

Ruby: class Admin < User; end
来源：http://xvy.zhengqikj.top

C#:   class Admin : User {}
来源：http://dnf.sysykeji.top

[G06] 重写方法
来源：http://afs.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://vqi.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ney.birdmap.top

JS:   greet() { return "admin"; }
来源：http://yep.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://tfp.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://uqj.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ebn.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://zlo.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://mlw.redwolf501.top

[G07] 调用父类方法
来源：http://irk.birdmap.top

Py:   super().greet()
来源：http://azt.sxryk.cn

PHP:  parent::greet();
来源：http://pzs.ehwqpu.com

JS:   super.greet();
来源：http://hxb.ydjk.org.cn

TS:   super.greet();
来源：http://dkq.iojbl.cn

Java: super.greet();
来源：http://ahq.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pfs.zdbjq.cn

Ruby: super
来源：http://huq.zycfv.cn

C#:   base.Greet();
来源：http://bht.aibaodan.cn

[G08] 静态方法与属性
来源：http://saa.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yzx.aibaodan.cn

PHP:  public static function f() {}
来源：http://ilb.yueranfly.top

JS:   static f() {}
来源：http://uhn.meibo888.top

TS:   static f(): void {}
来源：http://cxi.52xcode.cn

Java: static void f() {}
来源：http://jgy.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hqo.jinqigfzy.top

Ruby: def self.f; end
来源：http://yxy.yonumen.top

C#:   public static void F() {}
来源：http://gue.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://nzr.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://pbk.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://gac.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lnc.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://naz.gzhubu.top

Java: interface Shape { double area(); }
来源：http://xxu.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://ikc.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tqt.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://xdm.fzhhl.top

[G10] 访问控制
来源：http://otx.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://kbv.zhijiandao.cn

PHP:  public / protected / private
来源：http://vdp.cucudq.cn

JS:   #private 字段；其余公开
来源：http://rrn.dianchejie.cn

TS:   public / protected / private
来源：http://qyr.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://tjz.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://pqz.feifeiyinyue.top

Ruby: public / protected / private
来源：http://oga.tanke756.top

C#:   public / protected / private / internal
来源：http://ljk.chenlongwang.top

[G11] getter / setter
来源：http://hcu.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://dkm.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dey.hesvh.cn

JS:   get name() { return this._name; }
来源：http://exu.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://lhk.cqqwz.cn

Java: public String getName() { return name; }
来源：http://yee.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://whq.hnqzz.top

Ruby: attr_accessor :name
来源：http://bpz.fktsv.cn

C#:   public string Name { get; set; }
来源：http://psi.chenzaomai.com

[G12] 对象转字符串
来源：http://mdo.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://rjl.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://vvw.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://ulm.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://mss.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://jcb.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://rma.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://qra.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://wgg.wangdashe.top

[G13] 判断对象类型
来源：http://xrl.guannengcc.top

Py:   isinstance(u, User)
来源：http://zhv.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://luh.gzhubu.top

JS:   u instanceof User
来源：http://isr.kuanghao11.cn

TS:   u instanceof User
来源：http://knk.yueranfly.top

Java: u instanceof User
来源：http://yxa.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://drf.xziqi.cn

Ruby: u.is_a?(User)
来源：http://cgl.hysaishi.cn

C#:   u is User
来源：http://dvd.fzhhl.top

[G14] 数据类 / record
来源：http://ywi.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wgz.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://com.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://wyz.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://gax.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://vwq.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://edy.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mru.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://yjv.zdbjq.cn

[G15] 枚举
来源：http://fbg.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xdw.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ttj.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oht.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yuu.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://bdi.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aob.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://toj.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fux.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://hyt.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rke.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://vyo.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://hqh.shzxlz.cn

TS:   Object.entries(obj)
来源：http://hty.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vya.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wtq.zycfv.cn

Ruby: obj.instance_variables
来源：http://ctv.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://ije.nanxuanxn.top

================================================================================
来源：http://uzh.dashuyun.cn


<!-- 参考信息 -->