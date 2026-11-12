代发 wailian999

Go:   if s == "" {}
来源：http://gbt.chenlongwang.top

Ruby: if s.empty?
来源：http://tap.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://puv.meibo888.top

[E21] 超长截断加省略号
来源：http://npk.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xhx.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xef.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obg.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ruk.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bbc.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://wol.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zbn.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qeb.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://byw.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aya.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aye.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://urx.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jav.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://chv.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xhr.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://jez.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://djp.hammf.cn

================================================================================
来源：http://crs.yuanzhike.top

F. 文件与目录
来源：http://czj.vqdsnc.cn

================================================================================
来源：http://ybn.zhiwuduotai.top

[F01] 读取整个文件
来源：http://lrh.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rvi.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://wrw.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://czg.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xdm.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eky.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cyb.bjfxy.top

Ruby: File.read("a.txt")
来源：http://asa.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://yii.tarul.cn

[F02] 逐行读取文件
来源：http://hcx.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baz.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gfs.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wtq.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpe.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://era.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dcp.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ykg.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eos.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://aqj.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lgu.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ccx.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jkw.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pav.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wzm.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qpq.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://nlh.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwp.dashuyun.cn

[F04] 追加写入文件
来源：http://hyi.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfo.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iff.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://stt.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iqz.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vxm.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eho.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://piw.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lqi.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://ozf.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pwi.uphjek.com

PHP:  file_exists("a.txt");
来源：http://pjv.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://vky.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://tmb.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uxj.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wbm.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://cgr.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://pxh.cdnleiting.top

[F06] 删除文件
来源：http://unm.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://mbz.birdmap.top

PHP:  unlink("a.txt");
来源：http://ekg.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://lsk.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ovr.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cxd.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://zyx.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://bco.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://pyt.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://dcx.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uik.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pvk.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wls.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqo.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kiz.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjd.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aqj.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://omt.yangfankeji.com

[F08] 遍历目录
来源：http://tmb.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vhk.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pvd.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://ray.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://pjz.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vlc.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://yvl.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://vzg.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://cfm.ydzc1.top

[F09] 获取文件大小
来源：http://mmr.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://qhf.fengsongda.top

PHP:  filesize("a.txt");
来源：http://nrb.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://dga.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://fuj.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://chv.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://goj.yongpay.top

Ruby: File.size("a.txt")
来源：http://wao.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://bwq.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://msm.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://asg.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pkw.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zpv.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://cth.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tdn.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hib.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wkz.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zgs.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://yse.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jaz.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mlb.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qoa.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgu.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kwm.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nqm.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iov.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iwk.jinqigufen.top

[F12] CSV 读写
来源：http://uek.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nfj.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xyb.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijp.haohaochexian.top

TS:   // 同上
来源：http://mlg.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rla.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bdi.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://csz.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ndk.chenlongwang.top

================================================================================
来源：http://qah.yfazqb.com

G. 面向对象
来源：http://siu.yfazqb.com

================================================================================
来源：http://axo.guannengcc.top

[G01] 定义类
来源：http://ppu.ctjpmb.com

Py:   class User: pass
来源：http://qcp.pengpengdd.cyou

PHP:  class User {}
来源：http://prp.ppjwa.cn

JS:   class User {}
来源：http://nxi.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://wjf.yanxiufei.cn

Java: class User {}
来源：http://snc.cqqwz.cn

Go:   type User struct { Name string }
来源：http://kqz.fehbvm.com

Ruby: class User; end
来源：http://jbn.hfpthk.cn

C#:   class User {}
来源：http://yns.chenjidiqi.icu

[G02] 构造函数
来源：http://kgy.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ncm.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://ifj.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://ebo.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://mjc.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://ztn.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ght.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://grp.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://bjr.chenjidiqi.icu

[G03] 实例属性
来源：http://xrc.guannengcc.top

Py:   self.name = "x"
来源：http://erh.hnqzz.top

PHP:  public string $name = "x";
来源：http://sux.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://htz.pengpengdd.cyou

TS:   name: string = "x";
来源：http://qto.tianlin.xyz

Java: private String name;
来源：http://vwr.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dea.tian-w.cn

Ruby: @name = "x"
来源：http://rhr.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://adj.xuetiantiany.cn

[G04] 定义方法
来源：http://neq.yj20258.top

Py:   def greet(self): return self.name
来源：http://xcn.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://eya.tian-w.cn

JS:   greet() { return this.name; }
来源：http://bge.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://zgy.zycfv.cn

Java: String greet() { return name; }
来源：http://tkm.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ncr.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://evx.52xcode.cn

C#:   public string Greet() => Name;
来源：http://hqu.xingfuxueyuan.xyz

[G05] 继承
来源：http://aal.chenlongwang.top

Py:   class Admin(User): pass
来源：http://sip.cashguo.top

PHP:  class Admin extends User {}
来源：http://njs.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://ocy.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://avz.bbcook.cn

Java: class Admin extends User {}
来源：http://dkn.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fsy.gzhubu.top

Ruby: class Admin < User; end
来源：http://gxx.epnwcf.com

C#:   class Admin : User {}
来源：http://hvr.feifeiyinyue.top

[G06] 重写方法
来源：http://alh.yongpay.top

Py:   def greet(self): return "admin"
来源：http://cuz.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://byi.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://mle.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://bbm.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://dka.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pqb.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://fqy.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://pko.jianghu66.top

[G07] 调用父类方法
来源：http://xrr.fengsongda.top

Py:   super().greet()
来源：http://ckm.yvedp.cn

PHP:  parent::greet();
来源：http://izl.yj20258.top

JS:   super.greet();
来源：http://epv.mhx1999.top

TS:   super.greet();
来源：http://rvv.jianghu66.top

Java: super.greet();
来源：http://owd.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gwk.xylfe.cn

Ruby: super
来源：http://ufw.bjfxy.top

C#:   base.Greet();
来源：http://ugs.jlsjyb.cn

[G08] 静态方法与属性
来源：http://jpe.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hvf.haohaochexian.top

PHP:  public static function f() {}
来源：http://xkq.zhengqikj.top

JS:   static f() {}
来源：http://nix.chenlongwang.top

TS:   static f(): void {}
来源：http://jwe.zhengqikj.top

Java: static void f() {}
来源：http://dzo.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://agh.cheryme.top

Ruby: def self.f; end
来源：http://xks.ydjk.org.cn

C#:   public static void F() {}
来源：http://exx.yvedp.cn

[G09] 接口 / 抽象类
来源：http://zey.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://qrt.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lpe.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://caq.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://ral.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://ilm.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://xme.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rdp.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://yxn.ywan-chungtsiang.top

[G10] 访问控制
来源：http://swq.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://oqk.aizwys.cn

PHP:  public / protected / private
来源：http://lbs.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://zwh.ehwqpu.com

TS:   public / protected / private
来源：http://fno.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://lyx.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ijf.yuanzhike.top

Ruby: public / protected / private
来源：http://qjy.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://krh.shuidangran.top

[G11] getter / setter
来源：http://aby.daria6918.cn

Py:   @property 与 @x.setter
来源：http://nkf.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jaj.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://zrv.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://zjx.snrcjt.cn

Java: public String getName() { return name; }
来源：http://ala.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://awt.ctjpmb.com

Ruby: attr_accessor :name
来源：http://kqe.yuxming.cn

C#:   public string Name { get; set; }
来源：http://mly.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://wxe.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://msd.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://njv.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://qfi.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://fcg.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://pzf.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zeo.andypj.xyz

Ruby: def to_s; @name; end
来源：http://ttm.yonumen.top

C#:   public override string ToString() => Name;
来源：http://uos.zhiwuduotai.top

[G13] 判断对象类型
来源：http://mjy.9152youxi.cn

Py:   isinstance(u, User)
来源：http://yig.daxiang520.top

PHP:  $u instanceof User
来源：http://lcx.dianchejie.cn

JS:   u instanceof User
来源：http://lga.fktsv.cn

TS:   u instanceof User
来源：http://gpx.ehwqpu.com

Java: u instanceof User
来源：http://ank.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://fwv.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://box.hysaishi.cn

C#:   u is User
来源：http://phc.pengpengdd.cyou

[G14] 数据类 / record
来源：http://eqd.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zvl.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://ebh.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://avg.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://thr.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://jzo.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://owa.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zxu.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://mnj.0kj1m.cn

[G15] 枚举
来源：http://ttq.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qss.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vho.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nbh.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fcv.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://kxi.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ytv.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://bby.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ghp.sweek.top

[G16] 对象转数组 / 字典
来源：http://dpd.sxryk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kzd.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://lpx.hammf.cn

JS:   Object.entries(obj)
来源：http://nff.iojbl.cn

TS:   Object.entries(obj)
来源：http://enr.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rhq.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jkg.fzhhl.top

Ruby: obj.instance_variables
来源：http://rcu.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://ifu.chenjidiqi.icu

================================================================================
来源：http://mvc.sjlbkw.cn

H. 异常与错误处理
来源：http://xes.tianlin.xyz

================================================================================
来源：http://bxn.9152youxi.cn

[H01] try / catch 基础
来源：http://tbe.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mwj.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dyd.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eki.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ear.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oqj.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fux.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rdh.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ljw.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://dav.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://cmg.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jzw.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kao.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ymx.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ium.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iig.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://auz.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmt.zdqjudy.top


<!-- 参考信息 -->