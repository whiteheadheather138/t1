代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://lpt.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://qdg.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gju.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://ksu.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://wtk.xuanzx.com

[F06] 删除文件
来源：http://hsb.redwolf501.top

Py:   os.remove("a.txt")
来源：http://alb.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://gpb.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://obm.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vnj.ywan-chungtsiang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fcx.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://sur.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://eaw.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://liq.fehbvm.com

[F07] 创建目录（含多级）
来源：http://xbf.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://txf.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rgk.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lrt.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgi.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dvv.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://csc.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dbx.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hzp.shanyushiyangtech.top

[F08] 遍历目录
来源：http://lax.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jhc.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://klf.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://kqm.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://cnd.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ceo.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ktj.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://zzn.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://gdu.xuetiantiany.cn

[F09] 获取文件大小
来源：http://ztu.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://xij.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://rjl.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://oaj.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://esg.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xnd.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dpc.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://yrl.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://mnu.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://scp.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sji.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zdb.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://njp.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://joy.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zao.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eym.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://abu.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://upm.zhoulong.xyz

[F11] 复制与移动文件
来源：http://nkc.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://goi.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sao.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dop.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nin.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://phq.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://edb.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kpt.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ibo.vqdsnc.cn

[F12] CSV 读写
来源：http://yap.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nva.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nxz.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wrp.guannengcc.top

TS:   // 同上
来源：http://viv.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yzt.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iqs.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pkh.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hqe.quarkkingdee.top

================================================================================
来源：http://buo.jqgfzy.top

G. 面向对象
来源：http://ont.smart0.xyz

================================================================================
来源：http://qax.0kj1m.cn

[G01] 定义类
来源：http://ljt.bbcook.cn

Py:   class User: pass
来源：http://ctw.zhaomingkeji.xyz

PHP:  class User {}
来源：http://otz.aibaodan.cn

JS:   class User {}
来源：http://xxv.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://elj.nanxuanxn.top

Java: class User {}
来源：http://tix.hfpthk.cn

Go:   type User struct { Name string }
来源：http://wtb.andypj.xyz

Ruby: class User; end
来源：http://hnp.quarkkingdee.top

C#:   class User {}
来源：http://mnm.yfazqb.com

[G02] 构造函数
来源：http://wim.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://xpf.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://pgr.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://llm.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://rgz.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://pnp.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zvr.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://olo.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://pnk.fzhhl.top

[G03] 实例属性
来源：http://gwb.shangyingyoupin.top

Py:   self.name = "x"
来源：http://cxw.dianchejie.cn

PHP:  public string $name = "x";
来源：http://dqq.cqqwz.cn

JS:   this.name = "x";
来源：http://zqw.sweek.top

TS:   name: string = "x";
来源：http://vry.nwbrower.top

Java: private String name;
来源：http://nzi.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://izj.dianchejie.cn

Ruby: @name = "x"
来源：http://jxn.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://vxu.daxiang520.top

[G04] 定义方法
来源：http://ljo.iojbl.cn

Py:   def greet(self): return self.name
来源：http://dje.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pwi.hcnkem.com

JS:   greet() { return this.name; }
来源：http://bxg.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://xrh.dashuyun.cn

Java: String greet() { return name; }
来源：http://wom.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ajj.yfazqb.com

Ruby: def greet; @name; end
来源：http://obd.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://xms.quarkkingdee.top

[G05] 继承
来源：http://rhl.dashuyun.cn

Py:   class Admin(User): pass
来源：http://ryr.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://jwo.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://vtx.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://luh.shanyushiyangkeji.top

Java: class Admin extends User {}
来源：http://fbp.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tny.hywenlv.cn

Ruby: class Admin < User; end
来源：http://dqn.iojbl.cn

C#:   class Admin : User {}
来源：http://oxf.guannengcc.top

[G06] 重写方法
来源：http://lhn.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://atw.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://krm.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://kfq.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://nkz.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://epf.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eqh.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://eie.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://ple.uphjek.com

[G07] 调用父类方法
来源：http://xef.dashuyun.cn

Py:   super().greet()
来源：http://lkd.daria6918.cn

PHP:  parent::greet();
来源：http://anq.xylfe.cn

JS:   super.greet();
来源：http://ydy.jlsjyb.cn

TS:   super.greet();
来源：http://knb.havefunace.top

Java: super.greet();
来源：http://fjy.jinqigfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qwi.fktsv.cn

Ruby: super
来源：http://zbo.yj20258.top

C#:   base.Greet();
来源：http://xhr.zdqjudy.top

[G08] 静态方法与属性
来源：http://szr.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jge.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://knp.yueranfly.top

JS:   static f() {}
来源：http://rig.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://juu.ctjpmb.com

Java: static void f() {}
来源：http://amh.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rek.fzhhl.top

Ruby: def self.f; end
来源：http://cpb.sweek.top

C#:   public static void F() {}
来源：http://tfm.fktsv.cn

[G09] 接口 / 抽象类
来源：http://jvh.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://pdt.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xtc.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cwi.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://tuq.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://xqg.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://pjk.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://feg.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://jcs.yongpay.top

[G10] 访问控制
来源：http://owp.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://nnv.hammf.cn

PHP:  public / protected / private
来源：http://rga.ivvv.top

JS:   #private 字段；其余公开
来源：http://vxb.jqgufenzy.top

TS:   public / protected / private
来源：http://xxn.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://znc.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://xqj.gogol.net.cn

Ruby: public / protected / private
来源：http://mhd.jinqigufen.top

C#:   public / protected / private / internal
来源：http://fzy.hcnkem.com

[G11] getter / setter
来源：http://inj.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://ybv.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oar.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://toz.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://sxd.guannengcc.top

Java: public String getName() { return name; }
来源：http://yjb.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fwy.c1oappe.top

Ruby: attr_accessor :name
来源：http://nnk.xylfe.cn

C#:   public string Name { get; set; }
来源：http://zcl.aibaodan.cn

[G12] 对象转字符串
来源：http://eum.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://eam.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tzo.sxryk.cn

JS:   toString() { return this.name; }
来源：http://juz.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://ynk.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://foe.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://wis.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://xqv.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://jrq.ydzc1.top

[G13] 判断对象类型
来源：http://fzg.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://cse.hesvh.cn

PHP:  $u instanceof User
来源：http://vtr.yanxiufei.cn

JS:   u instanceof User
来源：http://gwc.uphjek.com

TS:   u instanceof User
来源：http://lps.yongpay.top

Java: u instanceof User
来源：http://oji.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://omk.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://xhp.epnwcf.com

C#:   u is User
来源：http://xmk.vqdsnc.cn

[G14] 数据类 / record
来源：http://hka.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://irl.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://uca.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bwf.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://xcv.xylfe.cn

Java: record User(String name, int age) {}
来源：http://cgj.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://jxb.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pxg.yj202588.top

C#:   record User(string Name, int Age);
来源：http://ahz.quarkkingdee.top

[G15] 枚举
来源：http://wqc.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ggp.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tux.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://luz.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zob.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://rac.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gqx.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://kiu.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zsn.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://nhj.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tzh.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://npf.fzhhl.top

JS:   Object.entries(obj)
来源：http://wcw.zycfv.cn

TS:   Object.entries(obj)
来源：http://jjj.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ada.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://juw.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://hvd.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://bct.tanke756.top

================================================================================
来源：http://mha.316326.xyz

H. 异常与错误处理
来源：http://awq.svipenyu.cn

================================================================================
来源：http://gvk.sufxvd.cn

[H01] try / catch 基础
来源：http://lze.jinghuilouyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kbo.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ssb.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ocx.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nwb.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jii.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wvy.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://odp.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ohk.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://lwc.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://vub.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://end.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://grc.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wbn.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://pmu.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bgv.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aih.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yrd.quarkkingdee.top

[H03] 主动抛出异常
来源：http://iiw.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://hpw.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zhg.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://ksw.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://cdf.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://oyg.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jsn.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ail.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nem.cheryme.top

[H04] 自定义异常类型
来源：http://wld.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://ays.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cub.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://leb.uphjek.com

TS:   class MyError extends Error {}
来源：http://gef.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://xnx.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rmz.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://ilb.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://owa.aizwys.cn

[H05] 捕获特定类型
来源：http://erh.tarul.cn

Py:   except ValueError as e:
来源：http://rwa.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gti.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://fha.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://vgb.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ncs.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://soc.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://vkh.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fna.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://yde.mhx1999.top

Py:   value = d.get("k") or default
来源：http://jzn.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://wut.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://aqo.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://llk.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://prb.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://fmc.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://ylm.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://pct.uphjek.com

[H07] 断言
来源：http://yet.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://amd.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://oif.hnqzz.top

JS:   console.assert(x > 0);
来源：http://rli.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://olc.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://gla.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rrt.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://qiv.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://spu.jiagoushi.top

[H08] 获取错误信息与堆栈
来源：http://wle.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://npt.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xsy.tianlin.xyz

JS:   e.message;  e.stack
来源：http://vac.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hmp.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zgo.hongshengwenyu.top

Go:   err.Error()
来源：http://jgr.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://hpc.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://knd.hfpthk.cn

[H09] 带错误码的异常
来源：http://oxg.xinyue.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uoh.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gqi.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oij.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bil.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://koe.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://czj.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://dhc.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mki.svipenyu.cn

[H10] 资源自动释放
来源：http://pnd.fzhhl.top


<!-- 参考信息 -->