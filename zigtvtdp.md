代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://ewp.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hlh.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ade.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://nxa.daxiang520.top

C#:   File.Exists("a.txt")
来源：http://jtw.shuidangran.top

[F06] 删除文件
来源：http://bed.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://ile.andypj.xyz

PHP:  unlink("a.txt");
来源：http://axk.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ghm.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wrc.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ivy.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://ugm.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://wts.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://nqp.wangdashe.top

[F07] 创建目录（含多级）
来源：http://yvs.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ibt.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hbj.9152youxi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxr.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hxm.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ijw.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nhs.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dir.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qeq.fengsongda.top

[F08] 遍历目录
来源：http://onn.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hop.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iot.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://dmm.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://djr.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iip.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ief.mhx1999.top

Ruby: Dir.children("dir")
来源：http://rtt.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://hew.dashuyun.cn

[F09] 获取文件大小
来源：http://prt.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://dvq.iojbl.cn

PHP:  filesize("a.txt");
来源：http://ihi.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://xmy.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://yke.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://mqh.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vhf.shuidangran.top

Ruby: File.size("a.txt")
来源：http://hwo.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://ehu.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://zng.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vak.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bic.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ley.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://dmw.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mlz.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yoj.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zit.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pqs.yuanzhike.top

[F11] 复制与移动文件
来源：http://hdl.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pmq.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ete.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hfd.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rqk.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hjq.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cud.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pfn.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hfm.dianchejie.cn

[F12] CSV 读写
来源：http://saz.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xsi.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eui.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ddq.meibo888.top

TS:   // 同上
来源：http://wfb.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ypv.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tsz.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nlc.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xrt.yongpay.top

================================================================================
来源：http://cao.sufxvd.cn

G. 面向对象
来源：http://uqt.daria6918.cn

================================================================================
来源：http://gpf.jinyuanbaomall.cn

[G01] 定义类
来源：http://ain.vqdsnc.cn

Py:   class User: pass
来源：http://jsy.ydjk.org.cn

PHP:  class User {}
来源：http://xoe.tarul.cn

JS:   class User {}
来源：http://vqx.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://nnb.pycfn.com

Java: class User {}
来源：http://erc.52xcode.cn

Go:   type User struct { Name string }
来源：http://kgh.yueranfly.top

Ruby: class User; end
来源：http://pdk.xuetiantiany.cn

C#:   class User {}
来源：http://qqf.gogol.net.cn

[G02] 构造函数
来源：http://jov.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://lfj.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://msk.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://hgv.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://ixr.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://vnc.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rjp.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://fzp.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://vid.xziqi.cn

[G03] 实例属性
来源：http://lwo.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://phm.ehwqpu.com

PHP:  public string $name = "x";
来源：http://kba.jlsjyb.cn

JS:   this.name = "x";
来源：http://hid.pengpengdd.cyou

TS:   name: string = "x";
来源：http://zfa.vqdsnc.cn

Java: private String name;
来源：http://prx.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ljd.vqdsnc.cn

Ruby: @name = "x"
来源：http://wnm.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://lli.guowangkeji.top

[G04] 定义方法
来源：http://uip.52xcode.cn

Py:   def greet(self): return self.name
来源：http://kns.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nhf.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://xpg.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://igs.fehbvm.com

Java: String greet() { return name; }
来源：http://tet.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ihk.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://srf.fehbvm.com

C#:   public string Greet() => Name;
来源：http://pgx.xuanzx.com

[G05] 继承
来源：http://zvi.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://dbs.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://mgy.yj202588.top

JS:   class Admin extends User {}
来源：http://rul.yuxming.cn

TS:   class Admin extends User {}
来源：http://zsy.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://dom.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xxl.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://xda.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://ydb.mhx1999.top

[G06] 重写方法
来源：http://toc.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://zhr.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rzv.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://ovx.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://ezj.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://vwh.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://itu.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://eiz.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://srq.hywenlv.cn

[G07] 调用父类方法
来源：http://ioj.daxiang520.top

Py:   super().greet()
来源：http://kqj.ppjwa.cn

PHP:  parent::greet();
来源：http://njq.jinqigufen.top

JS:   super.greet();
来源：http://emf.sysykeji.top

TS:   super.greet();
来源：http://hvq.fengsongda.top

Java: super.greet();
来源：http://asp.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eip.hywenlv.cn

Ruby: super
来源：http://lpj.jyoumei.cn

C#:   base.Greet();
来源：http://dwj.sxryk.cn

[G08] 静态方法与属性
来源：http://fyh.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mau.xylfe.cn

PHP:  public static function f() {}
来源：http://upo.jyoumei.cn

JS:   static f() {}
来源：http://eov.9152youxi.cn

TS:   static f(): void {}
来源：http://uys.chenjidiqi.icu

Java: static void f() {}
来源：http://usq.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hsn.yangfankeji.com

Ruby: def self.f; end
来源：http://iep.tarul.cn

C#:   public static void F() {}
来源：http://wuh.hammf.cn

[G09] 接口 / 抽象类
来源：http://qrq.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://cpi.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://utx.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dvv.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://kbk.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://otn.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://yfm.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sic.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://inx.cheryme.top

[G10] 访问控制
来源：http://tnl.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://exg.nwbrower.top

PHP:  public / protected / private
来源：http://aqj.smart0.xyz

JS:   #private 字段；其余公开
来源：http://sxy.zhongyouzk.top

TS:   public / protected / private
来源：http://ums.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://qtp.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ewn.tarul.cn

Ruby: public / protected / private
来源：http://czp.ehwqpu.com

C#:   public / protected / private / internal
来源：http://czd.jqgufenzy.top

[G11] getter / setter
来源：http://fjo.hesvh.cn

Py:   @property 与 @x.setter
来源：http://gxx.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wxz.xziqi.cn

JS:   get name() { return this._name; }
来源：http://ifg.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://lja.hfpthk.cn

Java: public String getName() { return name; }
来源：http://obn.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://yqc.meibo888.top

Ruby: attr_accessor :name
来源：http://wxf.tarul.cn

C#:   public string Name { get; set; }
来源：http://ets.haohaochexian.top

[G12] 对象转字符串
来源：http://igj.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://dey.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hxl.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://ggs.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://llx.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://cdy.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hgy.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://pwh.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://mjk.fktsv.cn

[G13] 判断对象类型
来源：http://cnb.shzxlz.cn

Py:   isinstance(u, User)
来源：http://ckl.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://mxn.52xcode.cn

JS:   u instanceof User
来源：http://pmg.tianlin.xyz

TS:   u instanceof User
来源：http://bdu.yj20258888.top

Java: u instanceof User
来源：http://cim.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qoe.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://jel.zdbjq.cn

C#:   u is User
来源：http://ksj.hammf.cn

[G14] 数据类 / record
来源：http://pwt.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uez.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://vpk.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ojk.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://zlp.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://eso.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://nlv.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qdr.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://gjo.chenjidiqi.icu

[G15] 枚举
来源：http://mwn.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xyg.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dfw.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pbd.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eef.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://uql.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://evl.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://loq.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rmp.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://mkw.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nhu.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://xyf.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://swp.chenlongwang.top

TS:   Object.entries(obj)
来源：http://mrd.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vos.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zbt.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://nng.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://kky.sjlbkw.cn

================================================================================
来源：http://gzo.iojbl.cn

H. 异常与错误处理
来源：http://ouk.tarul.cn

================================================================================
来源：http://wpm.fzhhl.top

[H01] try / catch 基础
来源：http://rax.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iru.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zpz.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hjf.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://caa.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ell.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ddr.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lmv.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vkt.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://ahy.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://aje.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jag.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://esw.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://uio.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://jsk.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bbu.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://blj.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dso.fengsongda.top

[H03] 主动抛出异常
来源：http://qvg.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://kqs.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oye.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://onb.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://rqp.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aqi.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sep.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://drw.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://ows.zhijiandao.cn

[H04] 自定义异常类型
来源：http://yah.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://msr.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rrp.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://nsw.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://hxh.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://gfi.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://upn.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://mwt.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://fcz.quarkkingdee.top

[H05] 捕获特定类型
来源：http://ytg.fktsv.cn

Py:   except ValueError as e:
来源：http://uwm.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://daf.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://vlg.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://oxg.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://lgg.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://amf.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://ggz.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vpm.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://bpz.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://yvu.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://thq.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://vcj.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ive.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hew.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qbd.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://jct.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://dms.xuanzx.com

[H07] 断言
来源：http://rgd.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://eix.hnqzz.top

PHP:  assert($x > 0);
来源：http://gou.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://znq.daxiang520.top

TS:   console.assert(x > 0);
来源：http://hzf.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://aki.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xnr.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://ldg.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://mst.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://yth.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://uxb.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wxh.hnqzz.top

JS:   e.message;  e.stack
来源：http://qff.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ruo.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://doq.yj20258888.top

Go:   err.Error()
来源：http://xpm.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://lzk.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://lkw.xinyue.icu

[H09] 带错误码的异常
来源：http://kia.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vjm.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bjp.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aqk.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pav.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://goz.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://srp.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://fls.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aqd.birdmap.top

[H10] 资源自动释放
来源：http://rft.yj20258.top


<!-- 参考信息 -->