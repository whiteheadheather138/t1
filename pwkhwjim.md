代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://xve.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://mgn.yuxming.cn

Java: s.lines().toList()
来源：http://myo.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://bud.shuidangran.top

Ruby: s.lines
来源：http://cxn.yj20258888.top

C#:   s.Split('\n')
来源：http://ujr.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://hcc.xinyue.icu

Py:   if not s:
来源：http://mpa.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ibe.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sxs.ivvv.top

TS:   if (s === "") {}
来源：http://qom.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://mkg.52xcode.cn

Go:   if s == "" {}
来源：http://gbv.jiagoushi.top

Ruby: if s.empty?
来源：http://jam.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://paz.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://can.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fik.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://unc.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wvq.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yaj.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xaj.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://pdk.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dtd.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yfc.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://cuh.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gjm.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jhx.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sdn.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tue.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oyn.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ybp.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://ihp.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cnk.feifeiyinyue.top

================================================================================
来源：http://cer.jinghuilouyu.cn

F. 文件与目录
来源：http://zcg.feifeiyinyue.top

================================================================================
来源：http://xcv.zhijiandao.cn

[F01] 读取整个文件
来源：http://egq.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ykk.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://dfp.ybcxt.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xtm.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ila.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gqt.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ivh.shuidangran.top

Ruby: File.read("a.txt")
来源：http://mlt.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://quk.zhengqikj.top

[F02] 逐行读取文件
来源：http://ciy.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fqe.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dhr.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lyw.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yom.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ice.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gtn.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bwl.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qus.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://red.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vao.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jva.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vba.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yvr.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rvx.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kvj.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://tqz.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ksj.hysaishi.cn

[F04] 追加写入文件
来源：http://ujp.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mdd.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bzz.cdnleiting.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yqi.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tgw.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eos.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nte.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://icl.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hyq.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://leh.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lja.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://grq.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://lsb.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://nrm.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://phn.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lit.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://itg.ivvv.top

C#:   File.Exists("a.txt")
来源：http://aky.redwolf501.top

[F06] 删除文件
来源：http://bax.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://ikt.xuanzx.com

PHP:  unlink("a.txt");
来源：http://bfu.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://sjq.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://cho.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fmd.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://gut.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://byz.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://lsm.yueranfly.top

[F07] 创建目录（含多级）
来源：http://rvw.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://irz.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dly.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sbv.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zme.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lfh.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ktf.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ifg.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xiq.fzhhl.top

[F08] 遍历目录
来源：http://hgr.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ekg.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tpo.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://vyh.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://uhk.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ztu.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jvc.sweek.top

Ruby: Dir.children("dir")
来源：http://gys.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://hdm.ppjwa.cn

[F09] 获取文件大小
来源：http://rqs.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://nao.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://bco.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://loq.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://ehw.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tju.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://usr.meibo888.top

Ruby: File.size("a.txt")
来源：http://oox.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://rsj.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://ihe.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jpc.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kqx.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rlf.fzhhl.top

TS:   path.extname("a.txt")
来源：http://dmb.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kwl.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bjf.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xam.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xgc.uphjek.com

[F11] 复制与移动文件
来源：http://yxs.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ujr.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fyo.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jth.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etp.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gnv.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mgr.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qpk.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qwv.yfazqb.com

[F12] CSV 读写
来源：http://jja.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oep.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ttn.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://smw.316326.xyz

TS:   // 同上
来源：http://jig.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://grp.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nra.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ndz.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://clu.fzhhl.top

================================================================================
来源：http://xto.tianlin.xyz

G. 面向对象
来源：http://lhk.cqqwz.cn

================================================================================
来源：http://mzx.yj202588.top

[G01] 定义类
来源：http://tho.cdnleiting.top

Py:   class User: pass
来源：http://xfn.zdqjudy.top

PHP:  class User {}
来源：http://cbi.ydzc1.top

JS:   class User {}
来源：http://oqt.tarul.cn

TS:   class User { name: string = ""; }
来源：http://yve.hcnkem.com

Java: class User {}
来源：http://uhg.yj20258.top

Go:   type User struct { Name string }
来源：http://fou.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://jjf.ydjk.org.cn

C#:   class User {}
来源：http://rad.quarkkingdee.top

[G02] 构造函数
来源：http://poq.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://mfi.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://xfd.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://edr.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://xcl.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://qvq.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xut.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://wcd.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://rbi.yj202588.top

[G03] 实例属性
来源：http://jsf.jianghu66.top

Py:   self.name = "x"
来源：http://exr.jyoumei.cn

PHP:  public string $name = "x";
来源：http://bhd.quarkkingdee.top

JS:   this.name = "x";
来源：http://wli.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://csq.ywan-chungtsiang.top

Java: private String name;
来源：http://tse.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cqr.sysykeji.top

Ruby: @name = "x"
来源：http://jot.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://tcb.yuanzhike.top

[G04] 定义方法
来源：http://qhh.sysykeji.top

Py:   def greet(self): return self.name
来源：http://zmg.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jsk.yj20258.top

JS:   greet() { return this.name; }
来源：http://osf.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://chr.cucudq.cn

Java: String greet() { return name; }
来源：http://wkj.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://kha.9152youxi.cn

Ruby: def greet; @name; end
来源：http://ffg.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://akt.zhixingplan.top

[G05] 继承
来源：http://sju.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://wyb.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://lqe.gogol.net.cn

JS:   class Admin extends User {}
来源：http://sjl.dashuyun.cn

TS:   class Admin extends User {}
来源：http://uej.smart0.xyz

Java: class Admin extends User {}
来源：http://zlw.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ntm.zdbjq.cn

Ruby: class Admin < User; end
来源：http://waj.cheryme.top

C#:   class Admin : User {}
来源：http://hir.zycfv.cn

[G06] 重写方法
来源：http://zyj.havefunace.top

Py:   def greet(self): return "admin"
来源：http://ejt.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wen.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://pdc.tanke756.top

TS:   greet(): string { return "admin"; }
来源：http://svh.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://ior.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ogo.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://ibd.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://ibf.sysykeji.top

[G07] 调用父类方法
来源：http://grn.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://dbh.jqgufenzy.top

PHP:  parent::greet();
来源：http://erc.hywenlv.cn

JS:   super.greet();
来源：http://gmy.ctjpmb.com

TS:   super.greet();
来源：http://pbi.hongshengwenyu.top

Java: super.greet();
来源：http://pwf.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qxs.zdbjq.cn

Ruby: super
来源：http://vvf.gzhubu.top

C#:   base.Greet();
来源：http://pdj.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://bjn.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zto.yueranfly.top

PHP:  public static function f() {}
来源：http://wir.wangdashe.top

JS:   static f() {}
来源：http://tku.uphjek.com

TS:   static f(): void {}
来源：http://rei.yj202588.top

Java: static void f() {}
来源：http://pbj.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://riy.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://ykf.gzhubu.top

C#:   public static void F() {}
来源：http://vcm.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://wah.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://rei.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cfs.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://icn.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://xmh.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://ysc.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://trr.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bjz.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://eug.uphjek.com

[G10] 访问控制
来源：http://utb.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://wvd.hongshengwenyu.top

PHP:  public / protected / private
来源：http://ppy.hnxiangtu.top

JS:   #private 字段；其余公开
来源：http://urv.zdbjq.cn

TS:   public / protected / private
来源：http://ntw.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://jrj.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://cox.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://frg.vehdjk.com

C#:   public / protected / private / internal
来源：http://qvb.chenzaomai.com

[G11] getter / setter
来源：http://hxa.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://kyt.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cjg.xinyue.icu

JS:   get name() { return this._name; }
来源：http://dei.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://rzi.zycfv.cn

Java: public String getName() { return name; }
来源：http://hqh.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tgv.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://tyg.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://zjp.cqqwz.cn

[G12] 对象转字符串
来源：http://zis.uphjek.com

Py:   def __str__(self): return self.name
来源：http://bbw.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://imk.yueranfly.top

JS:   toString() { return this.name; }
来源：http://ubk.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://ejv.yanxiufei.cn

Java: @Override public String toString() { return name; }
来源：http://rlh.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://puk.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://lok.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://pdf.mhx1999.top

[G13] 判断对象类型
来源：http://kxf.chenzaomai.com

Py:   isinstance(u, User)
来源：http://ipc.jiagoushi.top

PHP:  $u instanceof User
来源：http://esh.pycfn.com

JS:   u instanceof User
来源：http://zhf.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ueb.zhixingplan.top

Java: u instanceof User
来源：http://sbe.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://gmg.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://auh.snrcjt.cn

C#:   u is User
来源：http://cez.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://sjt.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yxx.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://vcp.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://ztw.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://cxh.shuidangran.top

Java: record User(String name, int age) {}
来源：http://tvo.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://ukt.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://enh.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://fgi.gaohongyu789.top

[G15] 枚举
来源：http://tmc.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jma.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ath.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rxo.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://odk.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://ago.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://apt.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://zuu.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aaj.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://etg.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fih.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://ccv.shuidangran.top

JS:   Object.entries(obj)
来源：http://cee.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://hsj.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dqo.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ima.cheryme.top

Ruby: obj.instance_variables
来源：http://zht.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://fdf.tianlin.xyz

================================================================================
来源：http://rax.gotoacloud.top

H. 异常与错误处理
来源：http://lyw.ybcxt.top

================================================================================
来源：http://fmn.c1oappe.top

[H01] try / catch 基础
来源：http://xbg.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zga.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ynt.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bsb.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ndg.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://klj.yuanzhike.top


<!-- 参考信息 -->