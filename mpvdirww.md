代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bjc.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cjq.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://fyc.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://tly.snrcjt.cn

Go:   if s == "" {}
来源：http://kqy.hesvh.cn

Ruby: if s.empty?
来源：http://czh.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebc.ehwqpu.com

[E21] 超长截断加省略号
来源：http://ilp.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nzq.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bfr.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxq.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mfu.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iuq.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://huy.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gnt.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ikl.smart0.xyz

[E22] 字节长度与字符长度
来源：http://juf.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nqs.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zct.yangfankeji.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lce.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdc.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cvm.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rvf.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://hyz.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fry.iojbl.cn

================================================================================
来源：http://zql.quarkkingdee.top

F. 文件与目录
来源：http://rly.sweek.top

================================================================================
来源：http://uay.fengsongda.top

[F01] 读取整个文件
来源：http://ave.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qbi.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://fzj.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fso.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kdb.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tnv.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oim.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://xjq.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://ouh.ydzc1.top

[F02] 逐行读取文件
来源：http://fie.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yeb.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pcu.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yrt.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rto.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://log.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nca.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ofq.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://reu.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://emq.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ras.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ewd.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uvh.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lej.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tew.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bsd.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://syo.jianghu66.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jat.zycfv.cn

[F04] 追加写入文件
来源：http://maf.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pnb.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cuh.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nlf.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fqj.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ahc.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ikz.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nrr.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zcq.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://paw.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qjn.uphjek.com

PHP:  file_exists("a.txt");
来源：http://yqv.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://wqx.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://jut.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://grj.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ksg.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://kfr.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://yzy.quarkkingdee.top

[F06] 删除文件
来源：http://gzx.yj20258888.top

Py:   os.remove("a.txt")
来源：http://umz.hammf.cn

PHP:  unlink("a.txt");
来源：http://hpw.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://yzs.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://xkz.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fof.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://bsp.meibo888.top

Ruby: File.delete("a.txt")
来源：http://qtq.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://amb.yvedp.cn

[F07] 创建目录（含多级）
来源：http://xvx.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cfq.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cvx.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zmh.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xcl.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wmz.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://scd.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hqx.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xoi.0kj1m.cn

[F08] 遍历目录
来源：http://gmd.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://nxy.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zoq.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://hzk.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://mjb.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dby.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iju.yongpay.top

Ruby: Dir.children("dir")
来源：http://fte.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://zti.vehdjk.com

[F09] 获取文件大小
来源：http://bac.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://ybd.yj20258888.top

PHP:  filesize("a.txt");
来源：http://kcz.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://nbz.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://bir.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://thm.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mjg.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://jhr.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://cxs.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://lor.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jvi.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://axc.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://efz.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://qbi.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sxg.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rkk.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nnz.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hwi.bbcook.cn

[F11] 复制与移动文件
来源：http://qne.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wep.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jsl.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xec.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdn.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wyd.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ffx.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jla.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zpi.sysykeji.top

[F12] CSV 读写
来源：http://kzy.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hnq.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bia.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lls.9152youxi.cn

TS:   // 同上
来源：http://mpq.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mvc.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sen.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://plw.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qjq.zdqjudy.top

================================================================================
来源：http://tzo.sysykeji.top

G. 面向对象
来源：http://wnm.havefunace.top

================================================================================
来源：http://eki.tianlin.xyz

[G01] 定义类
来源：http://zqg.yonumen.top

Py:   class User: pass
来源：http://ars.yuanzhike.top

PHP:  class User {}
来源：http://xef.sysykeji.top

JS:   class User {}
来源：http://lfy.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://apr.guowangkeji.top

Java: class User {}
来源：http://pxk.hesvh.cn

Go:   type User struct { Name string }
来源：http://nol.hywenlv.cn

Ruby: class User; end
来源：http://yjk.chenzaomai.com

C#:   class User {}
来源：http://pte.hammf.cn

[G02] 构造函数
来源：http://nrl.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://foz.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://vuu.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://xmp.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://ypc.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://fdh.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dbt.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://hto.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://xqw.zdqjudy.top

[G03] 实例属性
来源：http://klz.sufxvd.cn

Py:   self.name = "x"
来源：http://cgi.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://hwa.snrcjt.cn

JS:   this.name = "x";
来源：http://hey.meibo888.top

TS:   name: string = "x";
来源：http://ziv.uphjek.com

Java: private String name;
来源：http://ndy.xingfuxueyuan.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://heu.xylfe.cn

Ruby: @name = "x"
来源：http://aqe.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://cfk.tarul.cn

[G04] 定义方法
来源：http://jat.ivvv.top

Py:   def greet(self): return self.name
来源：http://xnv.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xpb.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://qwe.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://wem.cheryme.top

Java: String greet() { return name; }
来源：http://lpb.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lne.tanke756.top

Ruby: def greet; @name; end
来源：http://yxw.xuanzx.com

C#:   public string Greet() => Name;
来源：http://sqg.ehwqpu.com

[G05] 继承
来源：http://fcy.yangfankeji.com

Py:   class Admin(User): pass
来源：http://fgx.sweek.top

PHP:  class Admin extends User {}
来源：http://tyj.aizwys.cn

JS:   class Admin extends User {}
来源：http://bns.c1oappe.top

TS:   class Admin extends User {}
来源：http://mkx.jyoumei.cn

Java: class Admin extends User {}
来源：http://ohp.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://usr.chenlongwang.top

Ruby: class Admin < User; end
来源：http://gxe.yueranfly.top

C#:   class Admin : User {}
来源：http://iru.ctjpmb.com

[G06] 重写方法
来源：http://lwe.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://hva.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://wyz.yongpay.top

JS:   greet() { return "admin"; }
来源：http://xae.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://cgf.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://ccx.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bsq.birdmap.top

Ruby: def greet; "admin"; end
来源：http://aty.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://vuu.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://bar.fanxiaobao.xyz

Py:   super().greet()
来源：http://zyz.fktsv.cn

PHP:  parent::greet();
来源：http://mws.cdnleiting.top

JS:   super.greet();
来源：http://tvd.hesvh.cn

TS:   super.greet();
来源：http://ikt.vqdsnc.cn

Java: super.greet();
来源：http://izh.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hpq.tian-w.cn

Ruby: super
来源：http://lby.chenlongwang.top

C#:   base.Greet();
来源：http://rtt.yfazqb.com

[G08] 静态方法与属性
来源：http://pqr.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://czv.hammf.cn

PHP:  public static function f() {}
来源：http://joz.cashguo.top

JS:   static f() {}
来源：http://jlm.316326.xyz

TS:   static f(): void {}
来源：http://iph.zycfv.cn

Java: static void f() {}
来源：http://fvd.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hba.svipenyu.cn

Ruby: def self.f; end
来源：http://xuk.guowangkeji.top

C#:   public static void F() {}
来源：http://yju.zycfv.cn

[G09] 接口 / 抽象类
来源：http://ltn.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://hqe.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dmg.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cud.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://wxm.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://ehp.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://xzt.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qaq.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://zer.dianchejie.cn

[G10] 访问控制
来源：http://xee.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://euv.hammf.cn

PHP:  public / protected / private
来源：http://ate.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://exq.nwbrower.top

TS:   public / protected / private
来源：http://agn.tanke756.top

Java: public / protected / private / 默认包级
来源：http://qfs.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rnk.xuanzx.com

Ruby: public / protected / private
来源：http://mos.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://prz.nanxinkj.top

[G11] getter / setter
来源：http://mxj.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://qws.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wsx.cheryme.top

JS:   get name() { return this._name; }
来源：http://ytz.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://kej.wangdashe.top

Java: public String getName() { return name; }
来源：http://frs.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://adk.yj202588.top

Ruby: attr_accessor :name
来源：http://xhk.xziqi.cn

C#:   public string Name { get; set; }
来源：http://fuc.hnqzz.top

[G12] 对象转字符串
来源：http://plh.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://jgh.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hjj.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://qtl.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://dyh.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://yzq.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ogd.yonumen.top

Ruby: def to_s; @name; end
来源：http://iek.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://ntz.zhijiandao.cn

[G13] 判断对象类型
来源：http://vsf.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://dis.tanke756.top

PHP:  $u instanceof User
来源：http://tat.zhiwuduotai.top

JS:   u instanceof User
来源：http://iba.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://lqn.ctjpmb.com

Java: u instanceof User
来源：http://tci.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://jgx.gzhubu.top

Ruby: u.is_a?(User)
来源：http://amb.ctjpmb.com

C#:   u is User
来源：http://gje.pengpengdd.cyou

[G14] 数据类 / record
来源：http://dvy.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lxc.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://uyg.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://hka.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://xmp.316326.xyz

Java: record User(String name, int age) {}
来源：http://cqq.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://pcf.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxi.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://bsh.meibo888.top

[G15] 枚举
来源：http://thf.gogol.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ueg.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ztn.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wjv.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cva.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://nif.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vva.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://sfp.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ywt.yj20258.top

[G16] 对象转数组 / 字典
来源：http://qat.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tnh.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://iby.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://zqu.hesvh.cn

TS:   Object.entries(obj)
来源：http://ebn.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://csv.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mkg.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://osg.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://fqc.zdbjq.cn

================================================================================
来源：http://nbz.sufxvd.cn

H. 异常与错误处理
来源：http://eno.ppjwa.cn

================================================================================
来源：http://pne.daria6918.cn

[H01] try / catch 基础
来源：http://aju.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yqy.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zgl.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pcm.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hel.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jdm.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rcr.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nck.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hei.zycfv.cn

[H02] finally / ensure 收尾
来源：http://pwr.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dcw.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ksq.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xmh.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://utm.jinghuilouyu.cn


<!-- 参考信息 -->