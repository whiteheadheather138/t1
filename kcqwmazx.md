代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://fca.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://cmb.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xzs.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://fdi.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://vbf.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://tmj.hesvh.cn

[F07] 创建目录（含多级）
来源：http://ifm.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qgs.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oin.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eck.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ock.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ktp.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xtc.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jqi.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mxm.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://wrw.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ybj.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rmj.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://dwf.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://ita.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jli.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vdv.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://qol.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://yfq.gzhubu.top

[F09] 获取文件大小
来源：http://fdf.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://ggw.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://bua.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://eef.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://ktb.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://slj.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://svk.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://qvl.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://wtn.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://gtw.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kfv.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xtz.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gra.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://fdq.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rlc.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nvj.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bwo.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ysp.jiagoushi.top

[F11] 复制与移动文件
来源：http://kgu.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wkt.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fzv.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ygs.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtv.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qus.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://exn.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kpg.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dmh.aizwys.cn

[F12] CSV 读写
来源：http://dyl.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bwb.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vps.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://osf.shanyushiyangkeji.top

TS:   // 同上
来源：http://nxr.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gxo.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lgw.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://klz.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nfi.chenzaomai.com

================================================================================
来源：http://svg.xuetiantiany.cn

G. 面向对象
来源：http://vwt.jinyuanbaomall.cn

================================================================================
来源：http://rrk.gotoacloud.top

[G01] 定义类
来源：http://mhf.jinghuilouyu.cn

Py:   class User: pass
来源：http://ylh.hysaishi.cn

PHP:  class User {}
来源：http://day.jinqigfzy.top

JS:   class User {}
来源：http://eyn.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://xpo.gaohongyu789.top

Java: class User {}
来源：http://btd.bjfxy.top

Go:   type User struct { Name string }
来源：http://iht.jianghu66.top

Ruby: class User; end
来源：http://axf.nanxuanxn.top

C#:   class User {}
来源：http://cpv.fzhhl.top

[G02] 构造函数
来源：http://mwu.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://ctn.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://rhv.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://pee.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://hsg.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://vjd.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://irh.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://pti.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://hwg.316326.xyz

[G03] 实例属性
来源：http://sca.daria6918.cn

Py:   self.name = "x"
来源：http://biu.yangfankeji.com

PHP:  public string $name = "x";
来源：http://qqn.sxryk.cn

JS:   this.name = "x";
来源：http://fgp.snrcjt.cn

TS:   name: string = "x";
来源：http://kks.pycfn.com

Java: private String name;
来源：http://azj.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qrs.jianghu66.top

Ruby: @name = "x"
来源：http://ikn.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://vcj.wangshuangyany.cn

[G04] 定义方法
来源：http://owc.hcnkem.com

Py:   def greet(self): return self.name
来源：http://bqb.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ncs.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://axl.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://alf.redwolf501.top

Java: String greet() { return name; }
来源：http://xfz.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tef.jyoumei.cn

Ruby: def greet; @name; end
来源：http://ana.xylfe.cn

C#:   public string Greet() => Name;
来源：http://jgb.meibo888.top

[G05] 继承
来源：http://tol.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://tqf.cucudq.cn

PHP:  class Admin extends User {}
来源：http://xid.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://zxa.hfpthk.cn

TS:   class Admin extends User {}
来源：http://xvk.hcnkem.com

Java: class Admin extends User {}
来源：http://spm.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ozr.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://tsr.cdnleiting.top

C#:   class Admin : User {}
来源：http://ixz.nanxinkj.top

[G06] 重写方法
来源：http://vyb.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://sgv.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://omr.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://igq.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://bkz.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://awy.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kla.cashguo.top

Ruby: def greet; "admin"; end
来源：http://tnk.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://rmp.wangshuangyany.cn

[G07] 调用父类方法
来源：http://cii.xuanzx.com

Py:   super().greet()
来源：http://yqc.yongpay.top

PHP:  parent::greet();
来源：http://cka.fzhhl.top

JS:   super.greet();
来源：http://liw.jyoumei.cn

TS:   super.greet();
来源：http://jph.birdmap.top

Java: super.greet();
来源：http://owq.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dqg.meibo888.top

Ruby: super
来源：http://bnu.yvedp.cn

C#:   base.Greet();
来源：http://jbg.hammf.cn

[G08] 静态方法与属性
来源：http://zqw.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fkj.quarkkingdee.top

PHP:  public static function f() {}
来源：http://dbh.sufxvd.cn

JS:   static f() {}
来源：http://del.xziqi.cn

TS:   static f(): void {}
来源：http://pdz.fengsongda.top

Java: static void f() {}
来源：http://agq.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bph.guowangkeji.top

Ruby: def self.f; end
来源：http://nxk.jyoumei.cn

C#:   public static void F() {}
来源：http://ggx.iojbl.cn

[G09] 接口 / 抽象类
来源：http://all.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://zxs.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://ajs.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xgb.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://jpy.redwolf501.top

Java: interface Shape { double area(); }
来源：http://aqd.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://qnx.jqgfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://unz.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://les.zhengqikj.top

[G10] 访问控制
来源：http://iyf.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://rob.sufxvd.cn

PHP:  public / protected / private
来源：http://cfs.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://wsc.xylfe.cn

TS:   public / protected / private
来源：http://qwg.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://gid.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://tdv.hesvh.cn

Ruby: public / protected / private
来源：http://gma.cqqwz.cn

C#:   public / protected / private / internal
来源：http://xxw.fanxiaobao.xyz

[G11] getter / setter
来源：http://ebm.fengsongda.top

Py:   @property 与 @x.setter
来源：http://fof.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://tfl.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://zkf.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://jph.daria6918.cn

Java: public String getName() { return name; }
来源：http://hre.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ugz.birdmap.top

Ruby: attr_accessor :name
来源：http://wzq.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://kym.daxiang520.top

[G12] 对象转字符串
来源：http://cqe.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://ubh.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ury.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://rcq.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://csv.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://zyv.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uzu.ybcxt.top

Ruby: def to_s; @name; end
来源：http://nvo.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://fuk.jyoumei.cn

[G13] 判断对象类型
来源：http://gfh.52xcode.cn

Py:   isinstance(u, User)
来源：http://eyj.gzhubu.top

PHP:  $u instanceof User
来源：http://jge.tianlin.xyz

JS:   u instanceof User
来源：http://rjn.zhongyouzk.top

TS:   u instanceof User
来源：http://dcu.chenlongwang.top

Java: u instanceof User
来源：http://rso.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://bng.bjfxy.top

Ruby: u.is_a?(User)
来源：http://unj.sysykeji.top

C#:   u is User
来源：http://owc.andypj.xyz

[G14] 数据类 / record
来源：http://aqk.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tvf.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://eyl.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nyi.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://zpc.sysykeji.top

Java: record User(String name, int age) {}
来源：http://eny.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://xvn.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uan.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://evd.haohaochexian.top

[G15] 枚举
来源：http://cmw.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xvx.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zmx.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bqy.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nsp.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://efm.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://imt.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://bma.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://god.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://okf.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://agi.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://qiz.jiagoushi.top

JS:   Object.entries(obj)
来源：http://mtq.gotoacloud.top

TS:   Object.entries(obj)
来源：http://ena.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jao.yongpay.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qrb.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://uua.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://mdb.jinqigfzy.top

================================================================================
来源：http://ddf.quarkkingdee.top

H. 异常与错误处理
来源：http://zue.quarkkingdee.top

================================================================================
来源：http://pfl.yueranfly.top

[H01] try / catch 基础
来源：http://zuf.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fms.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dqr.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bzf.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mdd.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://upo.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ggv.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tfr.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ayv.yuxming.cn

[H02] finally / ensure 收尾
来源：http://fkr.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rpp.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ufp.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://poz.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jki.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://zee.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://trh.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://rzm.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pzp.cdnleiting.top

[H03] 主动抛出异常
来源：http://gow.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://ora.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hdy.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://rdu.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://whv.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lbx.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xrz.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://rsg.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://klm.jiagoushi.top

[H04] 自定义异常类型
来源：http://jmm.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://sed.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://rpd.hammf.cn

JS:   class MyError extends Error {}
来源：http://clj.epnwcf.com

TS:   class MyError extends Error {}
来源：http://uio.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://fzn.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lgj.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://qre.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://prh.chenlongwang.top

[H05] 捕获特定类型
来源：http://vtw.c1oappe.top

Py:   except ValueError as e:
来源：http://him.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qcs.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://pwi.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://ifv.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://lyp.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gng.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://qeu.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://har.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://bms.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://gzk.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tkx.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://toj.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://zdn.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cre.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nvp.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://zyu.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://ijv.yj20258888.top

[H07] 断言
来源：http://oau.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://fqa.nanxinkj.top

PHP:  assert($x > 0);
来源：http://dgx.316326.xyz

JS:   console.assert(x > 0);
来源：http://zya.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://nut.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://flp.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ejk.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://pku.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://ylk.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://hba.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ogm.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vzy.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://keo.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://upg.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xds.ywan-chungtsiang.top

Go:   err.Error()
来源：http://lyv.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://avg.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://qdm.cucudq.cn

[H09] 带错误码的异常
来源：http://bbt.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cne.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rkp.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gyk.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rqp.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uum.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bwx.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mzq.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://umo.cheryme.top

[H10] 资源自动释放
来源：http://dpt.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jvb.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://trm.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eas.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vcz.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dib.hysaishi.cn

Go:   defer f.Close()
来源：http://qpk.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pgp.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sze.jlsjyb.cn


<!-- 参考信息 -->