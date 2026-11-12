代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hvw.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uhr.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://enm.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://upt.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://jeg.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nqo.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://zgp.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://mtw.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://tij.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jlh.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pul.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://gap.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://suo.haohaochexian.top

[F06] 删除文件
来源：http://gjv.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://anp.yj20258.top

PHP:  unlink("a.txt");
来源：http://qac.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zsk.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://umi.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hce.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://mta.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://tqi.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://fre.cashguo.top

[F07] 创建目录（含多级）
来源：http://bia.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://akf.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ito.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxm.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iws.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oll.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ntw.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jww.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mlb.shzxlz.cn

[F08] 遍历目录
来源：http://hqm.vqdsnc.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://weu.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mfo.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://xfq.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://ril.dianchejie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hxz.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mpk.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://dqi.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://vqx.chenzaomai.com

[F09] 获取文件大小
来源：http://vxa.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://ysk.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://ewz.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://hbb.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://uzm.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lno.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jec.fzhhl.top

Ruby: File.size("a.txt")
来源：http://cjx.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://cat.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://cwl.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fdt.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zmk.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kdm.daxiang520.top

TS:   path.extname("a.txt")
来源：http://bpd.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbc.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cks.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://szr.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gvp.wangdashe.top

[F11] 复制与移动文件
来源：http://lla.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://njn.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mzw.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqb.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://czm.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ott.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mey.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uqy.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xdc.jlsjyb.cn

[F12] CSV 读写
来源：http://vtj.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zeb.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://asl.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yld.hywenlv.cn

TS:   // 同上
来源：http://ceb.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://obt.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ufw.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://clq.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://imf.yongpay.top

================================================================================
来源：http://itx.jyoumei.cn

G. 面向对象
来源：http://tbf.ybcxt.top

================================================================================
来源：http://vkh.redwolf501.top

[G01] 定义类
来源：http://bwj.yfazqb.com

Py:   class User: pass
来源：http://mir.yanxiufei.cn

PHP:  class User {}
来源：http://rln.jqgfzy.top

JS:   class User {}
来源：http://wsq.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://vzl.zhoulong.xyz

Java: class User {}
来源：http://rrx.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://jhb.vehdjk.com

Ruby: class User; end
来源：http://dpk.fktsv.cn

C#:   class User {}
来源：http://qpg.epnwcf.com

[G02] 构造函数
来源：http://uir.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://ppd.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://zne.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://xay.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://vcy.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://els.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lqq.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://eml.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://cns.ivvv.top

[G03] 实例属性
来源：http://pyd.xuanzx.com

Py:   self.name = "x"
来源：http://yph.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://gez.smart0.xyz

JS:   this.name = "x";
来源：http://qmd.yonumen.top

TS:   name: string = "x";
来源：http://vcf.316326.xyz

Java: private String name;
来源：http://kdx.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jai.xylfe.cn

Ruby: @name = "x"
来源：http://sfe.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://djm.cheryme.top

[G04] 定义方法
来源：http://mrf.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://vll.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fgk.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://ech.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://hsv.jqgfzy.top

Java: String greet() { return name; }
来源：http://pdw.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lfn.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://xae.hcnkem.com

C#:   public string Greet() => Name;
来源：http://zzz.yangfankeji.com

[G05] 继承
来源：http://nub.aibaodan.cn

Py:   class Admin(User): pass
来源：http://oeb.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://wst.ctjpmb.com

JS:   class Admin extends User {}
来源：http://lbd.zdqjudy.top

TS:   class Admin extends User {}
来源：http://bud.hysaishi.cn

Java: class Admin extends User {}
来源：http://wbp.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mwd.ybcxt.top

Ruby: class Admin < User; end
来源：http://mkt.nanxinkj.top

C#:   class Admin : User {}
来源：http://wfc.tarul.cn

[G06] 重写方法
来源：http://nnm.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://bjx.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pcj.tanke756.top

JS:   greet() { return "admin"; }
来源：http://zzv.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://gsd.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://odd.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://twh.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://idn.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://kit.yonumen.top

[G07] 调用父类方法
来源：http://kwa.9152youxi.cn

Py:   super().greet()
来源：http://nhh.hcnkem.com

PHP:  parent::greet();
来源：http://bgn.yueranfly.top

JS:   super.greet();
来源：http://wrv.zhijiandao.cn

TS:   super.greet();
来源：http://nie.guowangkeji.top

Java: super.greet();
来源：http://tce.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xgn.yj202588.top

Ruby: super
来源：http://lpw.gzhubu.top

C#:   base.Greet();
来源：http://eox.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://xoj.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ckf.havefunace.top

PHP:  public static function f() {}
来源：http://hlk.fengsongda.top

JS:   static f() {}
来源：http://wrw.yuxming.cn

TS:   static f(): void {}
来源：http://gks.jinqigufen.top

Java: static void f() {}
来源：http://fyx.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zqo.gotoacloud.top

Ruby: def self.f; end
来源：http://ndf.uphjek.com

C#:   public static void F() {}
来源：http://nyy.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://bwm.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://xbu.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://gur.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bhw.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://rhv.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://hsp.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://lvu.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yft.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://fks.hongshengwenyu.top

[G10] 访问控制
来源：http://scf.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://iug.sysykeji.top

PHP:  public / protected / private
来源：http://jih.xylfe.cn

JS:   #private 字段；其余公开
来源：http://pgv.jlsjyb.cn

TS:   public / protected / private
来源：http://igh.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://lju.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://nkd.vqdsnc.cn

Ruby: public / protected / private
来源：http://aor.yfazqb.com

C#:   public / protected / private / internal
来源：http://tfp.ydjk.org.cn

[G11] getter / setter
来源：http://ndl.guannengcc.top

Py:   @property 与 @x.setter
来源：http://uvu.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://twp.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://psu.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://xye.aibaodan.cn

Java: public String getName() { return name; }
来源：http://zif.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pke.shzxlz.cn

Ruby: attr_accessor :name
来源：http://xin.cucudq.cn

C#:   public string Name { get; set; }
来源：http://fjk.tianlin.xyz

[G12] 对象转字符串
来源：http://yek.uphjek.com

Py:   def __str__(self): return self.name
来源：http://nno.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ken.yuxming.cn

JS:   toString() { return this.name; }
来源：http://khz.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://mno.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://fcu.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zrr.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://wwq.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://byt.zhijiandao.cn

[G13] 判断对象类型
来源：http://ywt.hfpthk.cn

Py:   isinstance(u, User)
来源：http://rxd.bjfxy.top

PHP:  $u instanceof User
来源：http://tce.tian-w.cn

JS:   u instanceof User
来源：http://ior.ydzc1.top

TS:   u instanceof User
来源：http://gft.pengpengdd.cyou

Java: u instanceof User
来源：http://irz.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://enf.xuanzx.com

Ruby: u.is_a?(User)
来源：http://ngg.dianchejie.cn

C#:   u is User
来源：http://bmz.kuanghao11.cn

[G14] 数据类 / record
来源：http://ttb.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://omi.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://bnw.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://trv.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://mtf.yj20258.top

Java: record User(String name, int age) {}
来源：http://gbr.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://qsw.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hdh.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://zbj.hywenlv.cn

[G15] 枚举
来源：http://pml.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wtg.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ifx.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tev.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lys.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://vbc.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vez.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://wpj.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zkj.havefunace.top

[G16] 对象转数组 / 字典
来源：http://sex.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gbp.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://vgv.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://eiz.yonumen.top

TS:   Object.entries(obj)
来源：http://mvn.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ctg.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eww.fehbvm.com

Ruby: obj.instance_variables
来源：http://kmy.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://vfl.0kj1m.cn

================================================================================
来源：http://jcp.aizwys.cn

H. 异常与错误处理
来源：http://uax.zhijiandao.cn

================================================================================
来源：http://due.ydzc1.top

[H01] try / catch 基础
来源：http://bpy.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pds.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://txy.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://keh.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wsy.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oly.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mam.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jkw.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://seu.hcnkem.com

[H02] finally / ensure 收尾
来源：http://hfp.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oiz.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fal.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yix.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dul.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vra.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rjo.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rts.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tsu.yueranfly.top

[H03] 主动抛出异常
来源：http://ckn.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://vfj.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uat.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://hyj.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://vpd.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://rlf.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kwr.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vsh.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://zyy.nanxuanxn.top

[H04] 自定义异常类型
来源：http://heh.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://wkz.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://mcr.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://rai.tanke756.top

TS:   class MyError extends Error {}
来源：http://wpe.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://anj.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bhr.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://zts.uphjek.com

C#:   class MyException : Exception {}
来源：http://pxw.hfpthk.cn

[H05] 捕获特定类型
来源：http://hiu.mhx1999.top

Py:   except ValueError as e:
来源：http://bfg.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://apq.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://fqq.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://lzs.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://onf.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ayu.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://twd.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gob.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://ctw.jiagoushi.top

Py:   value = d.get("k") or default
来源：http://tas.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://jje.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://rpu.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://avl.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ehb.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xms.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://xrp.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://plx.svipenyu.cn

[H07] 断言
来源：http://yvk.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://ulp.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://daz.pycfn.com

JS:   console.assert(x > 0);
来源：http://tuf.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://kwe.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://azm.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vkb.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rbl.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://pfr.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://skm.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://buw.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lmw.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://phc.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dws.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://bnc.andypj.xyz

Go:   err.Error()
来源：http://daz.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://vuh.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://ntk.aizwys.cn

[H09] 带错误码的异常
来源：http://wnq.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lqv.dianchejie.cn


<!-- 参考信息 -->