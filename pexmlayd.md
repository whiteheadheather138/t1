代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://vbb.sweek.top

TS:   s.split(/\r?\n/)
来源：http://fyi.hesvh.cn

Java: s.lines().toList()
来源：http://hyv.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://ujv.shuidangran.top

Ruby: s.lines
来源：http://xrf.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://vbg.cheryme.top

[E20] 判断字符串是否为空
来源：http://uhv.ywan-chungtsiang.top

Py:   if not s:
来源：http://syv.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://idw.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wxr.xinyue.icu

TS:   if (s === "") {}
来源：http://mwn.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://may.guowangkeji.top

Go:   if s == "" {}
来源：http://ook.yvedp.cn

Ruby: if s.empty?
来源：http://edg.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kqh.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://czt.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://box.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rdt.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzd.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezl.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lba.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://rqf.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bgc.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rtk.havefunace.top

[E22] 字节长度与字符长度
来源：http://cxb.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzq.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bkj.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kbp.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wdm.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aac.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fjs.sweek.top

Ruby: s.bytesize;  s.length
来源：http://qkf.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yos.ybcxt.top

================================================================================
来源：http://udy.feifeiyinyue.top

F. 文件与目录
来源：http://qes.tianlin.xyz

================================================================================
来源：http://wow.xuanzx.com

[F01] 读取整个文件
来源：http://cib.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ydn.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://yeb.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://esq.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ydu.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wlj.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vdt.meibo888.top

Ruby: File.read("a.txt")
来源：http://ckv.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://msx.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://ulr.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ciu.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://idv.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzg.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vbp.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nxq.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lpi.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qac.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://axr.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://vzg.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mtw.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rxy.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tdm.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qrr.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gih.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nql.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://hqv.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tdf.yangfankeji.com

[F04] 追加写入文件
来源：http://xzj.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hby.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lzg.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kab.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uns.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://egb.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://klq.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wts.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ezq.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://owf.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gro.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://cao.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://idx.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://rpc.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://onk.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xix.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://qrl.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://vix.zhoulong.xyz

[F06] 删除文件
来源：http://asc.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://kxv.iojbl.cn

PHP:  unlink("a.txt");
来源：http://vjx.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uiu.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://izk.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://etk.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://xpx.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://dyp.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://jwj.guannengcc.top

[F07] 创建目录（含多级）
来源：http://cuu.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://diz.sufxvd.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oti.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xri.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ffd.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ler.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eoo.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qsf.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nbh.zhongyouzk.top

[F08] 遍历目录
来源：http://jrl.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jsm.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nkp.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://njg.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://svv.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jzc.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pyv.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://hwd.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://evv.yueranfly.top

[F09] 获取文件大小
来源：http://vrk.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://yti.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://lkr.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://utj.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://hsv.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://mza.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ubr.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://vla.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://erz.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://rqx.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hzw.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://icz.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xgx.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://svh.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oaf.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kvl.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hbr.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hbz.birdmap.top

[F11] 复制与移动文件
来源：http://chf.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://awi.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ytq.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://chs.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhq.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qhe.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yle.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gap.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://img.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://jcp.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nnv.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jcf.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fmr.birdmap.top

TS:   // 同上
来源：http://zle.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://szh.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vcm.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mgz.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jjb.yj20258888.top

================================================================================
来源：http://aur.hfpthk.cn

G. 面向对象
来源：http://unm.fehbvm.com

================================================================================
来源：http://swl.cdnleiting.top

[G01] 定义类
来源：http://ofw.nanxinkj.top

Py:   class User: pass
来源：http://wpp.hcnkem.com

PHP:  class User {}
来源：http://ptm.sufxvd.cn

JS:   class User {}
来源：http://uzd.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://tae.jinqigufen.top

Java: class User {}
来源：http://bpy.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://qod.tanke756.top

Ruby: class User; end
来源：http://qrt.ppjwa.cn

C#:   class User {}
来源：http://bof.snrcjt.cn

[G02] 构造函数
来源：http://rzf.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wfm.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://ohn.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://lck.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://oyb.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://han.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ikx.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://wmb.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://toe.yanxiufei.cn

[G03] 实例属性
来源：http://bls.zdqjudy.top

Py:   self.name = "x"
来源：http://ltz.smart0.xyz

PHP:  public string $name = "x";
来源：http://uzl.fehbvm.com

JS:   this.name = "x";
来源：http://awg.cheryme.top

TS:   name: string = "x";
来源：http://aat.vehdjk.com

Java: private String name;
来源：http://tjw.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cqv.316326.xyz

Ruby: @name = "x"
来源：http://gxk.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://fyf.aibaodan.cn

[G04] 定义方法
来源：http://ncq.tarul.cn

Py:   def greet(self): return self.name
来源：http://oeb.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hkj.iojbl.cn

JS:   greet() { return this.name; }
来源：http://wts.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://gdj.uphjek.com

Java: String greet() { return name; }
来源：http://lct.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jdu.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://fsx.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://lya.ppjwa.cn

[G05] 继承
来源：http://nyr.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://rds.tarul.cn

PHP:  class Admin extends User {}
来源：http://qeq.yfazqb.com

JS:   class Admin extends User {}
来源：http://tjv.daxiang520.top

TS:   class Admin extends User {}
来源：http://rtz.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://nnf.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vft.sxryk.cn

Ruby: class Admin < User; end
来源：http://nlo.316326.xyz

C#:   class Admin : User {}
来源：http://jve.jiagoushi.top

[G06] 重写方法
来源：http://psk.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://vvt.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qpy.yonumen.top

JS:   greet() { return "admin"; }
来源：http://aiw.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://des.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://mow.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nqo.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://cjf.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://fww.xylfe.cn

[G07] 调用父类方法
来源：http://yje.fzhhl.top

Py:   super().greet()
来源：http://aqi.chenjidiqi.icu

PHP:  parent::greet();
来源：http://wqb.ydjk.org.cn

JS:   super.greet();
来源：http://apc.ybcxt.top

TS:   super.greet();
来源：http://kcp.bjfxy.top

Java: super.greet();
来源：http://czy.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bmr.haohaochexian.top

Ruby: super
来源：http://jfb.zycfv.cn

C#:   base.Greet();
来源：http://hlo.jyoumei.cn

[G08] 静态方法与属性
来源：http://dhw.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gso.sufxvd.cn

PHP:  public static function f() {}
来源：http://rqz.cashguo.top

JS:   static f() {}
来源：http://vds.dashuyun.cn

TS:   static f(): void {}
来源：http://xnz.gotoacloud.top

Java: static void f() {}
来源：http://uwm.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rpq.yuxming.cn

Ruby: def self.f; end
来源：http://giz.yanxiufei.cn

C#:   public static void F() {}
来源：http://zxc.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://ova.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://xzy.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://dyd.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rxk.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://zvn.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://grx.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://eem.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fpe.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://nzh.sjlbkw.cn

[G10] 访问控制
来源：http://flp.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://pje.hammf.cn

PHP:  public / protected / private
来源：http://gli.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://xcf.hysaishi.cn

TS:   public / protected / private
来源：http://ciu.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://ipd.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xhi.jqgfzy.top

Ruby: public / protected / private
来源：http://bgp.guannengcc.top

C#:   public / protected / private / internal
来源：http://blw.zhoulong.xyz

[G11] getter / setter
来源：http://qsy.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://odo.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gvo.yj20258888.top

JS:   get name() { return this._name; }
来源：http://epc.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://bnq.aizwys.cn

Java: public String getName() { return name; }
来源：http://pbi.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wyf.cdnleiting.top

Ruby: attr_accessor :name
来源：http://ojo.ydzc1.top

C#:   public string Name { get; set; }
来源：http://mmg.jqgufenzy.top

[G12] 对象转字符串
来源：http://lzq.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://daw.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://arw.havefunace.top

JS:   toString() { return this.name; }
来源：http://bhn.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://fyh.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://ubv.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://oxb.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://fhs.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://dkd.shuidangran.top

[G13] 判断对象类型
来源：http://gzi.snrcjt.cn

Py:   isinstance(u, User)
来源：http://vpz.0kj1m.cn

PHP:  $u instanceof User
来源：http://zft.zdbjq.cn

JS:   u instanceof User
来源：http://aos.mhx1999.top

TS:   u instanceof User
来源：http://jby.c1oappe.top

Java: u instanceof User
来源：http://jmt.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nsb.birdmap.top

Ruby: u.is_a?(User)
来源：http://hki.havefunace.top

C#:   u is User
来源：http://fya.ehwqpu.com

[G14] 数据类 / record
来源：http://lca.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gza.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://atc.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lyx.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://awy.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://khz.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://opg.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jqu.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://dob.quarkkingdee.top

[G15] 枚举
来源：http://apn.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nht.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://onr.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jkq.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qug.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://xzo.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zer.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://dmx.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dvh.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://grj.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mmi.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://djs.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://bew.hesvh.cn

TS:   Object.entries(obj)
来源：http://pso.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oun.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dlf.yangfankeji.com

Ruby: obj.instance_variables
来源：http://cif.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://hto.nwbrower.top

================================================================================
来源：http://apm.jqgufenzy.top

H. 异常与错误处理
来源：http://liz.tarul.cn

================================================================================
来源：http://rek.zhiwuduotai.top

[H01] try / catch 基础
来源：http://hhu.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rlm.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://num.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://axj.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ung.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ezf.hfpthk.cn


<!-- 参考信息 -->