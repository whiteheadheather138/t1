代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wlj.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://sfi.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://smc.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://acw.316326.xyz

[E22] 字节长度与字符长度
来源：http://jps.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gxz.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uji.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gtj.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wwf.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xnk.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zgt.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://btm.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://laz.jinghuilouyu.cn

================================================================================
来源：http://sdh.xziqi.cn

F. 文件与目录
来源：http://nvv.cdnleiting.top

================================================================================
来源：http://jhf.bbcook.cn

[F01] 读取整个文件
来源：http://afi.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sxb.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://cku.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dvh.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pmo.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xcj.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sbg.pycfn.com

Ruby: File.read("a.txt")
来源：http://avp.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://ruy.hammf.cn

[F02] 逐行读取文件
来源：http://oaj.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hus.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xfr.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzd.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lht.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lwz.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://muz.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mcw.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iug.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://mjx.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zys.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://lmx.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qne.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lda.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bvz.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ubs.zhaomingkeji.xyz

Ruby: File.write("a.txt", "hi")
来源：http://pnn.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://muv.jlsjyb.cn

[F04] 追加写入文件
来源：http://ujg.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zwt.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ksf.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://izc.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vcq.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aep.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blc.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uck.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tet.sweek.top

[F05] 判断文件或目录是否存在
来源：http://cnu.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ify.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://vwi.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://gmb.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://zxs.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://epj.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ocu.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://gjg.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://ecc.hongshengwenyu.top

[F06] 删除文件
来源：http://ace.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://zyo.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://tor.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://vkn.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://mvu.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wlg.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://gxf.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://gad.birdmap.top

C#:   File.Delete("a.txt");
来源：http://wbp.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://lef.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gxb.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cwp.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://akt.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxg.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yfi.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wgi.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://huy.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pqw.fengsongda.top

[F08] 遍历目录
来源：http://rfu.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://acy.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ywi.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://nvi.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://yxn.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyk.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tyy.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://xse.aibaodan.cn

C#:   Directory.GetFiles("dir")
来源：http://bvc.vqdsnc.cn

[F09] 获取文件大小
来源：http://rwb.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://kpi.epnwcf.com

PHP:  filesize("a.txt");
来源：http://rbl.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://xab.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://iav.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pxl.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mmh.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://yvj.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://esz.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://dsq.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bdc.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cct.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yaf.c1oappe.top

TS:   path.extname("a.txt")
来源：http://msh.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lnf.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yci.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mvn.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pku.redwolf501.top

[F11] 复制与移动文件
来源：http://zgl.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aoi.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mby.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vrd.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://znl.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://idf.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sek.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whb.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tbw.xuetiantiany.cn

[F12] CSV 读写
来源：http://nrj.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rav.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nji.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://skb.zhoulong.xyz

TS:   // 同上
来源：http://vpg.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://csn.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nga.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hpz.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pao.iojbl.cn

================================================================================
来源：http://hft.jqgufenzy.top

G. 面向对象
来源：http://zjk.jqgufenzy.top

================================================================================
来源：http://qeu.chenjidiqi.icu

[G01] 定义类
来源：http://fbv.guannengcc.top

Py:   class User: pass
来源：http://emk.cqqwz.cn

PHP:  class User {}
来源：http://vao.ppjwa.cn

JS:   class User {}
来源：http://ddi.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://dtm.shanyushiyangtech.top

Java: class User {}
来源：http://fbq.epnwcf.com

Go:   type User struct { Name string }
来源：http://gfe.cucudq.cn

Ruby: class User; end
来源：http://yqj.ydjk.org.cn

C#:   class User {}
来源：http://dpd.yongpay.top

[G02] 构造函数
来源：http://btf.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://dsr.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://itx.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://gjc.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://tyf.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://nje.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://szi.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://qfq.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://nek.hywenlv.cn

[G03] 实例属性
来源：http://tnq.hcnkem.com

Py:   self.name = "x"
来源：http://iab.hysaishi.cn

PHP:  public string $name = "x";
来源：http://xjz.wangshuangyany.cn

JS:   this.name = "x";
来源：http://knu.cheryme.top

TS:   name: string = "x";
来源：http://acr.yongpay.top

Java: private String name;
来源：http://kec.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mdv.xuetiantiany.cn

Ruby: @name = "x"
来源：http://lso.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://bli.hammf.cn

[G04] 定义方法
来源：http://qzi.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://wty.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://qkp.tian-w.cn

JS:   greet() { return this.name; }
来源：http://zoi.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://vty.fehbvm.com

Java: String greet() { return name; }
来源：http://llq.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gpl.yangfankeji.com

Ruby: def greet; @name; end
来源：http://kch.yongpay.top

C#:   public string Greet() => Name;
来源：http://hek.fzhhl.top

[G05] 继承
来源：http://wzm.epnwcf.com

Py:   class Admin(User): pass
来源：http://wqv.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://imw.cashguo.top

JS:   class Admin extends User {}
来源：http://mnt.yj20258888.top

TS:   class Admin extends User {}
来源：http://gej.meibo888.top

Java: class Admin extends User {}
来源：http://dad.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cqn.andypj.xyz

Ruby: class Admin < User; end
来源：http://rwb.aibaodan.cn

C#:   class Admin : User {}
来源：http://dsb.ydjk.org.cn

[G06] 重写方法
来源：http://enk.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://csh.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://imc.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://all.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://sdw.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://pix.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://spo.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://laa.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://tuj.xuetiantiany.cn

[G07] 调用父类方法
来源：http://wil.hongshengwenyu.top

Py:   super().greet()
来源：http://hhs.nanxinkj.top

PHP:  parent::greet();
来源：http://tdl.sxryk.cn

JS:   super.greet();
来源：http://uhp.zhijiandao.cn

TS:   super.greet();
来源：http://pes.jinqigufen.top

Java: super.greet();
来源：http://unm.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uhl.shzxlz.cn

Ruby: super
来源：http://vhk.cashguo.top

C#:   base.Greet();
来源：http://pzn.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://oro.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oky.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://eed.redwolf501.top

JS:   static f() {}
来源：http://tfr.cqqwz.cn

TS:   static f(): void {}
来源：http://nts.zhengqikj.top

Java: static void f() {}
来源：http://gtg.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tty.0kj1m.cn

Ruby: def self.f; end
来源：http://iid.ehwqpu.com

C#:   public static void F() {}
来源：http://qjj.zycfv.cn

[G09] 接口 / 抽象类
来源：http://vwn.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://swn.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oxh.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cwq.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://llt.sxryk.cn

Java: interface Shape { double area(); }
来源：http://uvf.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://ynd.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://flx.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://egh.shanyushiyangkeji.top

[G10] 访问控制
来源：http://cnk.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://vdt.yvedp.cn

PHP:  public / protected / private
来源：http://tkp.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://dwc.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://iiu.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://psg.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://knt.pycfn.com

Ruby: public / protected / private
来源：http://eno.guowangkeji.top

C#:   public / protected / private / internal
来源：http://ogy.jinqigufen.top

[G11] getter / setter
来源：http://rbh.aizwys.cn

Py:   @property 与 @x.setter
来源：http://qcq.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cza.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://mhb.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://kue.uphjek.com

Java: public String getName() { return name; }
来源：http://xrv.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bca.yongpay.top

Ruby: attr_accessor :name
来源：http://sav.havefunace.top

C#:   public string Name { get; set; }
来源：http://oxf.havefunace.top

[G12] 对象转字符串
来源：http://zrt.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://reo.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://flj.pycfn.com

JS:   toString() { return this.name; }
来源：http://ael.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://mmq.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://mpw.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://qiz.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://ral.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://yuu.aizwys.cn

[G13] 判断对象类型
来源：http://vsr.chenlongwang.top

Py:   isinstance(u, User)
来源：http://qpr.sjlbkw.cn

PHP:  $u instanceof User
来源：http://bqo.jiagoushi.top

JS:   u instanceof User
来源：http://lip.bbcook.cn

TS:   u instanceof User
来源：http://ejw.hysaishi.cn

Java: u instanceof User
来源：http://tnt.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://klf.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://fxe.quarkkingdee.top

C#:   u is User
来源：http://jzv.feifeiyinyue.top

[G14] 数据类 / record
来源：http://pqv.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ini.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://wyh.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://iiw.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://pws.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://lah.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://vui.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ogq.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://sqe.zhongyouzk.top

[G15] 枚举
来源：http://duc.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zel.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hwb.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qzt.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tvx.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://wrl.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ywc.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://khd.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jvk.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://cuu.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hwk.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://ogk.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://bxi.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://rxp.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gma.meibo888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fsf.vehdjk.com

Ruby: obj.instance_variables
来源：http://lzz.0kj1m.cn

C#:   // 用反射或 System.Text.Json
来源：http://owe.shangyingyoupin.top

================================================================================
来源：http://nqu.yangfankeji.com

H. 异常与错误处理
来源：http://xzq.cashguo.top

================================================================================
来源：http://jez.epnwcf.com

[H01] try / catch 基础
来源：http://mip.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bpv.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mmv.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bmw.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wzk.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lgr.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wxa.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tvh.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gbq.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://cpd.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://cyf.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://zno.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://gny.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nlz.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cyo.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nxd.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nwj.hongshengwenyu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eom.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://kiq.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://fyo.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wxp.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://ruj.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://bsj.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bux.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jgj.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://sav.ywan-chungtsiang.top


<!-- 参考信息 -->