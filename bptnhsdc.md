代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://tee.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://aoc.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ksu.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://vky.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://xwg.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://zxt.cheryme.top

[F07] 创建目录（含多级）
来源：http://qrz.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jrv.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xhg.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsl.gaohongyu789.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xwk.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hfn.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://piw.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ymq.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gaa.cucudq.cn

[F08] 遍历目录
来源：http://duh.yj202588.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xtl.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gsp.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://rix.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://pfj.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nip.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dkc.iojbl.cn

Ruby: Dir.children("dir")
来源：http://spm.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://fgl.tarul.cn

[F09] 获取文件大小
来源：http://hhj.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://pvk.c1oappe.top

PHP:  filesize("a.txt");
来源：http://kby.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://nar.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://vjn.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://diy.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://per.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://nfo.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://gah.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://rjt.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gdr.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eae.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nmr.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://igq.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mcr.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fdi.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lxk.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rfg.epnwcf.com

[F11] 复制与移动文件
来源：http://uhh.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eag.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ovc.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjp.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qgn.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://max.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kle.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xvs.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://frq.yj20258888.top

[F12] CSV 读写
来源：http://szq.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cwc.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://reh.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://idi.sufxvd.cn

TS:   // 同上
来源：http://dmg.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://goh.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tml.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://agi.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://asm.jinqigufen.top

================================================================================
来源：http://oav.316326.xyz

G. 面向对象
来源：http://otb.yj202588.top

================================================================================
来源：http://ewa.birdmap.top

[G01] 定义类
来源：http://qnp.dashuyun.cn

Py:   class User: pass
来源：http://wsm.sweek.top

PHP:  class User {}
来源：http://ute.yonumen.top

JS:   class User {}
来源：http://qco.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://xnu.cheryme.top

Java: class User {}
来源：http://shb.smart0.xyz

Go:   type User struct { Name string }
来源：http://boe.hongshengwenyu.top

Ruby: class User; end
来源：http://zyr.jinqigfzy.top

C#:   class User {}
来源：http://cuo.gogol.net.cn

[G02] 构造函数
来源：http://myg.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://paw.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://gzq.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://ygd.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://zhe.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://uip.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kxj.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://nlt.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://zqx.jinqigufen.top

[G03] 实例属性
来源：http://udp.0kj1m.cn

Py:   self.name = "x"
来源：http://glo.cdnleiting.top

PHP:  public string $name = "x";
来源：http://sfb.zhoulong.xyz

JS:   this.name = "x";
来源：http://fsd.fengsongda.top

TS:   name: string = "x";
来源：http://ksq.yonumen.top

Java: private String name;
来源：http://qpp.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rsa.wangdashe.top

Ruby: @name = "x"
来源：http://bkp.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://dvi.52xcode.cn

[G04] 定义方法
来源：http://nzr.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://zta.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kwj.daria6918.cn

JS:   greet() { return this.name; }
来源：http://qat.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://leo.zycfv.cn

Java: String greet() { return name; }
来源：http://iqi.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gqo.sxryk.cn

Ruby: def greet; @name; end
来源：http://one.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://avb.shangyingyoupin.top

[G05] 继承
来源：http://epa.yuxming.cn

Py:   class Admin(User): pass
来源：http://xxf.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://yym.cashguo.top

JS:   class Admin extends User {}
来源：http://kdm.fengsongda.top

TS:   class Admin extends User {}
来源：http://mhj.yongpay.top

Java: class Admin extends User {}
来源：http://mjw.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nzq.yangfankeji.com

Ruby: class Admin < User; end
来源：http://abc.zdbjq.cn

C#:   class Admin : User {}
来源：http://ota.haohaochexian.top

[G06] 重写方法
来源：http://khz.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://bru.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nol.pycfn.com

JS:   greet() { return "admin"; }
来源：http://wcc.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://ljr.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://kks.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gzf.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://ptc.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://dvq.sweek.top

[G07] 调用父类方法
来源：http://epq.nwbrower.top

Py:   super().greet()
来源：http://uzs.316326.xyz

PHP:  parent::greet();
来源：http://fhi.yj20258.top

JS:   super.greet();
来源：http://ucq.bjfxy.top

TS:   super.greet();
来源：http://hau.sxryk.cn

Java: super.greet();
来源：http://bag.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ggi.jqgfzy.top

Ruby: super
来源：http://lpn.redwolf501.top

C#:   base.Greet();
来源：http://ugb.cdnleiting.top

[G08] 静态方法与属性
来源：http://ytv.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sja.hnqzz.top

PHP:  public static function f() {}
来源：http://xur.c1oappe.top

JS:   static f() {}
来源：http://kyw.yonumen.top

TS:   static f(): void {}
来源：http://afe.hnxiangtu.top

Java: static void f() {}
来源：http://rhw.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ggv.hesvh.cn

Ruby: def self.f; end
来源：http://eeh.gzhubu.top

C#:   public static void F() {}
来源：http://enu.hesvh.cn

[G09] 接口 / 抽象类
来源：http://pwj.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://pve.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://whi.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iwi.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://ewl.meibo888.top

Java: interface Shape { double area(); }
来源：http://zzg.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://qgx.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pbv.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://mue.bbcook.cn

[G10] 访问控制
来源：http://nhi.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://tej.vqdsnc.cn

PHP:  public / protected / private
来源：http://ssu.316326.xyz

JS:   #private 字段；其余公开
来源：http://hfx.gotoacloud.top

TS:   public / protected / private
来源：http://wez.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://rzn.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://umd.bjfxy.top

Ruby: public / protected / private
来源：http://hfn.ppjwa.cn

C#:   public / protected / private / internal
来源：http://cey.xziqi.cn

[G11] getter / setter
来源：http://dfd.cashguo.top

Py:   @property 与 @x.setter
来源：http://dhh.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dkt.bbcook.cn

JS:   get name() { return this._name; }
来源：http://hpr.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://fpq.zycfv.cn

Java: public String getName() { return name; }
来源：http://lhy.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://huy.zycfv.cn

Ruby: attr_accessor :name
来源：http://kuy.pycfn.com

C#:   public string Name { get; set; }
来源：http://oko.yangfankeji.com

[G12] 对象转字符串
来源：http://sxs.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://ozn.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://czn.bbcook.cn

JS:   toString() { return this.name; }
来源：http://lui.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://nhi.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://ktj.iojbl.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cqx.sxryk.cn

Ruby: def to_s; @name; end
来源：http://fzo.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://nwj.shzxlz.cn

[G13] 判断对象类型
来源：http://mse.jianghu66.top

Py:   isinstance(u, User)
来源：http://oor.hfpthk.cn

PHP:  $u instanceof User
来源：http://mgi.hongshengwenyu.top

JS:   u instanceof User
来源：http://mjz.jianghu66.top

TS:   u instanceof User
来源：http://rcc.yuxming.cn

Java: u instanceof User
来源：http://egk.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dpp.yonumen.top

Ruby: u.is_a?(User)
来源：http://ein.sweek.top

C#:   u is User
来源：http://hui.kuanghao11.cn

[G14] 数据类 / record
来源：http://loy.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://anx.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://jxo.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://rhh.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://ikq.316326.xyz

Java: record User(String name, int age) {}
来源：http://rju.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://uwd.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tfz.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://pyc.yanxiufei.cn

[G15] 枚举
来源：http://wtv.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tdv.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ogf.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qvk.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dki.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://rpr.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hbe.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://zbd.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hlv.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://glb.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ahm.andypj.xyz

PHP:  get_object_vars($obj);
来源：http://ynl.birdmap.top

JS:   Object.entries(obj)
来源：http://jem.shzxlz.cn

TS:   Object.entries(obj)
来源：http://eat.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jey.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jki.smart0.xyz

Ruby: obj.instance_variables
来源：http://msz.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://wlq.zdbjq.cn

================================================================================
来源：http://kna.hywenlv.cn

H. 异常与错误处理
来源：http://gpl.shzxlz.cn

================================================================================
来源：http://xlv.ydjk.org.cn

[H01] try / catch 基础
来源：http://qly.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://toy.dianchejie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rzr.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fyi.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://utd.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wcw.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qpe.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://agf.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gch.birdmap.top

[H02] finally / ensure 收尾
来源：http://ngc.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://scc.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bvo.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pzc.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rpv.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://gge.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pyw.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gqt.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://pqe.sweek.top

[H03] 主动抛出异常
来源：http://dgj.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://mgl.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lft.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://tdj.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://tky.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zah.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yan.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pit.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://dmv.yueranfly.top

[H04] 自定义异常类型
来源：http://mbk.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://lse.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://vlf.aizwys.cn

JS:   class MyError extends Error {}
来源：http://zpe.ivvv.top

TS:   class MyError extends Error {}
来源：http://mts.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://qpi.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pnt.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://pye.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://jwc.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://lry.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://wjm.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oss.xinyue.icu

JS:   if (e instanceof TypeError) {}
来源：http://pjd.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://und.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://vob.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wrk.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://wro.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aik.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://bmb.guannengcc.top

Py:   value = d.get("k") or default
来源：http://iur.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://kld.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nzh.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://nki.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jrr.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qeq.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://yqs.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://lfv.feifeiyinyue.top

[H07] 断言
来源：http://pjp.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://ojg.wangdashe.top

PHP:  assert($x > 0);
来源：http://aup.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://wvq.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://qyr.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://eqo.shanyushiyangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rnu.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://vuo.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://bxe.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://owt.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://sku.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vxu.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://hlm.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yzv.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wjc.fehbvm.com

Go:   err.Error()
来源：http://dvf.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://ggs.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://yqw.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://npt.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yfg.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kvq.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jwm.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nqn.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kwv.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rqe.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ksp.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://avg.jqgufenzy.top

[H10] 资源自动释放
来源：http://tjm.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://joz.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xxn.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://reh.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rol.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jbb.wangdashe.top

Go:   defer f.Close()
来源：http://xba.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hnp.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mjg.dashuyun.cn


<!-- 参考信息 -->