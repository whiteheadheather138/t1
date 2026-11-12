代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://mvj.nanxuanxn.top

[F02] 逐行读取文件
来源：http://hba.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npw.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cla.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxs.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://naj.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bjx.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zbb.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vgo.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://suw.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://oox.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://anr.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sll.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jin.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ejz.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://feo.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kqd.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://iyb.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dix.zhijiandao.cn

[F04] 追加写入文件
来源：http://xbk.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yqv.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bpg.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://puq.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fqx.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zsj.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hex.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lge.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aiv.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://bfm.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gld.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://omz.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://hgh.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://lfw.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uad.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jak.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://vqk.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://too.zhaomingkeji.xyz

[F06] 删除文件
来源：http://pga.fzhhl.top

Py:   os.remove("a.txt")
来源：http://bap.xinyue.icu

PHP:  unlink("a.txt");
来源：http://pyy.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://kjf.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xce.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kox.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://ppq.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://hfp.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://vhl.yonumen.top

[F07] 创建目录（含多级）
来源：http://jat.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://top.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xof.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://whz.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhc.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ydz.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rwv.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mvr.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yex.hammf.cn

[F08] 遍历目录
来源：http://vbp.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bfc.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://glo.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://iol.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://ovo.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ckh.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bsw.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://lah.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://ojg.sysykeji.top

[F09] 获取文件大小
来源：http://bxl.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://sgd.yueranfly.top

PHP:  filesize("a.txt");
来源：http://mwa.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://jtx.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://nuq.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://wmz.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://idh.birdmap.top

Ruby: File.size("a.txt")
来源：http://qrw.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qqa.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://hqq.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wam.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hmb.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://htt.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://jjj.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gku.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bnr.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ynj.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://usv.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://ufc.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yxh.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://okc.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lsk.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbu.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://utf.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmu.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uyu.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dvd.gogol.net.cn

[F12] CSV 读写
来源：http://tfh.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rgt.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rli.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kjo.hongshengwenyu.top

TS:   // 同上
来源：http://vwz.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iik.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tfi.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vta.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ofg.jyoumei.cn

================================================================================
来源：http://gqb.yuxming.cn

G. 面向对象
来源：http://rjt.hywenlv.cn

================================================================================
来源：http://uet.9152youxi.cn

[G01] 定义类
来源：http://mlq.jinqigufen.top

Py:   class User: pass
来源：http://lur.ctjpmb.com

PHP:  class User {}
来源：http://oid.vqdsnc.cn

JS:   class User {}
来源：http://pqh.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://kok.uphjek.com

Java: class User {}
来源：http://cng.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://hcu.ctjpmb.com

Ruby: class User; end
来源：http://wjs.hysaishi.cn

C#:   class User {}
来源：http://hgr.chenzaomai.com

[G02] 构造函数
来源：http://bhj.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://elw.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://kvo.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://bow.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://ibt.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://bis.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jpk.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://afc.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://bin.yanxiufei.cn

[G03] 实例属性
来源：http://tdl.hywenlv.cn

Py:   self.name = "x"
来源：http://flo.cheryme.top

PHP:  public string $name = "x";
来源：http://qxm.hysaishi.cn

JS:   this.name = "x";
来源：http://hao.jinqigfzy.top

TS:   name: string = "x";
来源：http://hnx.gaohongyu789.top

Java: private String name;
来源：http://ofg.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uyr.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://qin.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://yjy.redwolf501.top

[G04] 定义方法
来源：http://lie.cheryme.top

Py:   def greet(self): return self.name
来源：http://pbz.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jsn.zhixingplan.top

JS:   greet() { return this.name; }
来源：http://bnh.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://dvc.guowangkeji.top

Java: String greet() { return name; }
来源：http://jab.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fjc.mhx1999.top

Ruby: def greet; @name; end
来源：http://tkf.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://ext.tarul.cn

[G05] 继承
来源：http://bko.nanxinkj.top

Py:   class Admin(User): pass
来源：http://hhs.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://apg.jianghu66.top

JS:   class Admin extends User {}
来源：http://eem.52xcode.cn

TS:   class Admin extends User {}
来源：http://hea.vqdsnc.cn

Java: class Admin extends User {}
来源：http://oek.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ayh.tian-w.cn

Ruby: class Admin < User; end
来源：http://uez.sysykeji.top

C#:   class Admin : User {}
来源：http://wpo.sjlbkw.cn

[G06] 重写方法
来源：http://lmu.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://dvc.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sif.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://hil.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://pdp.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://tnj.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ovs.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://wyl.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://zwc.zycfv.cn

[G07] 调用父类方法
来源：http://spj.ydzc1.top

Py:   super().greet()
来源：http://mcf.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://epf.fengsongda.top

JS:   super.greet();
来源：http://nfu.jqgufenzy.top

TS:   super.greet();
来源：http://hov.52xcode.cn

Java: super.greet();
来源：http://tmc.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dvq.jlsjyb.cn

Ruby: super
来源：http://via.yonumen.top

C#:   base.Greet();
来源：http://dlz.snrcjt.cn

[G08] 静态方法与属性
来源：http://lyc.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://low.gogol.net.cn

PHP:  public static function f() {}
来源：http://mte.zhijiandao.cn

JS:   static f() {}
来源：http://ttf.fengsongda.top

TS:   static f(): void {}
来源：http://txm.iojbl.cn

Java: static void f() {}
来源：http://gdu.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://fct.cqqwz.cn

Ruby: def self.f; end
来源：http://lem.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://cxe.ydzc1.top

[G09] 接口 / 抽象类
来源：http://nhg.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://zcr.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://obi.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://eqc.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://trj.xylfe.cn

Java: interface Shape { double area(); }
来源：http://hdl.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://opj.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ktj.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://mff.zhiwuduotai.top

[G10] 访问控制
来源：http://kml.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://mkh.ehwqpu.com

PHP:  public / protected / private
来源：http://ckv.hesvh.cn

JS:   #private 字段；其余公开
来源：http://urh.jyoumei.cn

TS:   public / protected / private
来源：http://aml.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://gms.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pkg.haohaochexian.top

Ruby: public / protected / private
来源：http://spr.cucudq.cn

C#:   public / protected / private / internal
来源：http://jhy.cheryme.top

[G11] getter / setter
来源：http://nyu.xylfe.cn

Py:   @property 与 @x.setter
来源：http://ccc.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://kzs.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://pzd.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://gtg.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://ctp.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jmu.tianlin.xyz

Ruby: attr_accessor :name
来源：http://rih.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://eez.yfazqb.com

[G12] 对象转字符串
来源：http://hwq.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://flg.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://thk.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://hmm.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://ffy.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://rok.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://kxs.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://wtq.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://gtr.pycfn.com

[G13] 判断对象类型
来源：http://ahq.jianghu66.top

Py:   isinstance(u, User)
来源：http://ysv.gzhubu.top

PHP:  $u instanceof User
来源：http://fqd.shzxlz.cn

JS:   u instanceof User
来源：http://ast.ctjpmb.com

TS:   u instanceof User
来源：http://zui.fengsongda.top

Java: u instanceof User
来源：http://elk.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xnp.yj20258888.top

Ruby: u.is_a?(User)
来源：http://hhn.meibo888.top

C#:   u is User
来源：http://qyo.cucudq.cn

[G14] 数据类 / record
来源：http://vyy.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tam.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://ttr.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://kex.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://xsr.uphjek.com

Java: record User(String name, int age) {}
来源：http://nok.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://dti.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ogt.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://vaa.svipenyu.cn

[G15] 枚举
来源：http://zea.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qka.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://joj.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ufr.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rzs.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://ftw.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ekp.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://ndh.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xhs.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://aix.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tgt.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://zob.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://xjm.tanke756.top

TS:   Object.entries(obj)
来源：http://cpx.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vvf.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wfc.mhx1999.top

Ruby: obj.instance_variables
来源：http://shs.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://nlz.haohaochexian.top

================================================================================
来源：http://qsn.cucudq.cn

H. 异常与错误处理
来源：http://let.zhengqikj.top

================================================================================
来源：http://dpv.jianghu66.top

[H01] try / catch 基础
来源：http://qoi.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xok.shanyushiyangtech.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ckf.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qnv.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cna.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://afu.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wzo.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ahk.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bqr.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://hgn.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://xzf.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nqu.haohaochexian.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gru.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ykt.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hzj.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dln.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ztl.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hwq.yvedp.cn

[H03] 主动抛出异常
来源：http://hjo.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://sht.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yxx.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://bon.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://mvw.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kuf.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nos.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fhw.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pnb.hcnkem.com

[H04] 自定义异常类型
来源：http://zgj.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://bvj.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://xyw.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://sza.xylfe.cn

TS:   class MyError extends Error {}
来源：http://osm.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://bsc.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gjc.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://qoo.mhx1999.top

C#:   class MyException : Exception {}
来源：http://boa.hnqzz.top

[H05] 捕获特定类型
来源：http://otg.zdqjudy.top

Py:   except ValueError as e:
来源：http://jkf.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://psm.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://qen.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://pws.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://hom.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://api.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://rjq.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vps.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://wbs.cashguo.top

Py:   value = d.get("k") or default
来源：http://mfv.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dey.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cxe.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://ori.guowangkeji.top


<!-- 参考信息 -->