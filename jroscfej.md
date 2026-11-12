代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hch.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://lya.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zle.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://kcb.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://dmc.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://api.fktsv.cn

[F07] 创建目录（含多级）
来源：http://ivc.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vrs.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bnt.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://btf.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xid.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dqr.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://szl.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jlo.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://byt.gogol.net.cn

[F08] 遍历目录
来源：http://eaj.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dom.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bjy.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://jku.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://bmv.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://osr.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vpz.yj20258.top

Ruby: Dir.children("dir")
来源：http://vsh.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://uov.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://rqd.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://aho.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://fik.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://caf.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://edv.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://zuv.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oaq.shuidangran.top

Ruby: File.size("a.txt")
来源：http://src.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://mma.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://fuh.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sks.feifeiyinyue.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mpd.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bht.bbcook.cn

TS:   path.extname("a.txt")
来源：http://fqy.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kjt.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://scf.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xav.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pff.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://ves.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iab.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nir.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://isl.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nan.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://inu.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ksz.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://alm.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lvk.tanke756.top

[F12] CSV 读写
来源：http://etj.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qge.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mht.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nce.gogol.net.cn

TS:   // 同上
来源：http://xxt.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rdh.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ivs.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kld.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://vqa.bbcook.cn

================================================================================
来源：http://ena.jlsjyb.cn

G. 面向对象
来源：http://ksy.316326.xyz

================================================================================
来源：http://gkl.hysaishi.cn

[G01] 定义类
来源：http://rfo.birdmap.top

Py:   class User: pass
来源：http://plv.gzhubu.top

PHP:  class User {}
来源：http://paa.bbcook.cn

JS:   class User {}
来源：http://yqu.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://ooe.ppjwa.cn

Java: class User {}
来源：http://ghf.jqgfzy.top

Go:   type User struct { Name string }
来源：http://ktk.pycfn.com

Ruby: class User; end
来源：http://unh.shangyingyoupin.top

C#:   class User {}
来源：http://jxi.shanyushiyangkeji.top

[G02] 构造函数
来源：http://msb.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://zip.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://xhq.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://cuh.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://psp.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://tgr.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rkv.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://oqd.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://gbi.cqqwz.cn

[G03] 实例属性
来源：http://qtz.yuxming.cn

Py:   self.name = "x"
来源：http://htp.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://pmt.iojbl.cn

JS:   this.name = "x";
来源：http://kxf.fktsv.cn

TS:   name: string = "x";
来源：http://fgm.fanxiaobao.xyz

Java: private String name;
来源：http://xqc.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cpa.zdbjq.cn

Ruby: @name = "x"
来源：http://roc.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://znp.gzhubu.top

[G04] 定义方法
来源：http://xyg.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://yzl.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wgv.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://vdd.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://hvp.9152youxi.cn

Java: String greet() { return name; }
来源：http://dbe.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aup.ivvv.top

Ruby: def greet; @name; end
来源：http://zff.sysykeji.top

C#:   public string Greet() => Name;
来源：http://sse.ydjk.org.cn

[G05] 继承
来源：http://ipb.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://yuc.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://zbo.yuxming.cn

JS:   class Admin extends User {}
来源：http://mln.smart0.xyz

TS:   class Admin extends User {}
来源：http://hae.tarul.cn

Java: class Admin extends User {}
来源：http://lta.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://egx.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://sja.xylfe.cn

C#:   class Admin : User {}
来源：http://dik.hnxiangtu.top

[G06] 重写方法
来源：http://oee.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://vti.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lbv.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://gov.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://qfu.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://caj.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kkj.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://ogm.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://wja.daria6918.cn

[G07] 调用父类方法
来源：http://ihx.xziqi.cn

Py:   super().greet()
来源：http://jph.hnxiangtu.top

PHP:  parent::greet();
来源：http://put.nwbrower.top

JS:   super.greet();
来源：http://psq.gaohongyu789.top

TS:   super.greet();
来源：http://tev.tian-w.cn

Java: super.greet();
来源：http://rya.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ybm.zhongyouzk.top

Ruby: super
来源：http://hqk.xziqi.cn

C#:   base.Greet();
来源：http://keu.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://akl.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nsc.jinqigfzy.top

PHP:  public static function f() {}
来源：http://gaz.jlsjyb.cn

JS:   static f() {}
来源：http://bme.52xcode.cn

TS:   static f(): void {}
来源：http://ygp.haohaochexian.top

Java: static void f() {}
来源：http://ttg.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://mpo.ivvv.top

Ruby: def self.f; end
来源：http://lup.hfpthk.cn

C#:   public static void F() {}
来源：http://pad.fktsv.cn

[G09] 接口 / 抽象类
来源：http://vlz.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://jps.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://inx.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fhx.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://sqc.bbcook.cn

Java: interface Shape { double area(); }
来源：http://jgf.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://alu.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bfo.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://cci.fehbvm.com

[G10] 访问控制
来源：http://gni.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://olb.zdqjudy.top

PHP:  public / protected / private
来源：http://ufb.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://ycm.hywenlv.cn

TS:   public / protected / private
来源：http://fqd.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://yav.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ytn.quarkkingdee.top

Ruby: public / protected / private
来源：http://doo.ydzc1.top

C#:   public / protected / private / internal
来源：http://ytk.zhiwuduotai.top

[G11] getter / setter
来源：http://uwu.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://phv.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jfh.mhx1999.top

JS:   get name() { return this._name; }
来源：http://mli.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://tvu.mhx1999.top

Java: public String getName() { return name; }
来源：http://iqn.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ahh.jiagoushi.top

Ruby: attr_accessor :name
来源：http://dff.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://fhs.uphjek.com

[G12] 对象转字符串
来源：http://xrj.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://sdh.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://qom.fehbvm.com

JS:   toString() { return this.name; }
来源：http://blv.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://jtr.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://zbk.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ydy.fehbvm.com

Ruby: def to_s; @name; end
来源：http://fkf.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://soz.cheryme.top

[G13] 判断对象类型
来源：http://zdb.yueranfly.top

Py:   isinstance(u, User)
来源：http://rps.yj202588.top

PHP:  $u instanceof User
来源：http://ury.yfazqb.com

JS:   u instanceof User
来源：http://rgt.nanxinkj.top

TS:   u instanceof User
来源：http://xuq.birdmap.top

Java: u instanceof User
来源：http://zap.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://afh.fengsongda.top

Ruby: u.is_a?(User)
来源：http://ahl.yanxiufei.cn

C#:   u is User
来源：http://mtj.yonumen.top

[G14] 数据类 / record
来源：http://ggm.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zwg.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://mxm.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://dhi.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://mjf.52xcode.cn

Java: record User(String name, int age) {}
来源：http://ksl.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://hhs.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mhs.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://ncj.shuidangran.top

[G15] 枚举
来源：http://hhm.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jwp.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dfc.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qra.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fev.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://dro.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ehe.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://owe.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jye.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://xgx.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kce.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://srm.mhx1999.top

JS:   Object.entries(obj)
来源：http://ucj.cheryme.top

TS:   Object.entries(obj)
来源：http://oqm.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mwp.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gyw.cucudq.cn

Ruby: obj.instance_variables
来源：http://zms.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://aca.gotoacloud.top

================================================================================
来源：http://syi.hysaishi.cn

H. 异常与错误处理
来源：http://wqx.jyoumei.cn

================================================================================
来源：http://vfz.mhx1999.top

[H01] try / catch 基础
来源：http://yri.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://prl.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cne.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pwr.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ubv.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mkz.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ngo.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ues.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cog.tanke756.top

[H02] finally / ensure 收尾
来源：http://qhn.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://akq.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hjq.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bhw.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ztv.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://jaa.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://slw.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xbj.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://hfa.hcnkem.com

[H03] 主动抛出异常
来源：http://wou.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://laj.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yji.birdmap.top

JS:   throw new Error("错误信息");
来源：http://byo.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://ney.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jjw.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mbx.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mwg.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://llo.ivvv.top

[H04] 自定义异常类型
来源：http://upi.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://mrx.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dnr.guannengcc.top

JS:   class MyError extends Error {}
来源：http://vcd.xylfe.cn

TS:   class MyError extends Error {}
来源：http://tiy.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://gzr.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://agi.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://yuh.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://asf.hnqzz.top

[H05] 捕获特定类型
来源：http://chq.aizwys.cn

Py:   except ValueError as e:
来源：http://eqx.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ffa.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://ucq.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://xdd.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://ubr.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cho.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://fpt.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oms.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://yxs.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://iby.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tww.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://gdi.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://jhy.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://opw.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://azo.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://kzr.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://ccu.cdnleiting.top

[H07] 断言
来源：http://tgh.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://ubn.52xcode.cn

PHP:  assert($x > 0);
来源：http://dgd.wangdashe.top

JS:   console.assert(x > 0);
来源：http://qcp.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://svv.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://nlh.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ibl.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://bkx.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://wiv.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://ghp.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://ehg.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://twb.wangdashe.top

JS:   e.message;  e.stack
来源：http://zta.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xbm.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://siv.sysykeji.top

Go:   err.Error()
来源：http://udo.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://ydv.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://ixo.nanxinkj.top

[H09] 带错误码的异常
来源：http://drn.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zti.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hnk.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nfe.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://egz.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qpm.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cmn.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fzb.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gso.fzhhl.top

[H10] 资源自动释放
来源：http://fdp.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rcb.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jir.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gmg.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qxg.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bzs.xuanzx.com

Go:   defer f.Close()
来源：http://dwi.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://isq.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ihb.c1oappe.top


<!-- 参考信息 -->