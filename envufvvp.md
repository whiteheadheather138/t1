代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zcu.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qye.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fjx.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cwh.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://jys.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zvf.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://hwo.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://fuv.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://vyh.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kxn.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ppj.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://qaw.quarkkingdee.top

C#:   File.Exists("a.txt")
来源：http://tso.shuidangran.top

[F06] 删除文件
来源：http://chw.fzhhl.top

Py:   os.remove("a.txt")
来源：http://hcu.zycfv.cn

PHP:  unlink("a.txt");
来源：http://bhn.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://tzc.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ibq.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://unx.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://gva.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://jwr.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://zih.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://yqz.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tfx.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ewr.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bsx.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tiw.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aac.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://obb.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kky.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oaf.fzhhl.top

[F08] 遍历目录
来源：http://peg.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://klf.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hcb.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://qfi.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://tmj.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://urq.andypj.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://hfo.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://vtp.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://iyy.quarkkingdee.top

[F09] 获取文件大小
来源：http://lzs.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ghh.andypj.xyz

PHP:  filesize("a.txt");
来源：http://mbp.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://gyt.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://gin.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oye.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ykk.cheryme.top

Ruby: File.size("a.txt")
来源：http://qqx.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://ueb.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://ctu.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ukv.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ojc.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kny.mhx1999.top

TS:   path.extname("a.txt")
来源：http://jtw.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rfl.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bpv.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rfa.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pll.tarul.cn

[F11] 复制与移动文件
来源：http://dwp.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rtt.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yhe.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zhq.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lae.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yjh.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lbt.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jxv.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://izg.sufxvd.cn

[F12] CSV 读写
来源：http://igv.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qzt.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ein.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cih.tian-w.cn

TS:   // 同上
来源：http://zpe.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nid.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bcm.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://msm.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://ymi.hammf.cn

================================================================================
来源：http://ikm.daria6918.cn

G. 面向对象
来源：http://hsw.sjlbkw.cn

================================================================================
来源：http://bzr.zdbjq.cn

[G01] 定义类
来源：http://akk.nwbrower.top

Py:   class User: pass
来源：http://iqz.xziqi.cn

PHP:  class User {}
来源：http://ebo.chenjidiqi.icu

JS:   class User {}
来源：http://pqd.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://eoh.shuidangran.top

Java: class User {}
来源：http://ifx.nwbrower.top

Go:   type User struct { Name string }
来源：http://fbd.tarul.cn

Ruby: class User; end
来源：http://hcb.zdbjq.cn

C#:   class User {}
来源：http://ber.cheryme.top

[G02] 构造函数
来源：http://ryr.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://wpr.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://svr.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://cvt.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://cuy.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://mye.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rbb.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://gan.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://ina.nwbrower.top

[G03] 实例属性
来源：http://sfr.wangdashe.top

Py:   self.name = "x"
来源：http://rjj.yangfankeji.com

PHP:  public string $name = "x";
来源：http://hsc.jinqigfzy.top

JS:   this.name = "x";
来源：http://tgr.dashuyun.cn

TS:   name: string = "x";
来源：http://iha.shangyingyoupin.top

Java: private String name;
来源：http://zmu.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dyc.yj202588.top

Ruby: @name = "x"
来源：http://hdx.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ych.iojbl.cn

[G04] 定义方法
来源：http://hfb.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://wkg.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hmn.nwbrower.top

JS:   greet() { return this.name; }
来源：http://vdi.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://zrn.cashguo.top

Java: String greet() { return name; }
来源：http://lns.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xvw.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://rsa.guannengcc.top

C#:   public string Greet() => Name;
来源：http://ncp.haohaochexian.top

[G05] 继承
来源：http://uhn.fehbvm.com

Py:   class Admin(User): pass
来源：http://bsi.havefunace.top

PHP:  class Admin extends User {}
来源：http://kuo.gogol.net.cn

JS:   class Admin extends User {}
来源：http://hhw.dashuyun.cn

TS:   class Admin extends User {}
来源：http://tqt.nwbrower.top

Java: class Admin extends User {}
来源：http://jkb.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://htv.yangfankeji.com

Ruby: class Admin < User; end
来源：http://vjb.andypj.xyz

C#:   class Admin : User {}
来源：http://zkw.fengsongda.top

[G06] 重写方法
来源：http://scy.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://ddg.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zhy.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://nnb.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://aiw.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://uxe.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iis.jianghu66.top

Ruby: def greet; "admin"; end
来源：http://whk.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://zhs.tian-w.cn

[G07] 调用父类方法
来源：http://qib.zhengqikj.top

Py:   super().greet()
来源：http://fnl.guannengcc.top

PHP:  parent::greet();
来源：http://vso.yanxiufei.cn

JS:   super.greet();
来源：http://wlt.zhengqikj.top

TS:   super.greet();
来源：http://pnw.0kj1m.cn

Java: super.greet();
来源：http://zzs.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://udx.cqqwz.cn

Ruby: super
来源：http://hbz.sysykeji.top

C#:   base.Greet();
来源：http://uih.jinqigfzy.top

[G08] 静态方法与属性
来源：http://rcl.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vnr.cashguo.top

PHP:  public static function f() {}
来源：http://inm.ehwqpu.com

JS:   static f() {}
来源：http://ecl.shuidangran.top

TS:   static f(): void {}
来源：http://zbw.yj202588.top

Java: static void f() {}
来源：http://omy.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dzf.dashuyun.cn

Ruby: def self.f; end
来源：http://vmb.pycfn.com

C#:   public static void F() {}
来源：http://aap.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://ufl.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://onw.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xml.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nfx.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://bth.yj202588.top

Java: interface Shape { double area(); }
来源：http://pzj.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://jnp.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ysn.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://tdq.zhongyouzk.top

[G10] 访问控制
来源：http://vac.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://yui.yonumen.top

PHP:  public / protected / private
来源：http://dhg.sysykeji.top

JS:   #private 字段；其余公开
来源：http://rqd.jinqigufen.top

TS:   public / protected / private
来源：http://mdq.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://vsf.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ary.aizwys.cn

Ruby: public / protected / private
来源：http://wci.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://uyi.birdmap.top

[G11] getter / setter
来源：http://kxz.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://iny.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://tpl.yj202588.top

JS:   get name() { return this._name; }
来源：http://qpt.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://fzs.jianghu66.top

Java: public String getName() { return name; }
来源：http://euk.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wqa.cdnleiting.top

Ruby: attr_accessor :name
来源：http://xxe.yj202588.top

C#:   public string Name { get; set; }
来源：http://bpb.hcnkem.com

[G12] 对象转字符串
来源：http://ttj.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://kmp.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jbc.xuanzx.com

JS:   toString() { return this.name; }
来源：http://ifd.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://wqh.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://egg.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://dev.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://dzr.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://nhc.iojbl.cn

[G13] 判断对象类型
来源：http://czs.uphjek.com

Py:   isinstance(u, User)
来源：http://zao.guannengcc.top

PHP:  $u instanceof User
来源：http://hho.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://tsv.yuxming.cn

TS:   u instanceof User
来源：http://yqp.xinyue.icu

Java: u instanceof User
来源：http://hvh.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qpn.zhiwuduotai.top

Ruby: u.is_a?(User)
来源：http://tnh.guowangkeji.top

C#:   u is User
来源：http://lzs.yuanzhike.top

[G14] 数据类 / record
来源：http://pgf.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://esu.sysykeji.top

PHP:  // 用 readonly 属性模拟
来源：http://djx.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://ffi.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://mny.bjfxy.top

Java: record User(String name, int age) {}
来源：http://sna.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://mqn.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aom.uphjek.com

C#:   record User(string Name, int Age);
来源：http://qwn.epnwcf.com

[G15] 枚举
来源：http://leo.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pvy.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://djl.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://opr.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bas.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://pst.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://llc.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://blf.pengpengdd.cyou

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vqy.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://rsh.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ulq.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://cpb.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://ztb.sysykeji.top

TS:   Object.entries(obj)
来源：http://qhn.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sne.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://fns.daria6918.cn

Ruby: obj.instance_variables
来源：http://sit.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://ttu.yj20258888.top

================================================================================
来源：http://gws.chenzaomai.com

H. 异常与错误处理
来源：http://gbk.cucudq.cn

================================================================================
来源：http://rpt.svipenyu.cn

[H01] try / catch 基础
来源：http://hnj.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gwq.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fxm.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cdj.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ytk.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uka.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yfj.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mfn.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ujg.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://bjf.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://xdx.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rbp.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vrg.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ogr.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://dqw.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nvn.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ova.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jat.vehdjk.com

[H03] 主动抛出异常
来源：http://izq.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://cjj.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wdg.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://oyn.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://ihc.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tkd.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nif.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bro.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://whx.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://dcb.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://cdg.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://kor.sweek.top

JS:   class MyError extends Error {}
来源：http://qlr.tanke756.top

TS:   class MyError extends Error {}
来源：http://tfm.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://lpq.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lxw.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://yad.yfazqb.com

C#:   class MyException : Exception {}
来源：http://uli.guowangkeji.top

[H05] 捕获特定类型
来源：http://dek.chenlongwang.top

Py:   except ValueError as e:
来源：http://dsv.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cjy.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://mrc.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://sut.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://pth.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dra.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://kzd.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gcb.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://xby.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://msx.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gxl.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://ave.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://ujp.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jcj.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qlz.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://wvl.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://xlo.yonumen.top

[H07] 断言
来源：http://ojc.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://ave.cdnleiting.top

PHP:  assert($x > 0);
来源：http://mzp.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://nmm.tanke756.top

TS:   console.assert(x > 0);
来源：http://kts.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://rsm.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pws.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iqd.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://zan.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://bsq.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://ylu.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ppc.hammf.cn

JS:   e.message;  e.stack
来源：http://klo.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://egl.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://agf.guowangkeji.top

Go:   err.Error()
来源：http://zet.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://dfh.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://jul.shzxlz.cn

[H09] 带错误码的异常
来源：http://dxg.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zvf.zhoulong.xyz


<!-- 参考信息 -->