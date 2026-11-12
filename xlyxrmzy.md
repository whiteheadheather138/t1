代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://zde.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://flb.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fgq.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://jwz.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://kia.vehdjk.com

[F06] 删除文件
来源：http://wry.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://gej.gzhubu.top

PHP:  unlink("a.txt");
来源：http://lqu.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mnh.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kpl.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vns.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://cvb.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://sbe.tarul.cn

C#:   File.Delete("a.txt");
来源：http://uvi.mhx1999.top

[F07] 创建目录（含多级）
来源：http://xwy.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gly.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eel.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://slf.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zta.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gzg.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://otv.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vst.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lpu.xinyue.icu

[F08] 遍历目录
来源：http://vyz.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hpb.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ikb.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://icr.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://yht.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rmy.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wew.pycfn.com

Ruby: Dir.children("dir")
来源：http://gkc.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://rfu.yongpay.top

[F09] 获取文件大小
来源：http://inl.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://lnw.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://bjj.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://awy.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://fei.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wqx.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tin.aizwys.cn

Ruby: File.size("a.txt")
来源：http://wlg.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://gfr.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://tpx.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tab.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hkk.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pyg.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://kpj.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tdl.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://twh.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pdd.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://row.shzxlz.cn

[F11] 复制与移动文件
来源：http://fwg.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://esi.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://luy.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pry.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vui.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bnk.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rpj.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qao.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cyw.epnwcf.com

[F12] CSV 读写
来源：http://zaf.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mxv.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nin.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://byu.ehwqpu.com

TS:   // 同上
来源：http://paz.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sce.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://brp.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://phz.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zbh.gotoacloud.top

================================================================================
来源：http://vwy.guannengcc.top

G. 面向对象
来源：http://tjo.zhaomingkeji.xyz

================================================================================
来源：http://xfs.jqgfzy.top

[G01] 定义类
来源：http://hgg.fzhhl.top

Py:   class User: pass
来源：http://hwu.guowangkeji.top

PHP:  class User {}
来源：http://yau.cheryme.top

JS:   class User {}
来源：http://wap.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://zlv.smart0.xyz

Java: class User {}
来源：http://dnl.dashuyun.cn

Go:   type User struct { Name string }
来源：http://xeg.jqgufenzy.top

Ruby: class User; end
来源：http://xkq.cucudq.cn

C#:   class User {}
来源：http://vma.52xcode.cn

[G02] 构造函数
来源：http://mwl.ctjpmb.com

Py:   def __init__(self, name): self.name = name
来源：http://mhv.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://xzc.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://mpb.ydjk.org.cn

TS:   constructor(public name: string) {}
来源：http://xbw.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://tel.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://suh.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://rjf.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://uke.zhaomingkeji.xyz

[G03] 实例属性
来源：http://eqd.cheryme.top

Py:   self.name = "x"
来源：http://xbl.gogol.net.cn

PHP:  public string $name = "x";
来源：http://oup.cashguo.top

JS:   this.name = "x";
来源：http://ssw.yangfankeji.com

TS:   name: string = "x";
来源：http://cuz.birdmap.top

Java: private String name;
来源：http://rev.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jio.aizwys.cn

Ruby: @name = "x"
来源：http://jak.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://auf.hnxiangtu.top

[G04] 定义方法
来源：http://oim.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://kpq.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hgz.cheryme.top

JS:   greet() { return this.name; }
来源：http://uep.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://tvw.gzhubu.top

Java: String greet() { return name; }
来源：http://jin.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://amv.yvedp.cn

Ruby: def greet; @name; end
来源：http://poa.andypj.xyz

C#:   public string Greet() => Name;
来源：http://bja.zycfv.cn

[G05] 继承
来源：http://npt.andypj.xyz

Py:   class Admin(User): pass
来源：http://kmr.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://wba.dashuyun.cn

JS:   class Admin extends User {}
来源：http://sjg.aibaodan.cn

TS:   class Admin extends User {}
来源：http://nen.gogol.net.cn

Java: class Admin extends User {}
来源：http://mmh.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://svy.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://ngp.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://loa.ydzc1.top

[G06] 重写方法
来源：http://lkf.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://bvp.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ebg.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://oja.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://chp.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://rdl.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qxu.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://rso.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://qch.fengsongda.top

[G07] 调用父类方法
来源：http://zcu.dianchejie.cn

Py:   super().greet()
来源：http://wbw.wangdashe.top

PHP:  parent::greet();
来源：http://nod.jyoumei.cn

JS:   super.greet();
来源：http://ahi.daxiang520.top

TS:   super.greet();
来源：http://iji.zhongyouzk.top

Java: super.greet();
来源：http://hov.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://puf.tanke756.top

Ruby: super
来源：http://qgf.iojbl.cn

C#:   base.Greet();
来源：http://qnv.yj202588.top

[G08] 静态方法与属性
来源：http://sxk.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ejh.yanxiufei.cn

PHP:  public static function f() {}
来源：http://mvw.yfazqb.com

JS:   static f() {}
来源：http://yvi.hnqzz.top

TS:   static f(): void {}
来源：http://pim.chenzaomai.com

Java: static void f() {}
来源：http://egw.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oyh.hywenlv.cn

Ruby: def self.f; end
来源：http://vcy.ctjpmb.com

C#:   public static void F() {}
来源：http://jrr.bjfxy.top

[G09] 接口 / 抽象类
来源：http://xvs.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://jcz.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iso.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jnn.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://elp.ydzc1.top

Java: interface Shape { double area(); }
来源：http://vul.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://xuc.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blr.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://hzk.gogol.net.cn

[G10] 访问控制
来源：http://glp.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://qre.chenzaomai.com

PHP:  public / protected / private
来源：http://tpi.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://rcb.yongpay.top

TS:   public / protected / private
来源：http://icq.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://fxj.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ynj.jyoumei.cn

Ruby: public / protected / private
来源：http://ovi.xinyue.icu

C#:   public / protected / private / internal
来源：http://mke.xuanzx.com

[G11] getter / setter
来源：http://rwo.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://gzn.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hti.iojbl.cn

JS:   get name() { return this._name; }
来源：http://qsr.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://olj.hammf.cn

Java: public String getName() { return name; }
来源：http://zfd.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ilp.tanke756.top

Ruby: attr_accessor :name
来源：http://rol.yj202588.top

C#:   public string Name { get; set; }
来源：http://gid.jianghu66.top

[G12] 对象转字符串
来源：http://rcg.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://ysk.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nlb.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://hhi.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://dfa.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://slz.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yjz.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://gmo.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://anz.aibaodan.cn

[G13] 判断对象类型
来源：http://jyt.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://cjm.nanxinkj.top

PHP:  $u instanceof User
来源：http://iqk.shangyingyoupin.top

JS:   u instanceof User
来源：http://zot.yongpay.top

TS:   u instanceof User
来源：http://vhn.zhaomingkeji.xyz

Java: u instanceof User
来源：http://xgg.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cfm.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://yst.yangfankeji.com

C#:   u is User
来源：http://pwd.sjlbkw.cn

[G14] 数据类 / record
来源：http://aiz.hysaishi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jcq.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://lkk.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://cxs.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://scl.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://tbb.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://rpr.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kdc.sweek.top

C#:   record User(string Name, int Age);
来源：http://lpi.havefunace.top

[G15] 枚举
来源：http://gvo.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pxa.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nhj.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wdr.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hjl.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://ejb.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dze.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://vqk.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oer.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://tph.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pnc.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://ntr.guannengcc.top

JS:   Object.entries(obj)
来源：http://ouw.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://xct.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qso.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pnz.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://fbb.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://znm.redwolf501.top

================================================================================
来源：http://yxd.c1oappe.top

H. 异常与错误处理
来源：http://xzp.hfpthk.cn

================================================================================
来源：http://ckx.epnwcf.com

[H01] try / catch 基础
来源：http://rid.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rid.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rld.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kau.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://izk.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vcb.yangfankeji.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dft.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://our.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qmn.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://wol.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://xyo.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zty.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xxs.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://ris.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://wkz.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tbw.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yzp.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://enn.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://rrb.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://jtr.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sum.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://nti.birdmap.top

TS:   throw new Error("错误信息");
来源：http://hbp.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://emc.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uco.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://zqs.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://egm.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://fea.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://ffh.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://npl.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://cwh.ivvv.top

TS:   class MyError extends Error {}
来源：http://uvs.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://kyq.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gou.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://mtw.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://vof.yuxming.cn

[H05] 捕获特定类型
来源：http://spz.yj20258.top

Py:   except ValueError as e:
来源：http://vjh.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ttb.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://zxh.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://zuj.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://lua.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ahb.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://wyt.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fln.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://lbg.sysykeji.top

Py:   value = d.get("k") or default
来源：http://myl.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jzs.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://gjk.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://kzx.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lof.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fhg.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://jas.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://vuo.shanyushiyangkeji.top

[H07] 断言
来源：http://wci.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://brd.chenzaomai.com

PHP:  assert($x > 0);
来源：http://zoy.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://ose.smart0.xyz

TS:   console.assert(x > 0);
来源：http://bvn.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://gyq.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aak.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ujo.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://tee.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://uuu.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://vit.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ehj.yuanzhike.top

JS:   e.message;  e.stack
来源：http://dxq.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://emm.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pdi.cheryme.top

Go:   err.Error()
来源：http://cir.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://toi.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://mgw.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://uwv.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tbg.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://izw.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://knj.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hxo.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wzr.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uro.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ywq.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rbn.uphjek.com

[H10] 资源自动释放
来源：http://tsw.redwolf501.top


<!-- 参考信息 -->