代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hbz.chenjidiqi.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://dgk.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qus.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://jxs.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://oic.hfpthk.cn

[F06] 删除文件
来源：http://rxg.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://dwp.havefunace.top

PHP:  unlink("a.txt");
来源：http://ttl.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://syz.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hdu.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wbn.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://ufs.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://ayt.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://zlq.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://jdo.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bdl.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xwr.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://trn.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ypc.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vtt.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://phk.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://enj.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mnp.jqgfzy.top

[F08] 遍历目录
来源：http://inx.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vix.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mlz.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://ioe.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://psv.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nji.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://trs.c1oappe.top

Ruby: Dir.children("dir")
来源：http://wpa.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://fwc.zhixingplan.top

[F09] 获取文件大小
来源：http://ibt.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://tpm.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://yit.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://roh.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://xva.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://ipn.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vvx.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://hgt.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://ghw.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://wne.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ybo.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mxv.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cfg.gzhubu.top

TS:   path.extname("a.txt")
来源：http://ira.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rrv.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xcn.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kow.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://prp.redwolf501.top

[F11] 复制与移动文件
来源：http://gck.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://erw.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://knj.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mcr.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qsv.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jda.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lru.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://czy.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cyy.fehbvm.com

[F12] CSV 读写
来源：http://qrk.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://clq.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://emi.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tbp.quarkkingdee.top

TS:   // 同上
来源：http://zbj.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qpl.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://som.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rla.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://exp.mhx1999.top

================================================================================
来源：http://spm.fzhhl.top

G. 面向对象
来源：http://adp.yj202588.top

================================================================================
来源：http://kbo.yj20258888.top

[G01] 定义类
来源：http://hbt.chenlongwang.top

Py:   class User: pass
来源：http://yri.jlsjyb.cn

PHP:  class User {}
来源：http://jeq.shuidangran.top

JS:   class User {}
来源：http://gfv.ivvv.top

TS:   class User { name: string = ""; }
来源：http://kiq.ybcxt.top

Java: class User {}
来源：http://dvc.wangdashe.top

Go:   type User struct { Name string }
来源：http://qys.xylfe.cn

Ruby: class User; end
来源：http://bla.tarul.cn

C#:   class User {}
来源：http://hnq.meibo888.top

[G02] 构造函数
来源：http://mck.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://joy.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://xot.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://yzv.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://moh.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://fpp.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qrp.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://ain.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://ykn.tanke756.top

[G03] 实例属性
来源：http://yaw.chenjidiqi.icu

Py:   self.name = "x"
来源：http://uki.epnwcf.com

PHP:  public string $name = "x";
来源：http://twl.yuxming.cn

JS:   this.name = "x";
来源：http://vyb.shuidangran.top

TS:   name: string = "x";
来源：http://fed.tian-w.cn

Java: private String name;
来源：http://gex.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://myq.hnqzz.top

Ruby: @name = "x"
来源：http://czr.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://nhl.nanxuanxn.top

[G04] 定义方法
来源：http://ncf.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://ekn.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://qgz.ybcxt.top

JS:   greet() { return this.name; }
来源：http://mgq.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://spf.yj20258.top

Java: String greet() { return name; }
来源：http://iih.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xhl.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://nzs.aizwys.cn

C#:   public string Greet() => Name;
来源：http://xjw.jinyuanbaomall.cn

[G05] 继承
来源：http://hld.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://pqa.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://syj.fktsv.cn

JS:   class Admin extends User {}
来源：http://hrk.dianchejie.cn

TS:   class Admin extends User {}
来源：http://lhh.jinqigufen.top

Java: class Admin extends User {}
来源：http://mgu.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qxa.wangdashe.top

Ruby: class Admin < User; end
来源：http://kjj.daxiang520.top

C#:   class Admin : User {}
来源：http://wig.zhijiandao.cn

[G06] 重写方法
来源：http://tuq.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://qtu.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://axk.tarul.cn

JS:   greet() { return "admin"; }
来源：http://jsh.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://mam.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://nje.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rjj.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://gfi.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://xed.hongshengwenyu.top

[G07] 调用父类方法
来源：http://mxg.tian-w.cn

Py:   super().greet()
来源：http://hpt.tian-w.cn

PHP:  parent::greet();
来源：http://xzp.bbcook.cn

JS:   super.greet();
来源：http://vhf.jinyuanbaomall.cn

TS:   super.greet();
来源：http://kvg.ppjwa.cn

Java: super.greet();
来源：http://mzs.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ojs.tian-w.cn

Ruby: super
来源：http://mqo.yuanzhike.top

C#:   base.Greet();
来源：http://guw.zhixingplan.top

[G08] 静态方法与属性
来源：http://wrp.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bou.kuanghao11.cn

PHP:  public static function f() {}
来源：http://xja.jinqigfzy.top

JS:   static f() {}
来源：http://qcj.zhijiandao.cn

TS:   static f(): void {}
来源：http://teo.hongshengwenyu.top

Java: static void f() {}
来源：http://tth.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kwy.xuetiantiany.cn

Ruby: def self.f; end
来源：http://usd.hysaishi.cn

C#:   public static void F() {}
来源：http://god.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://orm.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://soj.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://kdl.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ulw.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://lje.sweek.top

Java: interface Shape { double area(); }
来源：http://fas.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://wdg.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://akl.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://wvj.yongpay.top

[G10] 访问控制
来源：http://xjj.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://gpz.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://dtk.hnxiangtu.top

JS:   #private 字段；其余公开
来源：http://tca.ydjk.org.cn

TS:   public / protected / private
来源：http://rse.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://svg.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pik.yonumen.top

Ruby: public / protected / private
来源：http://owx.ybcxt.top

C#:   public / protected / private / internal
来源：http://fld.yongpay.top

[G11] getter / setter
来源：http://gpn.xziqi.cn

Py:   @property 与 @x.setter
来源：http://ggz.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fer.xylfe.cn

JS:   get name() { return this._name; }
来源：http://ued.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://yzd.chenzaomai.com

Java: public String getName() { return name; }
来源：http://ddw.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fhm.aibaodan.cn

Ruby: attr_accessor :name
来源：http://yfy.andypj.xyz

C#:   public string Name { get; set; }
来源：http://huf.zhixingplan.top

[G12] 对象转字符串
来源：http://thq.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://foj.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mhv.yj20258888.top

JS:   toString() { return this.name; }
来源：http://ldn.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://jkn.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://ufj.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://zwz.fktsv.cn

Ruby: def to_s; @name; end
来源：http://lif.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://kbu.haohaochexian.top

[G13] 判断对象类型
来源：http://tgf.gzhubu.top

Py:   isinstance(u, User)
来源：http://psl.meibo888.top

PHP:  $u instanceof User
来源：http://sow.zdqjudy.top

JS:   u instanceof User
来源：http://vfk.chenzaomai.com

TS:   u instanceof User
来源：http://ehi.sjlbkw.cn

Java: u instanceof User
来源：http://sjc.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dqd.redwolf501.top

Ruby: u.is_a?(User)
来源：http://sod.gotoacloud.top

C#:   u is User
来源：http://hrh.cashguo.top

[G14] 数据类 / record
来源：http://eka.hysaishi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wyn.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://mou.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://mnc.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://lll.haohaochexian.top

Java: record User(String name, int age) {}
来源：http://ien.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://bgf.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qap.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://uen.gzhubu.top

[G15] 枚举
来源：http://jgu.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rch.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dll.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://adr.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dks.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://wxz.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hgl.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://frt.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tqa.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://cwt.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ote.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://dyc.yuxming.cn

JS:   Object.entries(obj)
来源：http://ody.yj20258.top

TS:   Object.entries(obj)
来源：http://etg.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hfa.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ttu.xinyue.icu

Ruby: obj.instance_variables
来源：http://joe.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://msv.ivvv.top

================================================================================
来源：http://uut.iojbl.cn

H. 异常与错误处理
来源：http://fqb.dashuyun.cn

================================================================================
来源：http://gqc.yueranfly.top

[H01] try / catch 基础
来源：http://ayg.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tpc.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kak.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jfu.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kav.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fjh.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ivd.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://prd.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cjp.andypj.xyz

[H02] finally / ensure 收尾
来源：http://bmx.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ekz.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gdr.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sdy.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zhc.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gis.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://azv.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ezk.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jca.ctjpmb.com

[H03] 主动抛出异常
来源：http://xct.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://frc.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zce.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://tns.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://wgk.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://owi.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ece.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hjv.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://eqo.yuxming.cn

[H04] 自定义异常类型
来源：http://kiu.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://lvc.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gqc.birdmap.top

JS:   class MyError extends Error {}
来源：http://phd.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://neh.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://uto.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zbx.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://feq.bbcook.cn

C#:   class MyException : Exception {}
来源：http://oon.ctjpmb.com

[H05] 捕获特定类型
来源：http://ezh.xylfe.cn

Py:   except ValueError as e:
来源：http://qfa.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://phd.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://zvy.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://pig.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://ibz.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://htw.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://gni.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nok.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://ixw.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://jtp.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://bsu.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://mnj.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://ust.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hkw.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ggc.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://iya.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://ofc.gzhubu.top

[H07] 断言
来源：http://jps.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://jkm.xinyue.icu

PHP:  assert($x > 0);
来源：http://kcy.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://rpe.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://vhu.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://npj.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nxy.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://qrp.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://ter.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://bwl.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://eyw.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hbb.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://waj.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://drk.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cse.hysaishi.cn

Go:   err.Error()
来源：http://mtw.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://gsc.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://lbm.zhijiandao.cn

[H09] 带错误码的异常
来源：http://hdu.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bpb.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ekh.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xpt.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nsb.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://axu.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://icr.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oir.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://yti.gogol.net.cn

[H10] 资源自动释放
来源：http://oif.gaohongyu789.top


<!-- 参考信息 -->