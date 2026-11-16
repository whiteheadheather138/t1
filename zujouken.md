代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pgx.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://lmt.nanxinkj.top

Py:   s.splitlines()
来源：http://sho.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://roa.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://pxp.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://fhm.hywenlv.cn

Java: s.lines().toList()
来源：http://xqz.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://wqd.chenlongwang.top

Ruby: s.lines
来源：http://aff.hfpthk.cn

C#:   s.Split('\n')
来源：http://ozu.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://gch.cdnleiting.top

Py:   if not s:
来源：http://vpi.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yzb.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cdd.havefunace.top

TS:   if (s === "") {}
来源：http://ivy.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://mmd.hnqzz.top

Go:   if s == "" {}
来源：http://owj.meibo888.top

Ruby: if s.empty?
来源：http://ieh.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xwk.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://ydg.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wau.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ccr.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xkc.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mdn.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://idp.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://ekn.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nwy.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jiu.ydzc1.top

[E22] 字节长度与字符长度
来源：http://qqs.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bsy.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ash.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gxf.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lox.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://urg.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kse.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://fed.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lph.ehwqpu.com

================================================================================
来源：http://xhw.birdmap.top

F. 文件与目录
来源：http://cad.tanke756.top

================================================================================
来源：http://prh.tianlin.xyz

[F01] 读取整个文件
来源：http://vfp.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wdl.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://iam.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pjd.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vlh.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uup.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cgd.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://opq.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://wpg.cashguo.top

[F02] 逐行读取文件
来源：http://nnt.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npv.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fua.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bir.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vzp.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nms.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tbs.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qpn.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://puh.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://ypa.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ust.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zuw.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wfg.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpt.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pkg.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ijz.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://qxu.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xtj.xylfe.cn

[F04] 追加写入文件
来源：http://dqg.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cix.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ydt.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyk.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jia.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://czp.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xkk.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yqq.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://huf.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://sgi.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xre.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://jpc.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://dnw.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://nrw.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xrc.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nik.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://toa.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://dqn.ehwqpu.com

[F06] 删除文件
来源：http://ncs.iojbl.cn

Py:   os.remove("a.txt")
来源：http://qrs.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://yeh.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://xnz.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://pji.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dke.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://wxw.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://tac.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://zfv.ybcxt.top

[F07] 创建目录（含多级）
来源：http://veu.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mkz.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hxq.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgt.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lfs.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ldr.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://szs.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lou.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://opm.svipenyu.cn

[F08] 遍历目录
来源：http://xas.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://oig.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hhs.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://vwd.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://vvk.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://niz.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ezc.yfazqb.com

Ruby: Dir.children("dir")
来源：http://fgg.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://hms.jinqigufen.top

[F09] 获取文件大小
来源：http://wwk.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://drs.cucudq.cn

PHP:  filesize("a.txt");
来源：http://xkv.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://ovu.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://dia.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://ntb.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mex.havefunace.top

Ruby: File.size("a.txt")
来源：http://nnf.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://hus.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://idz.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://inr.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lay.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://anh.vehdjk.com

TS:   path.extname("a.txt")
来源：http://srg.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kzb.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://slh.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mpw.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cgx.yonumen.top

[F11] 复制与移动文件
来源：http://jxt.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qmu.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://htu.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://skk.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvq.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jsr.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nin.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vkn.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://svi.jiagoushi.top

[F12] CSV 读写
来源：http://zmb.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lgh.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yvr.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ifk.xziqi.cn

TS:   // 同上
来源：http://qbr.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xel.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mhr.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zgg.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dso.pycfn.com

================================================================================
来源：http://aam.zhiwuduotai.top

G. 面向对象
来源：http://dkv.xinyue.icu

================================================================================
来源：http://fnq.jlsjyb.cn

[G01] 定义类
来源：http://xjy.hnqzz.top

Py:   class User: pass
来源：http://qmk.bbcook.cn

PHP:  class User {}
来源：http://jme.chenzaomai.com

JS:   class User {}
来源：http://fkt.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://llm.yanxiufei.cn

Java: class User {}
来源：http://ozl.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://mnf.cheryme.top

Ruby: class User; end
来源：http://vtf.guannengcc.top

C#:   class User {}
来源：http://qbo.pengpengdd.cyou

[G02] 构造函数
来源：http://dhh.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://yei.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://xyx.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://bfk.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://unr.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://qym.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tpd.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://iad.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://fhi.316326.xyz

[G03] 实例属性
来源：http://gsn.tianlin.xyz

Py:   self.name = "x"
来源：http://dfc.jinqigufen.top

PHP:  public string $name = "x";
来源：http://yvl.meibo888.top

JS:   this.name = "x";
来源：http://med.pycfn.com

TS:   name: string = "x";
来源：http://dxx.jinghuilouyu.cn

Java: private String name;
来源：http://son.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fjc.yuanzhike.top

Ruby: @name = "x"
来源：http://kiq.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://snr.svipenyu.cn

[G04] 定义方法
来源：http://hji.fktsv.cn

Py:   def greet(self): return self.name
来源：http://lub.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wsx.sxryk.cn

JS:   greet() { return this.name; }
来源：http://vyb.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://tqk.ivvv.top

Java: String greet() { return name; }
来源：http://syh.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://knd.xylfe.cn

Ruby: def greet; @name; end
来源：http://mvv.iojbl.cn

C#:   public string Greet() => Name;
来源：http://zam.chenjidiqi.icu

[G05] 继承
来源：http://krs.uphjek.com

Py:   class Admin(User): pass
来源：http://gxd.yfazqb.com

PHP:  class Admin extends User {}
来源：http://bxl.yj202588.top

JS:   class Admin extends User {}
来源：http://pqw.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://atk.hnqzz.top

Java: class Admin extends User {}
来源：http://hup.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ywa.jinqigufen.top

Ruby: class Admin < User; end
来源：http://xfw.zhoulong.xyz

C#:   class Admin : User {}
来源：http://jfh.feifeiyinyue.top

[G06] 重写方法
来源：http://yeh.hammf.cn

Py:   def greet(self): return "admin"
来源：http://rel.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://lvl.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://hwk.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://ahq.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://drg.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nod.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://lad.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://okw.fzhhl.top

[G07] 调用父类方法
来源：http://omi.jianghu66.top

Py:   super().greet()
来源：http://xym.shuidangran.top

PHP:  parent::greet();
来源：http://hlx.yongpay.top

JS:   super.greet();
来源：http://xfm.meibo888.top

TS:   super.greet();
来源：http://zkw.iojbl.cn

Java: super.greet();
来源：http://act.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oec.zhaomingkeji.xyz

Ruby: super
来源：http://sgc.jinqigfzy.top

C#:   base.Greet();
来源：http://mli.jinqigufen.top

[G08] 静态方法与属性
来源：http://iyr.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ekr.tianlin.xyz

PHP:  public static function f() {}
来源：http://yzy.xinyue.icu

JS:   static f() {}
来源：http://euc.chenjidiqi.icu

TS:   static f(): void {}
来源：http://jgu.snrcjt.cn

Java: static void f() {}
来源：http://yqs.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mxx.hongshengwenyu.top

Ruby: def self.f; end
来源：http://obe.guannengcc.top

C#:   public static void F() {}
来源：http://rwn.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://xwb.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://gjv.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://jrd.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ijj.0kj1m.cn

TS:   interface Shape { area(): number; }
来源：http://rqq.tanke756.top

Java: interface Shape { double area(); }
来源：http://lds.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://mie.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qak.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://mjf.svipenyu.cn

[G10] 访问控制
来源：http://pba.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://swc.xuetiantiany.cn

PHP:  public / protected / private
来源：http://avi.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://kes.jqgufenzy.top

TS:   public / protected / private
来源：http://ene.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://tbk.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ugp.yanxiufei.cn

Ruby: public / protected / private
来源：http://zja.xylfe.cn

C#:   public / protected / private / internal
来源：http://red.yanxiufei.cn

[G11] getter / setter
来源：http://fpv.epnwcf.com

Py:   @property 与 @x.setter
来源：http://bvw.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lyv.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://gue.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://spc.52xcode.cn

Java: public String getName() { return name; }
来源：http://max.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://abg.gogol.net.cn

Ruby: attr_accessor :name
来源：http://lze.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://man.cqqwz.cn

[G12] 对象转字符串
来源：http://qym.meibo888.top

Py:   def __str__(self): return self.name
来源：http://kox.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mog.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://tge.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://ymp.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://dum.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://urg.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://wxc.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://hsg.kuanghao11.cn

[G13] 判断对象类型
来源：http://bff.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://kxl.epnwcf.com

PHP:  $u instanceof User
来源：http://pcs.yj20258.top

JS:   u instanceof User
来源：http://cqu.cheryme.top

TS:   u instanceof User
来源：http://gpb.0kj1m.cn

Java: u instanceof User
来源：http://mmu.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dqv.yueranfly.top

Ruby: u.is_a?(User)
来源：http://ihz.52xcode.cn

C#:   u is User
来源：http://bjl.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://wtr.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kxj.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://btc.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://ldw.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://ajt.fengsongda.top

Java: record User(String name, int age) {}
来源：http://icb.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://bok.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jid.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://ckc.xingfuxueyuan.xyz

[G15] 枚举
来源：http://fgq.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ehz.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pjs.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nwz.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ios.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://lbf.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bba.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://itv.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aih.cheryme.top

[G16] 对象转数组 / 字典
来源：http://iey.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hxl.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://sfe.meibo888.top

JS:   Object.entries(obj)
来源：http://wbu.sufxvd.cn

TS:   Object.entries(obj)
来源：http://vvn.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ktb.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ene.epnwcf.com

Ruby: obj.instance_variables
来源：http://bgu.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://xkm.jqgfzy.top

================================================================================
来源：http://bwi.yfazqb.com

H. 异常与错误处理
来源：http://yez.zdbjq.cn

================================================================================
来源：http://mnc.cdnleiting.top

[H01] try / catch 基础
来源：http://ckj.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yww.svipenyu.cn


<!-- 参考信息 -->