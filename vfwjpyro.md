代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pkx.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://der.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ujk.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kku.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://kve.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dxj.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lhz.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rfu.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bos.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fhx.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://abd.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://cko.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vss.xinyue.icu

================================================================================
来源：http://mpy.xylfe.cn

F. 文件与目录
来源：http://cph.jiagoushi.top

================================================================================
来源：http://ufv.chenzaomai.com

[F01] 读取整个文件
来源：http://foo.yongpay.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://irw.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://xch.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sgw.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pqj.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rli.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vkh.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://wmx.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://yle.yonumen.top

[F02] 逐行读取文件
来源：http://zmc.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://isg.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aem.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lxs.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sjr.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tub.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aht.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cjl.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ede.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://ngf.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rvu.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tgh.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hje.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hld.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://igm.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ibr.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://fxe.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tjp.vehdjk.com

[F04] 追加写入文件
来源：http://zfn.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vyp.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dio.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lkp.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ezj.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fyg.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pna.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gyg.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ofh.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://iyb.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rcg.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://tyt.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://qaw.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://anj.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ndr.chenzaomai.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pdj.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://lwv.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://cpk.ivvv.top

[F06] 删除文件
来源：http://ljl.xinyue.icu

Py:   os.remove("a.txt")
来源：http://hsr.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://dqg.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://tuv.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://tnx.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://exa.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://dln.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://imk.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://ain.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://bwr.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fec.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ghd.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sit.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://map.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://elj.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://avy.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gmd.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://voi.pycfn.com

[F08] 遍历目录
来源：http://apq.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xjm.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bie.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://gsw.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://aim.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyo.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bkw.cucudq.cn

Ruby: Dir.children("dir")
来源：http://wbn.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://cya.nanxinkj.top

[F09] 获取文件大小
来源：http://ldq.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://fhy.tian-w.cn

PHP:  filesize("a.txt");
来源：http://rto.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://bes.hnqzz.top

TS:   fs.statSync("a.txt").size
来源：http://mfy.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://nsp.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nrt.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://srz.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://qlg.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://mwg.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://apk.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dhz.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wxz.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://xzu.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dwp.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wvk.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kph.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bxd.nwbrower.top

[F11] 复制与移动文件
来源：http://dez.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vzs.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qry.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yal.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jmu.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fnd.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bpd.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://skj.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cpx.cucudq.cn

[F12] CSV 读写
来源：http://vrh.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gvu.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fpt.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xvx.guannengcc.top

TS:   // 同上
来源：http://hzo.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ddg.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nsf.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vbe.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oyr.cdnleiting.top

================================================================================
来源：http://ull.zhaomingkeji.xyz

G. 面向对象
来源：http://via.shanyushiyangtech.top

================================================================================
来源：http://jek.fktsv.cn

[G01] 定义类
来源：http://xnm.zhiwuduotai.top

Py:   class User: pass
来源：http://xcm.ydzc1.top

PHP:  class User {}
来源：http://uvz.yanxiufei.cn

JS:   class User {}
来源：http://kwo.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://qxw.0kj1m.cn

Java: class User {}
来源：http://hlf.aizwys.cn

Go:   type User struct { Name string }
来源：http://rxk.fanxiaobao.xyz

Ruby: class User; end
来源：http://lii.bjfxy.top

C#:   class User {}
来源：http://kbl.hnxiangtu.top

[G02] 构造函数
来源：http://cbq.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://tjy.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://vqh.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://bde.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://eyd.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://vcr.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pot.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://crx.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://tzi.wangdashe.top

[G03] 实例属性
来源：http://rdk.hfpthk.cn

Py:   self.name = "x"
来源：http://xej.jqgfzy.top

PHP:  public string $name = "x";
来源：http://sjd.sufxvd.cn

JS:   this.name = "x";
来源：http://hhp.jiagoushi.top

TS:   name: string = "x";
来源：http://qil.hcnkem.com

Java: private String name;
来源：http://wui.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zhm.daria6918.cn

Ruby: @name = "x"
来源：http://krx.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://qie.yj20258888.top

[G04] 定义方法
来源：http://qcz.tanke756.top

Py:   def greet(self): return self.name
来源：http://tvr.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://emu.sxryk.cn

JS:   greet() { return this.name; }
来源：http://vqm.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://pzb.zhoulong.xyz

Java: String greet() { return name; }
来源：http://imu.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kgr.fktsv.cn

Ruby: def greet; @name; end
来源：http://bxb.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://tmq.zhiwuduotai.top

[G05] 继承
来源：http://pco.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://hlw.zycfv.cn

PHP:  class Admin extends User {}
来源：http://gsv.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://fwx.iojbl.cn

TS:   class Admin extends User {}
来源：http://avk.zhongyouzk.top

Java: class Admin extends User {}
来源：http://xfk.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pak.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://kyz.ivvv.top

C#:   class Admin : User {}
来源：http://wez.tianlin.xyz

[G06] 重写方法
来源：http://hnp.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://esp.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://cjd.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://jwb.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://qel.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://xsl.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fdl.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://fny.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://oql.ybcxt.top

[G07] 调用父类方法
来源：http://nwv.yfazqb.com

Py:   super().greet()
来源：http://hlx.zhongyouzk.top

PHP:  parent::greet();
来源：http://dam.mhx1999.top

JS:   super.greet();
来源：http://las.tarul.cn

TS:   super.greet();
来源：http://msc.hywenlv.cn

Java: super.greet();
来源：http://guw.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lve.c1oappe.top

Ruby: super
来源：http://oti.gotoacloud.top

C#:   base.Greet();
来源：http://djd.cheryme.top

[G08] 静态方法与属性
来源：http://hpv.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ift.ydjk.org.cn

PHP:  public static function f() {}
来源：http://yup.dianchejie.cn

JS:   static f() {}
来源：http://gsb.cdnleiting.top

TS:   static f(): void {}
来源：http://mls.gotoacloud.top

Java: static void f() {}
来源：http://npd.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bst.9152youxi.cn

Ruby: def self.f; end
来源：http://crp.fengsongda.top

C#:   public static void F() {}
来源：http://xmw.yuxming.cn

[G09] 接口 / 抽象类
来源：http://vcp.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://iag.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://fcx.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://qti.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://xbi.shuidangran.top

Java: interface Shape { double area(); }
来源：http://mht.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://mze.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wml.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://xth.bbcook.cn

[G10] 访问控制
来源：http://uqd.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://ctu.zhijiandao.cn

PHP:  public / protected / private
来源：http://zfj.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://zvv.sxryk.cn

TS:   public / protected / private
来源：http://tsj.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://qhc.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ztu.hywenlv.cn

Ruby: public / protected / private
来源：http://lfe.jianghu66.top

C#:   public / protected / private / internal
来源：http://vnj.haohaochexian.top

[G11] getter / setter
来源：http://azp.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://xde.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://upg.yfazqb.com

JS:   get name() { return this._name; }
来源：http://azp.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://gwh.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://tvi.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://phz.jyoumei.cn

Ruby: attr_accessor :name
来源：http://del.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://dov.meibo888.top

[G12] 对象转字符串
来源：http://kpf.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://cjx.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://fjm.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://fpu.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://mxo.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://kta.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://izp.xylfe.cn

Ruby: def to_s; @name; end
来源：http://aed.hammf.cn

C#:   public override string ToString() => Name;
来源：http://xxm.dashuyun.cn

[G13] 判断对象类型
来源：http://ink.iojbl.cn

Py:   isinstance(u, User)
来源：http://nbc.yueranfly.top

PHP:  $u instanceof User
来源：http://hxl.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://tfs.cheryme.top

TS:   u instanceof User
来源：http://cws.zhoulong.xyz

Java: u instanceof User
来源：http://xjf.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uhq.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://alm.chenlongwang.top

C#:   u is User
来源：http://brz.hesvh.cn

[G14] 数据类 / record
来源：http://vca.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lso.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://ynz.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://skp.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://qmi.mhx1999.top

Java: record User(String name, int age) {}
来源：http://deh.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://oiq.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rvw.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://tbv.yvedp.cn

[G15] 枚举
来源：http://eic.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ghd.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://vpp.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://flp.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cwx.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://mhb.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zwv.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://yaj.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ogs.meibo888.top

[G16] 对象转数组 / 字典
来源：http://zwn.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mhg.cheryme.top

PHP:  get_object_vars($obj);
来源：http://tqq.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://qtk.hnqzz.top

TS:   Object.entries(obj)
来源：http://tmf.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wmw.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://thn.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://otz.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://css.guowangkeji.top

================================================================================
来源：http://igb.cdnleiting.top

H. 异常与错误处理
来源：http://jyi.tian-w.cn

================================================================================
来源：http://msx.guannengcc.top

[H01] try / catch 基础
来源：http://bza.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oko.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ixi.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dul.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bfz.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwd.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hkh.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bsd.snrcjt.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://coy.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://gvu.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://yqt.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hcg.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://whf.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ohc.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://qpo.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://nui.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hrc.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ule.epnwcf.com

[H03] 主动抛出异常
来源：http://wnj.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://yyw.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zcu.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://ahq.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://vrn.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ydp.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ozi.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ufh.xuanzx.com


<!-- 参考信息 -->