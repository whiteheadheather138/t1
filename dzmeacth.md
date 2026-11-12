代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://odq.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uwk.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vhb.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://spr.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://dpk.nanxuanxn.top

[F06] 删除文件
来源：http://grq.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://vdm.daria6918.cn

PHP:  unlink("a.txt");
来源：http://bly.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ltq.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://fxp.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ieu.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://cbm.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://dsa.316326.xyz

C#:   File.Delete("a.txt");
来源：http://nnq.birdmap.top

[F07] 创建目录（含多级）
来源：http://oyw.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qkx.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ohk.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aer.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ues.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zii.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mym.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://whk.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fct.fktsv.cn

[F08] 遍历目录
来源：http://fys.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zgg.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uea.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://jtg.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://cww.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://koc.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yon.cheryme.top

Ruby: Dir.children("dir")
来源：http://dlb.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://ief.jinqigufen.top

[F09] 获取文件大小
来源：http://jxx.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://qbc.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://uag.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://jay.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://rzz.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://dtb.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://luv.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://rhx.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://gme.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://cwt.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hvv.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rwd.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bgo.daria6918.cn

TS:   path.extname("a.txt")
来源：http://szz.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tse.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rik.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fow.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nlh.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://crc.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gjx.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zze.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://irf.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gdc.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gbq.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kni.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dqu.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tac.xziqi.cn

[F12] CSV 读写
来源：http://nmc.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xww.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yuv.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yen.iojbl.cn

TS:   // 同上
来源：http://oog.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gcj.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://des.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gjh.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wvz.epnwcf.com

================================================================================
来源：http://gnt.cashguo.top

G. 面向对象
来源：http://dil.sxryk.cn

================================================================================
来源：http://rxs.guowangkeji.top

[G01] 定义类
来源：http://eod.vehdjk.com

Py:   class User: pass
来源：http://fcz.shanyushiyangkeji.top

PHP:  class User {}
来源：http://nbi.yangfankeji.com

JS:   class User {}
来源：http://cet.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://wzz.sysykeji.top

Java: class User {}
来源：http://xhf.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://fws.yanxiufei.cn

Ruby: class User; end
来源：http://eeu.meibo888.top

C#:   class User {}
来源：http://ate.jinyuanbaomall.cn

[G02] 构造函数
来源：http://obk.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://gkh.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://ige.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://iqc.birdmap.top

TS:   constructor(public name: string) {}
来源：http://ywv.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://ckx.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://var.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://dty.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://vjo.zhongyouzk.top

[G03] 实例属性
来源：http://ibh.cucudq.cn

Py:   self.name = "x"
来源：http://vvi.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://fcx.chenlongwang.top

JS:   this.name = "x";
来源：http://zgt.yuxming.cn

TS:   name: string = "x";
来源：http://jvw.smart0.xyz

Java: private String name;
来源：http://fbm.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uzk.hammf.cn

Ruby: @name = "x"
来源：http://wwt.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://vbp.hongshengwenyu.top

[G04] 定义方法
来源：http://pmk.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://fvj.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fnm.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://dsj.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://ekk.zdbjq.cn

Java: String greet() { return name; }
来源：http://ljo.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sic.zhixingplan.top

Ruby: def greet; @name; end
来源：http://hzc.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://xpf.vehdjk.com

[G05] 继承
来源：http://jiy.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://ckr.52xcode.cn

PHP:  class Admin extends User {}
来源：http://did.yangfankeji.com

JS:   class Admin extends User {}
来源：http://bmx.yonumen.top

TS:   class Admin extends User {}
来源：http://wpk.jinqigufen.top

Java: class Admin extends User {}
来源：http://rvv.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pra.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://buw.fzhhl.top

C#:   class Admin : User {}
来源：http://asp.jinghuilouyu.cn

[G06] 重写方法
来源：http://jqz.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://jxu.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nlk.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://kbw.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://yss.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://sqf.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xqo.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://xhe.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://asg.wangshuangyany.cn

[G07] 调用父类方法
来源：http://see.gotoacloud.top

Py:   super().greet()
来源：http://bdk.fengsongda.top

PHP:  parent::greet();
来源：http://beq.sweek.top

JS:   super.greet();
来源：http://okn.jinqigfzy.top

TS:   super.greet();
来源：http://gni.yongpay.top

Java: super.greet();
来源：http://rfn.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gfa.aizwys.cn

Ruby: super
来源：http://sbu.aibaodan.cn

C#:   base.Greet();
来源：http://kis.gogol.net.cn

[G08] 静态方法与属性
来源：http://fsi.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zsp.cashguo.top

PHP:  public static function f() {}
来源：http://fvx.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://dsl.xuetiantiany.cn

TS:   static f(): void {}
来源：http://dap.jiagoushi.top

Java: static void f() {}
来源：http://bgk.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eaw.tarul.cn

Ruby: def self.f; end
来源：http://xjg.ehwqpu.com

C#:   public static void F() {}
来源：http://tek.hnqzz.top

[G09] 接口 / 抽象类
来源：http://gva.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ckj.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://pmx.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jim.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://wva.hcnkem.com

Java: interface Shape { double area(); }
来源：http://jkh.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://liu.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fub.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://qan.nwbrower.top

[G10] 访问控制
来源：http://znc.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://kcj.smart0.xyz

PHP:  public / protected / private
来源：http://izw.havefunace.top

JS:   #private 字段；其余公开
来源：http://vrj.ydjk.org.cn

TS:   public / protected / private
来源：http://iqj.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://pbc.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mcb.aizwys.cn

Ruby: public / protected / private
来源：http://svo.hnqzz.top

C#:   public / protected / private / internal
来源：http://yct.ivvv.top

[G11] getter / setter
来源：http://yfu.c1oappe.top

Py:   @property 与 @x.setter
来源：http://jqf.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zmu.ybcxt.top

JS:   get name() { return this._name; }
来源：http://uma.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://lxa.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://gnd.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nfz.yfazqb.com

Ruby: attr_accessor :name
来源：http://tfu.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://gha.dianchejie.cn

[G12] 对象转字符串
来源：http://muu.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://gzj.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sby.yonumen.top

JS:   toString() { return this.name; }
来源：http://tod.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://ueb.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://jmq.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ymy.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://nxz.jinqigufen.top

C#:   public override string ToString() => Name;
来源：http://vcm.gotoacloud.top

[G13] 判断对象类型
来源：http://xhg.52xcode.cn

Py:   isinstance(u, User)
来源：http://iqr.yueranfly.top

PHP:  $u instanceof User
来源：http://vpw.vqdsnc.cn

JS:   u instanceof User
来源：http://alj.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://sis.ydjk.org.cn

Java: u instanceof User
来源：http://pta.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uia.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://ijn.gaohongyu789.top

C#:   u is User
来源：http://akx.chenlongwang.top

[G14] 数据类 / record
来源：http://drn.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dus.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://uef.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://lwy.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://wnw.yj20258888.top

Java: record User(String name, int age) {}
来源：http://mwk.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://ztc.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pym.yonumen.top

C#:   record User(string Name, int Age);
来源：http://nsl.vehdjk.com

[G15] 枚举
来源：http://rge.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blr.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gtj.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://meg.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xct.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://ilr.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uyx.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://yhp.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cae.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://qgz.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ouw.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://qhr.0kj1m.cn

JS:   Object.entries(obj)
来源：http://anr.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://xrz.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mja.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://maf.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://reg.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://yix.pengpengdd.cyou

================================================================================
来源：http://mjs.tarul.cn

H. 异常与错误处理
来源：http://ieh.ehwqpu.com

================================================================================
来源：http://sfi.nwbrower.top

[H01] try / catch 基础
来源：http://cgw.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://czl.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gsm.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iur.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mmb.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://czp.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wfe.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mmz.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://twe.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://msj.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://zoq.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vml.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eie.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ujd.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rtv.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gcx.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hzt.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://msg.yonumen.top

[H03] 主动抛出异常
来源：http://qot.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://ypb.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bxt.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://kff.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://sux.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fnw.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xuj.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fdt.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://uce.birdmap.top

[H04] 自定义异常类型
来源：http://rnc.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://ovj.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sti.sweek.top

JS:   class MyError extends Error {}
来源：http://xyo.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://quw.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://cxy.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gor.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://qoa.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://hql.gogol.net.cn

[H05] 捕获特定类型
来源：http://xju.sjlbkw.cn

Py:   except ValueError as e:
来源：http://gez.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pjk.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://iez.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://glc.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://int.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bhu.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://gnw.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qgy.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://emz.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://for.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://mbm.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rga.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://smj.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://egb.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hyc.yanxiufei.cn

Ruby: d&.dig(:a, :b)
来源：http://siw.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://erb.andypj.xyz

[H07] 断言
来源：http://rdn.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://req.hfpthk.cn

PHP:  assert($x > 0);
来源：http://oub.nwbrower.top

JS:   console.assert(x > 0);
来源：http://uyx.birdmap.top

TS:   console.assert(x > 0);
来源：http://iuw.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://jch.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gjz.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tdh.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://olg.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://gly.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://qwi.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ddq.nwbrower.top

JS:   e.message;  e.stack
来源：http://ekt.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nuz.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kqn.daria6918.cn

Go:   err.Error()
来源：http://uiz.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://nab.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://xjs.yj20258888.top

[H09] 带错误码的异常
来源：http://kbw.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://npv.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://pzk.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lwh.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uho.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jfj.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nac.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://eco.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rwb.birdmap.top

[H10] 资源自动释放
来源：http://tga.tianlin.xyz


<!-- 参考信息 -->