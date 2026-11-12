代发 wailian999

C#:   File.Exists("a.txt")
来源：http://bmc.ctjpmb.com

[F06] 删除文件
来源：http://gny.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://vjt.iojbl.cn

PHP:  unlink("a.txt");
来源：http://abs.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://edt.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://xzo.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kan.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://tpw.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://enb.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://krz.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://xas.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wmn.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mom.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zre.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxv.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iun.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://taz.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fro.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ylc.shzxlz.cn

[F08] 遍历目录
来源：http://ijk.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uln.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bbw.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://hpa.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://qdf.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yho.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zcx.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://xdg.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://qhd.hfpthk.cn

[F09] 获取文件大小
来源：http://dgk.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://emu.andypj.xyz

PHP:  filesize("a.txt");
来源：http://avw.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://pur.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://etc.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://tzi.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zcp.tian-w.cn

Ruby: File.size("a.txt")
来源：http://jow.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://rnh.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://ole.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ayt.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://giv.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dsm.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://ewr.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hay.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dae.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wmw.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jtm.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://url.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qfn.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uqy.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zpe.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kgi.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://meh.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xjl.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fev.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gza.yj202588.top

[F12] CSV 读写
来源：http://cel.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bdl.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wbo.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bxt.wangdashe.top

TS:   // 同上
来源：http://vdw.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ilb.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wbs.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lvs.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qib.sufxvd.cn

================================================================================
来源：http://dfj.yanxiufei.cn

G. 面向对象
来源：http://tpm.jyoumei.cn

================================================================================
来源：http://ufe.ppjwa.cn

[G01] 定义类
来源：http://uve.ywan-chungtsiang.top

Py:   class User: pass
来源：http://fvz.kuanghao11.cn

PHP:  class User {}
来源：http://ali.yj20258.top

JS:   class User {}
来源：http://cyw.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://bxh.zhongyouzk.top

Java: class User {}
来源：http://duq.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://ept.gotoacloud.top

Ruby: class User; end
来源：http://xlr.andypj.xyz

C#:   class User {}
来源：http://rgd.cheryme.top

[G02] 构造函数
来源：http://jav.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://byu.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://jrz.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://hft.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://vsh.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://upk.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xuu.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://rde.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://olc.yuanzhike.top

[G03] 实例属性
来源：http://tem.jqgfzy.top

Py:   self.name = "x"
来源：http://qyi.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://cay.jlsjyb.cn

JS:   this.name = "x";
来源：http://ufz.iojbl.cn

TS:   name: string = "x";
来源：http://azk.yvedp.cn

Java: private String name;
来源：http://ehk.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pfa.chenlongwang.top

Ruby: @name = "x"
来源：http://zwr.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://nap.cdnleiting.top

[G04] 定义方法
来源：http://qql.daria6918.cn

Py:   def greet(self): return self.name
来源：http://xzc.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cuy.yonumen.top

JS:   greet() { return this.name; }
来源：http://lss.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://ajp.yfazqb.com

Java: String greet() { return name; }
来源：http://jat.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jiz.chenlongwang.top

Ruby: def greet; @name; end
来源：http://psh.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://lss.zhengqikj.top

[G05] 继承
来源：http://zpj.redwolf501.top

Py:   class Admin(User): pass
来源：http://bmt.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://jby.sxryk.cn

JS:   class Admin extends User {}
来源：http://yvi.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://vej.cashguo.top

Java: class Admin extends User {}
来源：http://tug.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://llq.hywenlv.cn

Ruby: class Admin < User; end
来源：http://hii.yongpay.top

C#:   class Admin : User {}
来源：http://ehj.xinyue.icu

[G06] 重写方法
来源：http://llc.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://zhf.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gnj.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://til.wangdashe.top

TS:   greet(): string { return "admin"; }
来源：http://rlp.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://nfd.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ufq.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://tfx.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://hjb.pengpengdd.cyou

[G07] 调用父类方法
来源：http://pqy.ybcxt.top

Py:   super().greet()
来源：http://hzg.jinqigufen.top

PHP:  parent::greet();
来源：http://ajp.vqdsnc.cn

JS:   super.greet();
来源：http://nmq.wangdashe.top

TS:   super.greet();
来源：http://app.xylfe.cn

Java: super.greet();
来源：http://ocv.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uto.wangdashe.top

Ruby: super
来源：http://ryb.sxryk.cn

C#:   base.Greet();
来源：http://tzi.zdqjudy.top

[G08] 静态方法与属性
来源：http://aoi.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lih.gzhubu.top

PHP:  public static function f() {}
来源：http://xww.redwolf501.top

JS:   static f() {}
来源：http://txe.ybcxt.top

TS:   static f(): void {}
来源：http://bsz.jlsjyb.cn

Java: static void f() {}
来源：http://rcl.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://idp.zhixingplan.top

Ruby: def self.f; end
来源：http://cqx.yfazqb.com

C#:   public static void F() {}
来源：http://tsd.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://dcg.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://jij.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wnu.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ckb.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://xrh.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://owf.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://jbc.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ynb.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://vgs.shanyushiyangtech.top

[G10] 访问控制
来源：http://gbu.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://fwe.c1oappe.top

PHP:  public / protected / private
来源：http://gpp.yj20258888.top

JS:   #private 字段；其余公开
来源：http://yta.yuanzhike.top

TS:   public / protected / private
来源：http://xfa.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://yjo.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eps.dianchejie.cn

Ruby: public / protected / private
来源：http://rew.tanke756.top

C#:   public / protected / private / internal
来源：http://vhe.zdqjudy.top

[G11] getter / setter
来源：http://txi.ydzc1.top

Py:   @property 与 @x.setter
来源：http://wap.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://htn.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://eqn.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://sgw.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://vkz.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ykm.xuanzx.com

Ruby: attr_accessor :name
来源：http://xpq.epnwcf.com

C#:   public string Name { get; set; }
来源：http://cbu.gogol.net.cn

[G12] 对象转字符串
来源：http://auz.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://puq.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jdz.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://hfy.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://jgh.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://lbo.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://cbe.xuanzx.com

Ruby: def to_s; @name; end
来源：http://hse.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://khd.sxryk.cn

[G13] 判断对象类型
来源：http://peb.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://myq.fehbvm.com

PHP:  $u instanceof User
来源：http://imq.xuetiantiany.cn

JS:   u instanceof User
来源：http://hjw.jqgfzy.top

TS:   u instanceof User
来源：http://ozh.sjlbkw.cn

Java: u instanceof User
来源：http://jmx.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lgx.tanke756.top

Ruby: u.is_a?(User)
来源：http://jyt.jlsjyb.cn

C#:   u is User
来源：http://wvw.havefunace.top

[G14] 数据类 / record
来源：http://hbs.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lnq.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ktw.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://xrg.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://qal.sweek.top

Java: record User(String name, int age) {}
来源：http://cju.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://ksb.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tan.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://pnd.hesvh.cn

[G15] 枚举
来源：http://vjv.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mvs.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yii.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uxf.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ljr.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://pjz.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rgr.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://oxj.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://buk.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://eoz.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://psa.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://trt.hywenlv.cn

JS:   Object.entries(obj)
来源：http://kwy.ctjpmb.com

TS:   Object.entries(obj)
来源：http://ejr.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cyc.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mgh.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://rsy.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dnf.ppjwa.cn

================================================================================
来源：http://kys.hysaishi.cn

H. 异常与错误处理
来源：http://std.aibaodan.cn

================================================================================
来源：http://gwi.zhengqikj.top

[H01] try / catch 基础
来源：http://yrg.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mpo.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ylo.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dtc.chenlongwang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gry.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yir.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pbi.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://knr.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dad.guannengcc.top

[H02] finally / ensure 收尾
来源：http://kbb.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pzc.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zut.chenjidiqi.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://ird.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wxy.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lyi.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ttc.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://eis.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ibv.cashguo.top

[H03] 主动抛出异常
来源：http://cbr.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://wcc.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ybe.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://jkv.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://ohx.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tng.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mku.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rcg.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://mqg.tarul.cn

[H04] 自定义异常类型
来源：http://pyd.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://puc.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://ynb.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://gxt.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://ffz.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://rou.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qte.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://qjf.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://szk.jinqigufen.top

[H05] 捕获特定类型
来源：http://crc.jyoumei.cn

Py:   except ValueError as e:
来源：http://mbb.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iql.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://mdj.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://lov.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://kpo.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://obn.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://nxo.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lvl.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://zcn.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://lrf.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://yut.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://zqb.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://fob.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zwb.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ihl.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://ywr.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://esq.zycfv.cn

[H07] 断言
来源：http://pqb.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://asd.cheryme.top

PHP:  assert($x > 0);
来源：http://ayg.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://pzj.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://wkr.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://ukq.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gon.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://ece.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://qam.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://xgb.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://quz.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wkl.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://upw.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rjd.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://unf.wangdashe.top

Go:   err.Error()
来源：http://vut.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://eha.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://vno.meibo888.top

[H09] 带错误码的异常
来源：http://jvu.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cah.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nbi.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qfe.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fil.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lkw.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qnp.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nre.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://phi.vehdjk.com

[H10] 资源自动释放
来源：http://snp.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://yvb.wangdashe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qqm.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jvp.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fxu.fengsongda.top


<!-- 参考信息 -->