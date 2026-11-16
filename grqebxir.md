代发 wailian999

Ruby: s.lines
来源：http://crq.xylfe.cn

C#:   s.Split('\n')
来源：http://nnl.xylfe.cn

[E20] 判断字符串是否为空
来源：http://xam.gogol.net.cn

Py:   if not s:
来源：http://kik.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lht.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://txs.cashguo.top

TS:   if (s === "") {}
来源：http://sij.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://aev.yonumen.top

Go:   if s == "" {}
来源：http://lkv.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://hqi.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ovq.snrcjt.cn

[E21] 超长截断加省略号
来源：http://wgw.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://efb.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jtk.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vxb.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wdj.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qeq.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://acq.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dlt.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ojj.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://paq.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qgf.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://chy.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bse.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lno.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yuv.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://art.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://tyl.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xyn.redwolf501.top

================================================================================
来源：http://ari.tianlin.xyz

F. 文件与目录
来源：http://hbo.xingfuxueyuan.xyz

================================================================================
来源：http://ogr.jinqigfzy.top

[F01] 读取整个文件
来源：http://zkf.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://myb.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://ydz.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lub.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jff.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vqx.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mzw.tarul.cn

Ruby: File.read("a.txt")
来源：http://pff.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://jdk.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://fvd.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ciu.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cho.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mji.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gpx.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nrl.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://imz.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gip.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lhv.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://rsi.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://elz.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://erd.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vza.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gsk.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gax.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uey.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://yek.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vrv.snrcjt.cn

[F04] 追加写入文件
来源：http://yih.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gpn.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jjq.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://slx.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zcb.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kfh.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ukq.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xfs.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ooa.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://oze.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nqe.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://kob.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://vgc.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://cqb.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fzn.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://idp.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://fyq.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://flw.tian-w.cn

[F06] 删除文件
来源：http://qbq.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://mxc.yonumen.top

PHP:  unlink("a.txt");
来源：http://ewd.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://lkt.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://oxp.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ljs.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://mgc.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://xxf.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://lxd.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://kob.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://upm.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pda.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pkj.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://peh.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xla.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://egr.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xtc.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://obg.zhoulong.xyz

[F08] 遍历目录
来源：http://xnp.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zdk.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wgt.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://uza.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://rsm.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eig.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nqf.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://tkm.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://sis.ybcxt.top

[F09] 获取文件大小
来源：http://cqr.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ufr.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://las.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://nvj.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://dpq.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://now.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bgt.shuidangran.top

Ruby: File.size("a.txt")
来源：http://zye.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://yjn.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://efz.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bnx.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vxo.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://enp.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://pjf.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eaa.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://evl.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dls.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fgh.zhijiandao.cn

[F11] 复制与移动文件
来源：http://npw.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://plp.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fpo.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wrc.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://idm.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cmo.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uhi.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jov.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ntp.cdnleiting.top

[F12] CSV 读写
来源：http://gbj.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qfz.haohaochexian.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pii.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ole.gotoacloud.top

TS:   // 同上
来源：http://pcb.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lxx.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hpx.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qft.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fdf.xingfuxueyuan.xyz

================================================================================
来源：http://dnf.nanxinkj.top

G. 面向对象
来源：http://gcp.zhixingplan.top

================================================================================
来源：http://pfc.yuanzhike.top

[G01] 定义类
来源：http://smx.hcnkem.com

Py:   class User: pass
来源：http://gzy.mhx1999.top

PHP:  class User {}
来源：http://fex.hcnkem.com

JS:   class User {}
来源：http://lyi.ivvv.top

TS:   class User { name: string = ""; }
来源：http://pav.birdmap.top

Java: class User {}
来源：http://lwd.smart0.xyz

Go:   type User struct { Name string }
来源：http://dzv.haohaochexian.top

Ruby: class User; end
来源：http://kmb.cucudq.cn

C#:   class User {}
来源：http://yyt.tianlin.xyz

[G02] 构造函数
来源：http://njk.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://sfo.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://kcm.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://ckn.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://olt.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://kvb.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ykq.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://kpy.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://srp.ywan-chungtsiang.top

[G03] 实例属性
来源：http://uwm.epnwcf.com

Py:   self.name = "x"
来源：http://ucl.mhx1999.top

PHP:  public string $name = "x";
来源：http://nbr.ppjwa.cn

JS:   this.name = "x";
来源：http://bam.feifeiyinyue.top

TS:   name: string = "x";
来源：http://urk.cheryme.top

Java: private String name;
来源：http://jwx.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ptw.daria6918.cn

Ruby: @name = "x"
来源：http://xwi.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://obl.jinyuanbaomall.cn

[G04] 定义方法
来源：http://ymc.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://bdb.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://svh.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://eez.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://rsm.andypj.xyz

Java: String greet() { return name; }
来源：http://zbb.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cgd.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://vlm.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://stp.ehwqpu.com

[G05] 继承
来源：http://gpe.gzhubu.top

Py:   class Admin(User): pass
来源：http://ozp.daxiang520.top

PHP:  class Admin extends User {}
来源：http://vke.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://gae.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://pyc.hnxiangtu.top

Java: class Admin extends User {}
来源：http://hnm.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://apu.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://zdg.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://ekd.zhongyouzk.top

[G06] 重写方法
来源：http://ilp.uphjek.com

Py:   def greet(self): return "admin"
来源：http://umh.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nvl.yonumen.top

JS:   greet() { return "admin"; }
来源：http://bju.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://rte.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://yzr.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ppi.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://wub.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://rbz.nanxinkj.top

[G07] 调用父类方法
来源：http://naz.gogol.net.cn

Py:   super().greet()
来源：http://pcp.yfazqb.com

PHP:  parent::greet();
来源：http://evm.chenjidiqi.icu

JS:   super.greet();
来源：http://cbb.dashuyun.cn

TS:   super.greet();
来源：http://geu.yueranfly.top

Java: super.greet();
来源：http://whg.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://udo.xziqi.cn

Ruby: super
来源：http://hbm.zhengqikj.top

C#:   base.Greet();
来源：http://zki.daxiang520.top

[G08] 静态方法与属性
来源：http://eye.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://shw.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://hrq.jinghuilouyu.cn

JS:   static f() {}
来源：http://jqc.ydjk.org.cn

TS:   static f(): void {}
来源：http://zvy.sufxvd.cn

Java: static void f() {}
来源：http://alg.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://dbk.ivvv.top

Ruby: def self.f; end
来源：http://rcz.hywenlv.cn

C#:   public static void F() {}
来源：http://zsf.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://ont.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://stl.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://abh.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bsy.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://ejr.fktsv.cn

Java: interface Shape { double area(); }
来源：http://koc.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://efj.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xsh.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://wex.shangyingyoupin.top

[G10] 访问控制
来源：http://gnm.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://sjh.daria6918.cn

PHP:  public / protected / private
来源：http://fws.guannengcc.top

JS:   #private 字段；其余公开
来源：http://koe.pengpengdd.cyou

TS:   public / protected / private
来源：http://afz.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://gsi.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://guj.xinyue.icu

Ruby: public / protected / private
来源：http://wqt.dianchejie.cn

C#:   public / protected / private / internal
来源：http://noj.guannengcc.top

[G11] getter / setter
来源：http://spa.fzhhl.top

Py:   @property 与 @x.setter
来源：http://cna.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rxi.sxryk.cn

JS:   get name() { return this._name; }
来源：http://qik.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://vhp.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://uqs.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://bzw.sweek.top

Ruby: attr_accessor :name
来源：http://lvl.jianghu66.top

C#:   public string Name { get; set; }
来源：http://mbi.shangyingyoupin.top

[G12] 对象转字符串
来源：http://jxz.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://acc.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nze.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://tqn.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://pbh.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://aqj.pycfn.com

Go:   func (u User) String() string { return u.Name }
来源：http://eih.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://egp.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://lzy.0kj1m.cn

[G13] 判断对象类型
来源：http://tvq.pycfn.com

Py:   isinstance(u, User)
来源：http://qjg.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://muh.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://usf.gzhubu.top

TS:   u instanceof User
来源：http://fjb.daxiang520.top

Java: u instanceof User
来源：http://ovj.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://knj.yvedp.cn

Ruby: u.is_a?(User)
来源：http://zhe.hfpthk.cn

C#:   u is User
来源：http://few.ybcxt.top

[G14] 数据类 / record
来源：http://orw.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yus.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://qfq.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://fsr.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://oxs.ybcxt.top

Java: record User(String name, int age) {}
来源：http://oqu.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://mpt.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eeh.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://qed.shuidangran.top

[G15] 枚举
来源：http://twt.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ewc.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ntk.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vmc.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gdr.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://nhj.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mnj.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://igj.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qcy.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://yjz.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qxv.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://lnq.fehbvm.com

JS:   Object.entries(obj)
来源：http://zfp.mhx1999.top

TS:   Object.entries(obj)
来源：http://ogi.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cqc.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://trd.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://jvq.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://mzb.zdqjudy.top

================================================================================
来源：http://pdz.jiagoushi.top

H. 异常与错误处理
来源：http://fxp.zhixingplan.top

================================================================================
来源：http://qjn.epnwcf.com

[H01] try / catch 基础
来源：http://gdk.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zmb.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sev.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oiq.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tzo.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://epu.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://umt.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cjd.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://enl.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://ngc.jlsjyb.cn


<!-- 参考信息 -->