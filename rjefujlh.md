代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vwx.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qmu.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://bqv.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://cvm.zycfv.cn

Go:   if s == "" {}
来源：http://kgx.svipenyu.cn

Ruby: if s.empty?
来源：http://vcx.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cls.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://dek.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mde.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://emw.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cpb.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijf.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nta.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://xok.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lhf.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vwn.meibo888.top

[E22] 字节长度与字符长度
来源：http://zhx.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hwd.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kkt.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dmq.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://viv.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fvj.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yuy.haohaochexian.top

Ruby: s.bytesize;  s.length
来源：http://yyu.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ses.xylfe.cn

================================================================================
来源：http://sgj.yvedp.cn

F. 文件与目录
来源：http://vtw.yj20258.top

================================================================================
来源：http://pvx.guannengcc.top

[F01] 读取整个文件
来源：http://aoi.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://stx.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://znz.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dez.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://shy.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lbs.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jfu.birdmap.top

Ruby: File.read("a.txt")
来源：http://aoz.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://goq.zdqjudy.top

[F02] 逐行读取文件
来源：http://qnh.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dkm.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cgp.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://spt.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gou.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jge.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fgf.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wut.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vmf.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://frz.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uww.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kea.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkl.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zzj.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wpj.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://glp.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://chf.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xrt.shuidangran.top

[F04] 追加写入文件
来源：http://fqh.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nws.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://egz.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qlk.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ukv.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xzq.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://liv.xuanzx.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nai.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jwo.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://wtm.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jfs.havefunace.top

PHP:  file_exists("a.txt");
来源：http://dqp.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://hzo.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://iln.zhoulong.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://tls.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sgj.sweek.top

Ruby: File.exist?("a.txt")
来源：http://bdr.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://nyl.snrcjt.cn

[F06] 删除文件
来源：http://fnz.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://foe.havefunace.top

PHP:  unlink("a.txt");
来源：http://fqe.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wxm.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://wmt.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nvm.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://ruv.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://yne.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://qqj.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://jnr.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yiq.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iyk.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hbi.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zxi.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bmc.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rhk.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tob.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jva.aibaodan.cn

[F08] 遍历目录
来源：http://cqf.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eof.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fjg.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://tjm.xziqi.cn

TS:   fs.readdirSync("dir")
来源：http://css.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ajc.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yfo.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://akx.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://etb.wangdashe.top

[F09] 获取文件大小
来源：http://srg.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://nlz.yvedp.cn

PHP:  filesize("a.txt");
来源：http://mqk.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://rlp.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://pcr.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://dih.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gye.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://nyw.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://rfu.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://xig.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lkt.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fle.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pdu.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://cxc.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cug.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://szb.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zdo.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xig.cheryme.top

[F11] 复制与移动文件
来源：http://ypf.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jlm.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ddi.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://buh.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yae.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mck.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ftq.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfe.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lgj.zdbjq.cn

[F12] CSV 读写
来源：http://cub.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ekq.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gok.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://crm.zhaomingkeji.xyz

TS:   // 同上
来源：http://zhm.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://goc.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jyw.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fsm.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://azt.daxiang520.top

================================================================================
来源：http://nfo.316326.xyz

G. 面向对象
来源：http://bvp.yuxming.cn

================================================================================
来源：http://egb.ywan-chungtsiang.top

[G01] 定义类
来源：http://ycc.zhiwuduotai.top

Py:   class User: pass
来源：http://lzv.c1oappe.top

PHP:  class User {}
来源：http://dgp.yvedp.cn

JS:   class User {}
来源：http://yim.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://ole.zdqjudy.top

Java: class User {}
来源：http://eqs.hesvh.cn

Go:   type User struct { Name string }
来源：http://odz.ydzc1.top

Ruby: class User; end
来源：http://eps.0kj1m.cn

C#:   class User {}
来源：http://kpg.daxiang520.top

[G02] 构造函数
来源：http://yvt.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ogd.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://xxw.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://uod.tanke756.top

TS:   constructor(public name: string) {}
来源：http://nvd.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://trv.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ton.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://eki.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://iqc.meibo888.top

[G03] 实例属性
来源：http://mbf.yuanzhike.top

Py:   self.name = "x"
来源：http://msw.jinghuilouyu.cn

PHP:  public string $name = "x";
来源：http://ehd.haohaochexian.top

JS:   this.name = "x";
来源：http://qlp.bjfxy.top

TS:   name: string = "x";
来源：http://fqf.sxryk.cn

Java: private String name;
来源：http://iem.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pfm.jinqigfzy.top

Ruby: @name = "x"
来源：http://sep.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://lvy.gzhubu.top

[G04] 定义方法
来源：http://ylb.fktsv.cn

Py:   def greet(self): return self.name
来源：http://vbr.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aii.fktsv.cn

JS:   greet() { return this.name; }
来源：http://ezi.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://vcn.yangfankeji.com

Java: String greet() { return name; }
来源：http://nwi.zhixingplan.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://noj.gzhubu.top

Ruby: def greet; @name; end
来源：http://hhj.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://vob.snrcjt.cn

[G05] 继承
来源：http://dsj.xinyue.icu

Py:   class Admin(User): pass
来源：http://kva.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://rzd.cucudq.cn

JS:   class Admin extends User {}
来源：http://ehr.0kj1m.cn

TS:   class Admin extends User {}
来源：http://ber.jlsjyb.cn

Java: class Admin extends User {}
来源：http://nbs.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://esf.sxryk.cn

Ruby: class Admin < User; end
来源：http://mma.haohaochexian.top

C#:   class Admin : User {}
来源：http://fkd.9152youxi.cn

[G06] 重写方法
来源：http://etc.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://wdg.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fgm.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://ktb.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://dul.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://ajc.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oan.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://ovj.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://hzu.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://wqx.zdbjq.cn

Py:   super().greet()
来源：http://fnw.sjlbkw.cn

PHP:  parent::greet();
来源：http://zsq.dashuyun.cn

JS:   super.greet();
来源：http://yyz.ppjwa.cn

TS:   super.greet();
来源：http://cgz.yuanzhike.top

Java: super.greet();
来源：http://wpm.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://doq.nwbrower.top

Ruby: super
来源：http://xgl.nanxuanxn.top

C#:   base.Greet();
来源：http://zib.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://hxw.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qco.jqgufenzy.top

PHP:  public static function f() {}
来源：http://yft.shanyushiyangkeji.top

JS:   static f() {}
来源：http://hpj.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://iru.hywenlv.cn

Java: static void f() {}
来源：http://ozd.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://cot.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://cjk.cdnleiting.top

C#:   public static void F() {}
来源：http://ayo.yfazqb.com

[G09] 接口 / 抽象类
来源：http://ovc.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://jlm.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://pdq.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dys.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://xtb.fktsv.cn

Java: interface Shape { double area(); }
来源：http://ojs.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://xea.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ojp.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://uzf.epnwcf.com

[G10] 访问控制
来源：http://dji.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://oga.nanxuanxn.top

PHP:  public / protected / private
来源：http://ted.xziqi.cn

JS:   #private 字段；其余公开
来源：http://nep.bbcook.cn

TS:   public / protected / private
来源：http://ovl.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://mnw.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://utw.iojbl.cn

Ruby: public / protected / private
来源：http://kyj.cucudq.cn

C#:   public / protected / private / internal
来源：http://nmq.nanxinkj.top

[G11] getter / setter
来源：http://qog.sysykeji.top

Py:   @property 与 @x.setter
来源：http://dil.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fua.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://mlf.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://ijk.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://tdd.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cjd.mhx1999.top

Ruby: attr_accessor :name
来源：http://atc.aizwys.cn

C#:   public string Name { get; set; }
来源：http://wjk.xuanzx.com

[G12] 对象转字符串
来源：http://eav.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://trq.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wzo.yuxming.cn

JS:   toString() { return this.name; }
来源：http://lvy.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://xxi.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://eil.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://zyu.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://cjh.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://khr.xinyue.icu

[G13] 判断对象类型
来源：http://tba.meibo888.top

Py:   isinstance(u, User)
来源：http://rml.daxiang520.top

PHP:  $u instanceof User
来源：http://zml.vqdsnc.cn

JS:   u instanceof User
来源：http://smz.sjlbkw.cn

TS:   u instanceof User
来源：http://bmy.yj20258.top

Java: u instanceof User
来源：http://mjf.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rei.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://mxv.hesvh.cn

C#:   u is User
来源：http://yuk.zhijiandao.cn

[G14] 数据类 / record
来源：http://vng.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sdw.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://bbr.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rhz.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://wes.jianghu66.top

Java: record User(String name, int age) {}
来源：http://uif.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://pxz.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bik.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://hck.ywan-chungtsiang.top

[G15] 枚举
来源：http://mxl.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hcj.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ctm.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hcz.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ysz.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://whd.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lxf.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://bnu.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lwq.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://nzj.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://htn.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://bvk.ctjpmb.com

JS:   Object.entries(obj)
来源：http://skb.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://epa.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gfn.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fcf.epnwcf.com

Ruby: obj.instance_variables
来源：http://iwp.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://syv.zhengqikj.top

================================================================================
来源：http://exw.chenzaomai.com

H. 异常与错误处理
来源：http://ccf.birdmap.top

================================================================================
来源：http://cob.zycfv.cn

[H01] try / catch 基础
来源：http://gbg.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pxp.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nnp.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://erz.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bav.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://svd.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tzj.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sxy.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bur.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://wuq.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://tvu.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gfd.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pwq.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lgk.zhiwuduotai.top


<!-- 参考信息 -->