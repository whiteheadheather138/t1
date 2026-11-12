代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://sgf.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kiv.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://spu.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://nej.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://pag.gotoacloud.top

[F06] 删除文件
来源：http://vji.shuidangran.top

Py:   os.remove("a.txt")
来源：http://igv.yj20258.top

PHP:  unlink("a.txt");
来源：http://kwo.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://rjj.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xmu.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://irs.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://jjw.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://eqk.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://ryb.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://fnr.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fbp.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nwo.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqd.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqp.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lry.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hxf.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wgy.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vjy.yj20258.top

[F08] 遍历目录
来源：http://abb.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://csp.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bmq.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://agc.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://jyh.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mhd.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://thq.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://svm.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://vcs.vqdsnc.cn

[F09] 获取文件大小
来源：http://zzs.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://wta.tian-w.cn

PHP:  filesize("a.txt");
来源：http://rdx.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://mqf.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://vmz.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://olh.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xyt.cashguo.top

Ruby: File.size("a.txt")
来源：http://uvc.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://blu.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://hhz.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://srt.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rla.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nrm.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://znc.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yxj.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uqz.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bll.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kmn.c1oappe.top

[F11] 复制与移动文件
来源：http://huv.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://itw.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kix.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hxs.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qim.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wzs.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rgx.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yld.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rcw.yj20258.top

[F12] CSV 读写
来源：http://jia.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sts.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://btg.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://znj.hcnkem.com

TS:   // 同上
来源：http://yfw.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bby.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zjn.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zqp.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gap.tarul.cn

================================================================================
来源：http://dwx.ivvv.top

G. 面向对象
来源：http://lly.jinqigufen.top

================================================================================
来源：http://dmm.9152youxi.cn

[G01] 定义类
来源：http://biu.quarkkingdee.top

Py:   class User: pass
来源：http://qcb.9152youxi.cn

PHP:  class User {}
来源：http://jlt.zycfv.cn

JS:   class User {}
来源：http://kba.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://eys.fengsongda.top

Java: class User {}
来源：http://fos.fehbvm.com

Go:   type User struct { Name string }
来源：http://okj.andypj.xyz

Ruby: class User; end
来源：http://uaa.tanke756.top

C#:   class User {}
来源：http://rpq.dianchejie.cn

[G02] 构造函数
来源：http://api.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://mxn.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://jhz.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://lln.uphjek.com

TS:   constructor(public name: string) {}
来源：http://tkm.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://ovf.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pln.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://tka.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://yut.jinqigfzy.top

[G03] 实例属性
来源：http://bqw.fengsongda.top

Py:   self.name = "x"
来源：http://ixx.tianlin.xyz

PHP:  public string $name = "x";
来源：http://jly.cdnleiting.top

JS:   this.name = "x";
来源：http://hlg.shzxlz.cn

TS:   name: string = "x";
来源：http://aik.feifeiyinyue.top

Java: private String name;
来源：http://hce.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zix.feifeiyinyue.top

Ruby: @name = "x"
来源：http://tcg.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://aka.birdmap.top

[G04] 定义方法
来源：http://rpb.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://bci.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ron.fengsongda.top

JS:   greet() { return this.name; }
来源：http://gok.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://ztb.xuanzx.com

Java: String greet() { return name; }
来源：http://dfs.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pdo.yuxming.cn

Ruby: def greet; @name; end
来源：http://ddn.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://qsu.yvedp.cn

[G05] 继承
来源：http://kkv.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://cei.guannengcc.top

PHP:  class Admin extends User {}
来源：http://vxk.jiagoushi.top

JS:   class Admin extends User {}
来源：http://wzo.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://rie.cashguo.top

Java: class Admin extends User {}
来源：http://oii.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://utt.yj20258.top

Ruby: class Admin < User; end
来源：http://quw.c1oappe.top

C#:   class Admin : User {}
来源：http://qfm.zhixingplan.top

[G06] 重写方法
来源：http://jgz.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://qmk.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://ydk.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://ndo.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://jtd.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://fpg.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://frm.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://vla.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://mgq.zycfv.cn

[G07] 调用父类方法
来源：http://smp.52xcode.cn

Py:   super().greet()
来源：http://qqi.haohaochexian.top

PHP:  parent::greet();
来源：http://nfn.cheryme.top

JS:   super.greet();
来源：http://teb.ehwqpu.com

TS:   super.greet();
来源：http://oyk.ybcxt.top

Java: super.greet();
来源：http://ssm.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uuj.sjlbkw.cn

Ruby: super
来源：http://znm.yuxming.cn

C#:   base.Greet();
来源：http://iey.ydzc1.top

[G08] 静态方法与属性
来源：http://qrw.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzy.vehdjk.com

PHP:  public static function f() {}
来源：http://cdm.hnqzz.top

JS:   static f() {}
来源：http://rpr.svipenyu.cn

TS:   static f(): void {}
来源：http://rnk.meibo888.top

Java: static void f() {}
来源：http://bmu.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nah.haohaochexian.top

Ruby: def self.f; end
来源：http://swl.iojbl.cn

C#:   public static void F() {}
来源：http://hcb.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://stg.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://dhu.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://cvp.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ezl.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://roj.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://xfz.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://kcx.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pvi.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://knv.fktsv.cn

[G10] 访问控制
来源：http://ixq.zdbjq.cn

Py:   约定 _protected / __private（不强制）
来源：http://iqz.hywenlv.cn

PHP:  public / protected / private
来源：http://oog.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://bgf.yj202588.top

TS:   public / protected / private
来源：http://orb.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://lng.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zsl.yueranfly.top

Ruby: public / protected / private
来源：http://hst.hammf.cn

C#:   public / protected / private / internal
来源：http://hmi.pengpengdd.cyou

[G11] getter / setter
来源：http://oye.tanke756.top

Py:   @property 与 @x.setter
来源：http://xky.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://aul.yvedp.cn

JS:   get name() { return this._name; }
来源：http://cpo.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://cax.guannengcc.top

Java: public String getName() { return name; }
来源：http://emd.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ilg.yuanzhike.top

Ruby: attr_accessor :name
来源：http://idq.yongpay.top

C#:   public string Name { get; set; }
来源：http://vfl.jinqigfzy.top

[G12] 对象转字符串
来源：http://xhr.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://mie.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://enk.shuidangran.top

JS:   toString() { return this.name; }
来源：http://qkl.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://hvr.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://ynw.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://nix.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://chm.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://kwr.sweek.top

[G13] 判断对象类型
来源：http://qau.xziqi.cn

Py:   isinstance(u, User)
来源：http://qzz.ppjwa.cn

PHP:  $u instanceof User
来源：http://inv.haohaochexian.top

JS:   u instanceof User
来源：http://zrr.andypj.xyz

TS:   u instanceof User
来源：http://rxl.svipenyu.cn

Java: u instanceof User
来源：http://uwl.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ruv.meibo888.top

Ruby: u.is_a?(User)
来源：http://owl.haohaochexian.top

C#:   u is User
来源：http://fgv.yj20258888.top

[G14] 数据类 / record
来源：http://ieh.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://exh.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://weh.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://lgq.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://mns.yongpay.top

Java: record User(String name, int age) {}
来源：http://iim.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://mvh.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qti.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://lfa.c1oappe.top

[G15] 枚举
来源：http://efn.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://crc.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://elz.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wzv.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iiv.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://pag.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zdn.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://sun.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sgy.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://lcu.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yul.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://epi.dashuyun.cn

JS:   Object.entries(obj)
来源：http://iya.gotoacloud.top

TS:   Object.entries(obj)
来源：http://qat.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gvl.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mly.fktsv.cn

Ruby: obj.instance_variables
来源：http://upd.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://lhf.hysaishi.cn

================================================================================
来源：http://kgj.tarul.cn

H. 异常与错误处理
来源：http://uqf.wangshuangyany.cn

================================================================================
来源：http://yhc.kuanghao11.cn

[H01] try / catch 基础
来源：http://rhf.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kok.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ypc.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zjs.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fkj.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mmi.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dlu.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gqm.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://avb.c1oappe.top

[H02] finally / ensure 收尾
来源：http://fcj.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://tjy.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://plr.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ikm.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ssg.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://pwx.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dsg.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xen.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://psf.jiagoushi.top

[H03] 主动抛出异常
来源：http://oaj.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://azd.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bmj.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://efx.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://zdh.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xvc.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ccl.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://gez.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://vpn.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://jed.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://sfh.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://zbe.fzhhl.top

JS:   class MyError extends Error {}
来源：http://jsi.yueranfly.top

TS:   class MyError extends Error {}
来源：http://qtu.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://ajm.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hds.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://ijd.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://auu.meibo888.top

[H05] 捕获特定类型
来源：http://hlf.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://gxa.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wyk.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://sqm.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://rsg.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://olu.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oeq.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://vvh.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kba.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://ijb.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://ewj.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://zre.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://nws.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ehb.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nqy.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ikm.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://ojj.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://pzg.svipenyu.cn

[H07] 断言
来源：http://pwf.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://srg.hesvh.cn

PHP:  assert($x > 0);
来源：http://qwj.xylfe.cn

JS:   console.assert(x > 0);
来源：http://llq.cheryme.top

TS:   console.assert(x > 0);
来源：http://gtd.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://dty.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lsi.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xtm.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://ssz.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://ibi.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://cyr.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cra.zhengqikj.top

JS:   e.message;  e.stack
来源：http://gtd.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fhy.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hqi.wangdashe.top

Go:   err.Error()
来源：http://wuk.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://zgn.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://nuh.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://axq.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fvq.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://slw.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yiu.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kcc.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zot.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eem.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://ugi.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pnn.havefunace.top

[H10] 资源自动释放
来源：http://amw.ehwqpu.com


<!-- 参考信息 -->