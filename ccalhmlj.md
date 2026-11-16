代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://xqt.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mpc.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pzx.yonumen.top

Go:   os.Remove("a.txt")
来源：http://ahs.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://hap.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://inq.guannengcc.top

[F07] 创建目录（含多级）
来源：http://gsn.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ngm.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lwq.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wov.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://swd.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lde.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oxl.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sur.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bym.dashuyun.cn

[F08] 遍历目录
来源：http://dej.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hgr.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://abh.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://xfe.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://svn.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vto.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wcw.xinyue.icu

Ruby: Dir.children("dir")
来源：http://dzx.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://tef.aibaodan.cn

[F09] 获取文件大小
来源：http://hmr.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://miw.ydzc1.top

PHP:  filesize("a.txt");
来源：http://nxb.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://wke.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://evj.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://bzv.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dsc.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://cwz.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://cfk.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://kgv.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://usp.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vdf.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hgt.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://hcl.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rur.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vvy.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://muk.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zqz.ehwqpu.com

[F11] 复制与移动文件
来源：http://uvf.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bho.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qit.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nhx.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://equ.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jwh.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fxp.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xsb.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mmf.yanxiufei.cn

[F12] CSV 读写
来源：http://ynq.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://twc.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vib.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ibb.nanxinkj.top

TS:   // 同上
来源：http://tgb.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vqn.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fbx.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lrc.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://eba.yj20258888.top

================================================================================
来源：http://emd.tianlin.xyz

G. 面向对象
来源：http://zqx.andypj.xyz

================================================================================
来源：http://lfl.yuanzhike.top

[G01] 定义类
来源：http://cue.jqgufenzy.top

Py:   class User: pass
来源：http://ovm.zhongyouzk.top

PHP:  class User {}
来源：http://vzt.yongpay.top

JS:   class User {}
来源：http://rqq.yonumen.top

TS:   class User { name: string = ""; }
来源：http://naw.ivvv.top

Java: class User {}
来源：http://ccd.aizwys.cn

Go:   type User struct { Name string }
来源：http://hqb.yvedp.cn

Ruby: class User; end
来源：http://ocr.hysaishi.cn

C#:   class User {}
来源：http://ykx.svipenyu.cn

[G02] 构造函数
来源：http://yxk.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://mju.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://blz.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://xot.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://lre.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://nla.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oth.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://rsg.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://lie.hammf.cn

[G03] 实例属性
来源：http://nfz.hfpthk.cn

Py:   self.name = "x"
来源：http://fls.yangfankeji.com

PHP:  public string $name = "x";
来源：http://ote.quarkkingdee.top

JS:   this.name = "x";
来源：http://zzs.hysaishi.cn

TS:   name: string = "x";
来源：http://zmm.dianchejie.cn

Java: private String name;
来源：http://jyk.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://khn.sysykeji.top

Ruby: @name = "x"
来源：http://sqj.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://ihi.hnqzz.top

[G04] 定义方法
来源：http://ewv.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://owu.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qjb.yvedp.cn

JS:   greet() { return this.name; }
来源：http://shc.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://swq.chenzaomai.com

Java: String greet() { return name; }
来源：http://idx.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iim.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://nkf.c1oappe.top

C#:   public string Greet() => Name;
来源：http://xiq.jianghu66.top

[G05] 继承
来源：http://aog.yj20258.top

Py:   class Admin(User): pass
来源：http://aac.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://wgq.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://afj.epnwcf.com

TS:   class Admin extends User {}
来源：http://yrn.zdbjq.cn

Java: class Admin extends User {}
来源：http://zxh.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tre.c1oappe.top

Ruby: class Admin < User; end
来源：http://xfi.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://kpp.zycfv.cn

[G06] 重写方法
来源：http://ijf.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://nty.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cim.vqdsnc.cn

JS:   greet() { return "admin"; }
来源：http://zmf.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://tur.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://cjk.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yom.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://vqq.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://xue.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://awj.yvedp.cn

Py:   super().greet()
来源：http://woj.jqgufenzy.top

PHP:  parent::greet();
来源：http://ouj.52xcode.cn

JS:   super.greet();
来源：http://gui.hcnkem.com

TS:   super.greet();
来源：http://kln.shanyushiyangtech.top

Java: super.greet();
来源：http://owp.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lvr.zdqjudy.top

Ruby: super
来源：http://dir.zhiwuduotai.top

C#:   base.Greet();
来源：http://ufb.yuxming.cn

[G08] 静态方法与属性
来源：http://xdf.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ncd.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://srx.xylfe.cn

JS:   static f() {}
来源：http://cmu.gogol.net.cn

TS:   static f(): void {}
来源：http://kyh.gotoacloud.top

Java: static void f() {}
来源：http://tev.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://vzm.nwbrower.top

Ruby: def self.f; end
来源：http://gnj.0kj1m.cn

C#:   public static void F() {}
来源：http://xrh.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://uuj.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://apt.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kxy.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xqh.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://yhs.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://tjp.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://zbc.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://noa.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://own.zdbjq.cn

[G10] 访问控制
来源：http://ilc.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://iqp.uphjek.com

PHP:  public / protected / private
来源：http://tiu.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://axl.ydzc1.top

TS:   public / protected / private
来源：http://dky.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://bea.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tuz.hammf.cn

Ruby: public / protected / private
来源：http://otv.bjfxy.top

C#:   public / protected / private / internal
来源：http://kcj.pengpengdd.cyou

[G11] getter / setter
来源：http://ttj.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://fez.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://tjy.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://pfd.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://rmb.bjfxy.top

Java: public String getName() { return name; }
来源：http://mfx.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://otb.epnwcf.com

Ruby: attr_accessor :name
来源：http://qqk.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://ral.ppjwa.cn

[G12] 对象转字符串
来源：http://sos.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://eoa.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bgh.meibo888.top

JS:   toString() { return this.name; }
来源：http://gsp.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://uib.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://ghn.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://zhu.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://rxi.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://scs.fengsongda.top

[G13] 判断对象类型
来源：http://qis.ehwqpu.com

Py:   isinstance(u, User)
来源：http://jxb.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://dvu.gzhubu.top

JS:   u instanceof User
来源：http://hzx.pycfn.com

TS:   u instanceof User
来源：http://nzr.ybcxt.top

Java: u instanceof User
来源：http://iyn.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tyk.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://aay.hfpthk.cn

C#:   u is User
来源：http://kqd.bbcook.cn

[G14] 数据类 / record
来源：http://hcq.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jwv.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://osa.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://sms.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://smb.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://epm.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://oys.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kfu.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://ndj.jianghu66.top

[G15] 枚举
来源：http://afd.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://urs.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lkm.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://srb.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://miw.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://wzg.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cov.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://ckd.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nns.epnwcf.com

[G16] 对象转数组 / 字典
来源：http://khf.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ppk.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://dul.fktsv.cn

JS:   Object.entries(obj)
来源：http://wjj.zhixingplan.top

TS:   Object.entries(obj)
来源：http://bsy.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pdg.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kkh.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://gve.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://vqs.yongpay.top

================================================================================
来源：http://amw.pycfn.com

H. 异常与错误处理
来源：http://zak.dashuyun.cn

================================================================================
来源：http://wcb.yongpay.top

[H01] try / catch 基础
来源：http://ebh.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yby.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xxd.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ywb.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bfx.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mkq.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dny.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://moy.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dfa.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://hwh.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://ken.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rqq.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gco.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://opj.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qdc.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://nue.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eht.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://htm.sweek.top

[H03] 主动抛出异常
来源：http://haw.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://epl.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kyu.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://wmw.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://vrb.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nsa.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://onp.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ugl.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://rmx.hnxiangtu.top

[H04] 自定义异常类型
来源：http://tuq.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://szd.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nry.pycfn.com

JS:   class MyError extends Error {}
来源：http://kmu.c1oappe.top

TS:   class MyError extends Error {}
来源：http://vgm.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://uxv.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lwk.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://dlc.316326.xyz

C#:   class MyException : Exception {}
来源：http://bqr.ivvv.top

[H05] 捕获特定类型
来源：http://lvr.cdnleiting.top

Py:   except ValueError as e:
来源：http://ftq.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pja.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://nyf.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://ifm.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://umh.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ook.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://iys.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dci.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://ohd.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://zig.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://jup.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fuo.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://nhm.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://evj.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ktg.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://jsd.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://dlg.chenzaomai.com

[H07] 断言
来源：http://niw.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://ujt.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://gtv.jianghu66.top

JS:   console.assert(x > 0);
来源：http://vgd.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://jiz.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://zui.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ijx.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vkj.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://pwb.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://usz.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://ptu.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cht.fengsongda.top

JS:   e.message;  e.stack
来源：http://dwx.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tjd.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ovq.yuxming.cn

Go:   err.Error()
来源：http://ogv.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://aye.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://irf.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://dop.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ppb.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lar.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fri.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://glw.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hoy.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xxj.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sar.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://bet.zhijiandao.cn

[H10] 资源自动释放
来源：http://njv.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vmm.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gtu.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rsk.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qaz.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cdr.zhixingplan.top

Go:   defer f.Close()
来源：http://dvv.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eti.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hmr.shangyingyoupin.top


<!-- 参考信息 -->