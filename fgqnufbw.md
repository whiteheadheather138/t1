代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tbn.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uwn.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jjo.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwu.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sro.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vmy.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://byk.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tzz.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://jxx.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://csg.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://eur.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://nui.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://erq.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yue.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qbj.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://ovu.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://bpd.zhixingplan.top

[F06] 删除文件
来源：http://jpi.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://ljj.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://czl.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://hwh.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://jqf.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bjg.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://gfq.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://yxp.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://sph.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://owh.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xmw.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nwa.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aoc.xuetiantiany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gso.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://swj.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://txl.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://znt.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vmf.hcnkem.com

[F08] 遍历目录
来源：http://lhb.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://chb.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://txa.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://kgz.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://uiq.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ibh.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fgw.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://ift.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://dwl.xylfe.cn

[F09] 获取文件大小
来源：http://ici.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://odw.fktsv.cn

PHP:  filesize("a.txt");
来源：http://fmu.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://hpc.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://pze.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://tlg.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yno.shuidangran.top

Ruby: File.size("a.txt")
来源：http://rqd.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://ool.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://xbk.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jrm.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qvg.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://voo.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://mfp.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sry.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nqi.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://spq.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zrz.gaohongyu789.top

[F11] 复制与移动文件
来源：http://bgm.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zue.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://acm.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vsb.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qqy.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wop.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kjg.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tpa.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jwv.sufxvd.cn

[F12] CSV 读写
来源：http://mwt.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aax.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ckv.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qes.daria6918.cn

TS:   // 同上
来源：http://cqr.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dzc.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gjf.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oei.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ngd.birdmap.top

================================================================================
来源：http://yji.xinyue.icu

G. 面向对象
来源：http://mai.ydzc1.top

================================================================================
来源：http://qkv.cdnleiting.top

[G01] 定义类
来源：http://lgk.sjlbkw.cn

Py:   class User: pass
来源：http://yog.ybcxt.top

PHP:  class User {}
来源：http://qqr.tian-w.cn

JS:   class User {}
来源：http://ssm.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://xqy.wangdashe.top

Java: class User {}
来源：http://iqc.0kj1m.cn

Go:   type User struct { Name string }
来源：http://pvf.gotoacloud.top

Ruby: class User; end
来源：http://ucw.sysykeji.top

C#:   class User {}
来源：http://atu.mhx1999.top

[G02] 构造函数
来源：http://jfm.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://nfe.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://dgh.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://pki.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://hma.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://eqv.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xtv.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://cjq.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://smc.chenzaomai.com

[G03] 实例属性
来源：http://rbj.hysaishi.cn

Py:   self.name = "x"
来源：http://zkx.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://mdg.ivvv.top

JS:   this.name = "x";
来源：http://zzu.yfazqb.com

TS:   name: string = "x";
来源：http://nre.jqgfzy.top

Java: private String name;
来源：http://iri.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rkl.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://khw.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://yys.sysykeji.top

[G04] 定义方法
来源：http://vnd.cheryme.top

Py:   def greet(self): return self.name
来源：http://etl.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pyi.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://qrg.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://ziv.bjfxy.top

Java: String greet() { return name; }
来源：http://oej.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://czw.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://ngf.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://sii.yvedp.cn

[G05] 继承
来源：http://ldk.hysaishi.cn

Py:   class Admin(User): pass
来源：http://frv.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://abh.ybcxt.top

JS:   class Admin extends User {}
来源：http://xcs.chenlongwang.top

TS:   class Admin extends User {}
来源：http://ozj.cheryme.top

Java: class Admin extends User {}
来源：http://tra.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kor.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://kyn.ctjpmb.com

C#:   class Admin : User {}
来源：http://xcs.yangfankeji.com

[G06] 重写方法
来源：http://duq.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://ydd.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zjs.cashguo.top

JS:   greet() { return "admin"; }
来源：http://ihs.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://fit.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://dzw.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kru.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://ttb.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://syg.uphjek.com

[G07] 调用父类方法
来源：http://ofv.fengsongda.top

Py:   super().greet()
来源：http://eho.redwolf501.top

PHP:  parent::greet();
来源：http://rqz.xziqi.cn

JS:   super.greet();
来源：http://zce.vehdjk.com

TS:   super.greet();
来源：http://fer.aibaodan.cn

Java: super.greet();
来源：http://dkx.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vsk.yj20258.top

Ruby: super
来源：http://enz.feifeiyinyue.top

C#:   base.Greet();
来源：http://xpl.aizwys.cn

[G08] 静态方法与属性
来源：http://yly.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nqm.fengsongda.top

PHP:  public static function f() {}
来源：http://sfk.xuetiantiany.cn

JS:   static f() {}
来源：http://zde.bbcook.cn

TS:   static f(): void {}
来源：http://qqu.ywan-chungtsiang.top

Java: static void f() {}
来源：http://puv.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://igb.ybcxt.top

Ruby: def self.f; end
来源：http://ogb.cqqwz.cn

C#:   public static void F() {}
来源：http://kjk.bbcook.cn

[G09] 接口 / 抽象类
来源：http://jea.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://hhr.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://hqw.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jlt.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://lco.shuidangran.top

Java: interface Shape { double area(); }
来源：http://qnw.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://kqu.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://srz.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://ewz.cheryme.top

[G10] 访问控制
来源：http://ryr.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://mru.gaohongyu789.top

PHP:  public / protected / private
来源：http://xzb.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://rny.hfpthk.cn

TS:   public / protected / private
来源：http://uxr.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://wiu.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vat.havefunace.top

Ruby: public / protected / private
来源：http://pdz.daria6918.cn

C#:   public / protected / private / internal
来源：http://ofl.andypj.xyz

[G11] getter / setter
来源：http://arb.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://kyk.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nvr.cashguo.top

JS:   get name() { return this._name; }
来源：http://ngv.mhx1999.top

TS:   get name(): string { return this._name; }
来源：http://kfu.wangdashe.top

Java: public String getName() { return name; }
来源：http://wkz.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gmc.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://xni.bjfxy.top

C#:   public string Name { get; set; }
来源：http://dvw.cashguo.top

[G12] 对象转字符串
来源：http://vva.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://kbj.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xbr.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://srv.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://nca.yanxiufei.cn

Java: @Override public String toString() { return name; }
来源：http://jup.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://qyx.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://qse.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://yje.hysaishi.cn

[G13] 判断对象类型
来源：http://kwy.fktsv.cn

Py:   isinstance(u, User)
来源：http://hqf.jqgufenzy.top

PHP:  $u instanceof User
来源：http://bzp.meibo888.top

JS:   u instanceof User
来源：http://tyq.gzhubu.top

TS:   u instanceof User
来源：http://wem.vqdsnc.cn

Java: u instanceof User
来源：http://ffm.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wzj.uphjek.com

Ruby: u.is_a?(User)
来源：http://aqd.yongpay.top

C#:   u is User
来源：http://mve.sufxvd.cn

[G14] 数据类 / record
来源：http://oqq.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fvm.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://lkw.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pnu.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://zfj.52xcode.cn

Java: record User(String name, int age) {}
来源：http://rsu.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://ely.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jqq.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://uzt.hesvh.cn

[G15] 枚举
来源：http://nly.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ldl.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pia.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dfj.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pdp.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://yvf.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tik.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://zkb.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://owl.tanke756.top

[G16] 对象转数组 / 字典
来源：http://fcu.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tfi.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://geq.yonumen.top

JS:   Object.entries(obj)
来源：http://alz.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://fpf.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ked.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ykb.hfpthk.cn

Ruby: obj.instance_variables
来源：http://mir.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://qxx.yongpay.top

================================================================================
来源：http://dpf.jyoumei.cn

H. 异常与错误处理
来源：http://gnd.yongpay.top

================================================================================
来源：http://swc.jlsjyb.cn

[H01] try / catch 基础
来源：http://iqu.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qyx.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fyj.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nzu.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wbv.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nrg.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wsk.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tin.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vjk.xylfe.cn

[H02] finally / ensure 收尾
来源：http://pod.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://giz.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nea.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mxe.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lfn.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://ojj.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gko.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lsj.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vnv.hnxiangtu.top

[H03] 主动抛出异常
来源：http://unh.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://jww.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nrn.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://byw.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://lwb.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fzb.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vdf.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sip.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uix.cqqwz.cn

[H04] 自定义异常类型
来源：http://hex.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://xar.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://yks.bjfxy.top

JS:   class MyError extends Error {}
来源：http://brj.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://lzl.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://ptr.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://goa.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://afv.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://sht.yuanzhike.top

[H05] 捕获特定类型
来源：http://wrm.daria6918.cn

Py:   except ValueError as e:
来源：http://snx.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pkj.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://fmj.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://ndm.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://osg.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xuf.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://rzn.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mct.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://mdq.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://sdw.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://iqx.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://dlu.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://mwo.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kgn.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://epp.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://gri.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://ovg.xinyue.icu

[H07] 断言
来源：http://awi.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://uah.yvedp.cn

PHP:  assert($x > 0);
来源：http://jkk.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://mbh.andypj.xyz

TS:   console.assert(x > 0);
来源：http://veo.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://pfg.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oby.shanyushiyangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://jmt.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://fbv.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://wiz.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://tog.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yst.hammf.cn

JS:   e.message;  e.stack
来源：http://txl.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dru.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kuw.guannengcc.top

Go:   err.Error()
来源：http://yjl.yuanzhike.top


<!-- 参考信息 -->