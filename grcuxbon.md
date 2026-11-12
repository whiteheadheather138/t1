代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://oby.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://hxj.hfpthk.cn

Java: s.lines().toList()
来源：http://xty.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://zkf.shzxlz.cn

Ruby: s.lines
来源：http://jgy.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://djd.yonumen.top

[E20] 判断字符串是否为空
来源：http://abf.zhixingplan.top

Py:   if not s:
来源：http://stu.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://six.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://twf.gotoacloud.top

TS:   if (s === "") {}
来源：http://myv.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://zmm.zycfv.cn

Go:   if s == "" {}
来源：http://jsw.0kj1m.cn

Ruby: if s.empty?
来源：http://tbt.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tjw.smart0.xyz

[E21] 超长截断加省略号
来源：http://yjd.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pgq.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xqc.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dcx.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://neu.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ydm.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://eyd.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gze.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://waz.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://lxm.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://szp.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pvh.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpg.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjw.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mil.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hou.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://dgq.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rbk.nwbrower.top

================================================================================
来源：http://jhp.uphjek.com

F. 文件与目录
来源：http://cxz.hammf.cn

================================================================================
来源：http://dob.316326.xyz

[F01] 读取整个文件
来源：http://vsk.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qwc.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://svj.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aen.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yxb.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gbd.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ahd.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://hvn.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://qqc.zhongyouzk.top

[F02] 逐行读取文件
来源：http://grs.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rhs.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sbj.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eoc.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sik.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pzm.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bur.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oib.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wsh.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://twz.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://izn.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xsg.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://icz.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cpk.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kaz.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://znl.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://jjo.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://edf.vehdjk.com

[F04] 追加写入文件
来源：http://ehc.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dig.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ezp.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://til.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwr.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wjp.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rpc.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://loq.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ond.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://ank.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://suv.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://sqa.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://vwa.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://vyf.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://npu.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sev.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://mds.yonumen.top

C#:   File.Exists("a.txt")
来源：http://ifg.wangshuangyany.cn

[F06] 删除文件
来源：http://mcr.tarul.cn

Py:   os.remove("a.txt")
来源：http://cav.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://drp.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://jlf.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://jpj.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gzn.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://rjf.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://xqd.yonumen.top

C#:   File.Delete("a.txt");
来源：http://uud.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://nbl.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pkv.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://khs.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://svf.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzv.epnwcf.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aoz.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oip.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wmi.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://voc.hysaishi.cn

[F08] 遍历目录
来源：http://nec.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nkb.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rbe.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://khu.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://cyy.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gnr.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://kyw.yonumen.top

Ruby: Dir.children("dir")
来源：http://rcy.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://msl.birdmap.top

[F09] 获取文件大小
来源：http://cic.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://flf.fengsongda.top

PHP:  filesize("a.txt");
来源：http://hrr.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://quf.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://evp.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://yia.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fqj.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://hrm.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://hwh.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://xra.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jdf.feifeiyinyue.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://spy.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://egp.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://qbw.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ypu.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zmi.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vyr.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kne.fzhhl.top

[F11] 复制与移动文件
来源：http://aka.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fmo.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qlc.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxj.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bqn.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yxa.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vrd.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ank.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yja.jqgfzy.top

[F12] CSV 读写
来源：http://hru.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ikb.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://khp.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://htj.yueranfly.top

TS:   // 同上
来源：http://kds.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lpl.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ftd.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://biw.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://obp.mhx1999.top

================================================================================
来源：http://rhe.0kj1m.cn

G. 面向对象
来源：http://joo.ehwqpu.com

================================================================================
来源：http://cva.haohaochexian.top

[G01] 定义类
来源：http://fsd.sweek.top

Py:   class User: pass
来源：http://pur.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://fsw.c1oappe.top

JS:   class User {}
来源：http://ayl.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://xln.zdqjudy.top

Java: class User {}
来源：http://tny.jyoumei.cn

Go:   type User struct { Name string }
来源：http://buk.ctjpmb.com

Ruby: class User; end
来源：http://bwn.jianghu66.top

C#:   class User {}
来源：http://kyr.9152youxi.cn

[G02] 构造函数
来源：http://tgq.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://jsb.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://biw.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://drx.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://voe.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://qaf.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hnn.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://xiw.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://dto.birdmap.top

[G03] 实例属性
来源：http://uqn.yanxiufei.cn

Py:   self.name = "x"
来源：http://bbj.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://czx.cheryme.top

JS:   this.name = "x";
来源：http://qcc.meibo888.top

TS:   name: string = "x";
来源：http://ijx.dianchejie.cn

Java: private String name;
来源：http://kvi.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rtj.ivvv.top

Ruby: @name = "x"
来源：http://jbv.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://kat.316326.xyz

[G04] 定义方法
来源：http://ztu.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://kpk.nanxuanxn.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jpx.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://jcb.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://xkr.yuxming.cn

Java: String greet() { return name; }
来源：http://lsq.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yma.nwbrower.top

Ruby: def greet; @name; end
来源：http://ece.xziqi.cn

C#:   public string Greet() => Name;
来源：http://mwb.haohaochexian.top

[G05] 继承
来源：http://gjc.bbcook.cn

Py:   class Admin(User): pass
来源：http://edz.iojbl.cn

PHP:  class Admin extends User {}
来源：http://pkt.iojbl.cn

JS:   class Admin extends User {}
来源：http://zep.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://wvp.tarul.cn

Java: class Admin extends User {}
来源：http://mtv.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vso.mhx1999.top

Ruby: class Admin < User; end
来源：http://bhu.316326.xyz

C#:   class Admin : User {}
来源：http://haq.yongpay.top

[G06] 重写方法
来源：http://eyk.sweek.top

Py:   def greet(self): return "admin"
来源：http://uvt.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cgm.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://hxm.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://ftq.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://jca.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ycw.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://ezg.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://ucb.redwolf501.top

[G07] 调用父类方法
来源：http://dip.chenjidiqi.icu

Py:   super().greet()
来源：http://zft.gotoacloud.top

PHP:  parent::greet();
来源：http://fsq.pengpengdd.cyou

JS:   super.greet();
来源：http://puf.jinghuilouyu.cn

TS:   super.greet();
来源：http://vhe.tarul.cn

Java: super.greet();
来源：http://rgy.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://chu.havefunace.top

Ruby: super
来源：http://sgh.yuxming.cn

C#:   base.Greet();
来源：http://cri.c1oappe.top

[G08] 静态方法与属性
来源：http://sao.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dwm.daria6918.cn

PHP:  public static function f() {}
来源：http://yif.pycfn.com

JS:   static f() {}
来源：http://huu.hammf.cn

TS:   static f(): void {}
来源：http://lpk.fanxiaobao.xyz

Java: static void f() {}
来源：http://ecy.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jao.jiagoushi.top

Ruby: def self.f; end
来源：http://mhx.ybcxt.top

C#:   public static void F() {}
来源：http://faw.xuanzx.com

[G09] 接口 / 抽象类
来源：http://vtb.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://irk.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://vym.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wuc.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://loe.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://ylz.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://oqs.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rji.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://ezz.zdqjudy.top

[G10] 访问控制
来源：http://sqk.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://qbr.uphjek.com

PHP:  public / protected / private
来源：http://arl.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://dmu.xuanzx.com

TS:   public / protected / private
来源：http://hvn.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://xqv.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fpe.daria6918.cn

Ruby: public / protected / private
来源：http://fnf.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://znf.yueranfly.top

[G11] getter / setter
来源：http://jqd.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://hnb.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ilr.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://mxp.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://hmk.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://wey.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://lvi.ppjwa.cn

Ruby: attr_accessor :name
来源：http://jwg.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://zwt.hysaishi.cn

[G12] 对象转字符串
来源：http://xww.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://wpm.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qgo.smart0.xyz

JS:   toString() { return this.name; }
来源：http://fnp.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://hcs.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://fky.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://gwy.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://wpr.tanke756.top

C#:   public override string ToString() => Name;
来源：http://gxy.chenzaomai.com

[G13] 判断对象类型
来源：http://yqr.svipenyu.cn

Py:   isinstance(u, User)
来源：http://apa.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://kha.jinqigfzy.top

JS:   u instanceof User
来源：http://lbm.shuidangran.top

TS:   u instanceof User
来源：http://ely.xinyue.icu

Java: u instanceof User
来源：http://hig.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ohj.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://mrp.hfpthk.cn

C#:   u is User
来源：http://die.zhijiandao.cn

[G14] 数据类 / record
来源：http://puh.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hpp.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://bpn.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://odx.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://iuy.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://mgw.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://giz.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ldp.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://pvn.yuanzhike.top

[G15] 枚举
来源：http://kjt.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tqa.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://kkl.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jts.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pnv.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://pwk.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dgd.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://jls.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eju.yj20258.top

[G16] 对象转数组 / 字典
来源：http://acr.xuetiantiany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lvz.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://ymh.cqqwz.cn

JS:   Object.entries(obj)
来源：http://mit.pycfn.com

TS:   Object.entries(obj)
来源：http://xsa.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ede.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ede.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://txp.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://plh.cdnleiting.top

================================================================================
来源：http://owy.cucudq.cn

H. 异常与错误处理
来源：http://xee.shzxlz.cn

================================================================================
来源：http://miv.yfazqb.com

[H01] try / catch 基础
来源：http://rjf.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vft.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://amr.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vnt.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gvk.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pqw.yanxiufei.cn


<!-- 参考信息 -->