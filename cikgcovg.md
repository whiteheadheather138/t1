代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gay.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pub.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://orj.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wmm.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hgr.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tfn.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://bgi.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kjg.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dim.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fmb.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cns.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oxp.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://afl.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://zro.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rfq.pycfn.com

[F04] 追加写入文件
来源：http://ejg.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jvr.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vid.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qqd.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txb.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ecw.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iyz.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vaz.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://awa.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://tww.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dac.meibo888.top

PHP:  file_exists("a.txt");
来源：http://txx.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://oax.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://nvx.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vsw.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xmi.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://vzv.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://dow.chenzaomai.com

[F06] 删除文件
来源：http://tjl.yj20258.top

Py:   os.remove("a.txt")
来源：http://bzk.birdmap.top

PHP:  unlink("a.txt");
来源：http://rdy.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://xwl.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oxy.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dul.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://ysw.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://qax.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://cbi.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://vrh.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rgj.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dtf.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xbx.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ses.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bpf.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wso.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rvk.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://das.iojbl.cn

[F08] 遍历目录
来源：http://pma.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://nts.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://orx.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://mlh.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://ain.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fyd.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kyd.fengsongda.top

Ruby: Dir.children("dir")
来源：http://eav.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://hya.daxiang520.top

[F09] 获取文件大小
来源：http://gze.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://tzi.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://omv.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://mfz.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://tdx.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qdd.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bzy.cucudq.cn

Ruby: File.size("a.txt")
来源：http://czo.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://exk.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://drr.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ukg.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bgq.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gyp.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://uka.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iuj.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jwy.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://igy.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hzw.yj20258.top

[F11] 复制与移动文件
来源：http://scf.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ldc.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dzp.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hqe.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rpp.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hyp.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dyz.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ydw.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hmh.316326.xyz

[F12] CSV 读写
来源：http://tdo.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://orb.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://luf.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iny.chenjidiqi.icu

TS:   // 同上
来源：http://wln.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yxt.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iyu.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aww.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pti.hcnkem.com

================================================================================
来源：http://pqb.kuanghao11.cn

G. 面向对象
来源：http://qpt.nwbrower.top

================================================================================
来源：http://oqh.tianlin.xyz

[G01] 定义类
来源：http://gug.uphjek.com

Py:   class User: pass
来源：http://lzx.hfpthk.cn

PHP:  class User {}
来源：http://xqf.ywan-chungtsiang.top

JS:   class User {}
来源：http://sdl.yj20258.top

TS:   class User { name: string = ""; }
来源：http://imn.jinghuilouyu.cn

Java: class User {}
来源：http://dhs.tian-w.cn

Go:   type User struct { Name string }
来源：http://lip.sufxvd.cn

Ruby: class User; end
来源：http://exb.wangshuangyany.cn

C#:   class User {}
来源：http://wwk.vehdjk.com

[G02] 构造函数
来源：http://kuk.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://ihz.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://gbh.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://frg.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://nrs.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://bem.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vuv.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://nsz.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://mfp.birdmap.top

[G03] 实例属性
来源：http://xon.ybcxt.top

Py:   self.name = "x"
来源：http://gtp.yonumen.top

PHP:  public string $name = "x";
来源：http://byg.bjfxy.top

JS:   this.name = "x";
来源：http://rdo.9152youxi.cn

TS:   name: string = "x";
来源：http://dpo.cashguo.top

Java: private String name;
来源：http://ifu.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uul.haohaochexian.top

Ruby: @name = "x"
来源：http://nuj.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://lml.aibaodan.cn

[G04] 定义方法
来源：http://dqr.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://mtg.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qjv.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://qvq.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://wss.aizwys.cn

Java: String greet() { return name; }
来源：http://oku.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://giu.yonumen.top

Ruby: def greet; @name; end
来源：http://gfw.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://buy.mhx1999.top

[G05] 继承
来源：http://npw.sufxvd.cn

Py:   class Admin(User): pass
来源：http://jyd.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://elf.uphjek.com

JS:   class Admin extends User {}
来源：http://why.hnqzz.top

TS:   class Admin extends User {}
来源：http://bcb.c1oappe.top

Java: class Admin extends User {}
来源：http://qjm.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tmn.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://exo.yj20258.top

C#:   class Admin : User {}
来源：http://xzk.zhoulong.xyz

[G06] 重写方法
来源：http://yui.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://ecz.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vpx.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://ggb.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://kjd.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://pyk.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eof.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://kmy.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://pty.hysaishi.cn

[G07] 调用父类方法
来源：http://nhi.shzxlz.cn

Py:   super().greet()
来源：http://kpu.hesvh.cn

PHP:  parent::greet();
来源：http://eem.xziqi.cn

JS:   super.greet();
来源：http://rcp.iojbl.cn

TS:   super.greet();
来源：http://uoa.ydjk.org.cn

Java: super.greet();
来源：http://rsm.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ugw.sweek.top

Ruby: super
来源：http://cep.zhijiandao.cn

C#:   base.Greet();
来源：http://eid.chenlongwang.top

[G08] 静态方法与属性
来源：http://qyb.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fte.cdnleiting.top

PHP:  public static function f() {}
来源：http://snr.jinyuanbaomall.cn

JS:   static f() {}
来源：http://hgh.shuidangran.top

TS:   static f(): void {}
来源：http://erf.ydzc1.top

Java: static void f() {}
来源：http://xul.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ucz.bjfxy.top

Ruby: def self.f; end
来源：http://ieq.fzhhl.top

C#:   public static void F() {}
来源：http://qkk.tarul.cn

[G09] 接口 / 抽象类
来源：http://wyi.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://fjs.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://xdu.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zwa.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://gpa.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://ogn.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://jaw.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://efa.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://iee.hnqzz.top

[G10] 访问控制
来源：http://fwi.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://tox.nwbrower.top

PHP:  public / protected / private
来源：http://lvw.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://jrf.aibaodan.cn

TS:   public / protected / private
来源：http://ddb.tarul.cn

Java: public / protected / private / 默认包级
来源：http://qty.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aio.zhiwuduotai.top

Ruby: public / protected / private
来源：http://sjs.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://ghz.yuxming.cn

[G11] getter / setter
来源：http://ggq.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://urd.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rsr.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://yco.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://ofo.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://oka.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wlt.yj20258.top

Ruby: attr_accessor :name
来源：http://qys.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://cry.316326.xyz

[G12] 对象转字符串
来源：http://toj.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://ibi.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xig.birdmap.top

JS:   toString() { return this.name; }
来源：http://krr.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://bys.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://vup.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://ijd.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://hfb.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://ouk.dianchejie.cn

[G13] 判断对象类型
来源：http://qey.zycfv.cn

Py:   isinstance(u, User)
来源：http://cqr.gaohongyu789.top

PHP:  $u instanceof User
来源：http://oaj.zhijiandao.cn

JS:   u instanceof User
来源：http://rpb.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://tte.vehdjk.com

Java: u instanceof User
来源：http://qvv.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ysw.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://tkg.iojbl.cn

C#:   u is User
来源：http://bxb.nanxuanxn.top

[G14] 数据类 / record
来源：http://ubl.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nnd.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://bnx.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://gff.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://kqw.ydzc1.top

Java: record User(String name, int age) {}
来源：http://rem.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://jrq.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ilt.aibaodan.cn

C#:   record User(string Name, int Age);
来源：http://lct.guowangkeji.top

[G15] 枚举
来源：http://rkp.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nri.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://xff.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hne.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bgb.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://kug.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://akk.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://ppn.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iiz.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://pnn.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fdi.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://xub.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://qeh.fengsongda.top

TS:   Object.entries(obj)
来源：http://iuf.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rze.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jht.hcnkem.com

Ruby: obj.instance_variables
来源：http://owa.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://olg.daria6918.cn

================================================================================
来源：http://vyy.gaohongyu789.top

H. 异常与错误处理
来源：http://sns.c1oappe.top

================================================================================
来源：http://fik.yvedp.cn

[H01] try / catch 基础
来源：http://mml.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mmq.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lfq.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hbo.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oif.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://amf.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ngx.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uka.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gxi.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://skx.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://fen.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://frl.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://myl.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mkn.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://wqf.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cfg.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rvz.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://kgi.quarkkingdee.top

[H03] 主动抛出异常
来源：http://eld.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://rih.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dao.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://xpo.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://dfm.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://pqu.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xqn.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pbf.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://chk.daria6918.cn

[H04] 自定义异常类型
来源：http://mjq.pycfn.com

Py:   class MyError(Exception): pass
来源：http://sid.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cdj.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://jgk.epnwcf.com

TS:   class MyError extends Error {}
来源：http://mtd.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://xho.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oha.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://gke.tarul.cn

C#:   class MyException : Exception {}
来源：http://eic.zhoulong.xyz

[H05] 捕获特定类型
来源：http://fjf.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://dxp.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uim.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://jic.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://pxd.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://kqn.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cou.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://khd.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dab.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://nhb.yj202588.top

Py:   value = d.get("k") or default
来源：http://wfr.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://fgy.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://twl.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://fjz.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sev.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zru.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://vtc.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://fqw.zhixingplan.top


<!-- 参考信息 -->