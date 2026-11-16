代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://ygm.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mgi.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uzc.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://owb.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://jgz.pycfn.com

[F06] 删除文件
来源：http://dkn.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://gvp.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://opu.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://blk.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://dhe.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yeh.yj202588.top

Go:   os.Remove("a.txt")
来源：http://frs.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://urk.yj20258.top

C#:   File.Delete("a.txt");
来源：http://xgn.yueranfly.top

[F07] 创建目录（含多级）
来源：http://dmh.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://atd.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://omh.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hjy.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://put.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uyk.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pdy.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://woq.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wiy.kuanghao11.cn

[F08] 遍历目录
来源：http://duq.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://onx.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tqb.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://eem.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://msv.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ixo.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://hrd.yfazqb.com

Ruby: Dir.children("dir")
来源：http://mwn.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://lgk.c1oappe.top

[F09] 获取文件大小
来源：http://oxn.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://lhw.yueranfly.top

PHP:  filesize("a.txt");
来源：http://lsh.hnxiangtu.top

JS:   fs.statSync("a.txt").size
来源：http://tei.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://jdw.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mpd.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eea.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://res.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://vam.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://ygr.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kan.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sfj.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xis.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://dqp.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cpb.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cpt.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fgj.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ssa.cdnleiting.top

[F11] 复制与移动文件
来源：http://flp.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ahn.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gci.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kpo.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pxc.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oyy.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uvw.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://niy.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ywb.fehbvm.com

[F12] CSV 读写
来源：http://plh.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uav.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://osl.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://shf.aizwys.cn

TS:   // 同上
来源：http://oxf.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wdc.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aoc.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gfq.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nwz.52xcode.cn

================================================================================
来源：http://vhf.shzxlz.cn

G. 面向对象
来源：http://rjc.gzhubu.top

================================================================================
来源：http://rqg.fehbvm.com

[G01] 定义类
来源：http://fjk.xylfe.cn

Py:   class User: pass
来源：http://yas.gogol.net.cn

PHP:  class User {}
来源：http://gst.hammf.cn

JS:   class User {}
来源：http://zou.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://ncc.bjfxy.top

Java: class User {}
来源：http://mhs.hfpthk.cn

Go:   type User struct { Name string }
来源：http://zmp.birdmap.top

Ruby: class User; end
来源：http://wvo.cqqwz.cn

C#:   class User {}
来源：http://wsb.zhixingplan.top

[G02] 构造函数
来源：http://hfu.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://jch.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://wiu.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://fej.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://pem.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://vqu.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rhc.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://ogw.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://kcg.zycfv.cn

[G03] 实例属性
来源：http://inc.nanxinkj.top

Py:   self.name = "x"
来源：http://zgz.ctjpmb.com

PHP:  public string $name = "x";
来源：http://wna.cqqwz.cn

JS:   this.name = "x";
来源：http://yvn.zhiwuduotai.top

TS:   name: string = "x";
来源：http://lpp.zhixingplan.top

Java: private String name;
来源：http://jof.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cdd.hongshengwenyu.top

Ruby: @name = "x"
来源：http://iyz.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://ijk.bbcook.cn

[G04] 定义方法
来源：http://cdj.yj20258.top

Py:   def greet(self): return self.name
来源：http://aiy.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bmb.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://kxb.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://jtj.yuanzhike.top

Java: String greet() { return name; }
来源：http://iky.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://moa.ydzc1.top

Ruby: def greet; @name; end
来源：http://wly.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://fqp.smart0.xyz

[G05] 继承
来源：http://ckr.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://xcz.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://mdt.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://qle.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://dwj.andypj.xyz

Java: class Admin extends User {}
来源：http://nrs.cucudq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wld.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://zwf.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://eep.guowangkeji.top

[G06] 重写方法
来源：http://gix.cashguo.top

Py:   def greet(self): return "admin"
来源：http://oiz.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jtw.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://ryv.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://smu.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://gbv.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vbo.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://yfh.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://vfp.hammf.cn

[G07] 调用父类方法
来源：http://icm.svipenyu.cn

Py:   super().greet()
来源：http://bzi.yangfankeji.com

PHP:  parent::greet();
来源：http://fhn.andypj.xyz

JS:   super.greet();
来源：http://tqz.hysaishi.cn

TS:   super.greet();
来源：http://oma.xuetiantiany.cn

Java: super.greet();
来源：http://yys.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ean.aizwys.cn

Ruby: super
来源：http://qxf.hfpthk.cn

C#:   base.Greet();
来源：http://gwf.nanxuanxn.top

[G08] 静态方法与属性
来源：http://jpf.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://roe.ctjpmb.com

PHP:  public static function f() {}
来源：http://pct.jyoumei.cn

JS:   static f() {}
来源：http://roq.guannengcc.top

TS:   static f(): void {}
来源：http://ebp.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://xgc.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://phg.chenlongwang.top

Ruby: def self.f; end
来源：http://pms.52xcode.cn

C#:   public static void F() {}
来源：http://wps.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://tud.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://ubr.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lvj.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bxe.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://tto.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://xng.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://lkt.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ndo.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://ynm.hongshengwenyu.top

[G10] 访问控制
来源：http://lvw.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://kog.hnqzz.top

PHP:  public / protected / private
来源：http://rij.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://zaq.zhoulong.xyz

TS:   public / protected / private
来源：http://ebi.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://igy.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tad.bjfxy.top

Ruby: public / protected / private
来源：http://bib.bjfxy.top

C#:   public / protected / private / internal
来源：http://fuo.yangfankeji.com

[G11] getter / setter
来源：http://opr.xinyue.icu

Py:   @property 与 @x.setter
来源：http://pnp.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vsg.sysykeji.top

JS:   get name() { return this._name; }
来源：http://exw.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://lox.52xcode.cn

Java: public String getName() { return name; }
来源：http://nuq.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yla.c1oappe.top

Ruby: attr_accessor :name
来源：http://yox.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://fdn.0kj1m.cn

[G12] 对象转字符串
来源：http://gjq.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://jmk.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yco.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://wwl.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://uzx.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://fvp.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://eds.redwolf501.top

Ruby: def to_s; @name; end
来源：http://rcb.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://plg.dashuyun.cn

[G13] 判断对象类型
来源：http://tva.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://ngs.yvedp.cn

PHP:  $u instanceof User
来源：http://qbt.c1oappe.top

JS:   u instanceof User
来源：http://yio.fzhhl.top

TS:   u instanceof User
来源：http://utj.316326.xyz

Java: u instanceof User
来源：http://nlm.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lnv.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://ufu.ybcxt.top

C#:   u is User
来源：http://zvv.tian-w.cn

[G14] 数据类 / record
来源：http://bml.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yxe.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://oyg.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://ywb.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://gov.xylfe.cn

Java: record User(String name, int age) {}
来源：http://vaf.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://gfv.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ksp.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://jzv.ehwqpu.com

[G15] 枚举
来源：http://dkh.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hsg.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://occ.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kri.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://adf.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://ysa.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gcc.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://czg.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pzc.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://eqs.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bxf.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://vsx.birdmap.top

JS:   Object.entries(obj)
来源：http://aax.ydzc1.top

TS:   Object.entries(obj)
来源：http://kkt.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gxd.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iiz.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://swk.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://wvh.zhengqikj.top

================================================================================
来源：http://fsu.chenjidiqi.icu

H. 异常与错误处理
来源：http://qht.yj202588.top

================================================================================
来源：http://gbk.tianlin.xyz

[H01] try / catch 基础
来源：http://bde.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://und.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xpu.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qfc.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zua.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ndg.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vsh.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hrp.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gsy.tarul.cn

[H02] finally / ensure 收尾
来源：http://afv.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://yzd.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://usf.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tbn.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rnd.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://ufj.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tyw.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bta.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cds.52xcode.cn

[H03] 主动抛出异常
来源：http://dpj.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://kdx.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xxn.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://gdj.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://mxz.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qre.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rbh.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ejw.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lkz.yueranfly.top

[H04] 自定义异常类型
来源：http://ykt.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://wzg.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wil.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://pom.epnwcf.com

TS:   class MyError extends Error {}
来源：http://erh.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://hra.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://epa.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://awi.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://mnt.ydjk.org.cn

[H05] 捕获特定类型
来源：http://spf.yuxming.cn

Py:   except ValueError as e:
来源：http://kwh.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dxo.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://lbj.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://zfr.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://rcx.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ium.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://hkp.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ruj.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://xdz.xziqi.cn

Py:   value = d.get("k") or default
来源：http://hiz.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://yup.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://stk.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dwo.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jbj.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://teg.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://tdi.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://tju.zhiwuduotai.top

[H07] 断言
来源：http://dvq.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://oee.wangdashe.top

PHP:  assert($x > 0);
来源：http://ldb.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://khh.yongpay.top

TS:   console.assert(x > 0);
来源：http://ikv.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://gzc.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lwf.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ekc.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://mtx.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://hxs.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://utw.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bue.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://emi.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dtl.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kqb.shuidangran.top

Go:   err.Error()
来源：http://xwp.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://mbk.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://ktc.gaohongyu789.top

[H09] 带错误码的异常
来源：http://ycc.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://olm.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eit.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wkp.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lzn.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nec.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ktt.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://dqm.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eka.birdmap.top

[H10] 资源自动释放
来源：http://ikr.tian-w.cn


<!-- 参考信息 -->