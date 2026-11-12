代发 wailian999

[F01] 读取整个文件
来源：http://nub.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cdd.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://nws.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://egw.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iwt.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bgt.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ayt.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://aws.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://pwr.aibaodan.cn

[F02] 逐行读取文件
来源：http://wot.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yrb.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://suo.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hbp.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eke.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gcz.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rlh.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xqv.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yrj.yj20258.top

[F03] 写入文件（覆盖）
来源：http://fhm.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gek.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dgl.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vec.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cxc.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nwi.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eel.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://fgm.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cqo.uphjek.com

[F04] 追加写入文件
来源：http://vbw.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pep.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cno.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://knl.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tsq.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://quh.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hpy.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bck.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://trm.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://vrf.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mfh.cashguo.top

PHP:  file_exists("a.txt");
来源：http://hdb.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://ddb.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://mkw.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fxx.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gga.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://nxk.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://uwk.yonumen.top

[F06] 删除文件
来源：http://nil.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://bda.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://wie.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uia.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://bdb.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dxm.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://wfa.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://utn.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://bah.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://foe.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dnr.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zku.tanke756.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gix.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uzp.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sfy.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tli.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://und.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lpj.wangshuangyany.cn

[F08] 遍历目录
来源：http://cyb.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://caa.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mzv.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://kca.sweek.top

TS:   fs.readdirSync("dir")
来源：http://qyu.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hiq.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uyj.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://mzk.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://jen.mhx1999.top

[F09] 获取文件大小
来源：http://jmq.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://xdz.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://pst.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://kle.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://kcl.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://ldz.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qvk.birdmap.top

Ruby: File.size("a.txt")
来源：http://jwr.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://qlc.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://ios.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kcv.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zir.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dws.bbcook.cn

TS:   path.extname("a.txt")
来源：http://xlz.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://afa.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wyz.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fwv.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://chm.sxryk.cn

[F11] 复制与移动文件
来源：http://xgv.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ltu.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dzd.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kcg.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpg.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ule.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qyu.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ezk.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dvp.9152youxi.cn

[F12] CSV 读写
来源：http://roj.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rcg.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wqh.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xgb.jinyuanbaomall.cn

TS:   // 同上
来源：http://hwg.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wdv.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jvg.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pep.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kle.ydzc1.top

================================================================================
来源：http://ebz.snrcjt.cn

G. 面向对象
来源：http://ddb.jiagoushi.top

================================================================================
来源：http://btw.yuxming.cn

[G01] 定义类
来源：http://wpc.iojbl.cn

Py:   class User: pass
来源：http://too.zhijiandao.cn

PHP:  class User {}
来源：http://awh.meibo888.top

JS:   class User {}
来源：http://gck.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://cos.hongshengwenyu.top

Java: class User {}
来源：http://cmj.uphjek.com

Go:   type User struct { Name string }
来源：http://ylm.birdmap.top

Ruby: class User; end
来源：http://wte.birdmap.top

C#:   class User {}
来源：http://qme.ybcxt.top

[G02] 构造函数
来源：http://fkz.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://yca.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://zgt.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://vom.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://isd.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://izs.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rxn.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://uxl.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://bok.52xcode.cn

[G03] 实例属性
来源：http://anf.xinyue.icu

Py:   self.name = "x"
来源：http://aio.hnqzz.top

PHP:  public string $name = "x";
来源：http://mxd.meibo888.top

JS:   this.name = "x";
来源：http://bet.yvedp.cn

TS:   name: string = "x";
来源：http://zsa.xuanzx.com

Java: private String name;
来源：http://ihx.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://opd.yj20258.top

Ruby: @name = "x"
来源：http://eqo.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://mfa.gotoacloud.top

[G04] 定义方法
来源：http://vmu.zycfv.cn

Py:   def greet(self): return self.name
来源：http://ksk.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://eov.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://cud.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://dqr.hcnkem.com

Java: String greet() { return name; }
来源：http://yde.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rjq.aizwys.cn

Ruby: def greet; @name; end
来源：http://xol.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://ism.kuanghao11.cn

[G05] 继承
来源：http://bkx.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://mjm.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://yec.snrcjt.cn

JS:   class Admin extends User {}
来源：http://hso.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://rvv.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://eky.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wqo.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://jpj.sjlbkw.cn

C#:   class Admin : User {}
来源：http://ovq.jinghuilouyu.cn

[G06] 重写方法
来源：http://yqd.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://rms.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qru.sweek.top

JS:   greet() { return "admin"; }
来源：http://gss.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://vyk.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://gpk.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rqu.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://lep.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://zjq.hfpthk.cn

[G07] 调用父类方法
来源：http://hju.ydjk.org.cn

Py:   super().greet()
来源：http://uyk.fehbvm.com

PHP:  parent::greet();
来源：http://qrd.sysykeji.top

JS:   super.greet();
来源：http://chy.shanyushiyangtech.top

TS:   super.greet();
来源：http://dvs.wangdashe.top

Java: super.greet();
来源：http://cxu.yonumen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mxa.fehbvm.com

Ruby: super
来源：http://ggp.hysaishi.cn

C#:   base.Greet();
来源：http://uds.chenzaomai.com

[G08] 静态方法与属性
来源：http://tkl.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kvn.yonumen.top

PHP:  public static function f() {}
来源：http://bjj.havefunace.top

JS:   static f() {}
来源：http://gyd.guowangkeji.top

TS:   static f(): void {}
来源：http://kht.52xcode.cn

Java: static void f() {}
来源：http://euk.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://kln.gogol.net.cn

Ruby: def self.f; end
来源：http://jgs.meibo888.top

C#:   public static void F() {}
来源：http://yjw.daria6918.cn

[G09] 接口 / 抽象类
来源：http://ksw.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://emu.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://pnp.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uvw.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://jbi.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://pgr.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://sbs.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lyj.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://efv.yangfankeji.com

[G10] 访问控制
来源：http://jmv.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://yvo.sjlbkw.cn

PHP:  public / protected / private
来源：http://vme.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://zmh.havefunace.top

TS:   public / protected / private
来源：http://aam.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://mtr.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bcz.hywenlv.cn

Ruby: public / protected / private
来源：http://ykp.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://zrp.ydjk.org.cn

[G11] getter / setter
来源：http://ldb.fzhhl.top

Py:   @property 与 @x.setter
来源：http://enw.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xhs.yfazqb.com

JS:   get name() { return this._name; }
来源：http://him.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://eiy.xziqi.cn

Java: public String getName() { return name; }
来源：http://ksk.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://spw.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://eas.sysykeji.top

C#:   public string Name { get; set; }
来源：http://itq.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://zad.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://svq.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://fxg.xuanzx.com

JS:   toString() { return this.name; }
来源：http://fvv.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://yki.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://vds.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hpi.ybcxt.top

Ruby: def to_s; @name; end
来源：http://pom.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://wuz.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://txq.jinqigufen.top

Py:   isinstance(u, User)
来源：http://pys.daria6918.cn

PHP:  $u instanceof User
来源：http://arc.feifeiyinyue.top

JS:   u instanceof User
来源：http://qhn.dashuyun.cn

TS:   u instanceof User
来源：http://qfg.zhijiandao.cn

Java: u instanceof User
来源：http://syz.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://llz.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://pdc.52xcode.cn

C#:   u is User
来源：http://fkt.yuxming.cn

[G14] 数据类 / record
来源：http://zki.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://klx.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://eqr.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://qkb.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://tbw.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://cyy.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://lfb.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vct.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://drr.xinyue.icu

[G15] 枚举
来源：http://mud.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qxy.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cha.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ada.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ois.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://nsv.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kst.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://zzu.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xbn.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://qsi.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://giy.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://sej.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://yjm.cheryme.top

TS:   Object.entries(obj)
来源：http://hzy.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qiy.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iwb.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://jvp.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://kam.shangyingyoupin.top

================================================================================
来源：http://twv.jianghu66.top

H. 异常与错误处理
来源：http://ddo.tanke756.top

================================================================================
来源：http://uof.zhiwuduotai.top

[H01] try / catch 基础
来源：http://fzq.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sxg.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eve.yj202588.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tvf.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ant.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iqz.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qqd.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gip.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xhe.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://tru.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://toi.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rbf.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mgw.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://nnk.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://tvl.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tju.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rbe.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://rwm.redwolf501.top

[H03] 主动抛出异常
来源：http://nsl.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://eit.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gqz.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://nya.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://awq.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://clz.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rdh.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://apd.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zhd.guowangkeji.top

[H04] 自定义异常类型
来源：http://rgg.pycfn.com

Py:   class MyError(Exception): pass
来源：http://wnq.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://zmn.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://ydp.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://tir.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://dkh.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qvb.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://gyb.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://jug.chenlongwang.top

[H05] 捕获特定类型
来源：http://dyk.daria6918.cn

Py:   except ValueError as e:
来源：http://oyi.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://whv.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://jrv.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://wxs.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://pwr.bjfxy.top


<!-- 参考信息 -->