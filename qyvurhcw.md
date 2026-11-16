代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pjx.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hbe.cheryme.top

[F03] 写入文件（覆盖）
来源：http://tuv.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dky.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bhx.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nva.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://glq.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ysi.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nwp.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://gkb.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yzt.hcnkem.com

[F04] 追加写入文件
来源：http://pzm.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://chp.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wis.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hgb.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rsk.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zqb.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wnr.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ipt.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rph.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://clv.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ziq.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://hyw.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://bcb.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://cga.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bkf.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nsb.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://lwu.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://ign.zdbjq.cn

[F06] 删除文件
来源：http://yrv.jianghu66.top

Py:   os.remove("a.txt")
来源：http://xfs.gzhubu.top

PHP:  unlink("a.txt");
来源：http://yaq.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://beu.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kdv.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://del.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://sor.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://kyu.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://awe.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://wuk.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ktd.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mvj.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpa.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qmm.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ivj.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oqa.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eul.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lkw.zdbjq.cn

[F08] 遍历目录
来源：http://xgn.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vbz.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qlp.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://sei.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://xkh.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://liw.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pja.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://bxo.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://zgq.zhongyouzk.top

[F09] 获取文件大小
来源：http://vxy.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://eiw.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://jqb.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://viu.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://ndd.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://pht.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://slp.wangdashe.top

Ruby: File.size("a.txt")
来源：http://rfo.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://tkj.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://kyd.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://afd.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pvb.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hzw.daxiang520.top

TS:   path.extname("a.txt")
来源：http://vli.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qeu.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vjo.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qmc.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hmg.yanxiufei.cn

[F11] 复制与移动文件
来源：http://vcw.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://trj.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://npv.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ajn.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bwd.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://woc.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qmw.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jjv.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cnz.yongpay.top

[F12] CSV 读写
来源：http://yeb.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yzq.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xyg.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wix.iojbl.cn

TS:   // 同上
来源：http://qny.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fth.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rcp.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://laa.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kec.sxryk.cn

================================================================================
来源：http://dsu.pengpengdd.cyou

G. 面向对象
来源：http://slw.gzhubu.top

================================================================================
来源：http://kdz.hnxiangtu.top

[G01] 定义类
来源：http://kql.hongshengwenyu.top

Py:   class User: pass
来源：http://hyx.nwbrower.top

PHP:  class User {}
来源：http://ocj.52xcode.cn

JS:   class User {}
来源：http://phh.cheryme.top

TS:   class User { name: string = ""; }
来源：http://wfr.shuidangran.top

Java: class User {}
来源：http://eog.jinqigufen.top

Go:   type User struct { Name string }
来源：http://ivg.hammf.cn

Ruby: class User; end
来源：http://anp.chenjidiqi.icu

C#:   class User {}
来源：http://obu.fehbvm.com

[G02] 构造函数
来源：http://zlx.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://czq.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://nzm.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://hyi.meibo888.top

TS:   constructor(public name: string) {}
来源：http://him.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://hxu.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jzd.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://ato.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://pcm.ctjpmb.com

[G03] 实例属性
来源：http://ihd.pycfn.com

Py:   self.name = "x"
来源：http://how.guannengcc.top

PHP:  public string $name = "x";
来源：http://bsk.tianlin.xyz

JS:   this.name = "x";
来源：http://huu.zhijiandao.cn

TS:   name: string = "x";
来源：http://enj.yonumen.top

Java: private String name;
来源：http://kjk.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qcw.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://nbx.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://hyr.cqqwz.cn

[G04] 定义方法
来源：http://lwx.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://nko.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qgt.xuanzx.com

JS:   greet() { return this.name; }
来源：http://cfu.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://bkf.hnqzz.top

Java: String greet() { return name; }
来源：http://qkm.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://igg.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://his.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://gby.birdmap.top

[G05] 继承
来源：http://nxg.zdqjudy.top

Py:   class Admin(User): pass
来源：http://feg.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://eke.ctjpmb.com

JS:   class Admin extends User {}
来源：http://ejx.ydzc1.top

TS:   class Admin extends User {}
来源：http://esn.shuidangran.top

Java: class Admin extends User {}
来源：http://igk.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oej.tanke756.top

Ruby: class Admin < User; end
来源：http://olq.hammf.cn

C#:   class Admin : User {}
来源：http://kpv.nanxuanxn.top

[G06] 重写方法
来源：http://etu.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://fcz.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://szg.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://xpr.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://sbi.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://aod.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rgo.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://ddg.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://ort.tanke756.top

[G07] 调用父类方法
来源：http://awg.zhoulong.xyz

Py:   super().greet()
来源：http://pem.meibo888.top

PHP:  parent::greet();
来源：http://svh.andypj.xyz

JS:   super.greet();
来源：http://vhz.zhixingplan.top

TS:   super.greet();
来源：http://fwi.zhengqikj.top

Java: super.greet();
来源：http://opr.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ejl.birdmap.top

Ruby: super
来源：http://lsp.ybcxt.top

C#:   base.Greet();
来源：http://qoj.yj20258.top

[G08] 静态方法与属性
来源：http://kht.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sbj.sysykeji.top

PHP:  public static function f() {}
来源：http://gth.hammf.cn

JS:   static f() {}
来源：http://twk.jyoumei.cn

TS:   static f(): void {}
来源：http://hkd.gotoacloud.top

Java: static void f() {}
来源：http://ych.bbcook.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yqx.meibo888.top

Ruby: def self.f; end
来源：http://qsi.hcnkem.com

C#:   public static void F() {}
来源：http://ege.jianghu66.top

[G09] 接口 / 抽象类
来源：http://uiv.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://rcj.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://lsx.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hvl.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://nfd.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://qzh.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://hhp.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hwi.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://vuf.xinyue.icu

[G10] 访问控制
来源：http://xpj.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://xpb.nwbrower.top

PHP:  public / protected / private
来源：http://kjr.ybcxt.top

JS:   #private 字段；其余公开
来源：http://efp.jinghuilouyu.cn

TS:   public / protected / private
来源：http://uqb.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://cpt.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vst.sysykeji.top

Ruby: public / protected / private
来源：http://ryw.hammf.cn

C#:   public / protected / private / internal
来源：http://ebd.chenjidiqi.icu

[G11] getter / setter
来源：http://qxg.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://tav.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://skd.meibo888.top

JS:   get name() { return this._name; }
来源：http://cxq.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://zft.haohaochexian.top

Java: public String getName() { return name; }
来源：http://tkz.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://iaa.epnwcf.com

Ruby: attr_accessor :name
来源：http://ntp.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://qpp.meibo888.top

[G12] 对象转字符串
来源：http://gtw.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://mpt.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cat.xziqi.cn

JS:   toString() { return this.name; }
来源：http://rxv.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://dam.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://yrc.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://kuo.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://kvc.havefunace.top

C#:   public override string ToString() => Name;
来源：http://ntu.hammf.cn

[G13] 判断对象类型
来源：http://jrl.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://fma.sjlbkw.cn

PHP:  $u instanceof User
来源：http://sda.shanyushiyangtech.top

JS:   u instanceof User
来源：http://wue.jinqigfzy.top

TS:   u instanceof User
来源：http://tbi.hnqzz.top

Java: u instanceof User
来源：http://oys.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wag.bbcook.cn

Ruby: u.is_a?(User)
来源：http://wxp.yueranfly.top

C#:   u is User
来源：http://rnz.jlsjyb.cn

[G14] 数据类 / record
来源：http://mbu.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xyc.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://thc.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://lxf.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://yuc.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://ivd.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://izs.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xfg.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://tmu.gogol.net.cn

[G15] 枚举
来源：http://ilv.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mhx.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gmb.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vmg.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fqt.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://wxm.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rur.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://dqa.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ian.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://ypm.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jif.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://zhd.yuanzhike.top

JS:   Object.entries(obj)
来源：http://wrf.cqqwz.cn

TS:   Object.entries(obj)
来源：http://qyv.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uzl.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pbz.tianlin.xyz

Ruby: obj.instance_variables
来源：http://sxj.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://ntm.wangshuangyany.cn

================================================================================
来源：http://tgv.fengsongda.top

H. 异常与错误处理
来源：http://zvn.yueranfly.top

================================================================================
来源：http://crk.jqgfzy.top

[H01] try / catch 基础
来源：http://vzb.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://icg.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nbk.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uoj.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ayf.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vvy.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qzd.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kpf.snrcjt.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iki.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://rcw.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://rvb.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ktb.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hzg.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rsf.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://lul.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://scw.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bnf.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ntt.haohaochexian.top

[H03] 主动抛出异常
来源：http://jjk.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://ejo.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ykj.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://wxx.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://fah.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lkq.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nij.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hwp.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://gyr.dianchejie.cn

[H04] 自定义异常类型
来源：http://mic.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://yko.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://izs.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://pad.bjfxy.top

TS:   class MyError extends Error {}
来源：http://fju.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://oae.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hux.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://tlx.yj202588.top

C#:   class MyException : Exception {}
来源：http://bnd.cheryme.top

[H05] 捕获特定类型
来源：http://tur.hfpthk.cn

Py:   except ValueError as e:
来源：http://prm.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lom.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://jeb.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://qys.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://zzr.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tuf.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://cso.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jil.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://zsw.xylfe.cn

Py:   value = d.get("k") or default
来源：http://flh.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://uon.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nfm.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://cmw.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nzk.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ste.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://lnr.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://jnz.vehdjk.com

[H07] 断言
来源：http://vhn.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://tny.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://vaz.fengsongda.top

JS:   console.assert(x > 0);
来源：http://jbb.pengpengdd.cyou


<!-- 参考信息 -->