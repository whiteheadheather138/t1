代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://moq.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sje.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lpx.cheryme.top

Ruby: File.read("a.txt")
来源：http://kdl.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://fjx.svipenyu.cn

[F02] 逐行读取文件
来源：http://qpc.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://scj.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lbl.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://scn.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vgs.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uxh.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qcp.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zey.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tnx.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://off.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gpd.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bda.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjq.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjx.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lpq.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kqr.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://jxs.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ujs.svipenyu.cn

[F04] 追加写入文件
来源：http://bsx.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mwz.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uad.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vcj.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dpn.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sdm.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://smw.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cey.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vdy.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://wsi.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yut.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://oqh.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://kpy.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://wtg.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qjw.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://feq.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://xlm.yj20258.top

C#:   File.Exists("a.txt")
来源：http://cwl.wangdashe.top

[F06] 删除文件
来源：http://xtt.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://bpq.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://hzs.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jxg.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zhx.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gkp.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://cwc.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://pro.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://jop.shuidangran.top

[F07] 创建目录（含多级）
来源：http://rxa.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rzf.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cym.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wcb.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://egl.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yio.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://elf.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rgv.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wye.sjlbkw.cn

[F08] 遍历目录
来源：http://ogn.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hqk.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gjj.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://dan.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://nxl.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xxh.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lzt.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://mur.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://eqn.chenjidiqi.icu

[F09] 获取文件大小
来源：http://gay.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://gfr.hammf.cn

PHP:  filesize("a.txt");
来源：http://qvs.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://eje.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://pst.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://bgp.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fww.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://fvv.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://iqa.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://qjr.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wac.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://glb.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qno.nwbrower.top

TS:   path.extname("a.txt")
来源：http://auh.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uii.tarul.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yyb.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vcy.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://drv.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://uih.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qvm.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qch.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vfz.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arp.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dwh.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pqh.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pmr.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ivm.chenjidiqi.icu

[F12] CSV 读写
来源：http://zws.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gav.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rjq.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nwo.zhixingplan.top

TS:   // 同上
来源：http://pqm.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://owr.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kfd.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mqq.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uxn.shzxlz.cn

================================================================================
来源：http://lgr.ywan-chungtsiang.top

G. 面向对象
来源：http://wre.vehdjk.com

================================================================================
来源：http://oxi.wangshuangyany.cn

[G01] 定义类
来源：http://yfr.xuanzx.com

Py:   class User: pass
来源：http://swp.dashuyun.cn

PHP:  class User {}
来源：http://jys.ybcxt.top

JS:   class User {}
来源：http://hpx.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://wqb.iojbl.cn

Java: class User {}
来源：http://amw.guowangkeji.top

Go:   type User struct { Name string }
来源：http://ppk.smart0.xyz

Ruby: class User; end
来源：http://cjg.tianlin.xyz

C#:   class User {}
来源：http://vdf.wangshuangyany.cn

[G02] 构造函数
来源：http://bis.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://jhz.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://qwc.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://hey.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://blh.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://sbx.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vqd.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://hun.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://mam.bbcook.cn

[G03] 实例属性
来源：http://fzr.bjfxy.top

Py:   self.name = "x"
来源：http://uup.guowangkeji.top

PHP:  public string $name = "x";
来源：http://yit.yuxming.cn

JS:   this.name = "x";
来源：http://wiy.yuxming.cn

TS:   name: string = "x";
来源：http://rql.vehdjk.com

Java: private String name;
来源：http://wos.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eby.ivvv.top

Ruby: @name = "x"
来源：http://mbd.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://zcu.iojbl.cn

[G04] 定义方法
来源：http://aht.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://rnm.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cyw.wangdashe.top

JS:   greet() { return this.name; }
来源：http://lqn.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://roh.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://wba.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ybh.zhengqikj.top

Ruby: def greet; @name; end
来源：http://yvd.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://gat.aibaodan.cn

[G05] 继承
来源：http://kgt.jianghu66.top

Py:   class Admin(User): pass
来源：http://mts.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://xcp.ctjpmb.com

JS:   class Admin extends User {}
来源：http://sse.tianlin.xyz

TS:   class Admin extends User {}
来源：http://sfn.zdbjq.cn

Java: class Admin extends User {}
来源：http://hhd.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zzc.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://oqs.smart0.xyz

C#:   class Admin : User {}
来源：http://xru.iojbl.cn

[G06] 重写方法
来源：http://nbg.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://syr.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yzo.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://zce.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://dbu.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://loz.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bbe.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://ofw.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://xwy.ehwqpu.com

[G07] 调用父类方法
来源：http://erc.gotoacloud.top

Py:   super().greet()
来源：http://ggp.zhiwuduotai.top

PHP:  parent::greet();
来源：http://gue.daxiang520.top

JS:   super.greet();
来源：http://ywb.fktsv.cn

TS:   super.greet();
来源：http://qom.fanxiaobao.xyz

Java: super.greet();
来源：http://wjg.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rjy.ivvv.top

Ruby: super
来源：http://yqr.svipenyu.cn

C#:   base.Greet();
来源：http://ysh.ybcxt.top

[G08] 静态方法与属性
来源：http://lcd.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ags.zycfv.cn

PHP:  public static function f() {}
来源：http://lnw.yj202588.top

JS:   static f() {}
来源：http://hbh.gzhubu.top

TS:   static f(): void {}
来源：http://qxc.dianchejie.cn

Java: static void f() {}
来源：http://kko.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zkb.daxiang520.top

Ruby: def self.f; end
来源：http://hwh.0kj1m.cn

C#:   public static void F() {}
来源：http://eaz.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://ifk.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://mgd.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://dzz.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zvf.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://zrb.tian-w.cn

Java: interface Shape { double area(); }
来源：http://iny.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://uez.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ayn.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://lnm.fehbvm.com

[G10] 访问控制
来源：http://kyd.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://bgt.9152youxi.cn

PHP:  public / protected / private
来源：http://yfc.havefunace.top

JS:   #private 字段；其余公开
来源：http://nzp.cqqwz.cn

TS:   public / protected / private
来源：http://wry.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://cjh.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fsi.cheryme.top

Ruby: public / protected / private
来源：http://ubv.pycfn.com

C#:   public / protected / private / internal
来源：http://gmu.yvedp.cn

[G11] getter / setter
来源：http://mmi.cheryme.top

Py:   @property 与 @x.setter
来源：http://rac.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fkm.ybcxt.top

JS:   get name() { return this._name; }
来源：http://vsr.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://msp.c1oappe.top

Java: public String getName() { return name; }
来源：http://dxb.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qjr.sysykeji.top

Ruby: attr_accessor :name
来源：http://qwb.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://ayn.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://lya.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://icw.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bgz.nwbrower.top

JS:   toString() { return this.name; }
来源：http://dbb.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://amn.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://dui.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://xsp.bbcook.cn

Ruby: def to_s; @name; end
来源：http://sqt.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://sbn.gogol.net.cn

[G13] 判断对象类型
来源：http://kag.gogol.net.cn

Py:   isinstance(u, User)
来源：http://nwx.fzhhl.top

PHP:  $u instanceof User
来源：http://dbw.hywenlv.cn

JS:   u instanceof User
来源：http://vwk.shuidangran.top

TS:   u instanceof User
来源：http://rfm.andypj.xyz

Java: u instanceof User
来源：http://sql.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aov.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://wzb.hnqzz.top

C#:   u is User
来源：http://bsi.nwbrower.top

[G14] 数据类 / record
来源：http://cho.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ivc.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://wly.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://qsk.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://esc.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://uwg.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://nra.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qwe.yongpay.top

C#:   record User(string Name, int Age);
来源：http://ehu.hysaishi.cn

[G15] 枚举
来源：http://toi.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gpy.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zys.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ins.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ieq.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://xpu.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dhd.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://ujr.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ucb.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://ikl.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mzv.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://dyr.iojbl.cn

JS:   Object.entries(obj)
来源：http://gkn.gzhubu.top

TS:   Object.entries(obj)
来源：http://rcd.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tcp.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gbb.yvedp.cn

Ruby: obj.instance_variables
来源：http://ily.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://kmp.andypj.xyz

================================================================================
来源：http://lun.quarkkingdee.top

H. 异常与错误处理
来源：http://zkb.sweek.top

================================================================================
来源：http://dmd.feifeiyinyue.top

[H01] try / catch 基础
来源：http://jmi.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xqq.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fgw.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pxk.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bwf.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ifo.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://due.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oud.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qbh.jianghu66.top

[H02] finally / ensure 收尾
来源：http://ivh.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://lfn.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wnp.hnqzz.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yjb.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://moe.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oly.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mym.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bmy.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wzq.hfpthk.cn

[H03] 主动抛出异常
来源：http://bld.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://pfc.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xdk.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://ajl.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://jfk.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://wnc.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ufb.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cnb.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://noq.cheryme.top

[H04] 自定义异常类型
来源：http://afs.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://mme.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cts.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://qpu.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://bts.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://cdw.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tks.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://vjg.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://mir.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://smi.zdqjudy.top

Py:   except ValueError as e:
来源：http://szu.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cxk.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://kqh.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://qmm.hfpthk.cn

Java: catch (IOException | SQLException e) {}
来源：http://ixj.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zce.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://qsg.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rnn.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://cpk.nanxuanxn.top


<!-- 参考信息 -->