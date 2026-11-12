代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://tmd.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://spj.hnxiangtu.top

Java: s.lines().toList()
来源：http://zby.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://lfj.cheryme.top

Ruby: s.lines
来源：http://nyi.jinqigufen.top

C#:   s.Split('\n')
来源：http://leh.316326.xyz

[E20] 判断字符串是否为空
来源：http://wxx.sjlbkw.cn

Py:   if not s:
来源：http://rpo.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nue.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://psa.jinqigfzy.top

TS:   if (s === "") {}
来源：http://dmq.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://vwq.jiagoushi.top

Go:   if s == "" {}
来源：http://jvs.bbcook.cn

Ruby: if s.empty?
来源：http://xgz.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cqg.yfazqb.com

[E21] 超长截断加省略号
来源：http://dpt.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://omu.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eqh.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tpd.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bbi.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wxf.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://zbc.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nzq.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rqx.meibo888.top

[E22] 字节长度与字符长度
来源：http://zpb.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jiv.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gun.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pcc.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://unl.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nbi.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mai.sweek.top

Ruby: s.bytesize;  s.length
来源：http://aab.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zwi.jinyuanbaomall.cn

================================================================================
来源：http://bir.jqgufenzy.top

F. 文件与目录
来源：http://qqs.ctjpmb.com

================================================================================
来源：http://ndd.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://oim.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mcn.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://oah.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ucc.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://euo.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ozw.yanxiufei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jbq.xylfe.cn

Ruby: File.read("a.txt")
来源：http://vio.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://pof.tianlin.xyz

[F02] 逐行读取文件
来源：http://ljx.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lyw.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sab.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rer.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gkp.jinqigfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://izw.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pdm.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tst.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mkv.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://qem.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bks.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://awd.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cgh.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijt.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ypq.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://epe.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://wfv.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cvl.chenzaomai.com

[F04] 追加写入文件
来源：http://sop.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ydv.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ygn.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tfk.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wmg.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://plp.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nuo.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vcd.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gls.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://xqj.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ijd.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://xhj.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://mmd.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://anf.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xxn.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eju.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://qnc.pycfn.com

C#:   File.Exists("a.txt")
来源：http://alw.sufxvd.cn

[F06] 删除文件
来源：http://dff.iojbl.cn

Py:   os.remove("a.txt")
来源：http://gza.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://jmj.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://xwm.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kxy.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oft.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://hcu.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://xmz.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://vvy.tarul.cn

[F07] 创建目录（含多级）
来源：http://thw.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://loo.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jvp.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lhu.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlw.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kqs.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tny.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ixq.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rkz.fanxiaobao.xyz

[F08] 遍历目录
来源：http://zmd.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bwi.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xug.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://dlk.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://nrp.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fpx.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bzm.cashguo.top

Ruby: Dir.children("dir")
来源：http://mfx.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://jrc.snrcjt.cn

[F09] 获取文件大小
来源：http://pwy.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://cbq.ybcxt.top

PHP:  filesize("a.txt");
来源：http://zsf.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://urj.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://fse.daxiang520.top

Java: Files.size(Path.of("a.txt"))
来源：http://bpj.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yyf.cashguo.top

Ruby: File.size("a.txt")
来源：http://wns.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://mbu.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://hbp.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oel.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zbp.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://poe.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://mfg.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://llk.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vlv.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pkb.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cvy.jiagoushi.top

[F11] 复制与移动文件
来源：http://zeh.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xtk.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjx.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgw.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mcr.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://crh.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cpt.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cju.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://riw.tarul.cn

[F12] CSV 读写
来源：http://oau.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mpb.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://buz.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tit.gotoacloud.top

TS:   // 同上
来源：http://ypu.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eea.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://npx.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kne.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lip.guannengcc.top

================================================================================
来源：http://vfc.xingfuxueyuan.xyz

G. 面向对象
来源：http://pcf.gaohongyu789.top

================================================================================
来源：http://deo.yangfankeji.com

[G01] 定义类
来源：http://inw.tianlin.xyz

Py:   class User: pass
来源：http://yvp.jinghuilouyu.cn

PHP:  class User {}
来源：http://xzw.jlsjyb.cn

JS:   class User {}
来源：http://sbv.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://hgp.uphjek.com

Java: class User {}
来源：http://pvm.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://cci.quarkkingdee.top

Ruby: class User; end
来源：http://lpi.xuanzx.com

C#:   class User {}
来源：http://zjh.fengsongda.top

[G02] 构造函数
来源：http://eal.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://wlr.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://ulw.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://wxw.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://emf.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://sia.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kic.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://gjj.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://jwf.xylfe.cn

[G03] 实例属性
来源：http://kms.yuxming.cn

Py:   self.name = "x"
来源：http://lch.guowangkeji.top

PHP:  public string $name = "x";
来源：http://ouc.sjlbkw.cn

JS:   this.name = "x";
来源：http://blj.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://dfy.shuidangran.top

Java: private String name;
来源：http://hrl.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ngv.zdqjudy.top

Ruby: @name = "x"
来源：http://jta.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://nxc.tian-w.cn

[G04] 定义方法
来源：http://nmp.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://elj.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hfw.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://mys.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://ebu.yonumen.top

Java: String greet() { return name; }
来源：http://bic.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://brt.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://fqu.hnqzz.top

C#:   public string Greet() => Name;
来源：http://kpe.andypj.xyz

[G05] 继承
来源：http://sen.havefunace.top

Py:   class Admin(User): pass
来源：http://scr.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://tkr.zdbjq.cn

JS:   class Admin extends User {}
来源：http://aot.ybcxt.top

TS:   class Admin extends User {}
来源：http://klf.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://hca.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://isk.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://ydv.havefunace.top

C#:   class Admin : User {}
来源：http://ltb.fzhhl.top

[G06] 重写方法
来源：http://ukr.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://ukf.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://lag.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://hta.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://iiw.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://qfp.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ymb.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://atj.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://axi.xziqi.cn

[G07] 调用父类方法
来源：http://bxz.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://kea.bbcook.cn

PHP:  parent::greet();
来源：http://nbz.hesvh.cn

JS:   super.greet();
来源：http://oor.shanyushiyangkeji.top

TS:   super.greet();
来源：http://bwy.ivvv.top

Java: super.greet();
来源：http://jio.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fbf.nwbrower.top

Ruby: super
来源：http://iun.yuanzhike.top

C#:   base.Greet();
来源：http://bxx.fengsongda.top

[G08] 静态方法与属性
来源：http://arc.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://okh.xuanzx.com

PHP:  public static function f() {}
来源：http://yat.jinyuanbaomall.cn

JS:   static f() {}
来源：http://lvu.quarkkingdee.top

TS:   static f(): void {}
来源：http://wiu.xinyue.icu

Java: static void f() {}
来源：http://hul.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vra.gotoacloud.top

Ruby: def self.f; end
来源：http://cxp.cucudq.cn

C#:   public static void F() {}
来源：http://hbg.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://hnh.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://noz.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://uyv.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dox.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://fjc.meibo888.top

Java: interface Shape { double area(); }
来源：http://uvr.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://hku.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yef.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://frj.zhixingplan.top

[G10] 访问控制
来源：http://zwc.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://ivu.pengpengdd.cyou

PHP:  public / protected / private
来源：http://rfk.yfazqb.com

JS:   #private 字段；其余公开
来源：http://gse.cqqwz.cn

TS:   public / protected / private
来源：http://uzu.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://jop.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gcx.jiagoushi.top

Ruby: public / protected / private
来源：http://vwq.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://qea.xinyue.icu

[G11] getter / setter
来源：http://jwt.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://oci.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://veq.vehdjk.com

JS:   get name() { return this._name; }
来源：http://nov.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://qgi.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://vbn.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://lde.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://tip.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://dky.yvedp.cn

[G12] 对象转字符串
来源：http://rut.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://ion.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mur.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://vch.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://syd.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://ecl.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://vht.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://iqy.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://bcn.zhijiandao.cn

[G13] 判断对象类型
来源：http://hkf.hnqzz.top

Py:   isinstance(u, User)
来源：http://sro.hcnkem.com

PHP:  $u instanceof User
来源：http://foc.gaohongyu789.top

JS:   u instanceof User
来源：http://ztb.nanxuanxn.top

TS:   u instanceof User
来源：http://blj.zdqjudy.top

Java: u instanceof User
来源：http://hat.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tuy.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://wjm.yongpay.top

C#:   u is User
来源：http://mhz.dianchejie.cn

[G14] 数据类 / record
来源：http://yqo.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zdj.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://rpt.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://hta.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://dxh.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://uzr.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://edi.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rlx.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://yyh.daria6918.cn

[G15] 枚举
来源：http://cty.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uey.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hjs.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nov.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rua.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://jte.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ibc.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://tta.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djs.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://gje.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://det.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://lmh.yonumen.top

JS:   Object.entries(obj)
来源：http://wij.birdmap.top

TS:   Object.entries(obj)
来源：http://owj.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ddt.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cee.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://rcg.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://nzl.vqdsnc.cn

================================================================================
来源：http://dui.yuanzhike.top

H. 异常与错误处理
来源：http://bjn.jqgufenzy.top

================================================================================
来源：http://jjx.jlsjyb.cn

[H01] try / catch 基础
来源：http://tge.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fwe.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tpz.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jpp.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nqw.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gzi.zhongyouzk.top


<!-- 参考信息 -->