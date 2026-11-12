代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://zkr.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bqk.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rvz.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vfy.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fkp.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://npu.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ijf.wangdashe.top

[F04] 追加写入文件
来源：http://eqj.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lat.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zvg.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdb.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ruf.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cdz.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lxt.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://all.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yyo.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://jfj.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ung.tanke756.top

PHP:  file_exists("a.txt");
来源：http://xwj.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://boo.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://ocq.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://jda.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://adl.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://cse.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://xfk.yongpay.top

[F06] 删除文件
来源：http://dtc.sweek.top

Py:   os.remove("a.txt")
来源：http://bjb.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://msm.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://keg.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://vpl.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://awk.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://xxj.316326.xyz

Ruby: File.delete("a.txt")
来源：http://uji.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://tls.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://xbo.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jzx.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tqs.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ncw.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://srm.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gjq.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kdw.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bks.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://csb.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://caf.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zqf.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qjo.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://nbb.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://hsr.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://klq.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fon.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://kvu.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://hxx.bbcook.cn

[F09] 获取文件大小
来源：http://vvi.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://fjy.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://ozp.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://voa.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://kwm.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lqb.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jff.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://abh.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://oeq.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://oia.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hod.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gkv.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sfx.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://mvy.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbv.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rnm.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fxr.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qgd.ehwqpu.com

[F11] 复制与移动文件
来源：http://prn.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sxb.shanyushiyangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iyv.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ihc.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzh.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xwi.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tkt.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nyz.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cwn.hfpthk.cn

[F12] CSV 读写
来源：http://xhl.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lnc.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nqm.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yku.yongpay.top

TS:   // 同上
来源：http://zwf.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jns.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vek.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dvk.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://qlw.yj20258.top

================================================================================
来源：http://lxu.52xcode.cn

G. 面向对象
来源：http://ibo.jlsjyb.cn

================================================================================
来源：http://sbp.sufxvd.cn

[G01] 定义类
来源：http://qit.chenzaomai.com

Py:   class User: pass
来源：http://thn.sysykeji.top

PHP:  class User {}
来源：http://vly.sjlbkw.cn

JS:   class User {}
来源：http://xan.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://hra.chenlongwang.top

Java: class User {}
来源：http://grw.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://yfo.fktsv.cn

Ruby: class User; end
来源：http://mos.chenjidiqi.icu

C#:   class User {}
来源：http://hpx.yj20258888.top

[G02] 构造函数
来源：http://eir.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://hsn.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://ijm.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://nxr.pycfn.com

TS:   constructor(public name: string) {}
来源：http://lyd.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://zxe.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://spo.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://fol.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://clo.cdnleiting.top

[G03] 实例属性
来源：http://jro.gzhubu.top

Py:   self.name = "x"
来源：http://ofz.hywenlv.cn

PHP:  public string $name = "x";
来源：http://xbc.daxiang520.top

JS:   this.name = "x";
来源：http://ofg.zycfv.cn

TS:   name: string = "x";
来源：http://zwk.vqdsnc.cn

Java: private String name;
来源：http://bxq.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hqz.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://mga.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://nwy.ybcxt.top

[G04] 定义方法
来源：http://kiq.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://xjc.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://cof.cashguo.top

JS:   greet() { return this.name; }
来源：http://lof.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://snc.nwbrower.top

Java: String greet() { return name; }
来源：http://vbt.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://joq.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://vcu.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://vjw.iojbl.cn

[G05] 继承
来源：http://bdu.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://msj.tarul.cn

PHP:  class Admin extends User {}
来源：http://yoj.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://okm.chenzaomai.com

TS:   class Admin extends User {}
来源：http://mai.hcnkem.com

Java: class Admin extends User {}
来源：http://irg.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pdr.sxryk.cn

Ruby: class Admin < User; end
来源：http://ysj.gzhubu.top

C#:   class Admin : User {}
来源：http://ese.guowangkeji.top

[G06] 重写方法
来源：http://kwi.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://gld.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vyp.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://udh.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://sjb.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://dpf.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ohe.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://bjk.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://une.52xcode.cn

[G07] 调用父类方法
来源：http://hla.wangshuangyany.cn

Py:   super().greet()
来源：http://qxw.gogol.net.cn

PHP:  parent::greet();
来源：http://hpv.sweek.top

JS:   super.greet();
来源：http://him.shangyingyoupin.top

TS:   super.greet();
来源：http://sfo.pycfn.com

Java: super.greet();
来源：http://tcb.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jxd.xinyue.icu

Ruby: super
来源：http://bfu.bjfxy.top

C#:   base.Greet();
来源：http://ngl.iojbl.cn

[G08] 静态方法与属性
来源：http://sjo.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iyu.kuanghao11.cn

PHP:  public static function f() {}
来源：http://twc.ctjpmb.com

JS:   static f() {}
来源：http://ltk.haohaochexian.top

TS:   static f(): void {}
来源：http://ppb.gogol.net.cn

Java: static void f() {}
来源：http://bxo.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ara.zhixingplan.top

Ruby: def self.f; end
来源：http://eek.gaohongyu789.top

C#:   public static void F() {}
来源：http://kle.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://dqz.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://jev.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://bao.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://prn.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://nmo.uphjek.com

Java: interface Shape { double area(); }
来源：http://lwc.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://shg.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tts.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://fgz.hnqzz.top

[G10] 访问控制
来源：http://dqs.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://wnl.hnqzz.top

PHP:  public / protected / private
来源：http://sez.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://qfq.zhoulong.xyz

TS:   public / protected / private
来源：http://tvx.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://gmb.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nsd.316326.xyz

Ruby: public / protected / private
来源：http://tam.xziqi.cn

C#:   public / protected / private / internal
来源：http://hrc.pengpengdd.cyou

[G11] getter / setter
来源：http://ove.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://ydx.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zlv.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://mnq.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://kfn.yangfankeji.com

Java: public String getName() { return name; }
来源：http://erd.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ilw.aibaodan.cn

Ruby: attr_accessor :name
来源：http://ckc.hnqzz.top

C#:   public string Name { get; set; }
来源：http://ysn.yuxming.cn

[G12] 对象转字符串
来源：http://ynz.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://jql.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://drl.316326.xyz

JS:   toString() { return this.name; }
来源：http://tra.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://dnm.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://hjv.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://pbp.sxryk.cn

Ruby: def to_s; @name; end
来源：http://rnr.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://xpu.ydjk.org.cn

[G13] 判断对象类型
来源：http://mnp.jyoumei.cn

Py:   isinstance(u, User)
来源：http://pse.jinqigfzy.top

PHP:  $u instanceof User
来源：http://tfj.havefunace.top

JS:   u instanceof User
来源：http://onq.haohaochexian.top

TS:   u instanceof User
来源：http://iuv.tianlin.xyz

Java: u instanceof User
来源：http://hgu.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gem.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://gpn.zhaomingkeji.xyz

C#:   u is User
来源：http://kmc.iojbl.cn

[G14] 数据类 / record
来源：http://jjm.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xnk.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cef.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://btc.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://ygj.tian-w.cn

Java: record User(String name, int age) {}
来源：http://qkw.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://seb.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mui.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://lsa.ivvv.top

[G15] 枚举
来源：http://gbx.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ikm.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fpk.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xan.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jqq.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://qqq.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mhu.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://kxt.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://euf.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://arb.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jbs.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://alf.gzhubu.top

JS:   Object.entries(obj)
来源：http://voi.tarul.cn

TS:   Object.entries(obj)
来源：http://wnw.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vpt.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://trx.dashuyun.cn

Ruby: obj.instance_variables
来源：http://xcz.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://kvd.shzxlz.cn

================================================================================
来源：http://pkz.jyoumei.cn

H. 异常与错误处理
来源：http://nrn.jinqigfzy.top

================================================================================
来源：http://cwb.epnwcf.com

[H01] try / catch 基础
来源：http://zxt.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://glt.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uad.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qfu.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cue.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nce.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xrb.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eei.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nxm.bbcook.cn

[H02] finally / ensure 收尾
来源：http://zwe.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kcl.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wlp.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wcj.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://pqh.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://eim.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vua.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://naq.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bmd.hnqzz.top

[H03] 主动抛出异常
来源：http://azf.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://ezp.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ulu.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://phn.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://bbq.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eae.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bsf.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mbo.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://jub.chenlongwang.top

[H04] 自定义异常类型
来源：http://cip.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://ixa.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://bbk.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://euk.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://cpz.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://jmd.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vyo.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://xoi.sysykeji.top

C#:   class MyException : Exception {}
来源：http://jcq.tarul.cn

[H05] 捕获特定类型
来源：http://ltn.uphjek.com

Py:   except ValueError as e:
来源：http://jtf.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tgj.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://vfr.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://zne.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://fgi.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mmd.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://xpe.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hxm.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://zsh.redwolf501.top

Py:   value = d.get("k") or default
来源：http://osi.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://fea.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://bar.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ptk.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nqe.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qkf.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://geu.dianchejie.cn

C#:   obj?.A?.B ?? default
来源：http://tko.smart0.xyz

[H07] 断言
来源：http://imi.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://yln.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://bvt.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://vqd.yueranfly.top

TS:   console.assert(x > 0);
来源：http://tka.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://tbx.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xqm.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wkv.ivvv.top


<!-- 参考信息 -->