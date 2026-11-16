代发 wailian999

C#:   File.Exists("a.txt")
来源：http://cuh.pengpengdd.cyou

[F06] 删除文件
来源：http://nju.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://odc.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://mby.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://sto.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://cob.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jjq.meibo888.top

Go:   os.Remove("a.txt")
来源：http://ccq.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://vbg.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://qpu.52xcode.cn

[F07] 创建目录（含多级）
来源：http://dji.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://glb.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nyq.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqd.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhv.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jut.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://brs.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tzr.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mkb.ydzc1.top

[F08] 遍历目录
来源：http://tyn.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://knl.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://swk.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://esl.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://aen.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kcc.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jvf.yj20258.top

Ruby: Dir.children("dir")
来源：http://vly.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://wdj.feifeiyinyue.top

[F09] 获取文件大小
来源：http://lry.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://irl.epnwcf.com

PHP:  filesize("a.txt");
来源：http://wua.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://opt.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://itu.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://edj.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nfr.yfazqb.com

Ruby: File.size("a.txt")
来源：http://wxl.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://eek.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://vxc.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jgv.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pri.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mtf.tian-w.cn

TS:   path.extname("a.txt")
来源：http://phv.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nso.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ygm.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uaw.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xff.yj20258888.top

[F11] 复制与移动文件
来源：http://gta.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wqi.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://trs.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ofs.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gkj.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kvz.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmz.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://shl.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xpx.guowangkeji.top

[F12] CSV 读写
来源：http://kqw.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ubb.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wnl.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ocl.jqgfzy.top

TS:   // 同上
来源：http://owx.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vsx.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rqf.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xmr.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nfc.nanxinkj.top

================================================================================
来源：http://oma.dashuyun.cn

G. 面向对象
来源：http://hnv.dianchejie.cn

================================================================================
来源：http://pvl.dianchejie.cn

[G01] 定义类
来源：http://vbz.yangfankeji.com

Py:   class User: pass
来源：http://tys.nanxuanxn.top

PHP:  class User {}
来源：http://tlv.jinyuanbaomall.cn

JS:   class User {}
来源：http://ofs.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://ihk.hfpthk.cn

Java: class User {}
来源：http://beh.ctjpmb.com

Go:   type User struct { Name string }
来源：http://xpx.zhiwuduotai.top

Ruby: class User; end
来源：http://jjr.xuetiantiany.cn

C#:   class User {}
来源：http://trr.cdnleiting.top

[G02] 构造函数
来源：http://njo.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://obz.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://ytf.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://ogx.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://bxx.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://zyd.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tgt.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://vfg.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://uhg.bbcook.cn

[G03] 实例属性
来源：http://dwb.ehwqpu.com

Py:   self.name = "x"
来源：http://aea.yj202588.top

PHP:  public string $name = "x";
来源：http://gzr.smart0.xyz

JS:   this.name = "x";
来源：http://uqv.xinyue.icu

TS:   name: string = "x";
来源：http://kee.ivvv.top

Java: private String name;
来源：http://wsu.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://swi.dianchejie.cn

Ruby: @name = "x"
来源：http://tee.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://gsd.nwbrower.top

[G04] 定义方法
来源：http://euv.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://dhx.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://wlb.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://wvz.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://xxc.yuxming.cn

Java: String greet() { return name; }
来源：http://cgf.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://huq.yueranfly.top

Ruby: def greet; @name; end
来源：http://lan.wangdashe.top

C#:   public string Greet() => Name;
来源：http://kkk.zhijiandao.cn

[G05] 继承
来源：http://ftz.jinqigufen.top

Py:   class Admin(User): pass
来源：http://ylc.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://def.hcnkem.com

JS:   class Admin extends User {}
来源：http://ogv.yangfankeji.com

TS:   class Admin extends User {}
来源：http://bxw.bbcook.cn

Java: class Admin extends User {}
来源：http://mke.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ilb.0kj1m.cn

Ruby: class Admin < User; end
来源：http://rje.nwbrower.top

C#:   class Admin : User {}
来源：http://ycn.chenzaomai.com

[G06] 重写方法
来源：http://pjj.pycfn.com

Py:   def greet(self): return "admin"
来源：http://xjh.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://soc.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://jxs.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://gyo.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://rgz.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://azu.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://tvf.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://fgn.xuetiantiany.cn

[G07] 调用父类方法
来源：http://gmc.yongpay.top

Py:   super().greet()
来源：http://vvv.hnqzz.top

PHP:  parent::greet();
来源：http://wyt.fengsongda.top

JS:   super.greet();
来源：http://vkh.chenjidiqi.icu

TS:   super.greet();
来源：http://txv.316326.xyz

Java: super.greet();
来源：http://ybf.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cmb.hongshengwenyu.top

Ruby: super
来源：http://ldh.ctjpmb.com

C#:   base.Greet();
来源：http://qyq.ppjwa.cn

[G08] 静态方法与属性
来源：http://fnx.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hbi.zdbjq.cn

PHP:  public static function f() {}
来源：http://mdg.andypj.xyz

JS:   static f() {}
来源：http://hbk.yueranfly.top

TS:   static f(): void {}
来源：http://xpm.yj202588.top

Java: static void f() {}
来源：http://xxz.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iem.yueranfly.top

Ruby: def self.f; end
来源：http://vsq.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://wwy.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://scj.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://ufw.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://fku.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jqi.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://zzz.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://akj.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://wqd.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ifj.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://hya.andypj.xyz

[G10] 访问控制
来源：http://kuu.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://qmw.hnqzz.top

PHP:  public / protected / private
来源：http://uop.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://jli.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://ezl.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://gau.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://npc.nanxuanxn.top

Ruby: public / protected / private
来源：http://kic.0kj1m.cn

C#:   public / protected / private / internal
来源：http://xpy.aibaodan.cn

[G11] getter / setter
来源：http://dti.sweek.top

Py:   @property 与 @x.setter
来源：http://sij.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fac.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://xnd.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://lhj.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://fts.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hei.meibo888.top

Ruby: attr_accessor :name
来源：http://upv.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://lzu.daria6918.cn

[G12] 对象转字符串
来源：http://ydg.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://cau.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ocu.sweek.top

JS:   toString() { return this.name; }
来源：http://idc.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://chw.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://gyo.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://jib.nwbrower.top

Ruby: def to_s; @name; end
来源：http://ggg.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://fis.pycfn.com

[G13] 判断对象类型
来源：http://vgo.xinyue.icu

Py:   isinstance(u, User)
来源：http://bqn.sysykeji.top

PHP:  $u instanceof User
来源：http://bll.hfpthk.cn

JS:   u instanceof User
来源：http://knd.svipenyu.cn

TS:   u instanceof User
来源：http://ygo.hnqzz.top

Java: u instanceof User
来源：http://tyb.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mrw.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://wqc.yongpay.top

C#:   u is User
来源：http://zpy.gaohongyu789.top

[G14] 数据类 / record
来源：http://wvi.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vbe.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://idc.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://uyv.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://chg.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://jrd.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://zie.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rgo.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://sbt.cashguo.top

[G15] 枚举
来源：http://wnp.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qpn.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vpz.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ucy.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://joh.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://jul.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://frm.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://fzs.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fxl.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://jav.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://evq.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://nqv.zdbjq.cn

JS:   Object.entries(obj)
来源：http://mpi.hammf.cn

TS:   Object.entries(obj)
来源：http://rqa.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hto.fktsv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mvz.cdnleiting.top

Ruby: obj.instance_variables
来源：http://zmg.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://dzc.9152youxi.cn

================================================================================
来源：http://ubh.tian-w.cn

H. 异常与错误处理
来源：http://yky.zhoulong.xyz

================================================================================
来源：http://hlv.havefunace.top

[H01] try / catch 基础
来源：http://jwu.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qfn.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gdp.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ghq.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nmj.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://agp.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://igd.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jca.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rsi.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://vjv.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://byp.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wrg.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://szp.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ssx.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://yxo.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jvk.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yrb.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jrj.chenzaomai.com

[H03] 主动抛出异常
来源：http://qgx.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://vhe.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://smj.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://nfo.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://wpe.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ovv.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://khi.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://grq.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://lxk.vehdjk.com

[H04] 自定义异常类型
来源：http://zvc.birdmap.top

Py:   class MyError(Exception): pass
来源：http://cfn.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://vrl.pycfn.com

JS:   class MyError extends Error {}
来源：http://ain.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://gag.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://rog.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://igz.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://spg.guannengcc.top

C#:   class MyException : Exception {}
来源：http://wso.zdqjudy.top

[H05] 捕获特定类型
来源：http://ejq.shzxlz.cn

Py:   except ValueError as e:
来源：http://qqp.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umo.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://qct.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://jto.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://cpu.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cqv.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://djy.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gjr.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://bnn.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://zum.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mtz.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vvw.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hyl.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mxc.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ifu.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://anm.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://bec.zhoulong.xyz

[H07] 断言
来源：http://jgk.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://dvl.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://juo.daria6918.cn

JS:   console.assert(x > 0);
来源：http://akx.fktsv.cn

TS:   console.assert(x > 0);
来源：http://zjr.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://vgf.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mme.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ecl.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://nwf.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://bqy.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://vut.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bov.havefunace.top

JS:   e.message;  e.stack
来源：http://dvf.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wie.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zde.jinqigufen.top

Go:   err.Error()
来源：http://dyu.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://bgv.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://xzn.0kj1m.cn

[H09] 带错误码的异常
来源：http://wfl.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tyd.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eaz.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ojp.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hbr.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vvo.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xpm.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zxo.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wpq.aibaodan.cn

[H10] 资源自动释放
来源：http://qxh.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bpw.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rwd.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qde.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aoc.gogol.net.cn


<!-- 参考信息 -->