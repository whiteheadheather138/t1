代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://upp.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zbd.zycfv.cn

TS:   if (s === "") {}
来源：http://tnr.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://qby.epnwcf.com

Go:   if s == "" {}
来源：http://txk.chenjidiqi.icu

Ruby: if s.empty?
来源：http://tmy.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ihr.jianghu66.top

[E21] 超长截断加省略号
来源：http://nle.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wql.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gog.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lxf.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bcx.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kgy.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://bjv.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lmz.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sad.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://hlf.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://noj.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pdk.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dxc.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://myx.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xwc.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jiy.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://jzg.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bwd.birdmap.top

================================================================================
来源：http://zjc.hongshengwenyu.top

F. 文件与目录
来源：http://otd.mhx1999.top

================================================================================
来源：http://wef.c1oappe.top

[F01] 读取整个文件
来源：http://zho.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oqo.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://bmf.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uif.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sim.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://nhm.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hhb.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://hdk.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://yad.fehbvm.com

[F02] 逐行读取文件
来源：http://uni.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lrg.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xvd.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://elo.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xnv.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://opn.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://acj.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hfn.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sln.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://fmi.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rgd.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xja.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cdy.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://anl.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fib.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rdg.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://glf.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cpj.zhiwuduotai.top

[F04] 追加写入文件
来源：http://tuv.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hzg.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zeg.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fjj.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yrw.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xhx.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ruk.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iov.birdmap.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://udb.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://wpk.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://abg.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://hrb.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://rnk.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://bpt.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fhe.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dcv.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://rhq.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://nkn.zhongyouzk.top

[F06] 删除文件
来源：http://qvo.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://gwg.xuanzx.com

PHP:  unlink("a.txt");
来源：http://qwr.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ovk.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jff.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vzf.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://hbk.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://lwi.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://qjp.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://cod.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jbq.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cbi.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ion.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fkj.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aot.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iph.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kdz.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mcb.smart0.xyz

[F08] 遍历目录
来源：http://ehh.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://pjp.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bkh.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://dab.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://san.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rmn.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://suj.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://ige.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://nxn.gotoacloud.top

[F09] 获取文件大小
来源：http://esy.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://myd.sweek.top

PHP:  filesize("a.txt");
来源：http://yfj.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://tri.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://uas.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jza.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jpn.yonumen.top

Ruby: File.size("a.txt")
来源：http://fyx.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://jai.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://fuj.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nhy.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yib.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ljw.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://akq.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mro.cheryme.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ejj.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rpw.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bpx.quarkkingdee.top

[F11] 复制与移动文件
来源：http://xys.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://imr.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zvk.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wag.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arc.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yup.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ojl.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zsn.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fvx.meibo888.top

[F12] CSV 读写
来源：http://wej.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://psn.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eka.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vgc.hammf.cn

TS:   // 同上
来源：http://reb.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yjp.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wgs.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nds.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zay.feifeiyinyue.top

================================================================================
来源：http://wfy.nanxinkj.top

G. 面向对象
来源：http://cws.gotoacloud.top

================================================================================
来源：http://ley.shanyushiyangkeji.top

[G01] 定义类
来源：http://fgl.hfpthk.cn

Py:   class User: pass
来源：http://ydv.chenlongwang.top

PHP:  class User {}
来源：http://xqo.yanxiufei.cn

JS:   class User {}
来源：http://aqt.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://lhw.aibaodan.cn

Java: class User {}
来源：http://uii.tarul.cn

Go:   type User struct { Name string }
来源：http://epa.nanxinkj.top

Ruby: class User; end
来源：http://dcj.zhixingplan.top

C#:   class User {}
来源：http://bpc.guowangkeji.top

[G02] 构造函数
来源：http://ncb.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://nsp.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://qsg.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://cms.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://hjy.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://vzg.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lsn.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://msj.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://mvr.epnwcf.com

[G03] 实例属性
来源：http://zvp.zhengqikj.top

Py:   self.name = "x"
来源：http://mnc.zhixingplan.top

PHP:  public string $name = "x";
来源：http://fdz.dashuyun.cn

JS:   this.name = "x";
来源：http://kcv.ctjpmb.com

TS:   name: string = "x";
来源：http://wcu.nanxinkj.top

Java: private String name;
来源：http://kzi.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mmo.bjfxy.top

Ruby: @name = "x"
来源：http://tdg.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://vqx.pycfn.com

[G04] 定义方法
来源：http://atz.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://pjm.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cpr.cashguo.top

JS:   greet() { return this.name; }
来源：http://gbf.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://lxx.zycfv.cn

Java: String greet() { return name; }
来源：http://ljh.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://faz.epnwcf.com

Ruby: def greet; @name; end
来源：http://icn.jianghu66.top

C#:   public string Greet() => Name;
来源：http://guw.shangyingyoupin.top

[G05] 继承
来源：http://yfv.aizwys.cn

Py:   class Admin(User): pass
来源：http://azt.sysykeji.top

PHP:  class Admin extends User {}
来源：http://arz.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://djr.shzxlz.cn

TS:   class Admin extends User {}
来源：http://ieg.xylfe.cn

Java: class Admin extends User {}
来源：http://xbv.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wjq.yuxming.cn

Ruby: class Admin < User; end
来源：http://rca.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://ocz.pengpengdd.cyou

[G06] 重写方法
来源：http://iex.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://sph.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rbs.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://gkd.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://esz.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://cuo.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yir.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://hzp.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://qyl.nanxuanxn.top

[G07] 调用父类方法
来源：http://rxd.shuidangran.top

Py:   super().greet()
来源：http://ots.epnwcf.com

PHP:  parent::greet();
来源：http://mrq.yongpay.top

JS:   super.greet();
来源：http://ojt.xuanzx.com

TS:   super.greet();
来源：http://glf.xuanzx.com

Java: super.greet();
来源：http://ouz.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lai.fengsongda.top

Ruby: super
来源：http://nal.kuanghao11.cn

C#:   base.Greet();
来源：http://bvw.jiagoushi.top

[G08] 静态方法与属性
来源：http://nae.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qtu.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://lfr.sufxvd.cn

JS:   static f() {}
来源：http://hod.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://pkt.pengpengdd.cyou

Java: static void f() {}
来源：http://rum.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xqo.fengsongda.top

Ruby: def self.f; end
来源：http://vjd.tianlin.xyz

C#:   public static void F() {}
来源：http://ubb.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://drz.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://mdt.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://yad.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ibe.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://lkm.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://rpr.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://upj.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kbc.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://vsh.tian-w.cn

[G10] 访问控制
来源：http://vwm.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://dbh.zhongyouzk.top

PHP:  public / protected / private
来源：http://rtg.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://iqd.hnqzz.top

TS:   public / protected / private
来源：http://iwj.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://akn.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hia.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://ety.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://dzt.yj20258.top

[G11] getter / setter
来源：http://twn.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://wzp.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hax.smart0.xyz

JS:   get name() { return this._name; }
来源：http://aac.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://irq.epnwcf.com

Java: public String getName() { return name; }
来源：http://qcw.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jlj.pycfn.com

Ruby: attr_accessor :name
来源：http://yvj.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://tvd.zhijiandao.cn

[G12] 对象转字符串
来源：http://hma.uphjek.com

Py:   def __str__(self): return self.name
来源：http://asa.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hsj.iojbl.cn

JS:   toString() { return this.name; }
来源：http://cyr.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://afu.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://zpt.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://hzz.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://djl.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://svb.jqgufenzy.top

[G13] 判断对象类型
来源：http://ahl.chenzaomai.com

Py:   isinstance(u, User)
来源：http://xav.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://thn.aibaodan.cn

JS:   u instanceof User
来源：http://edu.hywenlv.cn

TS:   u instanceof User
来源：http://lbb.c1oappe.top

Java: u instanceof User
来源：http://dsd.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gfq.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://ltz.xziqi.cn

C#:   u is User
来源：http://kek.hammf.cn

[G14] 数据类 / record
来源：http://ngx.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://adf.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://her.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://dxa.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://pal.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://xgy.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://klp.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tyv.sweek.top

C#:   record User(string Name, int Age);
来源：http://kfr.daria6918.cn

[G15] 枚举
来源：http://iga.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vti.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lwb.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jfh.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zak.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://vhr.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yol.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://vny.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://znk.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://rgw.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bfg.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://xdf.daria6918.cn

JS:   Object.entries(obj)
来源：http://ymr.xylfe.cn

TS:   Object.entries(obj)
来源：http://gzq.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gcu.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vrq.svipenyu.cn

Ruby: obj.instance_variables
来源：http://swa.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://nqm.hywenlv.cn

================================================================================
来源：http://qsz.wangshuangyany.cn

H. 异常与错误处理
来源：http://qxz.ydzc1.top

================================================================================
来源：http://lqt.0kj1m.cn

[H01] try / catch 基础
来源：http://wrl.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ddg.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qeo.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://llp.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lps.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nqz.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oiq.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://svc.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rkz.tarul.cn

[H02] finally / ensure 收尾
来源：http://gql.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pvw.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vil.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kww.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://tyg.jqgufenzy.top


<!-- 参考信息 -->