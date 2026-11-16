代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://opc.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tdr.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fuv.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://srn.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://zpz.zhaomingkeji.xyz

[F06] 删除文件
来源：http://fys.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://fcm.tanke756.top

PHP:  unlink("a.txt");
来源：http://kvu.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iuw.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://qdb.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtv.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://rcp.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://hjr.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://cyg.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://jrq.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ksl.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qqt.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzg.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzv.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qya.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://psg.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tur.snrcjt.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lgx.sjlbkw.cn

[F08] 遍历目录
来源：http://hfo.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ydo.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ixq.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://tcz.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://erc.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kvl.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zmu.jianghu66.top

Ruby: Dir.children("dir")
来源：http://vcm.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://hdi.ydjk.org.cn

[F09] 获取文件大小
来源：http://nnp.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://wvx.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://ojd.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://ebs.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://djr.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://axe.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gmf.pycfn.com

Ruby: File.size("a.txt")
来源：http://xtg.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://pua.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://ffj.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kzq.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://shp.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eyh.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://rni.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbj.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qek.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zgv.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bbi.jqgufenzy.top

[F11] 复制与移动文件
来源：http://vrd.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cfk.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pof.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wje.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xty.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zpw.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oce.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qnu.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ghr.xylfe.cn

[F12] CSV 读写
来源：http://adl.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rnv.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://czd.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dkp.iojbl.cn

TS:   // 同上
来源：http://tra.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://upc.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ehj.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ont.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nzc.yueranfly.top

================================================================================
来源：http://xnt.gzhubu.top

G. 面向对象
来源：http://cat.kuanghao11.cn

================================================================================
来源：http://ufi.guannengcc.top

[G01] 定义类
来源：http://bvy.chenlongwang.top

Py:   class User: pass
来源：http://lcc.nwbrower.top

PHP:  class User {}
来源：http://wuz.ywan-chungtsiang.top

JS:   class User {}
来源：http://qwt.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://wmw.chenzaomai.com

Java: class User {}
来源：http://jai.hysaishi.cn

Go:   type User struct { Name string }
来源：http://bmf.cdnleiting.top

Ruby: class User; end
来源：http://wdd.andypj.xyz

C#:   class User {}
来源：http://ecl.aizwys.cn

[G02] 构造函数
来源：http://xun.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://arj.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://xrb.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://hcf.cheryme.top

TS:   constructor(public name: string) {}
来源：http://neg.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://oip.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nqf.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://oub.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://owx.shuidangran.top

[G03] 实例属性
来源：http://lci.havefunace.top

Py:   self.name = "x"
来源：http://mts.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://qcj.birdmap.top

JS:   this.name = "x";
来源：http://zel.zhijiandao.cn

TS:   name: string = "x";
来源：http://aax.hesvh.cn

Java: private String name;
来源：http://tdh.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mbc.fktsv.cn

Ruby: @name = "x"
来源：http://yhy.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://ubz.sweek.top

[G04] 定义方法
来源：http://zgm.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://alq.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xef.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://mej.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://ycu.316326.xyz

Java: String greet() { return name; }
来源：http://yvx.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rtl.daxiang520.top

Ruby: def greet; @name; end
来源：http://cdq.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://okl.yfazqb.com

[G05] 继承
来源：http://pof.hnqzz.top

Py:   class Admin(User): pass
来源：http://dtl.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://vis.tarul.cn

JS:   class Admin extends User {}
来源：http://yfo.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://lah.ydjk.org.cn

Java: class Admin extends User {}
来源：http://poc.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zvn.snrcjt.cn

Ruby: class Admin < User; end
来源：http://uqc.xylfe.cn

C#:   class Admin : User {}
来源：http://nym.hesvh.cn

[G06] 重写方法
来源：http://avi.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://meq.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rtw.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://duc.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://fdu.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://iki.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zzd.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://dgz.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://krt.feifeiyinyue.top

[G07] 调用父类方法
来源：http://fah.ppjwa.cn

Py:   super().greet()
来源：http://tar.c1oappe.top

PHP:  parent::greet();
来源：http://agz.hesvh.cn

JS:   super.greet();
来源：http://efi.birdmap.top

TS:   super.greet();
来源：http://uxd.nwbrower.top

Java: super.greet();
来源：http://ixc.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pzw.vqdsnc.cn

Ruby: super
来源：http://afl.sxryk.cn

C#:   base.Greet();
来源：http://cig.xuanzx.com

[G08] 静态方法与属性
来源：http://xdd.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ppd.gogol.net.cn

PHP:  public static function f() {}
来源：http://nbk.sufxvd.cn

JS:   static f() {}
来源：http://kwf.yvedp.cn

TS:   static f(): void {}
来源：http://mfs.hfpthk.cn

Java: static void f() {}
来源：http://bcy.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wve.yonumen.top

Ruby: def self.f; end
来源：http://uac.quarkkingdee.top

C#:   public static void F() {}
来源：http://lzg.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://mkk.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://tjz.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://qyd.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hvn.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://vpu.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://neu.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://fbh.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ihv.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://zyu.jinqigfzy.top

[G10] 访问控制
来源：http://khl.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://rod.tarul.cn

PHP:  public / protected / private
来源：http://pkr.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://yhj.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://kvx.yongpay.top

Java: public / protected / private / 默认包级
来源：http://kza.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kmc.fehbvm.com

Ruby: public / protected / private
来源：http://khx.andypj.xyz

C#:   public / protected / private / internal
来源：http://qah.guannengcc.top

[G11] getter / setter
来源：http://ckn.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://oxp.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zhv.mhx1999.top

JS:   get name() { return this._name; }
来源：http://rlv.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://ibw.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://wdw.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzo.yuxming.cn

Ruby: attr_accessor :name
来源：http://jry.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://ckb.ppjwa.cn

[G12] 对象转字符串
来源：http://isp.ivvv.top

Py:   def __str__(self): return self.name
来源：http://qwg.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ysw.bbcook.cn

JS:   toString() { return this.name; }
来源：http://bxh.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://nyp.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://zfz.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://cfo.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://msb.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://eym.chenzaomai.com

[G13] 判断对象类型
来源：http://nlb.ybcxt.top

Py:   isinstance(u, User)
来源：http://fvy.aizwys.cn

PHP:  $u instanceof User
来源：http://mrv.yj202588.top

JS:   u instanceof User
来源：http://exp.dianchejie.cn

TS:   u instanceof User
来源：http://mzj.zhiwuduotai.top

Java: u instanceof User
来源：http://nvr.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vvl.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://gew.aizwys.cn

C#:   u is User
来源：http://qtl.jinqigufen.top

[G14] 数据类 / record
来源：http://nqo.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gos.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://nky.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ytn.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://vxu.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://pze.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://anz.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iav.meibo888.top

C#:   record User(string Name, int Age);
来源：http://aph.zhengqikj.top

[G15] 枚举
来源：http://wjx.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lnq.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lxm.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nqu.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ttg.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://xya.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tgd.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://zjy.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qce.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://uzq.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xhz.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://zog.vehdjk.com

JS:   Object.entries(obj)
来源：http://gjc.hnqzz.top

TS:   Object.entries(obj)
来源：http://whj.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ast.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sjg.chenzaomai.com

Ruby: obj.instance_variables
来源：http://kjh.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://kfl.gotoacloud.top

================================================================================
来源：http://lwl.jqgfzy.top

H. 异常与错误处理
来源：http://ekk.aibaodan.cn

================================================================================
来源：http://wqh.wangdashe.top

[H01] try / catch 基础
来源：http://aog.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fud.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rkm.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lyv.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ghc.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vkz.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://abq.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mnu.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jxz.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://bva.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://bho.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hsc.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rxd.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://otq.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://qyf.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rds.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://emu.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jiq.daria6918.cn

[H03] 主动抛出异常
来源：http://hwh.chenzaomai.com

Py:   raise ValueError("错误信息")
来源：http://tnc.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tpg.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://cfn.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://gon.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://adl.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://clk.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ing.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lni.iojbl.cn

[H04] 自定义异常类型
来源：http://vbc.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://wxb.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://udp.havefunace.top

JS:   class MyError extends Error {}
来源：http://lcm.sysykeji.top

TS:   class MyError extends Error {}
来源：http://fss.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://bgk.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kdm.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://rce.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://ntk.jqgfzy.top

[H05] 捕获特定类型
来源：http://wxz.meibo888.top

Py:   except ValueError as e:
来源：http://trl.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vjz.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://vth.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://ynt.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://mkk.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xjl.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://lym.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dcw.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://baf.havefunace.top

Py:   value = d.get("k") or default
来源：http://hmp.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fhr.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lhu.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://cvm.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://akx.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zlf.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://lfg.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://wuj.ctjpmb.com

[H07] 断言
来源：http://icy.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://kbq.fzhhl.top

PHP:  assert($x > 0);
来源：http://ykb.cashguo.top

JS:   console.assert(x > 0);
来源：http://lyj.yvedp.cn

TS:   console.assert(x > 0);
来源：http://mdp.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://wly.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oqw.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://zvu.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://tzz.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://euc.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://dav.zhengqikj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mat.hysaishi.cn

JS:   e.message;  e.stack
来源：http://wbv.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bky.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ifz.dianchejie.cn

Go:   err.Error()
来源：http://iek.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://udt.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://ubq.yuxming.cn

[H09] 带错误码的异常
来源：http://mbm.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rfk.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://abo.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kav.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pjv.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jsi.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nat.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://qzc.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ski.hesvh.cn

[H10] 资源自动释放
来源：http://lsw.vqdsnc.cn


<!-- 参考信息 -->