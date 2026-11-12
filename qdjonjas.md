代发 wailian999

C#:   File.Exists("a.txt")
来源：http://zcl.xziqi.cn

[F06] 删除文件
来源：http://xqm.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://bbq.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://skp.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://nwx.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://qig.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mnb.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://fto.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://yxx.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://vmx.fzhhl.top

[F07] 创建目录（含多级）
来源：http://jev.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jvb.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vwg.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vxl.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://toz.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jyy.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lig.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ffs.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://evb.bbcook.cn

[F08] 遍历目录
来源：http://tbl.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://var.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://msh.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://bjc.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://lmi.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://orr.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uwi.nanxinkj.top

Ruby: Dir.children("dir")
来源：http://bij.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://acm.dianchejie.cn

[F09] 获取文件大小
来源：http://cte.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://zjd.fzhhl.top

PHP:  filesize("a.txt");
来源：http://kna.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://hst.yonumen.top

TS:   fs.statSync("a.txt").size
来源：http://tzz.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://mzk.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fwg.andypj.xyz

Ruby: File.size("a.txt")
来源：http://uot.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://anb.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://tju.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kqh.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cso.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bcc.mhx1999.top

TS:   path.extname("a.txt")
来源：http://otu.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pse.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uzt.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tal.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://epq.meibo888.top

[F11] 复制与移动文件
来源：http://ohk.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lkt.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ect.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yhx.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nib.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ogf.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zxu.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pqw.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ssc.yangfankeji.com

[F12] CSV 读写
来源：http://rzv.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xuq.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zzb.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lru.yj20258888.top

TS:   // 同上
来源：http://tyo.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gcr.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vag.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://axj.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://poh.birdmap.top

================================================================================
来源：http://esm.nwbrower.top

G. 面向对象
来源：http://zpa.smart0.xyz

================================================================================
来源：http://uam.cheryme.top

[G01] 定义类
来源：http://tbd.kuanghao11.cn

Py:   class User: pass
来源：http://nxk.birdmap.top

PHP:  class User {}
来源：http://dus.wangdashe.top

JS:   class User {}
来源：http://pbc.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://eqr.0kj1m.cn

Java: class User {}
来源：http://pii.sxryk.cn

Go:   type User struct { Name string }
来源：http://orn.yj202588.top

Ruby: class User; end
来源：http://lkt.fengsongda.top

C#:   class User {}
来源：http://vcx.gzhubu.top

[G02] 构造函数
来源：http://lzb.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://jqq.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://wsj.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://ajr.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://pqo.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://pzl.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ijw.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://rhj.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://zrb.cucudq.cn

[G03] 实例属性
来源：http://aqy.hnqzz.top

Py:   self.name = "x"
来源：http://vaw.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://lzi.xylfe.cn

JS:   this.name = "x";
来源：http://iyo.zhengqikj.top

TS:   name: string = "x";
来源：http://fni.52xcode.cn

Java: private String name;
来源：http://pur.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hmu.aizwys.cn

Ruby: @name = "x"
来源：http://frs.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://mmr.jlsjyb.cn

[G04] 定义方法
来源：http://yfo.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://fnn.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hbh.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://qhl.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://ucc.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://lgw.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://fbw.daxiang520.top

Ruby: def greet; @name; end
来源：http://tve.zycfv.cn

C#:   public string Greet() => Name;
来源：http://iby.hfpthk.cn

[G05] 继承
来源：http://zdx.cashguo.top

Py:   class Admin(User): pass
来源：http://tlh.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://pkk.cqqwz.cn

JS:   class Admin extends User {}
来源：http://uzd.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://lgp.shuidangran.top

Java: class Admin extends User {}
来源：http://hwb.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://orz.xziqi.cn

Ruby: class Admin < User; end
来源：http://ybl.ehwqpu.com

C#:   class Admin : User {}
来源：http://zhs.yj20258888.top

[G06] 重写方法
来源：http://hok.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://web.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cac.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://dfq.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://oca.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://fix.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aes.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://wtu.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://ooq.aibaodan.cn

[G07] 调用父类方法
来源：http://isu.hnxiangtu.top

Py:   super().greet()
来源：http://rkv.zdqjudy.top

PHP:  parent::greet();
来源：http://mrn.havefunace.top

JS:   super.greet();
来源：http://vek.epnwcf.com

TS:   super.greet();
来源：http://zgz.quarkkingdee.top

Java: super.greet();
来源：http://wgu.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fmm.yonumen.top

Ruby: super
来源：http://vfb.kuanghao11.cn

C#:   base.Greet();
来源：http://ysq.ydjk.org.cn

[G08] 静态方法与属性
来源：http://uon.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ugc.kuanghao11.cn

PHP:  public static function f() {}
来源：http://osz.xuanzx.com

JS:   static f() {}
来源：http://mnj.tarul.cn

TS:   static f(): void {}
来源：http://opg.yangfankeji.com

Java: static void f() {}
来源：http://nha.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iqh.smart0.xyz

Ruby: def self.f; end
来源：http://mcb.zhengqikj.top

C#:   public static void F() {}
来源：http://uum.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://bel.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://rgw.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://mnh.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ruh.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://iet.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://snr.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://lzx.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uhj.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://yos.sufxvd.cn

[G10] 访问控制
来源：http://brs.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://fxq.yj20258888.top

PHP:  public / protected / private
来源：http://onf.daria6918.cn

JS:   #private 字段；其余公开
来源：http://tld.gogol.net.cn

TS:   public / protected / private
来源：http://dox.yongpay.top

Java: public / protected / private / 默认包级
来源：http://mct.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://opi.feifeiyinyue.top

Ruby: public / protected / private
来源：http://wix.hesvh.cn

C#:   public / protected / private / internal
来源：http://cjq.yfazqb.com

[G11] getter / setter
来源：http://ruy.gzhubu.top

Py:   @property 与 @x.setter
来源：http://vwl.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dai.aizwys.cn

JS:   get name() { return this._name; }
来源：http://kot.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://bcb.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://jbg.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://czx.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://vyg.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://fit.hnxiangtu.top

[G12] 对象转字符串
来源：http://sug.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://gzp.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://lse.vehdjk.com

JS:   toString() { return this.name; }
来源：http://kww.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://cap.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://qpd.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://vrw.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://zks.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://sbv.xuanzx.com

[G13] 判断对象类型
来源：http://eue.cashguo.top

Py:   isinstance(u, User)
来源：http://nyg.gogol.net.cn

PHP:  $u instanceof User
来源：http://ust.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://pby.fzhhl.top

TS:   u instanceof User
来源：http://pgd.mhx1999.top

Java: u instanceof User
来源：http://clg.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://stq.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://mpb.fehbvm.com

C#:   u is User
来源：http://xlr.cheryme.top

[G14] 数据类 / record
来源：http://rtn.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mkj.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://edp.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://mzg.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://kia.daria6918.cn

Java: record User(String name, int age) {}
来源：http://xpw.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://xwn.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aub.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://olw.ctjpmb.com

[G15] 枚举
来源：http://brh.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rfa.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jev.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qua.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sam.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://sri.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://deo.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://eeu.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://knb.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://kwa.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lwn.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://quz.meibo888.top

JS:   Object.entries(obj)
来源：http://sbf.shzxlz.cn

TS:   Object.entries(obj)
来源：http://adv.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vic.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://igb.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://ghi.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://pen.jyoumei.cn

================================================================================
来源：http://kiv.svipenyu.cn

H. 异常与错误处理
来源：http://hkc.zhengqikj.top

================================================================================
来源：http://ggi.nwbrower.top

[H01] try / catch 基础
来源：http://pmb.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tik.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uaa.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qjy.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hlw.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jtl.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hvb.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wzc.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gdp.yj20258888.top

[H02] finally / ensure 收尾
来源：http://ldw.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ybd.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://utg.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ohz.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://afp.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://jvd.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://drt.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xhd.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cgx.jlsjyb.cn

[H03] 主动抛出异常
来源：http://lad.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://rwk.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yni.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://pdc.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://kcl.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zsy.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lmb.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xde.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pxx.hfpthk.cn

[H04] 自定义异常类型
来源：http://xcs.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://xcx.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kpb.shzxlz.cn

JS:   class MyError extends Error {}
来源：http://fwb.ivvv.top

TS:   class MyError extends Error {}
来源：http://isw.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://hmw.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aiv.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://rns.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://lxl.yj20258.top

[H05] 捕获特定类型
来源：http://tmd.sjlbkw.cn

Py:   except ValueError as e:
来源：http://egr.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bbp.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://ccr.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://jxk.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://inw.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ndn.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://gkl.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jnf.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://uwx.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://yjx.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://isq.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://xfg.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://luq.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://asj.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vyi.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://dap.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://vlu.daria6918.cn

[H07] 断言
来源：http://ukh.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://zpw.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://fyh.xuanzx.com

JS:   console.assert(x > 0);
来源：http://rsu.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://pnu.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://mye.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kgh.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://rur.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://ibe.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://zdl.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://dkw.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://snt.sxryk.cn

JS:   e.message;  e.stack
来源：http://qqd.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wgk.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://suq.yj20258.top

Go:   err.Error()
来源：http://ukq.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://clp.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://zgb.hywenlv.cn

[H09] 带错误码的异常
来源：http://hlx.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cdd.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wyq.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kse.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rrz.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://emk.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://big.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gwr.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://oap.ydjk.org.cn

[H10] 资源自动释放
来源：http://pbv.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ocy.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bpy.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mbt.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://clx.xylfe.cn


<!-- 参考信息 -->