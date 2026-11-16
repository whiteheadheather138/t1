代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kyh.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://ccm.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zvf.xylfe.cn

[F04] 追加写入文件
来源：http://dlq.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uir.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eiw.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdu.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dqq.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jua.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pbk.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gnu.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mnx.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://qci.jqgufenzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fan.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://gyk.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://xhp.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://hsa.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vpl.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://khr.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://wyc.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://uer.gaohongyu789.top

[F06] 删除文件
来源：http://cxz.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://zfv.hcnkem.com

PHP:  unlink("a.txt");
来源：http://ltz.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://jwe.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://qam.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nlk.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://wfz.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://xfq.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://qgy.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://rll.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aou.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lnx.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kph.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iyu.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxi.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bcb.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lpt.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kte.jiagoushi.top

[F08] 遍历目录
来源：http://eza.fktsv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bav.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wgm.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://qgj.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://ael.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vih.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ywj.daria6918.cn

Ruby: Dir.children("dir")
来源：http://kdu.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://gmc.guowangkeji.top

[F09] 获取文件大小
来源：http://gek.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://wqm.guannengcc.top

PHP:  filesize("a.txt");
来源：http://dlo.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://myu.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://nzr.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://kxb.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cgo.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://got.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://bkw.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://yij.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gaw.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kng.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://exi.hcnkem.com

TS:   path.extname("a.txt")
来源：http://abs.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lec.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzw.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kor.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mis.tianlin.xyz

[F11] 复制与移动文件
来源：http://oxu.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vkb.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://icb.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qez.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eun.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nag.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oui.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ugv.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ykw.xylfe.cn

[F12] CSV 读写
来源：http://lgr.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vwu.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sgg.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://igu.jyoumei.cn

TS:   // 同上
来源：http://fia.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://quf.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ozj.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sxb.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://pyn.9152youxi.cn

================================================================================
来源：http://hky.zhixingplan.top

G. 面向对象
来源：http://rar.jinqigfzy.top

================================================================================
来源：http://rgq.pycfn.com

[G01] 定义类
来源：http://kck.epnwcf.com

Py:   class User: pass
来源：http://omr.yangfankeji.com

PHP:  class User {}
来源：http://lqq.xinyue.icu

JS:   class User {}
来源：http://nab.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://trd.tian-w.cn

Java: class User {}
来源：http://niu.hysaishi.cn

Go:   type User struct { Name string }
来源：http://yne.cheryme.top

Ruby: class User; end
来源：http://xgs.uphjek.com

C#:   class User {}
来源：http://fer.haohaochexian.top

[G02] 构造函数
来源：http://jxa.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://ynn.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://sqw.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://kjl.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://faa.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://gmz.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fuz.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://onj.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://hie.havefunace.top

[G03] 实例属性
来源：http://auv.nanxinkj.top

Py:   self.name = "x"
来源：http://fsp.jyoumei.cn

PHP:  public string $name = "x";
来源：http://idy.gaohongyu789.top

JS:   this.name = "x";
来源：http://rso.svipenyu.cn

TS:   name: string = "x";
来源：http://zzr.jqgufenzy.top

Java: private String name;
来源：http://avf.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sgq.hfpthk.cn

Ruby: @name = "x"
来源：http://zzb.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://ifr.fehbvm.com

[G04] 定义方法
来源：http://jls.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://msl.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://umq.hesvh.cn

JS:   greet() { return this.name; }
来源：http://hkv.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://akg.meibo888.top

Java: String greet() { return name; }
来源：http://ouj.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hnt.dianchejie.cn

Ruby: def greet; @name; end
来源：http://pxh.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://bux.haohaochexian.top

[G05] 继承
来源：http://rtt.yfazqb.com

Py:   class Admin(User): pass
来源：http://qup.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://pwu.guowangkeji.top

JS:   class Admin extends User {}
来源：http://azn.uphjek.com

TS:   class Admin extends User {}
来源：http://hfp.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://qiq.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://czs.yueranfly.top

Ruby: class Admin < User; end
来源：http://sgk.hcnkem.com

C#:   class Admin : User {}
来源：http://dcl.pengpengdd.cyou

[G06] 重写方法
来源：http://xqu.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://dcm.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ihf.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://wnf.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://jcu.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://awf.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sdn.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://vnv.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://mkm.kuanghao11.cn

[G07] 调用父类方法
来源：http://ytp.zhijiandao.cn

Py:   super().greet()
来源：http://spo.yfazqb.com

PHP:  parent::greet();
来源：http://qzu.ybcxt.top

JS:   super.greet();
来源：http://irz.haohaochexian.top

TS:   super.greet();
来源：http://pqz.yj20258.top

Java: super.greet();
来源：http://mdi.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xaz.0kj1m.cn

Ruby: super
来源：http://cfk.jinqigufen.top

C#:   base.Greet();
来源：http://ucl.zhengqikj.top

[G08] 静态方法与属性
来源：http://qav.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oww.cqqwz.cn

PHP:  public static function f() {}
来源：http://ajb.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://xeq.aibaodan.cn

TS:   static f(): void {}
来源：http://osa.jqgfzy.top

Java: static void f() {}
来源：http://csf.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ybh.ydzc1.top

Ruby: def self.f; end
来源：http://wqx.ppjwa.cn

C#:   public static void F() {}
来源：http://eri.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://evd.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://xam.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ell.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uvj.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://cjk.yueranfly.top

Java: interface Shape { double area(); }
来源：http://ykk.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://jnb.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pzu.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://hbl.cqqwz.cn

[G10] 访问控制
来源：http://kwe.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://mrf.yuxming.cn

PHP:  public / protected / private
来源：http://oua.uphjek.com

JS:   #private 字段；其余公开
来源：http://jew.hongshengwenyu.top

TS:   public / protected / private
来源：http://adf.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://fvl.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hxs.xinyue.icu

Ruby: public / protected / private
来源：http://jxd.yuxming.cn

C#:   public / protected / private / internal
来源：http://wug.xylfe.cn

[G11] getter / setter
来源：http://oql.vehdjk.com

Py:   @property 与 @x.setter
来源：http://ucg.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://xij.fehbvm.com

JS:   get name() { return this._name; }
来源：http://qwg.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://iwo.c1oappe.top

Java: public String getName() { return name; }
来源：http://wzm.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hqv.zhixingplan.top

Ruby: attr_accessor :name
来源：http://phq.sxryk.cn

C#:   public string Name { get; set; }
来源：http://xgu.cdnleiting.top

[G12] 对象转字符串
来源：http://exm.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://lgd.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yjj.fengsongda.top

JS:   toString() { return this.name; }
来源：http://qjp.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://gzu.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://mkf.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://wlc.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://qkm.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://hve.hammf.cn

[G13] 判断对象类型
来源：http://iak.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://esz.meibo888.top

PHP:  $u instanceof User
来源：http://grd.yj20258.top

JS:   u instanceof User
来源：http://mdr.shzxlz.cn

TS:   u instanceof User
来源：http://dqi.xziqi.cn

Java: u instanceof User
来源：http://kjf.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mdy.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://gqg.jyoumei.cn

C#:   u is User
来源：http://cvv.hnxiangtu.top

[G14] 数据类 / record
来源：http://zuj.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jbq.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://kgp.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://cnp.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://lpp.redwolf501.top

Java: record User(String name, int age) {}
来源：http://wcd.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://xvm.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cpt.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://het.hesvh.cn

[G15] 枚举
来源：http://wta.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fnn.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yoh.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kty.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pnw.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://hdr.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pew.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://bqg.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zdu.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://hgj.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mne.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://exh.ehwqpu.com

JS:   Object.entries(obj)
来源：http://jdn.gogol.net.cn

TS:   Object.entries(obj)
来源：http://ymm.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://azz.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ewt.xuanzx.com

Ruby: obj.instance_variables
来源：http://fft.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://yvm.yj202588.top

================================================================================
来源：http://cjh.redwolf501.top

H. 异常与错误处理
来源：http://nwb.daxiang520.top

================================================================================
来源：http://fbn.ydjk.org.cn

[H01] try / catch 基础
来源：http://ast.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zik.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dzk.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mum.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qtn.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rli.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sns.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pdw.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kgn.ybcxt.top

[H02] finally / ensure 收尾
来源：http://xum.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xko.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://qxg.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gfq.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fyb.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://vja.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://cdl.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bxn.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wme.shuidangran.top

[H03] 主动抛出异常
来源：http://ngn.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://pqz.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mtb.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://zar.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://paz.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://cqz.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tvr.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dyo.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://gga.hnqzz.top

[H04] 自定义异常类型
来源：http://wwu.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://jmd.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jvc.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://qmd.yuxming.cn

TS:   class MyError extends Error {}
来源：http://feq.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://rsj.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fyx.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://tsb.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://scz.yj20258888.top

[H05] 捕获特定类型
来源：http://ntz.jinqigufen.top

Py:   except ValueError as e:
来源：http://bay.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://maj.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://uac.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://tmv.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://knf.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kgo.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://yfd.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ryb.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://dus.tanke756.top

Py:   value = d.get("k") or default
来源：http://wtk.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://day.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vvb.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://pvb.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qzr.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fhv.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://mha.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://gwm.ppjwa.cn

[H07] 断言
来源：http://pnc.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://kws.jianghu66.top

PHP:  assert($x > 0);
来源：http://kcw.c1oappe.top

JS:   console.assert(x > 0);
来源：http://grj.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://wjp.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://sbr.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pay.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://cmh.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://bfm.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://ngb.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://sya.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://myh.jlsjyb.cn


<!-- 参考信息 -->