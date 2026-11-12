代发 wailian999

C#:   File.Exists("a.txt")
来源：http://dmf.chenlongwang.top

[F06] 删除文件
来源：http://rob.guannengcc.top

Py:   os.remove("a.txt")
来源：http://qwh.xylfe.cn

PHP:  unlink("a.txt");
来源：http://evl.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://stb.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xxb.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://twu.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://fxi.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://evf.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://fyf.yj202588.top

[F07] 创建目录（含多级）
来源：http://rrv.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fhf.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bon.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yhj.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://djd.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dra.ppjwa.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ppr.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bwz.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sum.andypj.xyz

[F08] 遍历目录
来源：http://nxo.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rrm.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xyj.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://odo.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://dwi.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dkd.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fcz.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://ffd.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://nyt.52xcode.cn

[F09] 获取文件大小
来源：http://xun.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://fmu.tarul.cn

PHP:  filesize("a.txt");
来源：http://pzq.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://pnu.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://kam.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://bxf.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xdx.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://kkh.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://eko.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://xyb.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qfz.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jzb.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tcl.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://jwf.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://izf.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xki.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ebq.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mjy.nanxinkj.top

[F11] 复制与移动文件
来源：http://mom.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tgr.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qwt.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jet.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://brc.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xmk.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ojo.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://orz.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uxv.xuetiantiany.cn

[F12] CSV 读写
来源：http://mly.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kqq.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mrj.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ghd.svipenyu.cn

TS:   // 同上
来源：http://qgi.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://upl.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dkc.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fyr.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://fho.zycfv.cn

================================================================================
来源：http://mrz.yongpay.top

G. 面向对象
来源：http://jdj.ydzc1.top

================================================================================
来源：http://dwg.sweek.top

[G01] 定义类
来源：http://rof.gotoacloud.top

Py:   class User: pass
来源：http://glk.ppjwa.cn

PHP:  class User {}
来源：http://pkh.sufxvd.cn

JS:   class User {}
来源：http://ein.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://ahv.sjlbkw.cn

Java: class User {}
来源：http://wog.tian-w.cn

Go:   type User struct { Name string }
来源：http://bll.ydzc1.top

Ruby: class User; end
来源：http://gxn.nwbrower.top

C#:   class User {}
来源：http://twd.yfazqb.com

[G02] 构造函数
来源：http://czs.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://hjv.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://nvf.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://kxc.cheryme.top

TS:   constructor(public name: string) {}
来源：http://jhk.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://wuw.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hnq.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://jkm.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://vtm.redwolf501.top

[G03] 实例属性
来源：http://ams.9152youxi.cn

Py:   self.name = "x"
来源：http://pqr.hesvh.cn

PHP:  public string $name = "x";
来源：http://nag.jyoumei.cn

JS:   this.name = "x";
来源：http://aul.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://xbx.316326.xyz

Java: private String name;
来源：http://tcw.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jzb.feifeiyinyue.top

Ruby: @name = "x"
来源：http://ase.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://wmy.316326.xyz

[G04] 定义方法
来源：http://esw.meibo888.top

Py:   def greet(self): return self.name
来源：http://abj.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pdg.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://kkz.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://ckz.ppjwa.cn

Java: String greet() { return name; }
来源：http://lfq.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hvc.cucudq.cn

Ruby: def greet; @name; end
来源：http://ouo.redwolf501.top

C#:   public string Greet() => Name;
来源：http://ohi.jinghuilouyu.cn

[G05] 继承
来源：http://snd.yj20258888.top

Py:   class Admin(User): pass
来源：http://hhw.jianghu66.top

PHP:  class Admin extends User {}
来源：http://thi.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://yjv.mhx1999.top

TS:   class Admin extends User {}
来源：http://mfw.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://wdr.cucudq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fpb.c1oappe.top

Ruby: class Admin < User; end
来源：http://rin.sufxvd.cn

C#:   class Admin : User {}
来源：http://bgm.bbcook.cn

[G06] 重写方法
来源：http://jgb.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://gpg.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://czw.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://oqr.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://eda.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://uta.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wgi.yonumen.top

Ruby: def greet; "admin"; end
来源：http://rdl.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://erp.jinqigufen.top

[G07] 调用父类方法
来源：http://nwp.hongshengwenyu.top

Py:   super().greet()
来源：http://tbh.gaohongyu789.top

PHP:  parent::greet();
来源：http://kxv.guannengcc.top

JS:   super.greet();
来源：http://cjs.hfpthk.cn

TS:   super.greet();
来源：http://zux.jinyuanbaomall.cn

Java: super.greet();
来源：http://orc.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dhb.jinqigufen.top

Ruby: super
来源：http://ljr.kuanghao11.cn

C#:   base.Greet();
来源：http://rfh.dashuyun.cn

[G08] 静态方法与属性
来源：http://fzl.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xzq.wangdashe.top

PHP:  public static function f() {}
来源：http://tkf.smart0.xyz

JS:   static f() {}
来源：http://dlf.tianlin.xyz

TS:   static f(): void {}
来源：http://pfn.bjfxy.top

Java: static void f() {}
来源：http://exm.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ijr.xinyue.icu

Ruby: def self.f; end
来源：http://ufz.cdnleiting.top

C#:   public static void F() {}
来源：http://ecu.meibo888.top

[G09] 接口 / 抽象类
来源：http://zwt.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://kvy.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://twf.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vzg.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://idq.uphjek.com

Java: interface Shape { double area(); }
来源：http://qsc.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://roy.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://unh.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://rup.hammf.cn

[G10] 访问控制
来源：http://ioy.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://ncq.havefunace.top

PHP:  public / protected / private
来源：http://ndz.epnwcf.com

JS:   #private 字段；其余公开
来源：http://bwn.zhoulong.xyz

TS:   public / protected / private
来源：http://gik.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://lfj.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hab.mhx1999.top

Ruby: public / protected / private
来源：http://cet.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://eip.sxryk.cn

[G11] getter / setter
来源：http://rdd.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://srj.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://fql.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://acd.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://xnu.316326.xyz

Java: public String getName() { return name; }
来源：http://aph.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pzd.yongpay.top

Ruby: attr_accessor :name
来源：http://cei.jqgufenzy.top

C#:   public string Name { get; set; }
来源：http://eyq.shangyingyoupin.top

[G12] 对象转字符串
来源：http://mji.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://lna.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dbw.havefunace.top

JS:   toString() { return this.name; }
来源：http://tpm.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://mzi.yangfankeji.com

Java: @Override public String toString() { return name; }
来源：http://jhh.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uts.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://top.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://wyh.cucudq.cn

[G13] 判断对象类型
来源：http://mrr.xinyue.icu

Py:   isinstance(u, User)
来源：http://esl.fktsv.cn

PHP:  $u instanceof User
来源：http://uoh.yfazqb.com

JS:   u instanceof User
来源：http://wcf.kuanghao11.cn

TS:   u instanceof User
来源：http://ppg.cheryme.top

Java: u instanceof User
来源：http://nma.havefunace.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://amg.tian-w.cn

Ruby: u.is_a?(User)
来源：http://ams.birdmap.top

C#:   u is User
来源：http://uvu.yfazqb.com

[G14] 数据类 / record
来源：http://xzq.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mpw.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://cvr.uphjek.com

JS:   // 无内置：普通类或对象字面量
来源：http://gmf.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://vcf.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://dyq.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://cjc.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fsj.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://gpp.yj20258888.top

[G15] 枚举
来源：http://ieq.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ppj.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oen.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cvr.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wlr.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://zla.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zmx.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://ltl.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fef.tanke756.top

[G16] 对象转数组 / 字典
来源：http://hyu.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nli.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://wgc.ivvv.top

JS:   Object.entries(obj)
来源：http://mlg.9152youxi.cn

TS:   Object.entries(obj)
来源：http://jtu.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yvp.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://msg.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://zli.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://tkv.shanyushiyangkeji.top

================================================================================
来源：http://hrc.xuetiantiany.cn

H. 异常与错误处理
来源：http://hga.tian-w.cn

================================================================================
来源：http://gac.redwolf501.top

[H01] try / catch 基础
来源：http://nkp.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jho.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ayq.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lgo.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://scb.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sys.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hlp.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ysh.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dnz.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://wmj.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nxy.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nkb.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kjf.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fyf.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ezj.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://nya.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://iph.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lri.hnqzz.top

[H03] 主动抛出异常
来源：http://gyu.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://udm.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pkl.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://pwa.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://frs.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hbq.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fey.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ful.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://bkg.gotoacloud.top

[H04] 自定义异常类型
来源：http://dbb.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://zlf.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://mts.redwolf501.top

JS:   class MyError extends Error {}
来源：http://abr.zycfv.cn

TS:   class MyError extends Error {}
来源：http://pih.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://mrm.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yet.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://zlz.yvedp.cn

C#:   class MyException : Exception {}
来源：http://beh.sufxvd.cn

[H05] 捕获特定类型
来源：http://zwm.iojbl.cn

Py:   except ValueError as e:
来源：http://opk.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nsm.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://mcc.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://ihz.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://zdg.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://meb.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://psv.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dlz.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://fgx.yj202588.top

Py:   value = d.get("k") or default
来源：http://pyo.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://pco.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nki.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xju.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zkm.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aro.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://htc.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://ukb.guowangkeji.top

[H07] 断言
来源：http://qgk.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://lsf.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://ica.nwbrower.top

JS:   console.assert(x > 0);
来源：http://buc.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://mxv.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://dps.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ebu.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://ory.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://iyn.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://jda.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://sqw.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://atx.cqqwz.cn

JS:   e.message;  e.stack
来源：http://gqs.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hqd.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pkr.sjlbkw.cn

Go:   err.Error()
来源：http://zuv.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://ily.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://nvj.fzhhl.top

[H09] 带错误码的异常
来源：http://owd.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jgu.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://njo.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wis.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://prv.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zjw.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gfr.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ajg.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://krw.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://yqk.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rub.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fnv.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hwx.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uku.dianchejie.cn


<!-- 参考信息 -->