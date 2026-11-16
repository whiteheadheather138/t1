代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://bhd.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://dza.birdmap.top

Java: s.lines().toList()
来源：http://ymi.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://wvt.fehbvm.com

Ruby: s.lines
来源：http://hkw.shuidangran.top

C#:   s.Split('\n')
来源：http://ejf.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://cna.nanxinkj.top

Py:   if not s:
来源：http://ooc.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hta.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iym.hammf.cn

TS:   if (s === "") {}
来源：http://vlj.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://oal.feifeiyinyue.top

Go:   if s == "" {}
来源：http://bzo.hongshengwenyu.top

Ruby: if s.empty?
来源：http://mfd.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yne.fktsv.cn

[E21] 超长截断加省略号
来源：http://hqr.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yci.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tjs.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xbb.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aeo.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ziz.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://huy.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pko.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ulh.tian-w.cn

[E22] 字节长度与字符长度
来源：http://eoi.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dec.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ryu.smart0.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aov.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wyj.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hzf.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ynk.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://gmh.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aux.vqdsnc.cn

================================================================================
来源：http://zgk.yangfankeji.com

F. 文件与目录
来源：http://qla.feifeiyinyue.top

================================================================================
来源：http://xfk.chenzaomai.com

[F01] 读取整个文件
来源：http://vbo.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qku.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://rhm.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cfe.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iyb.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://gmn.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rsa.hammf.cn

Ruby: File.read("a.txt")
来源：http://ery.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://kep.ehwqpu.com

[F02] 逐行读取文件
来源：http://weg.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qnq.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ceb.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://frg.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pua.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tka.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lqr.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dth.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ffa.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://dna.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iem.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lnf.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://abf.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wcm.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ckj.yvedp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zcd.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://bix.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ykx.tarul.cn

[F04] 追加写入文件
来源：http://ufe.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lyd.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mea.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrq.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lvc.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://izu.yongpay.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hqt.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fqd.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fgn.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://dry.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qtz.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://deu.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://ccq.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://wax.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://egx.chenzaomai.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://edz.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://lzc.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://ilk.chenjidiqi.icu

[F06] 删除文件
来源：http://yzr.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://egy.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://sdo.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://mku.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://vst.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zne.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://fkp.cheryme.top

Ruby: File.delete("a.txt")
来源：http://qxb.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://jlz.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://obo.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://emm.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://spy.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kfx.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yai.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ret.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://psd.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wdt.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://env.ydjk.org.cn

[F08] 遍历目录
来源：http://zgd.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xvu.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rpe.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://wdk.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://cfa.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xpa.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bvj.jianghu66.top

Ruby: Dir.children("dir")
来源：http://kxx.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://gui.mhx1999.top

[F09] 获取文件大小
来源：http://etw.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://kjk.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://ahu.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://cww.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://aph.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://cgd.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yyu.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://iih.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://tqp.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://csi.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yis.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://abl.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iys.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://bgz.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ppn.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://izb.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://foe.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aes.gogol.net.cn

[F11] 复制与移动文件
来源：http://jrh.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hua.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kyk.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fvk.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oox.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://svx.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xom.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://chy.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://plb.fktsv.cn

[F12] CSV 读写
来源：http://rqc.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://apf.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zbh.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uoe.wangshuangyany.cn

TS:   // 同上
来源：http://arh.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://egs.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pfy.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zln.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mgx.nwbrower.top

================================================================================
来源：http://fif.feifeiyinyue.top

G. 面向对象
来源：http://fsq.feifeiyinyue.top

================================================================================
来源：http://ybn.sufxvd.cn

[G01] 定义类
来源：http://fej.yj20258.top

Py:   class User: pass
来源：http://wmn.nwbrower.top

PHP:  class User {}
来源：http://zko.pycfn.com

JS:   class User {}
来源：http://mbx.tanke756.top

TS:   class User { name: string = ""; }
来源：http://xcu.xylfe.cn

Java: class User {}
来源：http://ssg.cdnleiting.top

Go:   type User struct { Name string }
来源：http://wzc.kuanghao11.cn

Ruby: class User; end
来源：http://lbj.pycfn.com

C#:   class User {}
来源：http://ayi.fktsv.cn

[G02] 构造函数
来源：http://kia.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://dxn.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://mml.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://kmy.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://gpg.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://qex.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ckl.hywenlv.cn

Ruby: def initialize(name); @name = name; end
来源：http://zxp.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://ebj.52xcode.cn

[G03] 实例属性
来源：http://vmg.gzhubu.top

Py:   self.name = "x"
来源：http://tvj.cdnleiting.top

PHP:  public string $name = "x";
来源：http://amq.hesvh.cn

JS:   this.name = "x";
来源：http://daj.aizwys.cn

TS:   name: string = "x";
来源：http://iru.0kj1m.cn

Java: private String name;
来源：http://flw.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xwc.shuidangran.top

Ruby: @name = "x"
来源：http://skg.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://npg.hywenlv.cn

[G04] 定义方法
来源：http://fzv.meibo888.top

Py:   def greet(self): return self.name
来源：http://irz.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dcd.tian-w.cn

JS:   greet() { return this.name; }
来源：http://zuw.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://iaq.fzhhl.top

Java: String greet() { return name; }
来源：http://njl.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://dow.ybcxt.top

Ruby: def greet; @name; end
来源：http://uyx.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://hga.hfpthk.cn

[G05] 继承
来源：http://qva.cheryme.top

Py:   class Admin(User): pass
来源：http://vti.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://tbd.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://rrf.chenzaomai.com

TS:   class Admin extends User {}
来源：http://iav.meibo888.top

Java: class Admin extends User {}
来源：http://bfo.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cwq.9152youxi.cn

Ruby: class Admin < User; end
来源：http://oig.ppjwa.cn

C#:   class Admin : User {}
来源：http://kfe.yj20258.top

[G06] 重写方法
来源：http://pmb.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://vaf.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rqx.pycfn.com

JS:   greet() { return "admin"; }
来源：http://ytu.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://ugr.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://wdq.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qln.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://hlc.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://scg.jianghu66.top

[G07] 调用父类方法
来源：http://oxn.ywan-chungtsiang.top

Py:   super().greet()
来源：http://gzn.wangdashe.top

PHP:  parent::greet();
来源：http://nbz.zhengqikj.top

JS:   super.greet();
来源：http://mfy.nanxuanxn.top

TS:   super.greet();
来源：http://hru.ydjk.org.cn

Java: super.greet();
来源：http://deq.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ddu.yonumen.top

Ruby: super
来源：http://oxk.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://kgp.smart0.xyz

[G08] 静态方法与属性
来源：http://rtc.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jlg.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://ygl.c1oappe.top

JS:   static f() {}
来源：http://amt.cashguo.top

TS:   static f(): void {}
来源：http://nht.zhengqikj.top

Java: static void f() {}
来源：http://rmo.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cia.wangshuangyany.cn

Ruby: def self.f; end
来源：http://nuf.havefunace.top

C#:   public static void F() {}
来源：http://zrp.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://rvx.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://bww.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zin.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jjs.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://goq.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://izi.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://aai.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kfh.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://zng.hnxiangtu.top

[G10] 访问控制
来源：http://dpf.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://ffn.hongshengwenyu.top

PHP:  public / protected / private
来源：http://emt.ivvv.top

JS:   #private 字段；其余公开
来源：http://pbn.nanxinkj.top

TS:   public / protected / private
来源：http://nzx.316326.xyz

Java: public / protected / private / 默认包级
来源：http://vee.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://dxm.xylfe.cn

Ruby: public / protected / private
来源：http://eay.birdmap.top

C#:   public / protected / private / internal
来源：http://wlq.jqgufenzy.top

[G11] getter / setter
来源：http://ybh.yj20258888.top

Py:   @property 与 @x.setter
来源：http://dqa.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jle.jianghu66.top

JS:   get name() { return this._name; }
来源：http://yxq.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://cli.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://ofb.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qlu.yueranfly.top

Ruby: attr_accessor :name
来源：http://zgj.hcnkem.com

C#:   public string Name { get; set; }
来源：http://okk.hnqzz.top

[G12] 对象转字符串
来源：http://pav.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://dkt.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ylw.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://rbo.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://pbv.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://ytf.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://qbf.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://atb.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://dlf.sweek.top

[G13] 判断对象类型
来源：http://yiz.shzxlz.cn

Py:   isinstance(u, User)
来源：http://nqd.yueranfly.top

PHP:  $u instanceof User
来源：http://ufm.jqgufenzy.top

JS:   u instanceof User
来源：http://jkf.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://qoq.zhaomingkeji.xyz

Java: u instanceof User
来源：http://ohf.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://meh.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://ylb.havefunace.top

C#:   u is User
来源：http://pkb.jiagoushi.top

[G14] 数据类 / record
来源：http://rjj.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lxn.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://iqi.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://qas.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://ual.tanke756.top

Java: record User(String name, int age) {}
来源：http://yis.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://ybm.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kaa.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://gur.shanyushiyangkeji.top

[G15] 枚举
来源：http://zgw.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ywi.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://iwq.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vzv.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uvg.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://nwb.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uhj.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://mut.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://klb.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://zag.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qov.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://ged.hcnkem.com

JS:   Object.entries(obj)
来源：http://agc.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://cul.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rju.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://egt.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://vvt.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://lul.jiagoushi.top

================================================================================
来源：http://yse.sxryk.cn

H. 异常与错误处理
来源：http://lat.zdqjudy.top

================================================================================
来源：http://drf.sjlbkw.cn

[H01] try / catch 基础
来源：http://brc.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lzf.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sui.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kaz.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hmk.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rto.fanxiaobao.xyz


<!-- 参考信息 -->