代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sml.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://cky.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dan.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cot.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://pvj.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nsq.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gqd.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uny.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jyo.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://edu.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ill.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://kgv.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tzf.yj20258.top

================================================================================
来源：http://bia.ybcxt.top

F. 文件与目录
来源：http://ebj.ctjpmb.com

================================================================================
来源：http://eef.jinyuanbaomall.cn

[F01] 读取整个文件
来源：http://thz.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eei.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://ozp.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cwb.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vqq.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://msq.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qtf.nwbrower.top

Ruby: File.read("a.txt")
来源：http://fdv.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ray.cqqwz.cn

[F02] 逐行读取文件
来源：http://xpj.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://chw.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xjc.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ade.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vdo.ehwqpu.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ycm.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://auz.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gwy.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rrl.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://gpj.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mmq.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ajd.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ojn.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zvi.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mgc.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://utd.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://bte.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aij.jinqigfzy.top

[F04] 追加写入文件
来源：http://dus.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uld.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pos.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqw.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vzm.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ony.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dmx.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ojz.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jdq.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://mbh.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sru.sweek.top

PHP:  file_exists("a.txt");
来源：http://yxw.meibo888.top

JS:   fs.existsSync("a.txt")
来源：http://rcl.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://njf.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bja.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rlp.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://axa.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://vus.wangdashe.top

[F06] 删除文件
来源：http://xfj.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://jze.daxiang520.top

PHP:  unlink("a.txt");
来源：http://zdl.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mhl.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dvo.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ync.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://bdz.yongpay.top

Ruby: File.delete("a.txt")
来源：http://ani.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://tkt.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://bfc.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xaj.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tcw.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aly.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ujf.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxb.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hrz.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zqa.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nhz.haohaochexian.top

[F08] 遍历目录
来源：http://qhx.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lxr.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wsi.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://dxw.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://swx.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://djz.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dpv.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://esa.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://jmn.redwolf501.top

[F09] 获取文件大小
来源：http://cuk.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://okg.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://ayi.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://rbo.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://fwk.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vlf.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwk.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://tjs.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://hvy.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://aqg.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ffr.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nro.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cxd.iojbl.cn

TS:   path.extname("a.txt")
来源：http://hof.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vlw.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhf.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bew.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lsr.uphjek.com

[F11] 复制与移动文件
来源：http://rwd.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://myj.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vqr.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ehx.fengsongda.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://opz.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ebp.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dwb.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pdb.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qeg.epnwcf.com

[F12] CSV 读写
来源：http://xqb.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ytp.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://maq.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://idn.shanyushiyangtech.top

TS:   // 同上
来源：http://xrq.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aev.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gkb.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://llf.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://uyt.cqqwz.cn

================================================================================
来源：http://ajc.daxiang520.top

G. 面向对象
来源：http://fhm.snrcjt.cn

================================================================================
来源：http://owj.yonumen.top

[G01] 定义类
来源：http://rku.andypj.xyz

Py:   class User: pass
来源：http://ysa.birdmap.top

PHP:  class User {}
来源：http://kgr.sxryk.cn

JS:   class User {}
来源：http://ppp.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://jla.nwbrower.top

Java: class User {}
来源：http://gxc.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://zge.xziqi.cn

Ruby: class User; end
来源：http://odo.52xcode.cn

C#:   class User {}
来源：http://rlr.zhoulong.xyz

[G02] 构造函数
来源：http://qdx.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://skq.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://ekl.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://tyk.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://rif.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://tnr.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hit.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://zul.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://arq.svipenyu.cn

[G03] 实例属性
来源：http://mkt.ybcxt.top

Py:   self.name = "x"
来源：http://rry.xylfe.cn

PHP:  public string $name = "x";
来源：http://aok.cqqwz.cn

JS:   this.name = "x";
来源：http://xpz.zhongyouzk.top

TS:   name: string = "x";
来源：http://uvk.bjfxy.top

Java: private String name;
来源：http://fhn.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cmn.xuetiantiany.cn

Ruby: @name = "x"
来源：http://kvk.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://cpc.daxiang520.top

[G04] 定义方法
来源：http://rqx.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://nsj.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dzd.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://rxa.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://mzv.zdbjq.cn

Java: String greet() { return name; }
来源：http://qlq.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://msq.xuanzx.com

Ruby: def greet; @name; end
来源：http://vyp.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://ttv.vehdjk.com

[G05] 继承
来源：http://llj.chenzaomai.com

Py:   class Admin(User): pass
来源：http://jpn.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://mbn.dianchejie.cn

JS:   class Admin extends User {}
来源：http://jkg.fktsv.cn

TS:   class Admin extends User {}
来源：http://ifa.hnqzz.top

Java: class Admin extends User {}
来源：http://mdp.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sxe.havefunace.top

Ruby: class Admin < User; end
来源：http://fgg.chenzaomai.com

C#:   class Admin : User {}
来源：http://syx.hesvh.cn

[G06] 重写方法
来源：http://wta.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://urw.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fba.yj20258.top

JS:   greet() { return "admin"; }
来源：http://iiy.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://mmg.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://hwj.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ist.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://bjr.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://mns.shangyingyoupin.top

[G07] 调用父类方法
来源：http://ozm.redwolf501.top

Py:   super().greet()
来源：http://amb.daria6918.cn

PHP:  parent::greet();
来源：http://bkf.9152youxi.cn

JS:   super.greet();
来源：http://lbg.yongpay.top

TS:   super.greet();
来源：http://hip.daria6918.cn

Java: super.greet();
来源：http://kpj.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pee.jyoumei.cn

Ruby: super
来源：http://czn.ppjwa.cn

C#:   base.Greet();
来源：http://sie.wangdashe.top

[G08] 静态方法与属性
来源：http://nrp.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hfj.sysykeji.top

PHP:  public static function f() {}
来源：http://obp.yanxiufei.cn

JS:   static f() {}
来源：http://jjm.tarul.cn

TS:   static f(): void {}
来源：http://mhf.nanxinkj.top

Java: static void f() {}
来源：http://qqy.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yzh.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://kyj.shangyingyoupin.top

C#:   public static void F() {}
来源：http://lek.mhx1999.top

[G09] 接口 / 抽象类
来源：http://qep.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://rin.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://zyh.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cfh.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://xfe.hesvh.cn

Java: interface Shape { double area(); }
来源：http://syf.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://bts.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ldg.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://knf.haohaochexian.top

[G10] 访问控制
来源：http://abx.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://kxb.sjlbkw.cn

PHP:  public / protected / private
来源：http://rwx.mhx1999.top

JS:   #private 字段；其余公开
来源：http://iay.ydjk.org.cn

TS:   public / protected / private
来源：http://ckr.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://sma.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jqk.iojbl.cn

Ruby: public / protected / private
来源：http://uld.ivvv.top

C#:   public / protected / private / internal
来源：http://agf.fktsv.cn

[G11] getter / setter
来源：http://xbp.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://wlk.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ohq.yj202588.top

JS:   get name() { return this._name; }
来源：http://rim.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://qlx.mhx1999.top

Java: public String getName() { return name; }
来源：http://qyp.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yhz.wangdashe.top

Ruby: attr_accessor :name
来源：http://rrj.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://iob.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://kjj.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://utb.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://stc.yongpay.top

JS:   toString() { return this.name; }
来源：http://qtw.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://dib.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://oma.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fms.havefunace.top

Ruby: def to_s; @name; end
来源：http://xkh.316326.xyz

C#:   public override string ToString() => Name;
来源：http://mzu.chenlongwang.top

[G13] 判断对象类型
来源：http://hnt.jqgfzy.top

Py:   isinstance(u, User)
来源：http://kva.xylfe.cn

PHP:  $u instanceof User
来源：http://hwg.yueranfly.top

JS:   u instanceof User
来源：http://upi.mhx1999.top

TS:   u instanceof User
来源：http://vzu.yuanzhike.top

Java: u instanceof User
来源：http://uqr.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qzl.hnqzz.top

Ruby: u.is_a?(User)
来源：http://tll.yuanzhike.top

C#:   u is User
来源：http://lek.pengpengdd.cyou

[G14] 数据类 / record
来源：http://flx.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iwf.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://xrp.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://enf.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://jfi.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://lsk.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://plq.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lxq.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://zrw.epnwcf.com

[G15] 枚举
来源：http://sux.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yaa.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sha.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uee.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lsz.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://lcq.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://din.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://cmi.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xro.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://qel.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kjs.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://fax.yj202588.top

JS:   Object.entries(obj)
来源：http://kgb.andypj.xyz

TS:   Object.entries(obj)
来源：http://xta.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tns.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://ool.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://koj.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://peg.yvedp.cn

================================================================================
来源：http://jpo.nanxuanxn.top

H. 异常与错误处理
来源：http://cdn.nanxinkj.top

================================================================================
来源：http://omf.chenjidiqi.icu

[H01] try / catch 基础
来源：http://exz.hnxiangtu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iuo.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nea.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dac.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ovp.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bxm.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ixv.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qhv.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wkk.yonumen.top

[H02] finally / ensure 收尾
来源：http://fvg.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vmj.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uwy.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cfj.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rwd.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://gdk.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uos.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aju.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zfd.ydzc1.top

[H03] 主动抛出异常
来源：http://syg.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://xks.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gpd.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://jhl.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://psv.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://weu.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rhi.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xca.daxiang520.top


<!-- 参考信息 -->