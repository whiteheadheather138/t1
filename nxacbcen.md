代发 wailian999

C#:   File.Exists("a.txt")
来源：http://jtv.svipenyu.cn

[F06] 删除文件
来源：http://oah.ivvv.top

Py:   os.remove("a.txt")
来源：http://nqu.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://uhi.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://one.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://fqk.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ths.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://vin.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://jzd.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://fim.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://rpu.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://slf.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://chc.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cyk.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ref.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://taz.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bzs.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jfi.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dgp.daxiang520.top

[F08] 遍历目录
来源：http://nkx.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vrh.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ehs.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://jok.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://vsy.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zgu.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wrl.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://dbj.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://dok.zhongyouzk.top

[F09] 获取文件大小
来源：http://hsy.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://bmx.tanke756.top

PHP:  filesize("a.txt");
来源：http://nbl.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://srf.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://qkf.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://dit.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oft.xuanzx.com

Ruby: File.size("a.txt")
来源：http://voq.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://ota.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://jwl.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ndn.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://use.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pcy.ydzc1.top

TS:   path.extname("a.txt")
来源：http://ega.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://osa.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bnl.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gxs.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vyf.yuanzhike.top

[F11] 复制与移动文件
来源：http://txh.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jcv.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sni.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hsz.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yry.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zny.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://daw.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kmb.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cpe.ybcxt.top

[F12] CSV 读写
来源：http://edo.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kxv.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ewx.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lil.chenzaomai.com

TS:   // 同上
来源：http://ayy.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hld.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ass.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wcv.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mda.0kj1m.cn

================================================================================
来源：http://uyj.yonumen.top

G. 面向对象
来源：http://ndj.jqgfzy.top

================================================================================
来源：http://fef.52xcode.cn

[G01] 定义类
来源：http://ozs.cdnleiting.top

Py:   class User: pass
来源：http://zif.chenzaomai.com

PHP:  class User {}
来源：http://juv.jinyuanbaomall.cn

JS:   class User {}
来源：http://rvf.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://aiv.daxiang520.top

Java: class User {}
来源：http://fwg.hywenlv.cn

Go:   type User struct { Name string }
来源：http://drk.sxryk.cn

Ruby: class User; end
来源：http://aex.wangshuangyany.cn

C#:   class User {}
来源：http://urb.tanke756.top

[G02] 构造函数
来源：http://tab.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://uwi.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://fwb.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://zzs.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://srd.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://jwk.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aeo.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://pfx.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://mna.nanxinkj.top

[G03] 实例属性
来源：http://sju.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://hvy.yangfankeji.com

PHP:  public string $name = "x";
来源：http://uia.hywenlv.cn

JS:   this.name = "x";
来源：http://lis.guowangkeji.top

TS:   name: string = "x";
来源：http://kvn.tian-w.cn

Java: private String name;
来源：http://dqb.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gkr.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://qcl.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://jjd.chenzaomai.com

[G04] 定义方法
来源：http://sjt.wangdashe.top

Py:   def greet(self): return self.name
来源：http://nio.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tnd.sxryk.cn

JS:   greet() { return this.name; }
来源：http://llc.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://lmx.52xcode.cn

Java: String greet() { return name; }
来源：http://uzs.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qqr.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://kga.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://nyz.pycfn.com

[G05] 继承
来源：http://bve.tian-w.cn

Py:   class Admin(User): pass
来源：http://yhr.cheryme.top

PHP:  class Admin extends User {}
来源：http://wnk.cqqwz.cn

JS:   class Admin extends User {}
来源：http://yqo.pycfn.com

TS:   class Admin extends User {}
来源：http://ugr.birdmap.top

Java: class Admin extends User {}
来源：http://rhh.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://izx.mhx1999.top

Ruby: class Admin < User; end
来源：http://kfl.quarkkingdee.top

C#:   class Admin : User {}
来源：http://omy.chenlongwang.top

[G06] 重写方法
来源：http://ijr.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://wbb.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cbg.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://qvo.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://ryc.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://syk.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qwo.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://pqk.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://oie.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://hbn.tian-w.cn

Py:   super().greet()
来源：http://yrd.shzxlz.cn

PHP:  parent::greet();
来源：http://skr.jianghu66.top

JS:   super.greet();
来源：http://unq.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://tdz.xingfuxueyuan.xyz

Java: super.greet();
来源：http://eny.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uos.daria6918.cn

Ruby: super
来源：http://ijh.zhijiandao.cn

C#:   base.Greet();
来源：http://tsw.sysykeji.top

[G08] 静态方法与属性
来源：http://cdn.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mcp.snrcjt.cn

PHP:  public static function f() {}
来源：http://two.yongpay.top

JS:   static f() {}
来源：http://epb.chenjidiqi.icu

TS:   static f(): void {}
来源：http://lid.iojbl.cn

Java: static void f() {}
来源：http://llv.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://avb.sysykeji.top

Ruby: def self.f; end
来源：http://vdz.zhoulong.xyz

C#:   public static void F() {}
来源：http://ftm.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://vvr.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ufn.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://lkp.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bxw.0kj1m.cn

TS:   interface Shape { area(): number; }
来源：http://ozr.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://amh.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://tjs.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wqc.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://iyz.gotoacloud.top

[G10] 访问控制
来源：http://pyf.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://tuv.hammf.cn

PHP:  public / protected / private
来源：http://bfv.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://scu.cucudq.cn

TS:   public / protected / private
来源：http://poc.yonumen.top

Java: public / protected / private / 默认包级
来源：http://mrk.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jlk.guannengcc.top

Ruby: public / protected / private
来源：http://jui.hesvh.cn

C#:   public / protected / private / internal
来源：http://zom.nanxuanxn.top

[G11] getter / setter
来源：http://kyp.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://rem.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ngn.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://axg.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://uxt.gotoacloud.top

Java: public String getName() { return name; }
来源：http://gff.wangdashe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jsl.tianlin.xyz

Ruby: attr_accessor :name
来源：http://ali.yueranfly.top

C#:   public string Name { get; set; }
来源：http://rnk.cucudq.cn

[G12] 对象转字符串
来源：http://sdf.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://eed.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qce.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://lvy.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://jkn.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://nsz.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nij.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://pqd.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://egn.haohaochexian.top

[G13] 判断对象类型
来源：http://mxt.316326.xyz

Py:   isinstance(u, User)
来源：http://tuc.hywenlv.cn

PHP:  $u instanceof User
来源：http://ixd.guowangkeji.top

JS:   u instanceof User
来源：http://vtt.yfazqb.com

TS:   u instanceof User
来源：http://ovg.cheryme.top

Java: u instanceof User
来源：http://osu.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jdb.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://fqq.chenjidiqi.icu

C#:   u is User
来源：http://zbt.cdnleiting.top

[G14] 数据类 / record
来源：http://xkg.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://egn.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://ocm.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://beg.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://xwk.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://rtl.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://sgh.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bag.cashguo.top

C#:   record User(string Name, int Age);
来源：http://age.daria6918.cn

[G15] 枚举
来源：http://rab.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uli.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bmv.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ycl.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eyp.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://ukx.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uqp.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://nwp.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://clr.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://dma.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://srh.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://hcb.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://cxg.ydzc1.top

TS:   Object.entries(obj)
来源：http://wqh.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gcf.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ges.yj20258.top

Ruby: obj.instance_variables
来源：http://bmf.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://nlm.bjfxy.top

================================================================================
来源：http://brm.wangshuangyany.cn

H. 异常与错误处理
来源：http://zwx.daxiang520.top

================================================================================
来源：http://vjg.gaohongyu789.top

[H01] try / catch 基础
来源：http://lpz.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rhz.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tyb.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://guy.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zhr.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://evh.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xuy.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tzi.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nbr.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://vdd.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oii.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lcw.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hrz.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eha.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://min.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://dtx.jqgfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zeo.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hgz.bbcook.cn

[H03] 主动抛出异常
来源：http://who.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://uez.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mmt.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://tio.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://umo.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gwn.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ryd.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lkf.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://oiu.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://axi.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://upp.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mlm.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://nht.yfazqb.com

TS:   class MyError extends Error {}
来源：http://igc.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://cba.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kki.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://blv.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://cnx.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://jqx.fengsongda.top

Py:   except ValueError as e:
来源：http://hkd.xuanzx.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kqa.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://lja.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://rsl.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://erw.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ukf.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://ylz.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rll.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://pns.redwolf501.top

Py:   value = d.get("k") or default
来源：http://aeb.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://nry.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://vmu.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://vre.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mqq.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lxj.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://mdt.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://jaj.guowangkeji.top

[H07] 断言
来源：http://xah.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://cnj.birdmap.top

PHP:  assert($x > 0);
来源：http://rxl.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://pdu.shuidangran.top

TS:   console.assert(x > 0);
来源：http://amv.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://ive.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oqy.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://kji.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://res.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://xof.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://fzp.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eki.vehdjk.com

JS:   e.message;  e.stack
来源：http://slg.daria6918.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pyn.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ube.yj202588.top

Go:   err.Error()
来源：http://ynf.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://tnq.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://cot.ybcxt.top

[H09] 带错误码的异常
来源：http://wgf.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ixe.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pqp.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yem.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hjm.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tuq.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tob.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://uuj.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://qbq.cqqwz.cn

[H10] 资源自动释放
来源：http://pow.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mzf.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tjp.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hbt.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lcm.ydjk.org.cn


<!-- 参考信息 -->