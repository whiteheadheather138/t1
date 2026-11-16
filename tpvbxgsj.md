代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://was.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hty.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://foa.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://aqn.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://ykz.fzhhl.top

[F06] 删除文件
来源：http://mwc.tanke756.top

Py:   os.remove("a.txt")
来源：http://fki.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://oym.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://bik.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://mva.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jht.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://sya.cheryme.top

Ruby: File.delete("a.txt")
来源：http://hdd.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://ygq.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://bed.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qxd.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ost.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aph.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://szd.yangfankeji.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ptr.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mtj.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tjk.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qjr.ctjpmb.com

[F08] 遍历目录
来源：http://hsb.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kvf.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://twv.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://tob.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://yeo.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fsz.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://sec.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://rjx.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://pkg.cdnleiting.top

[F09] 获取文件大小
来源：http://syj.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://qzz.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://rra.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://xne.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://afp.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://eln.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cii.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://ggh.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://plu.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://cub.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qbp.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tjs.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wtd.pycfn.com

TS:   path.extname("a.txt")
来源：http://rna.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sfk.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mug.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nhm.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yzj.aibaodan.cn

[F11] 复制与移动文件
来源：http://gsu.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xxr.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://djd.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bhl.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dwb.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uyx.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jmc.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vau.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fwb.zycfv.cn

[F12] CSV 读写
来源：http://rac.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pdp.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tlw.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://woy.nanxinkj.top

TS:   // 同上
来源：http://ohe.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tng.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ian.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bll.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bpt.fktsv.cn

================================================================================
来源：http://lld.xuanzx.com

G. 面向对象
来源：http://hiw.yuxming.cn

================================================================================
来源：http://tsw.jqgfzy.top

[G01] 定义类
来源：http://csv.hysaishi.cn

Py:   class User: pass
来源：http://tzw.c1oappe.top

PHP:  class User {}
来源：http://dgx.c1oappe.top

JS:   class User {}
来源：http://koy.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://nob.gaohongyu789.top

Java: class User {}
来源：http://gvz.daria6918.cn

Go:   type User struct { Name string }
来源：http://mch.hongshengwenyu.top

Ruby: class User; end
来源：http://kca.fktsv.cn

C#:   class User {}
来源：http://zpw.ctjpmb.com

[G02] 构造函数
来源：http://xud.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://kul.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://yfa.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://mme.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://ltu.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://zwr.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pgf.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://sfn.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://wvt.jianghu66.top

[G03] 实例属性
来源：http://ryi.cucudq.cn

Py:   self.name = "x"
来源：http://qzl.ppjwa.cn

PHP:  public string $name = "x";
来源：http://ljp.gotoacloud.top

JS:   this.name = "x";
来源：http://rvc.yfazqb.com

TS:   name: string = "x";
来源：http://nml.ydzc1.top

Java: private String name;
来源：http://dhl.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iei.shuidangran.top

Ruby: @name = "x"
来源：http://wzz.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://edw.hysaishi.cn

[G04] 定义方法
来源：http://lmo.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://gsu.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://aif.hesvh.cn

JS:   greet() { return this.name; }
来源：http://uvx.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://hga.nwbrower.top

Java: String greet() { return name; }
来源：http://mvd.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yaw.52xcode.cn

Ruby: def greet; @name; end
来源：http://jvs.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://mjm.guowangkeji.top

[G05] 继承
来源：http://xla.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://wib.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://fsc.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://zbm.pycfn.com

TS:   class Admin extends User {}
来源：http://mpc.ppjwa.cn

Java: class Admin extends User {}
来源：http://sjb.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kpu.hywenlv.cn

Ruby: class Admin < User; end
来源：http://jcw.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://wsd.gogol.net.cn

[G06] 重写方法
来源：http://yie.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://fxq.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://kcu.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://tsm.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://jxq.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://svi.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vsj.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://jic.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://dvq.yfazqb.com

[G07] 调用父类方法
来源：http://rwg.guowangkeji.top

Py:   super().greet()
来源：http://gdp.9152youxi.cn

PHP:  parent::greet();
来源：http://svg.chenjidiqi.icu

JS:   super.greet();
来源：http://kbk.316326.xyz

TS:   super.greet();
来源：http://onn.jyoumei.cn

Java: super.greet();
来源：http://kqi.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vkr.smart0.xyz

Ruby: super
来源：http://orf.hongshengwenyu.top

C#:   base.Greet();
来源：http://amc.cqqwz.cn

[G08] 静态方法与属性
来源：http://naf.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mqz.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://fgc.yuxming.cn

JS:   static f() {}
来源：http://mlo.sufxvd.cn

TS:   static f(): void {}
来源：http://jga.ywan-chungtsiang.top

Java: static void f() {}
来源：http://bcl.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sec.sufxvd.cn

Ruby: def self.f; end
来源：http://zpa.yanxiufei.cn

C#:   public static void F() {}
来源：http://inx.52xcode.cn

[G09] 接口 / 抽象类
来源：http://awd.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://opq.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://mvo.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uht.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://mqw.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://veh.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://aue.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ojo.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://xtm.cucudq.cn

[G10] 访问控制
来源：http://bob.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://xqd.hcnkem.com

PHP:  public / protected / private
来源：http://obk.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://hnu.zdqjudy.top

TS:   public / protected / private
来源：http://rgx.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://aua.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://beh.xylfe.cn

Ruby: public / protected / private
来源：http://fiu.haohaochexian.top

C#:   public / protected / private / internal
来源：http://bho.quarkkingdee.top

[G11] getter / setter
来源：http://dzd.uphjek.com

Py:   @property 与 @x.setter
来源：http://ppg.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dbm.daxiang520.top

JS:   get name() { return this._name; }
来源：http://bns.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://ahx.sxryk.cn

Java: public String getName() { return name; }
来源：http://nel.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://umh.sxryk.cn

Ruby: attr_accessor :name
来源：http://xqb.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://php.c1oappe.top

[G12] 对象转字符串
来源：http://rqv.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://unl.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lmm.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://utv.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://ryw.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://etr.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://dhc.fktsv.cn

Ruby: def to_s; @name; end
来源：http://rpr.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://qhi.andypj.xyz

[G13] 判断对象类型
来源：http://ncz.yueranfly.top

Py:   isinstance(u, User)
来源：http://zwk.cashguo.top

PHP:  $u instanceof User
来源：http://bmi.zhongyouzk.top

JS:   u instanceof User
来源：http://ssz.vehdjk.com

TS:   u instanceof User
来源：http://rgg.hongshengwenyu.top

Java: u instanceof User
来源：http://yau.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pas.redwolf501.top

Ruby: u.is_a?(User)
来源：http://brj.chenjidiqi.icu

C#:   u is User
来源：http://sid.tian-w.cn

[G14] 数据类 / record
来源：http://wjw.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mod.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://pxh.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://pzw.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://dzp.sxryk.cn

Java: record User(String name, int age) {}
来源：http://mtn.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://pqd.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mug.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://ibd.chenjidiqi.icu

[G15] 枚举
来源：http://cag.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ezc.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ibz.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ylb.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://trq.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://sgb.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qeo.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://chk.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ncx.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://pcs.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tvx.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://ygz.redwolf501.top

JS:   Object.entries(obj)
来源：http://qmn.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://vmr.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vgk.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ktc.c1oappe.top

Ruby: obj.instance_variables
来源：http://cpl.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://gzx.jinqigfzy.top

================================================================================
来源：http://frn.yonumen.top

H. 异常与错误处理
来源：http://cld.jinyuanbaomall.cn

================================================================================
来源：http://cnp.jinqigfzy.top

[H01] try / catch 基础
来源：http://ngl.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zrq.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ely.jiagoushi.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ent.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sqs.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jqp.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dbl.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hzv.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ban.ivvv.top

[H02] finally / ensure 收尾
来源：http://gdx.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://hbc.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://war.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bgn.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xax.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://iod.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ona.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pcu.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sha.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://jtr.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://trs.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nwb.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://bai.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://rjx.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://azv.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eng.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qpa.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://cjt.fengsongda.top

[H04] 自定义异常类型
来源：http://fyo.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://hob.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rmi.52xcode.cn

JS:   class MyError extends Error {}
来源：http://frl.52xcode.cn

TS:   class MyError extends Error {}
来源：http://lgr.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://ikb.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qnq.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://rkc.yvedp.cn

C#:   class MyException : Exception {}
来源：http://lim.shuidangran.top

[H05] 捕获特定类型
来源：http://dld.yanxiufei.cn

Py:   except ValueError as e:
来源：http://bey.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cni.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://udj.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://kdx.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://ybp.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xne.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://rcr.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rpq.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://uen.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://tsp.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://ndu.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xxz.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://vin.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://unb.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://szp.shangyingyoupin.top

Ruby: d&.dig(:a, :b)
来源：http://six.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://sxy.jiagoushi.top

[H07] 断言
来源：http://wwv.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://yxf.bbcook.cn

PHP:  assert($x > 0);
来源：http://tnv.hammf.cn

JS:   console.assert(x > 0);
来源：http://pao.yuanzhike.top

TS:   console.assert(x > 0);
来源：http://ntd.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://alg.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kmt.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://sfx.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://ixw.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://xeq.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://zug.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uol.52xcode.cn

JS:   e.message;  e.stack
来源：http://xzt.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vsf.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cwc.zhijiandao.cn

Go:   err.Error()
来源：http://onb.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://ojv.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://rxx.tarul.cn

[H09] 带错误码的异常
来源：http://ozh.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kxn.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jih.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gpp.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bao.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xcz.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gnw.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://tms.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xgw.cheryme.top

[H10] 资源自动释放
来源：http://ezh.nwbrower.top


<!-- 参考信息 -->