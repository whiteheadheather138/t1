代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://lxb.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mtf.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ycq.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nuc.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ahv.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://tcn.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ige.yuanzhike.top

[F04] 追加写入文件
来源：http://ufp.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://inf.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mtf.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjq.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzy.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aap.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ufy.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lqj.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://agw.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://hgc.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qaq.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://tqc.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://vfj.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://dsn.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://sql.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uzi.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://vpk.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://ekb.xylfe.cn

[F06] 删除文件
来源：http://swx.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://xbc.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://ftm.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://qyr.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nri.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ozt.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://jqg.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://sar.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://uux.daria6918.cn

[F07] 创建目录（含多级）
来源：http://lwe.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mfg.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gbs.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpo.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sdn.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://laf.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cas.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mxn.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aqs.jianghu66.top

[F08] 遍历目录
来源：http://hau.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nqq.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hjn.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://pfq.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://hsy.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lbo.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bwz.fehbvm.com

Ruby: Dir.children("dir")
来源：http://bxe.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://wsp.epnwcf.com

[F09] 获取文件大小
来源：http://jhe.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://lfl.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://zqt.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://crw.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://kof.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://pwv.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qga.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://thc.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://lmv.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://wrw.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wdr.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cak.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fum.c1oappe.top

TS:   path.extname("a.txt")
来源：http://xus.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://izp.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tgv.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nrj.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lxj.sysykeji.top

[F11] 复制与移动文件
来源：http://fmw.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zsq.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wea.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iaf.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ksx.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sxc.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hss.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rqg.vehdjk.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://czu.yj20258.top

[F12] CSV 读写
来源：http://sdg.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uoh.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ftq.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aws.shzxlz.cn

TS:   // 同上
来源：http://ucz.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rpc.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wdh.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mlx.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hdv.iojbl.cn

================================================================================
来源：http://nxl.gotoacloud.top

G. 面向对象
来源：http://rwu.andypj.xyz

================================================================================
来源：http://ccy.xinyue.icu

[G01] 定义类
来源：http://ycs.bjfxy.top

Py:   class User: pass
来源：http://ntf.yj20258888.top

PHP:  class User {}
来源：http://htb.vqdsnc.cn

JS:   class User {}
来源：http://bfj.yongpay.top

TS:   class User { name: string = ""; }
来源：http://adj.xuetiantiany.cn

Java: class User {}
来源：http://ytm.uphjek.com

Go:   type User struct { Name string }
来源：http://csa.cashguo.top

Ruby: class User; end
来源：http://vvc.shuidangran.top

C#:   class User {}
来源：http://cqi.xylfe.cn

[G02] 构造函数
来源：http://eok.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://ujj.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://gpf.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://pgx.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://ect.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://dij.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ohg.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://myi.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://olq.vehdjk.com

[G03] 实例属性
来源：http://mod.tarul.cn

Py:   self.name = "x"
来源：http://dyf.svipenyu.cn

PHP:  public string $name = "x";
来源：http://zwr.yuanzhike.top

JS:   this.name = "x";
来源：http://blt.hesvh.cn

TS:   name: string = "x";
来源：http://wyz.redwolf501.top

Java: private String name;
来源：http://nkv.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jbm.yangfankeji.com

Ruby: @name = "x"
来源：http://iyy.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lrw.zhongyouzk.top

[G04] 定义方法
来源：http://vkk.hcnkem.com

Py:   def greet(self): return self.name
来源：http://sks.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tly.aizwys.cn

JS:   greet() { return this.name; }
来源：http://dgk.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://mow.wangdashe.top

Java: String greet() { return name; }
来源：http://vpo.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dpg.yonumen.top

Ruby: def greet; @name; end
来源：http://oml.pycfn.com

C#:   public string Greet() => Name;
来源：http://vho.sweek.top

[G05] 继承
来源：http://dyh.jyoumei.cn

Py:   class Admin(User): pass
来源：http://vmo.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://wav.jiagoushi.top

JS:   class Admin extends User {}
来源：http://whm.jyoumei.cn

TS:   class Admin extends User {}
来源：http://aub.cucudq.cn

Java: class Admin extends User {}
来源：http://rlf.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oab.sxryk.cn

Ruby: class Admin < User; end
来源：http://suf.chenzaomai.com

C#:   class Admin : User {}
来源：http://bsi.jqgfzy.top

[G06] 重写方法
来源：http://qky.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://eit.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hrn.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://mpv.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://wio.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://wub.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lpl.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://jag.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://qoe.meibo888.top

[G07] 调用父类方法
来源：http://ptu.andypj.xyz

Py:   super().greet()
来源：http://nct.aibaodan.cn

PHP:  parent::greet();
来源：http://hzp.ydjk.org.cn

JS:   super.greet();
来源：http://uki.hesvh.cn

TS:   super.greet();
来源：http://wgd.cucudq.cn

Java: super.greet();
来源：http://zgd.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uhd.gaohongyu789.top

Ruby: super
来源：http://jmb.chenjidiqi.icu

C#:   base.Greet();
来源：http://rpe.jyoumei.cn

[G08] 静态方法与属性
来源：http://qfg.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://agz.hnqzz.top

PHP:  public static function f() {}
来源：http://yrh.zdqjudy.top

JS:   static f() {}
来源：http://svc.gotoacloud.top

TS:   static f(): void {}
来源：http://qer.daxiang520.top

Java: static void f() {}
来源：http://bzm.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ebk.sxryk.cn

Ruby: def self.f; end
来源：http://dsf.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://msh.yvedp.cn

[G09] 接口 / 抽象类
来源：http://ctg.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://mkb.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://psz.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://shm.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://csl.hesvh.cn

Java: interface Shape { double area(); }
来源：http://bau.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ijp.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lmt.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://rux.jlsjyb.cn

[G10] 访问控制
来源：http://sab.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://xjn.gaohongyu789.top

PHP:  public / protected / private
来源：http://xmj.birdmap.top

JS:   #private 字段；其余公开
来源：http://cut.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://res.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://fdu.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://mlc.epnwcf.com

Ruby: public / protected / private
来源：http://akn.tarul.cn

C#:   public / protected / private / internal
来源：http://eld.birdmap.top

[G11] getter / setter
来源：http://wtt.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://vdc.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dtl.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://eko.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://xdl.zycfv.cn

Java: public String getName() { return name; }
来源：http://yqh.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://msb.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://mnm.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://ujd.svipenyu.cn

[G12] 对象转字符串
来源：http://lhh.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://ucd.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ozk.xylfe.cn

JS:   toString() { return this.name; }
来源：http://izb.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://kgk.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://qgd.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tdc.yj202588.top

Ruby: def to_s; @name; end
来源：http://syw.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://whr.ppjwa.cn

[G13] 判断对象类型
来源：http://ezc.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://nfe.jinqigfzy.top

PHP:  $u instanceof User
来源：http://fff.zdbjq.cn

JS:   u instanceof User
来源：http://ijq.jinghuilouyu.cn

TS:   u instanceof User
来源：http://lvs.zhiwuduotai.top

Java: u instanceof User
来源：http://qtk.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://owb.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://tji.jlsjyb.cn

C#:   u is User
来源：http://ywc.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://wgx.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hpw.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://qoq.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://wmx.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://tzu.daxiang520.top

Java: record User(String name, int age) {}
来源：http://vef.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://ewe.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ysa.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://hun.svipenyu.cn

[G15] 枚举
来源：http://saf.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yby.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://asq.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ffd.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cks.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://fvi.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jzu.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://mzw.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://noa.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://ygc.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://axw.tanke756.top

PHP:  get_object_vars($obj);
来源：http://dsh.ehwqpu.com

JS:   Object.entries(obj)
来源：http://yum.haohaochexian.top

TS:   Object.entries(obj)
来源：http://fzs.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oyt.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nyo.sweek.top

Ruby: obj.instance_variables
来源：http://jes.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://xvu.hnqzz.top

================================================================================
来源：http://jwq.yj20258888.top

H. 异常与错误处理
来源：http://rzu.jqgufenzy.top

================================================================================
来源：http://eoz.xuanzx.com

[H01] try / catch 基础
来源：http://rnr.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bkf.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nvp.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qxg.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sok.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://had.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wig.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ywk.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xbj.yj20258.top

[H02] finally / ensure 收尾
来源：http://jrr.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://wsb.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://agv.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://vqw.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xgi.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://ghy.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://plq.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fbe.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://mfk.sweek.top

[H03] 主动抛出异常
来源：http://jte.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://hyp.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mrk.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://sta.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://cez.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://izc.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mrx.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://rxq.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://aut.yj20258888.top

[H04] 自定义异常类型
来源：http://une.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://ruv.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://imh.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://srw.redwolf501.top

TS:   class MyError extends Error {}
来源：http://bsl.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://eus.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jqi.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://jvi.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://pyl.uphjek.com

[H05] 捕获特定类型
来源：http://kkz.dashuyun.cn

Py:   except ValueError as e:
来源：http://mtg.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hdo.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://vom.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://qmf.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://azx.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://abn.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://bzt.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://djz.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://vtk.epnwcf.com

Py:   value = d.get("k") or default
来源：http://wty.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dto.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://oxy.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rsb.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://czo.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tkm.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://arh.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://qpn.xylfe.cn

[H07] 断言
来源：http://xom.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://rou.tian-w.cn

PHP:  assert($x > 0);
来源：http://jwm.ybcxt.top

JS:   console.assert(x > 0);
来源：http://trl.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://ied.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://jic.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vxd.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://vjy.tarul.cn


<!-- 参考信息 -->