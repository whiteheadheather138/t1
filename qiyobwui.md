代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wrp.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cjm.cqqwz.cn

TS:   if (s === "") {}
来源：http://pvq.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://eey.hysaishi.cn

Go:   if s == "" {}
来源：http://mfe.bbcook.cn

Ruby: if s.empty?
来源：http://ocy.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yrx.cucudq.cn

[E21] 超长截断加省略号
来源：http://zor.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aqq.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mql.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kir.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qca.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jjt.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://dgo.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rvc.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://btq.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://gej.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hfb.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yzf.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xlq.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bao.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://myb.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uto.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://dhg.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uru.yj20258.top

================================================================================
来源：http://sal.ydjk.org.cn

F. 文件与目录
来源：http://puj.52xcode.cn

================================================================================
来源：http://vjt.jinqigufen.top

[F01] 读取整个文件
来源：http://kwb.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hsb.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://qer.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://frn.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eln.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qhn.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rdc.cheryme.top

Ruby: File.read("a.txt")
来源：http://vac.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://uvn.yuanzhike.top

[F02] 逐行读取文件
来源：http://zgz.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bha.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uwc.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ipl.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pla.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lwf.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ozd.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kib.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vqg.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://pll.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vjt.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kdm.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://onu.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vnq.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://npr.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zet.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://uzp.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nfc.jinqigufen.top

[F04] 追加写入文件
来源：http://jhf.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pro.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ska.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sln.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ojw.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xhk.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mav.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bhu.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cev.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://ykw.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://skf.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://hgn.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://nne.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://qpk.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://chf.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nxr.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://pkr.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://adn.daria6918.cn

[F06] 删除文件
来源：http://goz.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://vzq.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://epb.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://auh.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://tfc.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rao.316326.xyz

Go:   os.Remove("a.txt")
来源：http://xfj.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://ewt.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://vmk.sweek.top

[F07] 创建目录（含多级）
来源：http://rug.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pok.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fxk.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcg.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rpy.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ptn.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uyb.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jok.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://veg.jqgufenzy.top

[F08] 遍历目录
来源：http://uzy.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xqh.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zpy.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://uzo.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://adj.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mxo.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gnp.fzhhl.top

Ruby: Dir.children("dir")
来源：http://nse.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://lhz.zhongyouzk.top

[F09] 获取文件大小
来源：http://jpb.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://cfh.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://byr.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://qbd.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://wtd.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://flw.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wqs.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://stt.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://jfi.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://vpf.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vms.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xyl.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zxv.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://eew.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://knz.cheryme.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ctj.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bfr.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yiq.snrcjt.cn

[F11] 复制与移动文件
来源：http://mcz.sjlbkw.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://utl.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xmf.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hrd.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wuv.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xjv.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://spt.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ujn.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://var.yonumen.top

[F12] CSV 读写
来源：http://xhr.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vdv.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivo.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tie.hnxiangtu.top

TS:   // 同上
来源：http://byj.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://phl.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cms.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vxs.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://edu.gotoacloud.top

================================================================================
来源：http://jmx.ivvv.top

G. 面向对象
来源：http://uhx.yj20258.top

================================================================================
来源：http://zpj.sweek.top

[G01] 定义类
来源：http://jdy.hysaishi.cn

Py:   class User: pass
来源：http://fvv.quarkkingdee.top

PHP:  class User {}
来源：http://ncb.gotoacloud.top

JS:   class User {}
来源：http://thw.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://ysz.jlsjyb.cn

Java: class User {}
来源：http://dot.daxiang520.top

Go:   type User struct { Name string }
来源：http://rwh.feifeiyinyue.top

Ruby: class User; end
来源：http://wyr.feifeiyinyue.top

C#:   class User {}
来源：http://ebz.ydjk.org.cn

[G02] 构造函数
来源：http://qrc.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://kmx.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://rhh.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://aks.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://fxe.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://exi.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kzp.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://riv.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://krl.sweek.top

[G03] 实例属性
来源：http://dtl.smart0.xyz

Py:   self.name = "x"
来源：http://xii.dianchejie.cn

PHP:  public string $name = "x";
来源：http://jhx.zycfv.cn

JS:   this.name = "x";
来源：http://yrq.sweek.top

TS:   name: string = "x";
来源：http://xdg.aizwys.cn

Java: private String name;
来源：http://kwe.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vkb.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://dxi.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://uzd.tian-w.cn

[G04] 定义方法
来源：http://vhn.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://hfq.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cfr.nwbrower.top

JS:   greet() { return this.name; }
来源：http://bbg.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://lkt.hesvh.cn

Java: String greet() { return name; }
来源：http://ipu.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kam.xuanzx.com

Ruby: def greet; @name; end
来源：http://pvz.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://itr.sweek.top

[G05] 继承
来源：http://uva.chenlongwang.top

Py:   class Admin(User): pass
来源：http://vam.smart0.xyz

PHP:  class Admin extends User {}
来源：http://zkr.yj202588.top

JS:   class Admin extends User {}
来源：http://elv.snrcjt.cn

TS:   class Admin extends User {}
来源：http://akt.zdqjudy.top

Java: class Admin extends User {}
来源：http://eii.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jde.zdqjudy.top

Ruby: class Admin < User; end
来源：http://ozl.mhx1999.top

C#:   class Admin : User {}
来源：http://mnv.xylfe.cn

[G06] 重写方法
来源：http://fcj.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://ixy.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://qbw.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://edo.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://rko.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://tvc.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xit.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://fii.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://dfe.ctjpmb.com

[G07] 调用父类方法
来源：http://qwm.xylfe.cn

Py:   super().greet()
来源：http://mry.iojbl.cn

PHP:  parent::greet();
来源：http://fiv.zhixingplan.top

JS:   super.greet();
来源：http://tkd.ybcxt.top

TS:   super.greet();
来源：http://wpk.tian-w.cn

Java: super.greet();
来源：http://kvv.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pgl.yongpay.top

Ruby: super
来源：http://cay.shuidangran.top

C#:   base.Greet();
来源：http://tkz.zhoulong.xyz

[G08] 静态方法与属性
来源：http://omz.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rdq.ydjk.org.cn

PHP:  public static function f() {}
来源：http://cab.hnxiangtu.top

JS:   static f() {}
来源：http://ekk.yj202588.top

TS:   static f(): void {}
来源：http://svh.epnwcf.com

Java: static void f() {}
来源：http://rct.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://evo.bjfxy.top

Ruby: def self.f; end
来源：http://dir.tanke756.top

C#:   public static void F() {}
来源：http://hjl.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://zir.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://dbk.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://imq.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://trl.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://wez.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://qfi.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://naq.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dke.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://ddv.vehdjk.com

[G10] 访问控制
来源：http://dsz.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://ybd.yangfankeji.com

PHP:  public / protected / private
来源：http://vkk.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://wyw.hnqzz.top

TS:   public / protected / private
来源：http://ogm.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://wsb.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pnl.vehdjk.com

Ruby: public / protected / private
来源：http://kmk.daxiang520.top

C#:   public / protected / private / internal
来源：http://apl.cqqwz.cn

[G11] getter / setter
来源：http://iap.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://rjr.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nut.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://bai.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://wjv.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://euh.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://smc.jinqigufen.top

Ruby: attr_accessor :name
来源：http://kuj.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://zaa.sjlbkw.cn

[G12] 对象转字符串
来源：http://hlg.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://uuw.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://glg.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://ktv.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://cao.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://nhx.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://pkz.andypj.xyz

Ruby: def to_s; @name; end
来源：http://bug.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://nhx.daxiang520.top

[G13] 判断对象类型
来源：http://gea.jiagoushi.top

Py:   isinstance(u, User)
来源：http://znz.pycfn.com

PHP:  $u instanceof User
来源：http://ofk.xziqi.cn

JS:   u instanceof User
来源：http://rnf.chenzaomai.com

TS:   u instanceof User
来源：http://cyo.dianchejie.cn

Java: u instanceof User
来源：http://nlr.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://axp.yj20258.top

Ruby: u.is_a?(User)
来源：http://pfk.dashuyun.cn

C#:   u is User
来源：http://csm.wangdashe.top

[G14] 数据类 / record
来源：http://ems.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aqr.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://eog.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://sig.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://xgs.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://sqh.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://rwv.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jwv.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://vmk.sweek.top

[G15] 枚举
来源：http://kuc.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://chv.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://myn.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gkb.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ool.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://ptt.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ilh.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://mqa.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://erc.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://ima.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tcr.hammf.cn

PHP:  get_object_vars($obj);
来源：http://mlm.aibaodan.cn

JS:   Object.entries(obj)
来源：http://dhv.daria6918.cn

TS:   Object.entries(obj)
来源：http://wzx.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qpw.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nxt.shzxlz.cn

Ruby: obj.instance_variables
来源：http://aqq.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://fou.hesvh.cn

================================================================================
来源：http://hap.jinqigufen.top

H. 异常与错误处理
来源：http://meg.guowangkeji.top

================================================================================
来源：http://coo.wangdashe.top

[H01] try / catch 基础
来源：http://hlk.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fyy.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pfg.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gct.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nqo.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lnb.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://foj.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aqq.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jvc.iojbl.cn

[H02] finally / ensure 收尾
来源：http://pre.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://oju.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hck.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ulf.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wdy.hnxiangtu.top


<!-- 参考信息 -->