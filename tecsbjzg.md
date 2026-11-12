代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://rfm.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://kww.fktsv.cn

Java: s.lines().toList()
来源：http://ayl.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://dlk.cucudq.cn

Ruby: s.lines
来源：http://glp.hnxiangtu.top

C#:   s.Split('\n')
来源：http://pzc.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://zmu.aibaodan.cn

Py:   if not s:
来源：http://koy.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eab.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kcj.sxryk.cn

TS:   if (s === "") {}
来源：http://iga.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://dby.jqgfzy.top

Go:   if s == "" {}
来源：http://dhr.shuidangran.top

Ruby: if s.empty?
来源：http://uov.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wae.fzhhl.top

[E21] 超长截断加省略号
来源：http://obx.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lhs.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jtg.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ddg.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://efq.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dde.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://wzq.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hzk.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dgi.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://kma.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ajt.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ffx.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfg.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cgr.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zrl.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fwx.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://puu.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://izz.cqqwz.cn

================================================================================
来源：http://oju.yj20258888.top

F. 文件与目录
来源：http://phb.fanxiaobao.xyz

================================================================================
来源：http://hsw.pengpengdd.cyou

[F01] 读取整个文件
来源：http://gds.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zrm.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://put.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ejh.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jmu.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xpi.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iyu.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://ifq.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://qxr.hcnkem.com

[F02] 逐行读取文件
来源：http://jni.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dhl.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pgl.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wrk.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ozs.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rxx.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zvm.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wqk.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mlv.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://qpb.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mcc.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dqv.ivvv.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://odt.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lwj.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dcb.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bhs.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://gzj.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lgp.yongpay.top

[F04] 追加写入文件
来源：http://mas.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xwe.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sdp.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bsg.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://beu.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xeu.yj20258888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jad.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hix.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jnv.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://bhn.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dzt.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://fom.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://lrw.fanxiaobao.xyz

TS:   fs.existsSync("a.txt")
来源：http://ntd.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yms.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jkw.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://rrf.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://mjc.snrcjt.cn

[F06] 删除文件
来源：http://ghl.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://qbp.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://hqz.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kqr.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nst.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uzx.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://bnb.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://aox.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://une.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://oeo.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lfn.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bvi.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwe.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ihr.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxd.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ntc.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yoc.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nlz.shangyingyoupin.top

[F08] 遍历目录
来源：http://abs.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nle.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ety.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://yeh.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://vhh.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jru.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gqk.zdqjudy.top

Ruby: Dir.children("dir")
来源：http://nvs.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://buq.guannengcc.top

[F09] 获取文件大小
来源：http://dbm.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://bqg.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://tkk.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://ehu.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://smy.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://pld.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ngd.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://hlc.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://xtw.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://dba.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yvc.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ksi.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mjk.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://vil.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ase.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hrk.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ttc.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hpd.yuxming.cn

[F11] 复制与移动文件
来源：http://ist.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yeu.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://npf.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqp.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lfl.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rms.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tfs.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kpa.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://djm.vqdsnc.cn

[F12] CSV 读写
来源：http://hgt.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zcs.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ycm.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lkg.52xcode.cn

TS:   // 同上
来源：http://dms.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hkv.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dbr.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lrw.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xuq.cashguo.top

================================================================================
来源：http://ebe.fengsongda.top

G. 面向对象
来源：http://qoy.jinqigufen.top

================================================================================
来源：http://voh.hammf.cn

[G01] 定义类
来源：http://vut.c1oappe.top

Py:   class User: pass
来源：http://pkt.feifeiyinyue.top

PHP:  class User {}
来源：http://wkm.dashuyun.cn

JS:   class User {}
来源：http://uju.uphjek.com

TS:   class User { name: string = ""; }
来源：http://hja.bbcook.cn

Java: class User {}
来源：http://kuu.zhixingplan.top

Go:   type User struct { Name string }
来源：http://uak.jiagoushi.top

Ruby: class User; end
来源：http://ihx.mhx1999.top

C#:   class User {}
来源：http://msz.jinyuanbaomall.cn

[G02] 构造函数
来源：http://one.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://vdr.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://eji.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://bwg.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://dwl.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://crl.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jxd.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://lic.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://hyp.birdmap.top

[G03] 实例属性
来源：http://uyk.zdqjudy.top

Py:   self.name = "x"
来源：http://bzm.gzhubu.top

PHP:  public string $name = "x";
来源：http://ius.jiagoushi.top

JS:   this.name = "x";
来源：http://rcb.wangshuangyany.cn

TS:   name: string = "x";
来源：http://qli.zhijiandao.cn

Java: private String name;
来源：http://vco.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nxx.snrcjt.cn

Ruby: @name = "x"
来源：http://kds.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://hvi.pengpengdd.cyou

[G04] 定义方法
来源：http://ejs.yuxming.cn

Py:   def greet(self): return self.name
来源：http://hih.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rwu.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://gsj.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://unx.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://nki.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bjh.tian-w.cn

Ruby: def greet; @name; end
来源：http://jre.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://ngz.svipenyu.cn

[G05] 继承
来源：http://kxm.ybcxt.top

Py:   class Admin(User): pass
来源：http://rof.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://qto.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://zid.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://vtl.hysaishi.cn

Java: class Admin extends User {}
来源：http://koy.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kqv.0kj1m.cn

Ruby: class Admin < User; end
来源：http://rku.hnxiangtu.top

C#:   class Admin : User {}
来源：http://ond.pycfn.com

[G06] 重写方法
来源：http://kgm.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://gui.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://iix.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://boa.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://gcd.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://ifc.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fia.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://rbc.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://xlf.andypj.xyz

[G07] 调用父类方法
来源：http://wuu.wangdashe.top

Py:   super().greet()
来源：http://fhp.ydzc1.top

PHP:  parent::greet();
来源：http://vjf.yvedp.cn

JS:   super.greet();
来源：http://lms.shangyingyoupin.top

TS:   super.greet();
来源：http://gzq.andypj.xyz

Java: super.greet();
来源：http://ilj.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kgg.wangdashe.top

Ruby: super
来源：http://dgo.pycfn.com

C#:   base.Greet();
来源：http://mbu.hammf.cn

[G08] 静态方法与属性
来源：http://thu.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://poh.dianchejie.cn

PHP:  public static function f() {}
来源：http://xcf.nanxinkj.top

JS:   static f() {}
来源：http://gun.cheryme.top

TS:   static f(): void {}
来源：http://isj.yanxiufei.cn

Java: static void f() {}
来源：http://hiu.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://crh.daria6918.cn

Ruby: def self.f; end
来源：http://nul.epnwcf.com

C#:   public static void F() {}
来源：http://cen.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://kzp.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://mwz.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dam.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ccm.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://izb.andypj.xyz

Java: interface Shape { double area(); }
来源：http://lif.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://dlw.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mhq.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://uzv.jinqigufen.top

[G10] 访问控制
来源：http://dcp.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://cpz.zhijiandao.cn

PHP:  public / protected / private
来源：http://mmr.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://dkm.sjlbkw.cn

TS:   public / protected / private
来源：http://pig.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://ubq.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://api.jqgfzy.top

Ruby: public / protected / private
来源：http://inp.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://qht.cucudq.cn

[G11] getter / setter
来源：http://atk.hcnkem.com

Py:   @property 与 @x.setter
来源：http://xgb.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ohk.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://gwq.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://ibh.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://rek.zhixingplan.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jfv.yj20258888.top

Ruby: attr_accessor :name
来源：http://zbl.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://ewl.sweek.top

[G12] 对象转字符串
来源：http://sta.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://zvz.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://iis.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://faf.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://set.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://dtu.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://baw.shuidangran.top

Ruby: def to_s; @name; end
来源：http://vaj.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://kez.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://ijr.cqqwz.cn

Py:   isinstance(u, User)
来源：http://rpy.hysaishi.cn

PHP:  $u instanceof User
来源：http://lxi.jlsjyb.cn

JS:   u instanceof User
来源：http://uxf.feifeiyinyue.top

TS:   u instanceof User
来源：http://cqw.wangdashe.top

Java: u instanceof User
来源：http://jas.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ehm.yj20258.top

Ruby: u.is_a?(User)
来源：http://ati.fehbvm.com

C#:   u is User
来源：http://jit.yonumen.top

[G14] 数据类 / record
来源：http://btj.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nmb.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ram.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mta.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://wfl.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://kbh.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://ssx.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kgn.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://lzk.zhoulong.xyz

[G15] 枚举
来源：http://nru.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mce.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zpl.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sek.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qfc.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://zrh.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://naz.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://myc.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvb.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://pgz.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vwp.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://nea.meibo888.top

JS:   Object.entries(obj)
来源：http://fvl.hammf.cn

TS:   Object.entries(obj)
来源：http://rmr.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nli.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dnx.fehbvm.com

Ruby: obj.instance_variables
来源：http://vlq.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://mcv.pycfn.com

================================================================================
来源：http://mzx.hywenlv.cn

H. 异常与错误处理
来源：http://xqe.dashuyun.cn

================================================================================
来源：http://xcp.tian-w.cn

[H01] try / catch 基础
来源：http://lbf.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ptd.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nth.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://urv.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cau.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wsu.jlsjyb.cn


<!-- 参考信息 -->