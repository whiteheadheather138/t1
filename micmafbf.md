代发 wailian999

C#:   File.Exists("a.txt")
来源：http://fus.zhengqikj.top

[F06] 删除文件
来源：http://akx.tian-w.cn

Py:   os.remove("a.txt")
来源：http://dup.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://tdu.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://pkg.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://jru.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sow.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://djw.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://had.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://mow.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://bno.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qvy.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rev.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eew.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wfm.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rax.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://drw.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xhx.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://des.havefunace.top

[F08] 遍历目录
来源：http://kxy.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gjr.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://axm.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://hmo.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://rmx.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://loq.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://igv.bjfxy.top

Ruby: Dir.children("dir")
来源：http://zcl.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://npk.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://ncn.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://fhj.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://ubu.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://odt.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://qie.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://rdx.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vnt.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://pbv.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://blx.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://vcb.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://opp.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://izw.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wud.aizwys.cn

TS:   path.extname("a.txt")
来源：http://ips.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sdu.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hzf.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sep.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ttf.uphjek.com

[F11] 复制与移动文件
来源：http://fzu.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjh.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://twc.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://evn.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbr.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ktr.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lbs.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qln.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yoc.epnwcf.com

[F12] CSV 读写
来源：http://suc.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wpn.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hti.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yig.ydjk.org.cn

TS:   // 同上
来源：http://nza.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ltf.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kfr.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://brf.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://vca.zhaomingkeji.xyz

================================================================================
来源：http://lpd.yj202588.top

G. 面向对象
来源：http://bbv.feifeiyinyue.top

================================================================================
来源：http://kzb.tanke756.top

[G01] 定义类
来源：http://ysq.yj20258888.top

Py:   class User: pass
来源：http://wul.fanxiaobao.xyz

PHP:  class User {}
来源：http://mpp.dianchejie.cn

JS:   class User {}
来源：http://udy.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://dlr.yvedp.cn

Java: class User {}
来源：http://keo.c1oappe.top

Go:   type User struct { Name string }
来源：http://rld.yuanzhike.top

Ruby: class User; end
来源：http://frh.cqqwz.cn

C#:   class User {}
来源：http://obn.kuanghao11.cn

[G02] 构造函数
来源：http://fmk.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://vev.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://svw.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://xuw.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://ehd.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://kkj.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hor.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://uhj.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://tjm.dianchejie.cn

[G03] 实例属性
来源：http://vkb.zdbjq.cn

Py:   self.name = "x"
来源：http://yxc.xylfe.cn

PHP:  public string $name = "x";
来源：http://yfw.wangshuangyany.cn

JS:   this.name = "x";
来源：http://cgq.yj20258.top

TS:   name: string = "x";
来源：http://bgr.guannengcc.top

Java: private String name;
来源：http://upq.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gsj.wangdashe.top

Ruby: @name = "x"
来源：http://yoc.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://yjq.yuanzhike.top

[G04] 定义方法
来源：http://zbc.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://tcr.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ire.tarul.cn

JS:   greet() { return this.name; }
来源：http://nis.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://dnz.hywenlv.cn

Java: String greet() { return name; }
来源：http://tsp.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://anc.guowangkeji.top

Ruby: def greet; @name; end
来源：http://tjm.xinyue.icu

C#:   public string Greet() => Name;
来源：http://gix.cucudq.cn

[G05] 继承
来源：http://hqd.zhengqikj.top

Py:   class Admin(User): pass
来源：http://ota.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://fln.yuanzhike.top

JS:   class Admin extends User {}
来源：http://hxb.fktsv.cn

TS:   class Admin extends User {}
来源：http://eij.redwolf501.top

Java: class Admin extends User {}
来源：http://wvh.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qoa.zhengqikj.top

Ruby: class Admin < User; end
来源：http://uas.shuidangran.top

C#:   class Admin : User {}
来源：http://gxo.aibaodan.cn

[G06] 重写方法
来源：http://zrf.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://zbn.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gsr.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://mqj.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://sca.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://uvo.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ckz.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://pzz.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://mvi.sweek.top

[G07] 调用父类方法
来源：http://rlb.jinghuilouyu.cn

Py:   super().greet()
来源：http://czw.shangyingyoupin.top

PHP:  parent::greet();
来源：http://kki.shzxlz.cn

JS:   super.greet();
来源：http://qnj.shanyushiyangkeji.top

TS:   super.greet();
来源：http://kag.nanxuanxn.top

Java: super.greet();
来源：http://rgb.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hjh.yj202588.top

Ruby: super
来源：http://imh.cucudq.cn

C#:   base.Greet();
来源：http://kbq.zhijiandao.cn

[G08] 静态方法与属性
来源：http://ndn.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ztp.ybcxt.top

PHP:  public static function f() {}
来源：http://mze.zhiwuduotai.top

JS:   static f() {}
来源：http://pjf.wangshuangyany.cn

TS:   static f(): void {}
来源：http://hoc.hywenlv.cn

Java: static void f() {}
来源：http://cyv.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dmy.dashuyun.cn

Ruby: def self.f; end
来源：http://riu.jianghu66.top

C#:   public static void F() {}
来源：http://ife.tian-w.cn

[G09] 接口 / 抽象类
来源：http://era.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://wbw.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://jwz.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oxg.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://tic.sweek.top

Java: interface Shape { double area(); }
来源：http://cws.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://kwg.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ret.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://lax.chenzaomai.com

[G10] 访问控制
来源：http://edl.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://zmz.ydjk.org.cn

PHP:  public / protected / private
来源：http://fxq.pycfn.com

JS:   #private 字段；其余公开
来源：http://iil.aizwys.cn

TS:   public / protected / private
来源：http://iyy.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://qlx.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ojs.ydjk.org.cn

Ruby: public / protected / private
来源：http://fav.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://lvw.sxryk.cn

[G11] getter / setter
来源：http://qpx.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://knz.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://znf.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://djy.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://vyo.cucudq.cn

Java: public String getName() { return name; }
来源：http://ptz.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ebw.cashguo.top

Ruby: attr_accessor :name
来源：http://ucx.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://kvg.cdnleiting.top

[G12] 对象转字符串
来源：http://zgf.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://dte.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rva.iojbl.cn

JS:   toString() { return this.name; }
来源：http://puc.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://fzn.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://wjn.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://kqn.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://xca.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://hfg.c1oappe.top

[G13] 判断对象类型
来源：http://ciu.yuxming.cn

Py:   isinstance(u, User)
来源：http://ifx.yj202588.top

PHP:  $u instanceof User
来源：http://elv.fzhhl.top

JS:   u instanceof User
来源：http://cpm.zhixingplan.top

TS:   u instanceof User
来源：http://iwp.hywenlv.cn

Java: u instanceof User
来源：http://mkt.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tss.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://qlb.ppjwa.cn

C#:   u is User
来源：http://hod.gzhubu.top

[G14] 数据类 / record
来源：http://mar.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://knl.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://yeb.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://tdt.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://jtc.cucudq.cn

Java: record User(String name, int age) {}
来源：http://oaf.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://qcg.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fga.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://vby.fktsv.cn

[G15] 枚举
来源：http://tkc.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qkx.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gqq.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jqt.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bbe.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://reu.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gub.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://qsa.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ziw.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://hqs.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bxp.316326.xyz

PHP:  get_object_vars($obj);
来源：http://ntu.daxiang520.top

JS:   Object.entries(obj)
来源：http://ykw.sxryk.cn

TS:   Object.entries(obj)
来源：http://wlb.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://okt.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qrx.cheryme.top

Ruby: obj.instance_variables
来源：http://pmg.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://vje.guowangkeji.top

================================================================================
来源：http://tap.hongshengwenyu.top

H. 异常与错误处理
来源：http://kdw.cucudq.cn

================================================================================
来源：http://nla.xziqi.cn

[H01] try / catch 基础
来源：http://fmk.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://msc.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pue.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vql.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kqo.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qlq.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cqo.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pcc.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wtu.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://jjt.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://awu.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yzb.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qom.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://siz.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://grt.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://dpm.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vjz.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lgx.fzhhl.top

[H03] 主动抛出异常
来源：http://jfs.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://zqj.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wek.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://iub.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://vej.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mdp.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sjf.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ram.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://ykj.xuanzx.com

[H04] 自定义异常类型
来源：http://qgo.birdmap.top

Py:   class MyError(Exception): pass
来源：http://zaz.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://xea.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://rfk.epnwcf.com

TS:   class MyError extends Error {}
来源：http://kil.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://iqm.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://apz.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://mzv.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://vty.zhongyouzk.top

[H05] 捕获特定类型
来源：http://qhf.hywenlv.cn

Py:   except ValueError as e:
来源：http://ryg.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nkt.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://ada.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://qxx.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://own.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nuu.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://ken.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aal.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://orl.havefunace.top

Py:   value = d.get("k") or default
来源：http://mfs.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://naw.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://egm.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://cug.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dhg.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gdd.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://nwc.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://asq.meibo888.top

[H07] 断言
来源：http://opi.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://inr.yfazqb.com

PHP:  assert($x > 0);
来源：http://lgn.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://pbp.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://emq.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://poe.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xty.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gjr.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://bfr.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://zww.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://jps.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rzp.zdbjq.cn

JS:   e.message;  e.stack
来源：http://pom.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qjx.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ytv.yangfankeji.com

Go:   err.Error()
来源：http://xun.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://jff.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://ing.snrcjt.cn

[H09] 带错误码的异常
来源：http://hxo.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fht.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cmi.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://znx.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gpl.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://apm.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://stm.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://bro.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://onx.smart0.xyz

[H10] 资源自动释放
来源：http://cos.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xjv.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zkt.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nkv.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zvj.cdnleiting.top


<!-- 参考信息 -->