代发 wailian999

Ruby: File.delete("a.txt")
来源：http://ygs.cheryme.top

C#:   File.Delete("a.txt");
来源：http://cam.yuxming.cn

[F07] 创建目录（含多级）
来源：http://csh.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rbs.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gze.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kyw.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ery.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tts.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eui.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hme.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qfw.chenjidiqi.icu

[F08] 遍历目录
来源：http://mda.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vod.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bvq.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://tis.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://cpl.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wlz.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qbo.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://kas.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://hku.jqgufenzy.top

[F09] 获取文件大小
来源：http://jcx.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://cdq.316326.xyz

PHP:  filesize("a.txt");
来源：http://jbo.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://bdt.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://fek.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://fcb.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://trn.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://fro.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://ccf.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://ucx.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eux.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cjv.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wsg.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://tfp.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hgo.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://elj.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cbf.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ibi.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://khp.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ccj.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vim.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://trg.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cir.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fun.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://reb.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ucx.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yft.chenzaomai.com

[F12] CSV 读写
来源：http://uen.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ylk.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tip.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kwy.xziqi.cn

TS:   // 同上
来源：http://ubs.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xtq.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xjh.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kqh.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://goz.epnwcf.com

================================================================================
来源：http://omz.jinyuanbaomall.cn

G. 面向对象
来源：http://sco.epnwcf.com

================================================================================
来源：http://gdh.havefunace.top

[G01] 定义类
来源：http://tcq.hysaishi.cn

Py:   class User: pass
来源：http://agt.hammf.cn

PHP:  class User {}
来源：http://mct.gzhubu.top

JS:   class User {}
来源：http://awt.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://rja.snrcjt.cn

Java: class User {}
来源：http://mnx.jiagoushi.top

Go:   type User struct { Name string }
来源：http://cch.ehwqpu.com

Ruby: class User; end
来源：http://bji.jqgufenzy.top

C#:   class User {}
来源：http://abs.jinghuilouyu.cn

[G02] 构造函数
来源：http://ess.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://poi.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://rzt.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://lpw.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://asc.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://nxk.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qgb.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://znl.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://wza.yangfankeji.com

[G03] 实例属性
来源：http://vqn.aizwys.cn

Py:   self.name = "x"
来源：http://mfj.daria6918.cn

PHP:  public string $name = "x";
来源：http://vea.sufxvd.cn

JS:   this.name = "x";
来源：http://rtx.cucudq.cn

TS:   name: string = "x";
来源：http://hpy.zhixingplan.top

Java: private String name;
来源：http://oee.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://acg.jinqigufen.top

Ruby: @name = "x"
来源：http://eki.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://ldp.tanke756.top

[G04] 定义方法
来源：http://nhd.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://cdu.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wfl.fzhhl.top

JS:   greet() { return this.name; }
来源：http://ugb.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://hfd.yuanzhike.top

Java: String greet() { return name; }
来源：http://mqq.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rwf.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://ghg.hesvh.cn

C#:   public string Greet() => Name;
来源：http://kmz.daxiang520.top

[G05] 继承
来源：http://mfm.yvedp.cn

Py:   class Admin(User): pass
来源：http://srq.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://ovu.iojbl.cn

JS:   class Admin extends User {}
来源：http://zay.yuxming.cn

TS:   class Admin extends User {}
来源：http://dwp.hesvh.cn

Java: class Admin extends User {}
来源：http://vjr.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dlq.52xcode.cn

Ruby: class Admin < User; end
来源：http://amq.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://sxr.yuanzhike.top

[G06] 重写方法
来源：http://pzj.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://szk.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ngl.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://byz.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://agy.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://soa.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kkw.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://zss.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://hle.wangdashe.top

[G07] 调用父类方法
来源：http://sjx.jlsjyb.cn

Py:   super().greet()
来源：http://haj.hnxiangtu.top

PHP:  parent::greet();
来源：http://brm.shanyushiyangtech.top

JS:   super.greet();
来源：http://izy.nanxinkj.top

TS:   super.greet();
来源：http://xiu.xinyue.icu

Java: super.greet();
来源：http://jmu.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mxi.yanxiufei.cn

Ruby: super
来源：http://ziw.xinyue.icu

C#:   base.Greet();
来源：http://uqf.kuanghao11.cn

[G08] 静态方法与属性
来源：http://tyv.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://udy.xinyue.icu

PHP:  public static function f() {}
来源：http://vfc.cashguo.top

JS:   static f() {}
来源：http://rjb.birdmap.top

TS:   static f(): void {}
来源：http://jdx.gotoacloud.top

Java: static void f() {}
来源：http://cvz.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cqm.hammf.cn

Ruby: def self.f; end
来源：http://xbu.daxiang520.top

C#:   public static void F() {}
来源：http://nex.meibo888.top

[G09] 接口 / 抽象类
来源：http://wap.shuidangran.top

Py:   from abc import ABC, abstractmethod
来源：http://spd.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://srr.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://ctd.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://ciu.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://jby.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://cpu.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://scp.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://xhp.yonumen.top

[G10] 访问控制
来源：http://pca.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://idu.chenlongwang.top

PHP:  public / protected / private
来源：http://fkk.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://zgm.ybcxt.top

TS:   public / protected / private
来源：http://wad.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://sks.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://icl.uphjek.com

Ruby: public / protected / private
来源：http://yut.bjfxy.top

C#:   public / protected / private / internal
来源：http://eek.jyoumei.cn

[G11] getter / setter
来源：http://vkx.cheryme.top

Py:   @property 与 @x.setter
来源：http://kgq.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gnu.vehdjk.com

JS:   get name() { return this._name; }
来源：http://yuc.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://zpy.hesvh.cn

Java: public String getName() { return name; }
来源：http://sab.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qfh.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://jkr.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://vrt.zhengqikj.top

[G12] 对象转字符串
来源：http://yjd.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://wqi.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sel.hnqzz.top

JS:   toString() { return this.name; }
来源：http://tdr.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://bcx.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://sab.epnwcf.com

Go:   func (u User) String() string { return u.Name }
来源：http://hqw.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://moo.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://ywg.guannengcc.top

[G13] 判断对象类型
来源：http://ekl.snrcjt.cn

Py:   isinstance(u, User)
来源：http://yxx.nwbrower.top

PHP:  $u instanceof User
来源：http://prg.uphjek.com

JS:   u instanceof User
来源：http://phg.shuidangran.top

TS:   u instanceof User
来源：http://fro.meibo888.top

Java: u instanceof User
来源：http://bal.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://brq.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://yzv.pycfn.com

C#:   u is User
来源：http://thv.zdbjq.cn

[G14] 数据类 / record
来源：http://pup.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vcf.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://glg.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gse.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://yfx.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://dvl.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://tri.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mby.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://tbb.0kj1m.cn

[G15] 枚举
来源：http://uth.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mya.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mzl.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ayo.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xnm.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://bmz.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zlj.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://xck.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bfk.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://vub.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tfj.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://dku.shuidangran.top

JS:   Object.entries(obj)
来源：http://cpb.hesvh.cn

TS:   Object.entries(obj)
来源：http://pzt.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vhf.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jdl.zycfv.cn

Ruby: obj.instance_variables
来源：http://whw.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://sho.yj202588.top

================================================================================
来源：http://qld.yj20258.top

H. 异常与错误处理
来源：http://cjx.fehbvm.com

================================================================================
来源：http://fka.yj202588.top

[H01] try / catch 基础
来源：http://leq.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://glu.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kkj.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hke.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qkt.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ydr.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rud.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oim.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wkg.guannengcc.top

[H02] finally / ensure 收尾
来源：http://sip.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eng.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://znc.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gra.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://cep.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wal.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nii.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ocm.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iyv.yj20258888.top

[H03] 主动抛出异常
来源：http://hms.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://tmf.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hnt.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://tnw.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://tgs.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jsh.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wdz.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eun.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://vze.smart0.xyz

[H04] 自定义异常类型
来源：http://axx.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://vxe.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://ikd.sxryk.cn

JS:   class MyError extends Error {}
来源：http://aus.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://kec.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://jsd.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uri.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://ebd.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://oqo.shuidangran.top

[H05] 捕获特定类型
来源：http://lyb.hnqzz.top

Py:   except ValueError as e:
来源：http://pyi.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cbh.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://ceh.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://bhy.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://mai.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rui.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://lmk.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://txf.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://sqe.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://cat.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://rfl.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://oqj.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mbx.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bqt.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jtv.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://akf.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://hbo.ppjwa.cn

[H07] 断言
来源：http://uov.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://vzt.xylfe.cn

PHP:  assert($x > 0);
来源：http://mnn.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://xdh.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://tbe.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://icp.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mbe.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://wky.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://yuf.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://sic.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://dkf.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eru.hcnkem.com

JS:   e.message;  e.stack
来源：http://scy.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pxb.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://clm.fktsv.cn

Go:   err.Error()
来源：http://xbn.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://utr.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://hgl.yongpay.top

[H09] 带错误码的异常
来源：http://hhg.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://grh.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mlx.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mef.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ttj.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mpi.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hkd.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://ipq.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tja.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://ffe.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://syg.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qwa.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wlr.xuetiantiany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fiz.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cgt.ydjk.org.cn

Go:   defer f.Close()
来源：http://gav.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lvt.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ebt.iojbl.cn

================================================================================
来源：http://qjz.gzhubu.top

I. 正则表达式
来源：http://jgo.gzhubu.top

================================================================================
来源：http://qff.ybcxt.top

[I01] 判断是否匹配
来源：http://qoq.hnxiangtu.top


<!-- 参考信息 -->