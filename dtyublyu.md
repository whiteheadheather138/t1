代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://irf.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gqy.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qsj.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://pax.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://apr.uphjek.com

[F06] 删除文件
来源：http://clr.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://udk.cashguo.top

PHP:  unlink("a.txt");
来源：http://dti.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://jfd.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ffz.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pme.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://fcb.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://cil.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://shx.fehbvm.com

[F07] 创建目录（含多级）
来源：http://xrt.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fqc.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mur.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yep.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qaj.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ory.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://okt.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gdu.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://szr.sxryk.cn

[F08] 遍历目录
来源：http://htv.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vrc.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dwl.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://cfe.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://kdm.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ksn.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pbd.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://prs.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://nyj.sweek.top

[F09] 获取文件大小
来源：http://tvg.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://awj.xinyue.icu

PHP:  filesize("a.txt");
来源：http://mkj.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://lmv.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://qlv.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://nsd.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bwo.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://hig.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://gdb.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://ecx.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fzg.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fzt.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jua.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://hfn.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://git.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lxn.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cev.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cin.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://cby.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qvs.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uus.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rlu.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aft.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tkt.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://euf.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hjs.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eoi.sysykeji.top

[F12] CSV 读写
来源：http://mkj.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hgp.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wvu.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tjv.tanke756.top

TS:   // 同上
来源：http://afi.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dle.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://quf.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gcu.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wtw.jinyuanbaomall.cn

================================================================================
来源：http://dhq.316326.xyz

G. 面向对象
来源：http://dat.ydjk.org.cn

================================================================================
来源：http://xyj.zdqjudy.top

[G01] 定义类
来源：http://hhw.havefunace.top

Py:   class User: pass
来源：http://hli.vqdsnc.cn

PHP:  class User {}
来源：http://lew.mhx1999.top

JS:   class User {}
来源：http://gcl.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://tiw.sweek.top

Java: class User {}
来源：http://pan.bjfxy.top

Go:   type User struct { Name string }
来源：http://omx.havefunace.top

Ruby: class User; end
来源：http://sdm.redwolf501.top

C#:   class User {}
来源：http://hph.hnqzz.top

[G02] 构造函数
来源：http://rzg.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://kax.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://rba.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://acf.yj20258.top

TS:   constructor(public name: string) {}
来源：http://alu.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://bmo.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qer.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://zyt.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://umu.cashguo.top

[G03] 实例属性
来源：http://drm.xziqi.cn

Py:   self.name = "x"
来源：http://pbi.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://ghy.bbcook.cn

JS:   this.name = "x";
来源：http://ifi.zhixingplan.top

TS:   name: string = "x";
来源：http://vub.jinqigufen.top

Java: private String name;
来源：http://law.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zhq.redwolf501.top

Ruby: @name = "x"
来源：http://mgt.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://rko.ctjpmb.com

[G04] 定义方法
来源：http://obp.hammf.cn

Py:   def greet(self): return self.name
来源：http://cbg.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dcr.smart0.xyz

JS:   greet() { return this.name; }
来源：http://hkq.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://tnz.snrcjt.cn

Java: String greet() { return name; }
来源：http://nyw.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wyn.nwbrower.top

Ruby: def greet; @name; end
来源：http://omv.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://vsm.zhaomingkeji.xyz

[G05] 继承
来源：http://rqc.yj20258888.top

Py:   class Admin(User): pass
来源：http://tkk.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://lat.hammf.cn

JS:   class Admin extends User {}
来源：http://efp.bbcook.cn

TS:   class Admin extends User {}
来源：http://fvs.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://its.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://krm.iojbl.cn

Ruby: class Admin < User; end
来源：http://dsm.meibo888.top

C#:   class Admin : User {}
来源：http://plz.jqgufenzy.top

[G06] 重写方法
来源：http://pws.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://lgt.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bbr.yj20258.top

JS:   greet() { return "admin"; }
来源：http://qwo.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://igj.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://ojc.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kmr.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://iim.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://oup.daxiang520.top

[G07] 调用父类方法
来源：http://gtw.zhijiandao.cn

Py:   super().greet()
来源：http://npf.ppjwa.cn

PHP:  parent::greet();
来源：http://qeh.sjlbkw.cn

JS:   super.greet();
来源：http://xul.ybcxt.top

TS:   super.greet();
来源：http://jjq.tarul.cn

Java: super.greet();
来源：http://vzq.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yew.vehdjk.com

Ruby: super
来源：http://ygb.birdmap.top

C#:   base.Greet();
来源：http://xda.aizwys.cn

[G08] 静态方法与属性
来源：http://qil.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pyc.yj20258.top

PHP:  public static function f() {}
来源：http://hvw.sysykeji.top

JS:   static f() {}
来源：http://myk.tanke756.top

TS:   static f(): void {}
来源：http://rey.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://pxk.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ilh.redwolf501.top

Ruby: def self.f; end
来源：http://eca.jqgfzy.top

C#:   public static void F() {}
来源：http://tsp.tarul.cn

[G09] 接口 / 抽象类
来源：http://bxh.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://zch.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lfu.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pqi.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://ald.mhx1999.top

Java: interface Shape { double area(); }
来源：http://znw.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://kiu.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mvw.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://geh.gzhubu.top

[G10] 访问控制
来源：http://zjj.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://zfo.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://inq.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://rap.hnxiangtu.top

TS:   public / protected / private
来源：http://bsm.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://ano.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://prx.xuanzx.com

Ruby: public / protected / private
来源：http://sdx.yongpay.top

C#:   public / protected / private / internal
来源：http://gej.xylfe.cn

[G11] getter / setter
来源：http://mea.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://mok.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hfh.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://aqi.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://gwj.yj20258.top

Java: public String getName() { return name; }
来源：http://dzm.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://oiy.cheryme.top

Ruby: attr_accessor :name
来源：http://val.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://hks.nanxinkj.top

[G12] 对象转字符串
来源：http://gba.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://rks.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://doo.vehdjk.com

JS:   toString() { return this.name; }
来源：http://zki.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://tfp.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://kiu.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ndm.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://tzm.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://fgw.jinqigfzy.top

[G13] 判断对象类型
来源：http://qff.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://aaw.jlsjyb.cn

PHP:  $u instanceof User
来源：http://jfy.sxryk.cn

JS:   u instanceof User
来源：http://pgp.hfpthk.cn

TS:   u instanceof User
来源：http://okk.yangfankeji.com

Java: u instanceof User
来源：http://yfl.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gkj.xylfe.cn

Ruby: u.is_a?(User)
来源：http://knw.cdnleiting.top

C#:   u is User
来源：http://jet.nanxinkj.top

[G14] 数据类 / record
来源：http://wqv.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kcz.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://ljv.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lxk.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://aup.fengsongda.top

Java: record User(String name, int age) {}
来源：http://ell.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://jdx.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vxg.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://jhr.fanxiaobao.xyz

[G15] 枚举
来源：http://zip.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ecg.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://qts.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nzi.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mzv.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://kuv.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rqf.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://ohx.aibaodan.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://juu.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://kxo.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mew.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://xqo.bbcook.cn

JS:   Object.entries(obj)
来源：http://hql.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://emf.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xxh.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gmd.chenlongwang.top

Ruby: obj.instance_variables
来源：http://zdl.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://ram.yongpay.top

================================================================================
来源：http://rgr.nanxuanxn.top

H. 异常与错误处理
来源：http://dlk.nanxuanxn.top

================================================================================
来源：http://svn.c1oappe.top

[H01] try / catch 基础
来源：http://rdo.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cqh.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vna.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qbl.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hxu.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fnv.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://txn.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mxf.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lpj.yvedp.cn

[H02] finally / ensure 收尾
来源：http://plr.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://hob.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qed.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rcl.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xxm.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://vak.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qns.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://dkl.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://flf.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://vhz.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://lsw.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qzt.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://wsv.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://ioh.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://vbn.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mve.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://izq.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://cwz.yuanzhike.top

[H04] 自定义异常类型
来源：http://ugk.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://sxe.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lqf.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://yqn.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://lrn.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://whs.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cjm.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://ian.guannengcc.top

C#:   class MyException : Exception {}
来源：http://gwr.gogol.net.cn

[H05] 捕获特定类型
来源：http://snf.svipenyu.cn

Py:   except ValueError as e:
来源：http://vlo.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eml.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://nyf.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://juk.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://bhm.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wrr.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://ocz.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mpy.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://vjd.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://cqg.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://wpc.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://ewc.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kfn.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uzy.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vxm.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://swu.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://zgp.316326.xyz

[H07] 断言
来源：http://lgv.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://wgo.gogol.net.cn

PHP:  assert($x > 0);
来源：http://thb.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://xlm.bbcook.cn

TS:   console.assert(x > 0);
来源：http://xuy.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://scw.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vcz.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zqi.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://kdy.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://tsd.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://igd.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jsw.chenzaomai.com

JS:   e.message;  e.stack
来源：http://acc.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://lta.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ctu.gzhubu.top

Go:   err.Error()
来源：http://azl.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://jir.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://gww.hfpthk.cn

[H09] 带错误码的异常
来源：http://rip.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kle.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://idk.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kzp.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gvk.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://twn.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zkl.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://qyz.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jug.9152youxi.cn

[H10] 资源自动释放
来源：http://uxd.guannengcc.top


<!-- 参考信息 -->