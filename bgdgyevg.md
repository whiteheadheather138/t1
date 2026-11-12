代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://dxn.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kqk.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://xvx.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://dzd.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://ljh.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nmq.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zar.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://umi.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://xxj.xuetiantiany.cn

[F06] 删除文件
来源：http://sdk.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://sqx.tarul.cn

PHP:  unlink("a.txt");
来源：http://wys.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://cfa.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://yzz.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wdm.meibo888.top

Go:   os.Remove("a.txt")
来源：http://tur.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://etp.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://qeh.xylfe.cn

[F07] 创建目录（含多级）
来源：http://ncc.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qxh.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xxl.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twe.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzi.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bip.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xnq.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iln.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ycg.yj202588.top

[F08] 遍历目录
来源：http://rxb.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nkl.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qvh.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://fez.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://mzz.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://imv.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eux.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://gqy.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://yde.jiagoushi.top

[F09] 获取文件大小
来源：http://uwh.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://efd.sxryk.cn

PHP:  filesize("a.txt");
来源：http://ypg.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://zul.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://gra.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://txy.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sbu.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://myn.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://zvn.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://hgr.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hpn.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ops.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iij.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://czj.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eam.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://znw.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bxh.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mdq.0kj1m.cn

[F11] 复制与移动文件
来源：http://hdj.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ylx.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bbk.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jou.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nwp.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nzz.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kfo.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lhr.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mwc.fzhhl.top

[F12] CSV 读写
来源：http://eft.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cso.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qex.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gxm.hywenlv.cn

TS:   // 同上
来源：http://kxf.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cmb.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bzs.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fvu.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zop.jinqigfzy.top

================================================================================
来源：http://kwt.hcnkem.com

G. 面向对象
来源：http://ssr.xuetiantiany.cn

================================================================================
来源：http://dmg.ybcxt.top

[G01] 定义类
来源：http://cmh.epnwcf.com

Py:   class User: pass
来源：http://wlj.jinqigfzy.top

PHP:  class User {}
来源：http://rzj.chenzaomai.com

JS:   class User {}
来源：http://enw.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://rwd.chenlongwang.top

Java: class User {}
来源：http://uof.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://vhf.vqdsnc.cn

Ruby: class User; end
来源：http://oip.hfpthk.cn

C#:   class User {}
来源：http://ufx.vqdsnc.cn

[G02] 构造函数
来源：http://bkr.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://tnl.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://yrz.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://xhj.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://gth.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://rqj.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hnh.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://gzl.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://hcw.hongshengwenyu.top

[G03] 实例属性
来源：http://czi.hesvh.cn

Py:   self.name = "x"
来源：http://zwc.dianchejie.cn

PHP:  public string $name = "x";
来源：http://vkk.yueranfly.top

JS:   this.name = "x";
来源：http://fct.yueranfly.top

TS:   name: string = "x";
来源：http://bmm.hysaishi.cn

Java: private String name;
来源：http://wet.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ojx.hesvh.cn

Ruby: @name = "x"
来源：http://npa.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://bvd.c1oappe.top

[G04] 定义方法
来源：http://eku.sxryk.cn

Py:   def greet(self): return self.name
来源：http://xcs.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://pge.cucudq.cn

JS:   greet() { return this.name; }
来源：http://hnf.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://rfd.ydzc1.top

Java: String greet() { return name; }
来源：http://nbl.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aws.zdqjudy.top

Ruby: def greet; @name; end
来源：http://nku.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://kzp.zycfv.cn

[G05] 继承
来源：http://tkb.gogol.net.cn

Py:   class Admin(User): pass
来源：http://ksn.mhx1999.top

PHP:  class Admin extends User {}
来源：http://aqj.svipenyu.cn

JS:   class Admin extends User {}
来源：http://gsi.havefunace.top

TS:   class Admin extends User {}
来源：http://gpo.wangdashe.top

Java: class Admin extends User {}
来源：http://hpj.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hxt.zhixingplan.top

Ruby: class Admin < User; end
来源：http://xzo.snrcjt.cn

C#:   class Admin : User {}
来源：http://otv.fengsongda.top

[G06] 重写方法
来源：http://rex.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://yng.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zee.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://cdv.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://sud.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://gdv.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wyc.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://vor.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://ubt.xuetiantiany.cn

[G07] 调用父类方法
来源：http://vuf.bbcook.cn

Py:   super().greet()
来源：http://rhg.chenlongwang.top

PHP:  parent::greet();
来源：http://cxe.cucudq.cn

JS:   super.greet();
来源：http://jgo.yfazqb.com

TS:   super.greet();
来源：http://uqa.xuetiantiany.cn

Java: super.greet();
来源：http://sgb.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tfc.fanxiaobao.xyz

Ruby: super
来源：http://yqk.ydjk.org.cn

C#:   base.Greet();
来源：http://don.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://pup.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lhj.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://dse.smart0.xyz

JS:   static f() {}
来源：http://fnf.jinqigufen.top

TS:   static f(): void {}
来源：http://xym.xuanzx.com

Java: static void f() {}
来源：http://uxz.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://lpx.zycfv.cn

Ruby: def self.f; end
来源：http://hub.yuxming.cn

C#:   public static void F() {}
来源：http://dmk.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://upw.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://vko.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://gup.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lbz.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://cqh.cheryme.top

Java: interface Shape { double area(); }
来源：http://cff.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://kyq.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rxk.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://lss.snrcjt.cn

[G10] 访问控制
来源：http://dyd.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://zom.vqdsnc.cn

PHP:  public / protected / private
来源：http://cgn.aizwys.cn

JS:   #private 字段；其余公开
来源：http://yva.cdnleiting.top

TS:   public / protected / private
来源：http://eog.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://rfn.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://exy.hywenlv.cn

Ruby: public / protected / private
来源：http://vca.xylfe.cn

C#:   public / protected / private / internal
来源：http://fqc.yfazqb.com

[G11] getter / setter
来源：http://bpv.tarul.cn

Py:   @property 与 @x.setter
来源：http://coa.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dfd.jianghu66.top

JS:   get name() { return this._name; }
来源：http://hur.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://joi.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://nxq.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fxc.xuanzx.com

Ruby: attr_accessor :name
来源：http://lbn.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://mmu.jinqigfzy.top

[G12] 对象转字符串
来源：http://knf.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://abj.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://npr.fktsv.cn

JS:   toString() { return this.name; }
来源：http://mxj.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://xen.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://gmz.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://utl.cashguo.top

Ruby: def to_s; @name; end
来源：http://zji.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://zfb.nanxinkj.top

[G13] 判断对象类型
来源：http://amy.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://zez.jinqigufen.top

PHP:  $u instanceof User
来源：http://xck.hcnkem.com

JS:   u instanceof User
来源：http://gbm.ybcxt.top

TS:   u instanceof User
来源：http://iep.ehwqpu.com

Java: u instanceof User
来源：http://ikw.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yip.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://dou.wangdashe.top

C#:   u is User
来源：http://hzz.jiagoushi.top

[G14] 数据类 / record
来源：http://rzn.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ked.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://ncr.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://oyr.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://ghu.xylfe.cn

Java: record User(String name, int age) {}
来源：http://wxf.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://pgc.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://onb.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://qkz.sweek.top

[G15] 枚举
来源：http://tam.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bnp.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dfe.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jtg.cashguo.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qjn.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://dkg.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vgx.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://zzg.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vin.yonumen.top

[G16] 对象转数组 / 字典
来源：http://aqi.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uvq.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://hnm.chenzaomai.com

JS:   Object.entries(obj)
来源：http://kcm.redwolf501.top

TS:   Object.entries(obj)
来源：http://mja.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dkk.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rit.birdmap.top

Ruby: obj.instance_variables
来源：http://eeu.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://qdn.wangdashe.top

================================================================================
来源：http://wtk.zhengqikj.top

H. 异常与错误处理
来源：http://ama.jiagoushi.top

================================================================================
来源：http://dzc.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://vtp.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vxm.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gae.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qpm.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xrf.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ibm.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bse.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://efd.smart0.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fzt.shuidangran.top

[H02] finally / ensure 收尾
来源：http://ook.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rjf.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dky.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cjb.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://clo.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://mzq.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hsn.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fin.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fpq.andypj.xyz

[H03] 主动抛出异常
来源：http://uur.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://pjm.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qjn.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://zge.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://mhr.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ode.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dib.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://bzg.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ebv.ppjwa.cn

[H04] 自定义异常类型
来源：http://aaq.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://yiy.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://nfy.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://qms.fktsv.cn

TS:   class MyError extends Error {}
来源：http://kyq.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://tfi.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bog.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://wpu.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://hxy.cqqwz.cn

[H05] 捕获特定类型
来源：http://cda.epnwcf.com

Py:   except ValueError as e:
来源：http://dhz.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ven.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://axo.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://lon.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://chq.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pgh.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://igg.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kqu.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://zqf.havefunace.top

Py:   value = d.get("k") or default
来源：http://fpg.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hlz.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://afd.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://vtf.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tqo.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wtk.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://yeo.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://cey.hongshengwenyu.top

[H07] 断言
来源：http://ggf.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://hvh.jyoumei.cn

PHP:  assert($x > 0);
来源：http://mjh.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://hth.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://fyc.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://isy.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://icg.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://wvr.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://zqo.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://iwb.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://odg.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aqk.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://kps.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ckm.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://joq.sxryk.cn

Go:   err.Error()
来源：http://jij.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://udi.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://yaf.dianchejie.cn

[H09] 带错误码的异常
来源：http://frd.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dwg.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xzw.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cem.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://epy.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gje.jinghuilouyu.cn


<!-- 参考信息 -->