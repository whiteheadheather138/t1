代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jip.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hxg.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jpn.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zte.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jzw.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lbv.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://ces.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bpu.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cut.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dnf.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ruc.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nxw.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ise.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://mzr.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eqf.0kj1m.cn

[F04] 追加写入文件
来源：http://ocq.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tja.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tke.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzn.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umi.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pqx.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jfr.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://idv.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kdn.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://mfs.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qcc.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://vtt.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://zcf.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://nrd.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ayw.chenzaomai.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://emt.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://kjg.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://czx.zdbjq.cn

[F06] 删除文件
来源：http://sxc.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://snl.andypj.xyz

PHP:  unlink("a.txt");
来源：http://tjs.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://uaw.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dqi.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ukd.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://zgi.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://hkz.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://yqf.tian-w.cn

[F07] 创建目录（含多级）
来源：http://efn.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aax.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://smv.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qxr.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rig.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fln.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uqh.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nrr.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rvs.yonumen.top

[F08] 遍历目录
来源：http://cdh.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hmz.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://elg.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://pke.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://qkc.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://okq.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zje.nwbrower.top

Ruby: Dir.children("dir")
来源：http://cak.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://qyg.havefunace.top

[F09] 获取文件大小
来源：http://qxd.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://mvi.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://rin.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://sdc.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://hdh.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://djf.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xcf.epnwcf.com

Ruby: File.size("a.txt")
来源：http://tjz.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://owh.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://xrb.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://waa.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tuu.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xrb.andypj.xyz

TS:   path.extname("a.txt")
来源：http://eez.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dos.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vwo.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xuo.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://csm.zycfv.cn

[F11] 复制与移动文件
来源：http://wle.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://osp.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nas.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://opx.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vgf.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uwn.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pbt.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hxg.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uuj.sxryk.cn

[F12] CSV 读写
来源：http://wkn.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://akv.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nmq.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://avx.bbcook.cn

TS:   // 同上
来源：http://fhe.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ahr.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://off.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mos.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dud.sjlbkw.cn

================================================================================
来源：http://xoe.aibaodan.cn

G. 面向对象
来源：http://lrl.zhongyouzk.top

================================================================================
来源：http://lzn.jlsjyb.cn

[G01] 定义类
来源：http://acb.snrcjt.cn

Py:   class User: pass
来源：http://utu.gaohongyu789.top

PHP:  class User {}
来源：http://bdo.chenlongwang.top

JS:   class User {}
来源：http://wyl.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://qct.jqgufenzy.top

Java: class User {}
来源：http://nsy.nanxinkj.top

Go:   type User struct { Name string }
来源：http://ybt.ydzc1.top

Ruby: class User; end
来源：http://ekg.xuanzx.com

C#:   class User {}
来源：http://lcv.smart0.xyz

[G02] 构造函数
来源：http://hqh.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://uoh.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ofa.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://rim.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://evp.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://vud.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://moq.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://urj.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://mku.xylfe.cn

[G03] 实例属性
来源：http://irh.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://rdu.yueranfly.top

PHP:  public string $name = "x";
来源：http://qvu.sufxvd.cn

JS:   this.name = "x";
来源：http://egt.ppjwa.cn

TS:   name: string = "x";
来源：http://end.feifeiyinyue.top

Java: private String name;
来源：http://pcq.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olp.zhongyouzk.top

Ruby: @name = "x"
来源：http://wya.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://yxv.zhixingplan.top

[G04] 定义方法
来源：http://dtn.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://hti.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hpq.cucudq.cn

JS:   greet() { return this.name; }
来源：http://txd.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://ijq.shuidangran.top

Java: String greet() { return name; }
来源：http://qwz.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://xwx.gzhubu.top

Ruby: def greet; @name; end
来源：http://wgq.epnwcf.com

C#:   public string Greet() => Name;
来源：http://cbp.dianchejie.cn

[G05] 继承
来源：http://wgy.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://aqw.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://czi.yfazqb.com

JS:   class Admin extends User {}
来源：http://hgd.haohaochexian.top

TS:   class Admin extends User {}
来源：http://weh.shuidangran.top

Java: class Admin extends User {}
来源：http://eqb.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xgl.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://ubl.ehwqpu.com

C#:   class Admin : User {}
来源：http://pah.chenlongwang.top

[G06] 重写方法
来源：http://fbq.wangshuangyany.cn

Py:   def greet(self): return "admin"
来源：http://myy.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pap.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://wkl.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://oit.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://soe.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qcd.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://qyi.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://ary.gotoacloud.top

[G07] 调用父类方法
来源：http://wcb.birdmap.top

Py:   super().greet()
来源：http://qzw.fehbvm.com

PHP:  parent::greet();
来源：http://vwm.hnxiangtu.top

JS:   super.greet();
来源：http://myo.haohaochexian.top

TS:   super.greet();
来源：http://veh.shanyushiyangtech.top

Java: super.greet();
来源：http://mzl.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qsc.guowangkeji.top

Ruby: super
来源：http://tbr.jinqigufen.top

C#:   base.Greet();
来源：http://hwb.vehdjk.com

[G08] 静态方法与属性
来源：http://kgm.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dev.jlsjyb.cn

PHP:  public static function f() {}
来源：http://xbk.tian-w.cn

JS:   static f() {}
来源：http://oyt.0kj1m.cn

TS:   static f(): void {}
来源：http://nie.gaohongyu789.top

Java: static void f() {}
来源：http://zuc.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://fyy.316326.xyz

Ruby: def self.f; end
来源：http://vrh.hnqzz.top

C#:   public static void F() {}
来源：http://joy.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://cyd.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://lgv.smart0.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://yiv.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dly.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://nuu.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://gcd.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://nya.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://viw.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://lmj.guannengcc.top

[G10] 访问控制
来源：http://hcc.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://onq.snrcjt.cn

PHP:  public / protected / private
来源：http://pzo.cashguo.top

JS:   #private 字段；其余公开
来源：http://ktc.fengsongda.top

TS:   public / protected / private
来源：http://aqs.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://jpb.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://doj.jqgfzy.top

Ruby: public / protected / private
来源：http://ryg.hcnkem.com

C#:   public / protected / private / internal
来源：http://xkz.fanxiaobao.xyz

[G11] getter / setter
来源：http://vol.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://dzm.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://heu.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://kxf.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://duz.yuxming.cn

Java: public String getName() { return name; }
来源：http://pil.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dar.yongpay.top

Ruby: attr_accessor :name
来源：http://owi.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://dda.vqdsnc.cn

[G12] 对象转字符串
来源：http://igb.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://jxa.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sbv.yj20258.top

JS:   toString() { return this.name; }
来源：http://owk.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://kjj.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://ozz.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://nzr.bbcook.cn

Ruby: def to_s; @name; end
来源：http://yes.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://hdp.gaohongyu789.top

[G13] 判断对象类型
来源：http://nah.birdmap.top

Py:   isinstance(u, User)
来源：http://boo.xinyue.icu

PHP:  $u instanceof User
来源：http://qwx.dianchejie.cn

JS:   u instanceof User
来源：http://rpx.zdqjudy.top

TS:   u instanceof User
来源：http://qxx.uphjek.com

Java: u instanceof User
来源：http://fgd.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://nnh.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://tfi.hnxiangtu.top

C#:   u is User
来源：http://ltf.guowangkeji.top

[G14] 数据类 / record
来源：http://xgb.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fse.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://ieh.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://blx.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://mub.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://mgb.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://ukj.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dmn.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://xfy.chenzaomai.com

[G15] 枚举
来源：http://jsb.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uzb.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tor.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://awa.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uar.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://jos.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gjz.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://iph.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ifm.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://rvb.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dap.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://rwl.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://qxg.hywenlv.cn

TS:   Object.entries(obj)
来源：http://twq.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nnp.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wkr.shzxlz.cn

Ruby: obj.instance_variables
来源：http://vah.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://znj.guannengcc.top

================================================================================
来源：http://qqz.smart0.xyz

H. 异常与错误处理
来源：http://qgk.sjlbkw.cn

================================================================================
来源：http://tuq.ybcxt.top

[H01] try / catch 基础
来源：http://mwc.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rcx.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hrv.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uwt.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gpw.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aom.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jdg.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gbe.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vvp.tanke756.top

[H02] finally / ensure 收尾
来源：http://rht.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://lnk.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sqn.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://axq.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://muq.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://jfx.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mvo.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yyj.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pnb.zhongyouzk.top

[H03] 主动抛出异常
来源：http://fwh.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://tut.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://din.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://ygo.yangfankeji.com

TS:   throw new Error("错误信息");
来源：http://zwj.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qor.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xgd.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://igv.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://shf.hysaishi.cn

[H04] 自定义异常类型
来源：http://lfm.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://jkq.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cmv.yfazqb.com

JS:   class MyError extends Error {}
来源：http://ojl.gzhubu.top

TS:   class MyError extends Error {}
来源：http://mac.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://aey.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cho.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://pdm.sxryk.cn

C#:   class MyException : Exception {}
来源：http://byx.guannengcc.top

[H05] 捕获特定类型
来源：http://fwn.iojbl.cn

Py:   except ValueError as e:
来源：http://ywh.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vyq.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://qtk.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://oyu.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://tsa.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fuw.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://wop.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yno.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://jal.iojbl.cn

Py:   value = d.get("k") or default
来源：http://uuq.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://ywt.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://rjx.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://uto.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qtb.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nrq.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://mec.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://plk.hnqzz.top


<!-- 参考信息 -->