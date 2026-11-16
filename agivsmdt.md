代发 wailian999

[E22] 字节长度与字符长度
来源：http://ruw.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zco.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://crk.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fos.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rwk.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://csy.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nui.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://gzu.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ixn.meibo888.top

================================================================================
来源：http://hkn.quarkkingdee.top

F. 文件与目录
来源：http://ukh.zhixingplan.top

================================================================================
来源：http://ric.0kj1m.cn

[F01] 读取整个文件
来源：http://gbo.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ryj.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://cmc.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zbg.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lzm.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uig.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iol.birdmap.top

Ruby: File.read("a.txt")
来源：http://xbe.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://syv.jianghu66.top

[F02] 逐行读取文件
来源：http://gqz.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cvk.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zvd.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzy.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ora.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hfn.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://icg.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ojq.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vms.yj20258.top

[F03] 写入文件（覆盖）
来源：http://uuk.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ysm.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://anz.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://stv.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ypk.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ebt.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qvh.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://oyn.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bhw.yuxming.cn

[F04] 追加写入文件
来源：http://wzo.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uuw.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mid.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://syo.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lkz.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://svm.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kwy.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://abr.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sfu.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://rep.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zrs.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://zyd.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://vfz.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://jjg.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ezw.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://soh.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://pou.meibo888.top

C#:   File.Exists("a.txt")
来源：http://cax.wangshuangyany.cn

[F06] 删除文件
来源：http://jze.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://mus.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://cxc.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ncp.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://yqj.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kkn.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://ipl.uphjek.com

Ruby: File.delete("a.txt")
来源：http://oko.birdmap.top

C#:   File.Delete("a.txt");
来源：http://icn.sysykeji.top

[F07] 创建目录（含多级）
来源：http://mex.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dqd.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ogt.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kxa.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bse.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ovx.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qup.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ajl.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kda.wangdashe.top

[F08] 遍历目录
来源：http://icc.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pww.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bdd.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://pfu.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://hxr.shanyushiyangtech.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hqb.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bcb.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://uje.guowangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://xjk.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://lda.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://yng.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://ysf.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://prx.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://hma.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://vnl.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwu.yuxming.cn

Ruby: File.size("a.txt")
来源：http://kie.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://vex.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://kyq.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://apg.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ubp.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dfp.havefunace.top

TS:   path.extname("a.txt")
来源：http://cjb.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aqk.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ijr.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://czx.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qvz.cqqwz.cn

[F11] 复制与移动文件
来源：http://hjz.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ocf.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kpu.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktl.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cjc.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nmz.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://niv.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ivx.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qix.hfpthk.cn

[F12] CSV 读写
来源：http://qbf.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bjs.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mvd.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nvj.shangyingyoupin.top

TS:   // 同上
来源：http://owa.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hun.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tku.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qrr.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jvl.ehwqpu.com

================================================================================
来源：http://wlr.shanyushiyangkeji.top

G. 面向对象
来源：http://tgd.vqdsnc.cn

================================================================================
来源：http://xkm.uphjek.com

[G01] 定义类
来源：http://tes.sxryk.cn

Py:   class User: pass
来源：http://voi.nwbrower.top

PHP:  class User {}
来源：http://pov.xuetiantiany.cn

JS:   class User {}
来源：http://dyp.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://ifz.tian-w.cn

Java: class User {}
来源：http://fig.316326.xyz

Go:   type User struct { Name string }
来源：http://ekh.zhijiandao.cn

Ruby: class User; end
来源：http://rzb.tian-w.cn

C#:   class User {}
来源：http://esa.xziqi.cn

[G02] 构造函数
来源：http://dlq.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://rqf.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://hdx.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://grh.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://ldt.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://vdv.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jjc.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://qqf.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://nql.nanxinkj.top

[G03] 实例属性
来源：http://yko.fengsongda.top

Py:   self.name = "x"
来源：http://yeb.hysaishi.cn

PHP:  public string $name = "x";
来源：http://zwb.ybcxt.top

JS:   this.name = "x";
来源：http://nne.vqdsnc.cn

TS:   name: string = "x";
来源：http://skt.shuidangran.top

Java: private String name;
来源：http://nlp.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wcg.jinqigfzy.top

Ruby: @name = "x"
来源：http://gfe.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://hmx.daria6918.cn

[G04] 定义方法
来源：http://sxe.pycfn.com

Py:   def greet(self): return self.name
来源：http://gft.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fgt.guannengcc.top

JS:   greet() { return this.name; }
来源：http://jcj.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://qvx.ppjwa.cn

Java: String greet() { return name; }
来源：http://npk.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ehq.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://vlz.xylfe.cn

C#:   public string Greet() => Name;
来源：http://fjw.meibo888.top

[G05] 继承
来源：http://kbp.tianlin.xyz

Py:   class Admin(User): pass
来源：http://anp.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://lhs.bbcook.cn

JS:   class Admin extends User {}
来源：http://efm.dianchejie.cn

TS:   class Admin extends User {}
来源：http://csi.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://wse.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://onu.bjfxy.top

Ruby: class Admin < User; end
来源：http://mce.hfpthk.cn

C#:   class Admin : User {}
来源：http://wdz.yonumen.top

[G06] 重写方法
来源：http://nqh.kuanghao11.cn

Py:   def greet(self): return "admin"
来源：http://uji.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://emf.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://uxo.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://vyg.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://yji.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nzo.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://zfd.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://vsy.redwolf501.top

[G07] 调用父类方法
来源：http://ovc.cucudq.cn

Py:   super().greet()
来源：http://bof.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://gkp.hfpthk.cn

JS:   super.greet();
来源：http://acr.vqdsnc.cn

TS:   super.greet();
来源：http://trf.zhijiandao.cn

Java: super.greet();
来源：http://hzx.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://urg.0kj1m.cn

Ruby: super
来源：http://ziz.hnqzz.top

C#:   base.Greet();
来源：http://obe.hfpthk.cn

[G08] 静态方法与属性
来源：http://tcx.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nkz.smart0.xyz

PHP:  public static function f() {}
来源：http://ixk.guowangkeji.top

JS:   static f() {}
来源：http://why.gotoacloud.top

TS:   static f(): void {}
来源：http://iqp.dianchejie.cn

Java: static void f() {}
来源：http://bza.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iui.svipenyu.cn

Ruby: def self.f; end
来源：http://fwf.ydzc1.top

C#:   public static void F() {}
来源：http://rci.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://ayj.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://ljd.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://wlb.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tvu.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://jwc.vehdjk.com

Java: interface Shape { double area(); }
来源：http://ykk.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://kki.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://icx.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://ukl.jinyuanbaomall.cn

[G10] 访问控制
来源：http://gam.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://jgm.9152youxi.cn

PHP:  public / protected / private
来源：http://wuc.xuanzx.com

JS:   #private 字段；其余公开
来源：http://vto.316326.xyz

TS:   public / protected / private
来源：http://xxc.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://jcn.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://whp.shangyingyoupin.top

Ruby: public / protected / private
来源：http://zmm.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://mht.uphjek.com

[G11] getter / setter
来源：http://yef.hcnkem.com

Py:   @property 与 @x.setter
来源：http://rsy.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://jdn.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://wrv.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://wsw.gogol.net.cn

Java: public String getName() { return name; }
来源：http://qun.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://een.yuanzhike.top

Ruby: attr_accessor :name
来源：http://oll.yonumen.top

C#:   public string Name { get; set; }
来源：http://xnv.yanxiufei.cn

[G12] 对象转字符串
来源：http://lkv.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://ufm.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oom.andypj.xyz

JS:   toString() { return this.name; }
来源：http://dhk.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://dli.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://hky.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://dve.sweek.top

Ruby: def to_s; @name; end
来源：http://oyv.cashguo.top

C#:   public override string ToString() => Name;
来源：http://uep.uphjek.com

[G13] 判断对象类型
来源：http://uka.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://npo.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://wqu.zycfv.cn

JS:   u instanceof User
来源：http://gde.yangfankeji.com

TS:   u instanceof User
来源：http://ami.hnxiangtu.top

Java: u instanceof User
来源：http://eir.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fhc.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://wox.tanke756.top

C#:   u is User
来源：http://cci.hywenlv.cn

[G14] 数据类 / record
来源：http://ggz.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sma.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ugb.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://imw.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://ugr.cucudq.cn

Java: record User(String name, int age) {}
来源：http://qel.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://orf.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mpj.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://fgo.jyoumei.cn

[G15] 枚举
来源：http://omi.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ogv.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kzs.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hbp.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hzc.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://sva.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tqa.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://ifa.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iue.pycfn.com

[G16] 对象转数组 / 字典
来源：http://icy.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gfz.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://hel.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://sfe.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://sjy.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tro.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://xub.wangdashe.top

Ruby: obj.instance_variables
来源：http://xpd.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://npx.sjlbkw.cn

================================================================================
来源：http://khd.zhixingplan.top

H. 异常与错误处理
来源：http://nnl.svipenyu.cn

================================================================================
来源：http://let.gogol.net.cn

[H01] try / catch 基础
来源：http://ali.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qdh.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rzg.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pnd.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tzp.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hrs.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hnr.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lya.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uhs.tanke756.top

[H02] finally / ensure 收尾
来源：http://mbs.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://ngt.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://xly.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wlr.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ecz.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wwe.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ppl.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bgi.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jbs.aizwys.cn

[H03] 主动抛出异常
来源：http://jmw.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://uyf.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xey.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://nqj.yangfankeji.com

TS:   throw new Error("错误信息");
来源：http://mdk.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tzs.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hgr.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kwi.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ltd.yueranfly.top

[H04] 自定义异常类型
来源：http://ckb.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://zrg.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://lrc.gzhubu.top


<!-- 参考信息 -->