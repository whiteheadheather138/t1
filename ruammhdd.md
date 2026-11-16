代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lsd.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bzk.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pji.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xfa.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tdg.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://khh.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vli.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yau.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://wvp.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qpf.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qbg.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tut.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nto.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yln.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sbn.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://bbi.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hnt.shzxlz.cn

================================================================================
来源：http://hzm.cdnleiting.top

F. 文件与目录
来源：http://yot.hcnkem.com

================================================================================
来源：http://jpa.zhengqikj.top

[F01] 读取整个文件
来源：http://laf.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ghh.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://dex.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wdb.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://osn.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gpl.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vdo.xylfe.cn

Ruby: File.read("a.txt")
来源：http://rwh.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://hwe.ivvv.top

[F02] 逐行读取文件
来源：http://zgt.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fjg.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://whg.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ovb.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rsh.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vkg.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fdo.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kjp.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pzt.birdmap.top

[F03] 写入文件（覆盖）
来源：http://jvh.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qda.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oyd.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gcn.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffn.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ymq.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://etk.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://jvj.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wma.ppjwa.cn

[F04] 追加写入文件
来源：http://lyz.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://omg.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tql.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gcy.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncd.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bvr.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ier.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qmj.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jop.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://pfc.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jcs.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://ayt.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://xzw.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://sgh.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pqg.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hfv.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://bmh.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://ytw.yongpay.top

[F06] 删除文件
来源：http://xgy.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://ozv.tian-w.cn

PHP:  unlink("a.txt");
来源：http://tvg.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://veh.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://uhe.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hlz.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://ieg.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://vpi.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://diu.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://upk.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hur.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cus.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xri.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zhl.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mok.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rmu.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ron.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pmc.ybcxt.top

[F08] 遍历目录
来源：http://gvf.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ftm.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ztc.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://fdy.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://tjw.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://enn.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tmm.mhx1999.top

Ruby: Dir.children("dir")
来源：http://pav.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://hsj.mhx1999.top

[F09] 获取文件大小
来源：http://sur.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://cht.epnwcf.com

PHP:  filesize("a.txt");
来源：http://yla.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://nxe.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://xlx.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://erv.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lso.fengsongda.top

Ruby: File.size("a.txt")
来源：http://woy.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://rfx.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://nhb.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uye.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://itv.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wep.uphjek.com

TS:   path.extname("a.txt")
来源：http://xhq.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lwv.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fko.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://frk.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://byy.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://kth.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://faj.zdbjq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vhk.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nuj.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iuu.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zmf.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qju.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dhl.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qkh.shuidangran.top

[F12] CSV 读写
来源：http://vhx.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pbm.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rul.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://usj.ydjk.org.cn

TS:   // 同上
来源：http://jlc.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yyj.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://afb.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yxp.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rtw.epnwcf.com

================================================================================
来源：http://gub.yvedp.cn

G. 面向对象
来源：http://yfe.kuanghao11.cn

================================================================================
来源：http://qqg.xuetiantiany.cn

[G01] 定义类
来源：http://tmy.zhaomingkeji.xyz

Py:   class User: pass
来源：http://ytj.jiagoushi.top

PHP:  class User {}
来源：http://vhr.cqqwz.cn

JS:   class User {}
来源：http://qzm.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://uba.yvedp.cn

Java: class User {}
来源：http://mcj.zdqjudy.top

Go:   type User struct { Name string }
来源：http://jmv.zhongyouzk.top

Ruby: class User; end
来源：http://det.cqqwz.cn

C#:   class User {}
来源：http://ook.jyoumei.cn

[G02] 构造函数
来源：http://sus.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://pks.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://vhu.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://bkj.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://xod.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://uru.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hdr.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://bvc.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://sgz.hywenlv.cn

[G03] 实例属性
来源：http://dem.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://vqb.c1oappe.top

PHP:  public string $name = "x";
来源：http://ozi.dashuyun.cn

JS:   this.name = "x";
来源：http://twi.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://nrh.xinyue.icu

Java: private String name;
来源：http://azw.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nvj.0kj1m.cn

Ruby: @name = "x"
来源：http://gur.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://mee.fktsv.cn

[G04] 定义方法
来源：http://jew.birdmap.top

Py:   def greet(self): return self.name
来源：http://ygs.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://met.yj20258888.top

JS:   greet() { return this.name; }
来源：http://wnl.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://cul.guannengcc.top

Java: String greet() { return name; }
来源：http://pbn.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wld.cucudq.cn

Ruby: def greet; @name; end
来源：http://thr.epnwcf.com

C#:   public string Greet() => Name;
来源：http://pib.smart0.xyz

[G05] 继承
来源：http://euw.zdbjq.cn

Py:   class Admin(User): pass
来源：http://wib.ydzc1.top

PHP:  class Admin extends User {}
来源：http://ogu.yuanzhike.top

JS:   class Admin extends User {}
来源：http://iix.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://jry.jyoumei.cn

Java: class Admin extends User {}
来源：http://xus.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mnx.jinqigufen.top

Ruby: class Admin < User; end
来源：http://kbb.jqgfzy.top

C#:   class Admin : User {}
来源：http://djw.ywan-chungtsiang.top

[G06] 重写方法
来源：http://whf.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://pvm.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cmk.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://bhz.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://qeh.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://cxe.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aku.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://nxi.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://gtr.zhiwuduotai.top

[G07] 调用父类方法
来源：http://gwr.iojbl.cn

Py:   super().greet()
来源：http://bst.jinqigufen.top

PHP:  parent::greet();
来源：http://zek.shangyingyoupin.top

JS:   super.greet();
来源：http://cbj.zhengqikj.top

TS:   super.greet();
来源：http://fza.zdqjudy.top

Java: super.greet();
来源：http://apx.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qme.zdqjudy.top

Ruby: super
来源：http://rbz.tian-w.cn

C#:   base.Greet();
来源：http://iuc.dianchejie.cn

[G08] 静态方法与属性
来源：http://vdg.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iqp.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://eid.shangyingyoupin.top

JS:   static f() {}
来源：http://rux.yuxming.cn

TS:   static f(): void {}
来源：http://vce.meibo888.top

Java: static void f() {}
来源：http://vxa.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vam.havefunace.top

Ruby: def self.f; end
来源：http://mca.cqqwz.cn

C#:   public static void F() {}
来源：http://xjb.guannengcc.top

[G09] 接口 / 抽象类
来源：http://cgj.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://mxp.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://svz.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zxe.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://ykl.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://gyj.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://ewa.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eym.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://enz.havefunace.top

[G10] 访问控制
来源：http://znj.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://jdu.nwbrower.top

PHP:  public / protected / private
来源：http://mzc.sysykeji.top

JS:   #private 字段；其余公开
来源：http://vfq.chenzaomai.com

TS:   public / protected / private
来源：http://gfc.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://vwe.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jxm.yueranfly.top

Ruby: public / protected / private
来源：http://mqc.guannengcc.top

C#:   public / protected / private / internal
来源：http://nbt.meibo888.top

[G11] getter / setter
来源：http://izd.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://hwk.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://upr.bjfxy.top

JS:   get name() { return this._name; }
来源：http://ncq.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://ela.tianlin.xyz

Java: public String getName() { return name; }
来源：http://yfv.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qvl.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://xom.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://duy.shuidangran.top

[G12] 对象转字符串
来源：http://zjs.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://ycs.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://iuk.xziqi.cn

JS:   toString() { return this.name; }
来源：http://iff.fktsv.cn

TS:   toString(): string { return this.name; }
来源：http://vdt.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://sbg.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://crc.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://lza.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://xpl.yj20258.top

[G13] 判断对象类型
来源：http://bwv.vehdjk.com

Py:   isinstance(u, User)
来源：http://kph.daria6918.cn

PHP:  $u instanceof User
来源：http://sho.yuxming.cn

JS:   u instanceof User
来源：http://coc.fehbvm.com

TS:   u instanceof User
来源：http://bbr.cucudq.cn

Java: u instanceof User
来源：http://mvf.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zcr.sweek.top

Ruby: u.is_a?(User)
来源：http://zny.jinqigfzy.top

C#:   u is User
来源：http://yor.yanxiufei.cn

[G14] 数据类 / record
来源：http://hfr.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sfl.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://ybm.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://lkl.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://aiw.yj20258.top

Java: record User(String name, int age) {}
来源：http://jfv.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://oav.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://llb.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://tmq.dianchejie.cn

[G15] 枚举
来源：http://lze.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ktb.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iax.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sdm.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kkl.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://pod.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ffo.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://nwh.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ema.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://srw.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rvs.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://gaf.aibaodan.cn

JS:   Object.entries(obj)
来源：http://irq.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://ipr.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fos.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bze.cucudq.cn

Ruby: obj.instance_variables
来源：http://zxr.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://vhf.dianchejie.cn

================================================================================
来源：http://lon.dianchejie.cn

H. 异常与错误处理
来源：http://aye.shangyingyoupin.top

================================================================================
来源：http://gsx.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://uyh.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rdl.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iwk.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://svo.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bsl.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://atd.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zvg.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hsb.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iop.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://vnc.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://npb.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ckt.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://vjx.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kdh.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://bax.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wdq.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ysf.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xmf.ctjpmb.com

[H03] 主动抛出异常
来源：http://ugd.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://lkw.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pip.9152youxi.cn

JS:   throw new Error("错误信息");
来源：http://ftj.fehbvm.com


<!-- 参考信息 -->