代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ckr.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://fnk.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dtj.xuanzx.com

Ruby: File.read("a.txt")
来源：http://sxn.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gwl.redwolf501.top

[F02] 逐行读取文件
来源：http://rgs.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gnx.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bug.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fio.ywan-chungtsiang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vhs.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ywr.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pug.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://que.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rsa.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://fmq.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hvt.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qej.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ova.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gxi.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wqr.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mxd.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://kaz.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aih.zhixingplan.top

[F04] 追加写入文件
来源：http://sjf.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zkc.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://shm.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jbw.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mxt.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://opq.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kei.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mqi.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ajd.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://adz.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kzr.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://wsk.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://iar.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://udo.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bnc.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ehv.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://ved.yongpay.top

C#:   File.Exists("a.txt")
来源：http://sym.cucudq.cn

[F06] 删除文件
来源：http://akd.smart0.xyz

Py:   os.remove("a.txt")
来源：http://pum.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://uos.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://brx.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://mve.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rfn.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://oxi.birdmap.top

Ruby: File.delete("a.txt")
来源：http://jfn.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://wpd.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://fsa.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cwh.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yqq.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qix.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgg.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sql.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bzi.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xvv.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://umm.tianlin.xyz

[F08] 遍历目录
来源：http://zod.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ozr.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yrw.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://bub.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://uuo.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jzl.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kni.yonumen.top

Ruby: Dir.children("dir")
来源：http://hlv.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://tsa.c1oappe.top

[F09] 获取文件大小
来源：http://crc.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://tbd.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://ewd.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://ohu.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://sxq.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://kfr.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qch.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://qne.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://cso.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://mjl.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bud.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kvq.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ccc.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://wui.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fux.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sgx.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://erb.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wxk.ehwqpu.com

[F11] 复制与移动文件
来源：http://hfl.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mdw.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sev.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tom.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://csi.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pgk.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qjl.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jyy.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://akd.guowangkeji.top

[F12] CSV 读写
来源：http://dcd.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zur.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nvj.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eav.hnqzz.top

TS:   // 同上
来源：http://hdt.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cnz.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wmp.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hrq.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ici.daria6918.cn

================================================================================
来源：http://nvy.cdnleiting.top

G. 面向对象
来源：http://pnm.ctjpmb.com

================================================================================
来源：http://mgn.mhx1999.top

[G01] 定义类
来源：http://dqg.zycfv.cn

Py:   class User: pass
来源：http://rir.zhengqikj.top

PHP:  class User {}
来源：http://xdd.hongshengwenyu.top

JS:   class User {}
来源：http://rwu.tarul.cn

TS:   class User { name: string = ""; }
来源：http://hds.gaohongyu789.top

Java: class User {}
来源：http://azn.yuanzhike.top

Go:   type User struct { Name string }
来源：http://ack.jqgfzy.top

Ruby: class User; end
来源：http://yqm.jqgfzy.top

C#:   class User {}
来源：http://qzy.dashuyun.cn

[G02] 构造函数
来源：http://scy.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://yfx.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://lkb.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://cdh.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://cvz.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://pdh.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tfr.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://pyo.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://efy.fengsongda.top

[G03] 实例属性
来源：http://bgu.aizwys.cn

Py:   self.name = "x"
来源：http://qce.smart0.xyz

PHP:  public string $name = "x";
来源：http://xsn.yvedp.cn

JS:   this.name = "x";
来源：http://gbn.gotoacloud.top

TS:   name: string = "x";
来源：http://kui.daxiang520.top

Java: private String name;
来源：http://lrk.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kwq.shangyingyoupin.top

Ruby: @name = "x"
来源：http://kuz.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://xsn.fehbvm.com

[G04] 定义方法
来源：http://hxw.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://byy.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yzr.yonumen.top

JS:   greet() { return this.name; }
来源：http://lfd.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://zrf.kuanghao11.cn

Java: String greet() { return name; }
来源：http://sms.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hpx.ehwqpu.com

Ruby: def greet; @name; end
来源：http://itd.yj20258888.top

C#:   public string Greet() => Name;
来源：http://ctn.hnxiangtu.top

[G05] 继承
来源：http://zwc.ppjwa.cn

Py:   class Admin(User): pass
来源：http://srn.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://yny.hnqzz.top

JS:   class Admin extends User {}
来源：http://cqy.yfazqb.com

TS:   class Admin extends User {}
来源：http://agf.wangdashe.top

Java: class Admin extends User {}
来源：http://ypf.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cwy.chenzaomai.com

Ruby: class Admin < User; end
来源：http://qij.0kj1m.cn

C#:   class Admin : User {}
来源：http://xkn.chenjidiqi.icu

[G06] 重写方法
来源：http://nsp.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://fzo.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://swo.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://xrc.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://xeb.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://sks.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gzv.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://tvs.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://umx.ppjwa.cn

[G07] 调用父类方法
来源：http://bxy.dianchejie.cn

Py:   super().greet()
来源：http://uaf.52xcode.cn

PHP:  parent::greet();
来源：http://qrd.zhaomingkeji.xyz

JS:   super.greet();
来源：http://ogb.fengsongda.top

TS:   super.greet();
来源：http://xed.smart0.xyz

Java: super.greet();
来源：http://mii.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qfh.sjlbkw.cn

Ruby: super
来源：http://ouj.hcnkem.com

C#:   base.Greet();
来源：http://nor.shuidangran.top

[G08] 静态方法与属性
来源：http://sdl.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ttd.sjlbkw.cn

PHP:  public static function f() {}
来源：http://ebn.ctjpmb.com

JS:   static f() {}
来源：http://qtb.fzhhl.top

TS:   static f(): void {}
来源：http://vmk.zhongyouzk.top

Java: static void f() {}
来源：http://xmy.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://owo.jinqigfzy.top

Ruby: def self.f; end
来源：http://guz.nanxuanxn.top

C#:   public static void F() {}
来源：http://ewt.vehdjk.com

[G09] 接口 / 抽象类
来源：http://bql.shuidangran.top

Py:   from abc import ABC, abstractmethod
来源：http://dsg.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://rly.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fhh.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://wyd.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://skv.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://rgz.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wel.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://tum.guannengcc.top

[G10] 访问控制
来源：http://ifi.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://pwu.chenlongwang.top

PHP:  public / protected / private
来源：http://uhd.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://ovk.haohaochexian.top

TS:   public / protected / private
来源：http://tin.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://joc.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kde.sjlbkw.cn

Ruby: public / protected / private
来源：http://ign.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://omv.fktsv.cn

[G11] getter / setter
来源：http://ndk.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://wgb.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rvl.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://rjv.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://mic.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://vjy.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nmw.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://jrb.bbcook.cn

C#:   public string Name { get; set; }
来源：http://sxj.nanxuanxn.top

[G12] 对象转字符串
来源：http://aso.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://hjc.jqgfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aim.xuanzx.com

JS:   toString() { return this.name; }
来源：http://eie.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://vir.yanxiufei.cn

Java: @Override public String toString() { return name; }
来源：http://fbs.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://pac.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://rnr.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://pvu.bjfxy.top

[G13] 判断对象类型
来源：http://qjq.sweek.top

Py:   isinstance(u, User)
来源：http://mpg.jinqigufen.top

PHP:  $u instanceof User
来源：http://fie.dashuyun.cn

JS:   u instanceof User
来源：http://rjs.yfazqb.com

TS:   u instanceof User
来源：http://mbm.hywenlv.cn

Java: u instanceof User
来源：http://szq.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ulg.fehbvm.com

Ruby: u.is_a?(User)
来源：http://pit.shuidangran.top

C#:   u is User
来源：http://sys.c1oappe.top

[G14] 数据类 / record
来源：http://tnz.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nme.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://khj.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://etl.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://ihv.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://zcn.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://leo.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://psc.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://jna.xinyue.icu

[G15] 枚举
来源：http://sqf.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mmu.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nnl.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sop.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://imn.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://qsz.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://las.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://hoa.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kmd.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://ibi.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uxk.zhaomingkeji.xyz

PHP:  get_object_vars($obj);
来源：http://mmp.svipenyu.cn

JS:   Object.entries(obj)
来源：http://xpn.nanxinkj.top

TS:   Object.entries(obj)
来源：http://ucp.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ltj.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iis.xinyue.icu

Ruby: obj.instance_variables
来源：http://kxq.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://moi.quarkkingdee.top

================================================================================
来源：http://wnl.daria6918.cn

H. 异常与错误处理
来源：http://omq.xinyue.icu

================================================================================
来源：http://vsz.bbcook.cn

[H01] try / catch 基础
来源：http://tan.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fff.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aas.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sqc.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ruo.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hdj.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jqy.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oto.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hzz.yueranfly.top

[H02] finally / ensure 收尾
来源：http://htu.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxx.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rgm.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vnd.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xmm.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mza.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eqb.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dmj.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ouj.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://kpr.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://dgl.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rdu.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://gqn.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://nsg.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uoa.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jxl.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sxv.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://jee.hcnkem.com

[H04] 自定义异常类型
来源：http://xsn.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://iab.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tzw.sxryk.cn

JS:   class MyError extends Error {}
来源：http://mpz.fengsongda.top

TS:   class MyError extends Error {}
来源：http://ety.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://wun.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vjp.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://rak.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://ptv.iojbl.cn

[H05] 捕获特定类型
来源：http://atm.yj202588.top

Py:   except ValueError as e:
来源：http://wdv.kuanghao11.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oef.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://ktm.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://dva.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://xar.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mfo.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://twr.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kcu.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://vmf.hesvh.cn


<!-- 参考信息 -->