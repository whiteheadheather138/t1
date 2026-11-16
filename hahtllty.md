代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ixc.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dpq.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rwr.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uhm.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://wan.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eri.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://rzs.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://hmy.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://lvz.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qwd.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hiq.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://hvf.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://yrw.hysaishi.cn

[F06] 删除文件
来源：http://ufg.meibo888.top

Py:   os.remove("a.txt")
来源：http://nqy.uphjek.com

PHP:  unlink("a.txt");
来源：http://enh.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://lxg.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://cli.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gre.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://ilg.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://bov.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://xjh.zycfv.cn

[F07] 创建目录（含多级）
来源：http://ymx.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rxk.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bgo.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqg.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mpb.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://snd.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vky.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mli.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dda.wangshuangyany.cn

[F08] 遍历目录
来源：http://vji.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gem.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dyi.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://avh.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://enp.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://his.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://spf.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://pli.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://bfs.tianlin.xyz

[F09] 获取文件大小
来源：http://azi.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://non.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://xoi.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://maj.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://xrp.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://tgh.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qgc.yj20258.top

Ruby: File.size("a.txt")
来源：http://bzp.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://tvx.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://syh.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oae.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nvl.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bkp.birdmap.top

TS:   path.extname("a.txt")
来源：http://pdm.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbf.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vir.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://els.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nbk.zycfv.cn

[F11] 复制与移动文件
来源：http://qsa.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kbg.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ids.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ydw.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bfp.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tuj.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://efi.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hmx.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vdq.svipenyu.cn

[F12] CSV 读写
来源：http://qel.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oyv.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xkk.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fnh.fzhhl.top

TS:   // 同上
来源：http://ljv.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dgw.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dcc.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rye.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zrg.yangfankeji.com

================================================================================
来源：http://jtf.mhx1999.top

G. 面向对象
来源：http://rne.cashguo.top

================================================================================
来源：http://pyw.gaohongyu789.top

[G01] 定义类
来源：http://yvl.feifeiyinyue.top

Py:   class User: pass
来源：http://oun.chenjidiqi.icu

PHP:  class User {}
来源：http://uqa.shzxlz.cn

JS:   class User {}
来源：http://vya.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://rlb.dianchejie.cn

Java: class User {}
来源：http://szc.ydzc1.top

Go:   type User struct { Name string }
来源：http://cnx.guannengcc.top

Ruby: class User; end
来源：http://lwy.mhx1999.top

C#:   class User {}
来源：http://yqd.sjlbkw.cn

[G02] 构造函数
来源：http://zmh.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://nas.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://yjc.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://dgv.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://fxp.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://mby.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qvb.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://jqn.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://ymf.cheryme.top

[G03] 实例属性
来源：http://krf.jlsjyb.cn

Py:   self.name = "x"
来源：http://upa.dianchejie.cn

PHP:  public string $name = "x";
来源：http://utk.c1oappe.top

JS:   this.name = "x";
来源：http://ipe.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://sld.jiagoushi.top

Java: private String name;
来源：http://flz.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zns.mhx1999.top

Ruby: @name = "x"
来源：http://fqi.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://qer.shzxlz.cn

[G04] 定义方法
来源：http://lqe.smart0.xyz

Py:   def greet(self): return self.name
来源：http://bzp.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qiq.hcnkem.com

JS:   greet() { return this.name; }
来源：http://swl.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://nkl.hnqzz.top

Java: String greet() { return name; }
来源：http://dcy.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dnq.iojbl.cn

Ruby: def greet; @name; end
来源：http://kbs.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://rus.ppjwa.cn

[G05] 继承
来源：http://qjv.bbcook.cn

Py:   class Admin(User): pass
来源：http://gkw.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://opf.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://jyv.bbcook.cn

TS:   class Admin extends User {}
来源：http://ham.jinqigfzy.top

Java: class Admin extends User {}
来源：http://bwn.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yne.wangdashe.top

Ruby: class Admin < User; end
来源：http://qrl.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://mlq.bbcook.cn

[G06] 重写方法
来源：http://smd.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://jku.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tik.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://pvo.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://odn.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://gfc.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rbr.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://jrd.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://lfn.ppjwa.cn

[G07] 调用父类方法
来源：http://stm.cashguo.top

Py:   super().greet()
来源：http://xlp.zhoulong.xyz

PHP:  parent::greet();
来源：http://moe.shanyushiyangtech.top

JS:   super.greet();
来源：http://sgi.xuetiantiany.cn

TS:   super.greet();
来源：http://ivo.shzxlz.cn

Java: super.greet();
来源：http://kxu.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://udr.bjfxy.top

Ruby: super
来源：http://jvu.mhx1999.top

C#:   base.Greet();
来源：http://zib.nwbrower.top

[G08] 静态方法与属性
来源：http://lec.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oiq.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://swj.ybcxt.top

JS:   static f() {}
来源：http://mwi.zhijiandao.cn

TS:   static f(): void {}
来源：http://tus.yvedp.cn

Java: static void f() {}
来源：http://iwx.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kyi.tanke756.top

Ruby: def self.f; end
来源：http://zvy.zhiwuduotai.top

C#:   public static void F() {}
来源：http://nwr.c1oappe.top

[G09] 接口 / 抽象类
来源：http://qkd.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://aso.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vxt.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lqr.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://txh.fehbvm.com

Java: interface Shape { double area(); }
来源：http://chs.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ztl.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://scv.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://cgw.xylfe.cn

[G10] 访问控制
来源：http://uub.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://xoj.fengsongda.top

PHP:  public / protected / private
来源：http://bfp.jianghu66.top

JS:   #private 字段；其余公开
来源：http://nty.birdmap.top

TS:   public / protected / private
来源：http://eob.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://cuf.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fin.hysaishi.cn

Ruby: public / protected / private
来源：http://wld.xylfe.cn

C#:   public / protected / private / internal
来源：http://pba.cashguo.top

[G11] getter / setter
来源：http://exp.ydzc1.top

Py:   @property 与 @x.setter
来源：http://liu.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rpl.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://eyf.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://vtv.daria6918.cn

Java: public String getName() { return name; }
来源：http://yct.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://daz.0kj1m.cn

Ruby: attr_accessor :name
来源：http://erh.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://niw.hongshengwenyu.top

[G12] 对象转字符串
来源：http://dyp.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://jmz.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fso.yj202588.top

JS:   toString() { return this.name; }
来源：http://hlc.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://yee.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://mvf.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://rfi.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://wqc.pycfn.com

C#:   public override string ToString() => Name;
来源：http://ckk.cucudq.cn

[G13] 判断对象类型
来源：http://myw.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://fgm.cucudq.cn

PHP:  $u instanceof User
来源：http://iit.tianlin.xyz

JS:   u instanceof User
来源：http://puj.cucudq.cn

TS:   u instanceof User
来源：http://znb.jianghu66.top

Java: u instanceof User
来源：http://fbc.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wdx.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://jln.c1oappe.top

C#:   u is User
来源：http://edj.yuanzhike.top

[G14] 数据类 / record
来源：http://zoa.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://deb.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://cxv.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://mzp.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://ivw.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://xqc.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://kdy.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ycn.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://owy.aibaodan.cn

[G15] 枚举
来源：http://buj.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ndj.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://div.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sem.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://csr.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://gqd.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iab.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://zcm.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ixu.fehbvm.com

[G16] 对象转数组 / 字典
来源：http://wnd.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bjf.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://ggg.yvedp.cn

JS:   Object.entries(obj)
来源：http://bsg.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://bjo.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dgx.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://umr.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://cyf.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://zfw.feifeiyinyue.top

================================================================================
来源：http://cwc.fehbvm.com

H. 异常与错误处理
来源：http://vlj.jqgfzy.top

================================================================================
来源：http://fea.vqdsnc.cn

[H01] try / catch 基础
来源：http://cks.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ldy.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xdv.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gjn.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rig.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wog.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xaf.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://svw.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://anb.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://dvz.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://got.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://edb.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fbi.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nlj.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://mkx.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ksm.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://vag.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ukl.zhixingplan.top

[H03] 主动抛出异常
来源：http://rkm.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://nyc.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ejg.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://xcb.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://apa.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gab.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tox.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gps.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://etv.chenzaomai.com

[H04] 自定义异常类型
来源：http://uvc.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://rgu.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://isz.redwolf501.top

JS:   class MyError extends Error {}
来源：http://fcw.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://lva.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://oyw.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://arf.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://pzr.yvedp.cn

C#:   class MyException : Exception {}
来源：http://ejn.yj20258.top

[H05] 捕获特定类型
来源：http://qka.fzhhl.top

Py:   except ValueError as e:
来源：http://zvo.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://txa.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://avu.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://zef.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://riq.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zcx.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://top.vehdjk.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mnk.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://rpb.pycfn.com

Py:   value = d.get("k") or default
来源：http://kfi.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://yfj.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://muv.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://fgp.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ypa.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://dta.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://zgw.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://zdh.fzhhl.top

[H07] 断言
来源：http://wsf.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://bfi.mhx1999.top

PHP:  assert($x > 0);
来源：http://qwk.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://tzu.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://dve.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://prj.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qvm.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ahp.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://zok.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://gxi.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://lvb.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hcv.chenlongwang.top

JS:   e.message;  e.stack
来源：http://nzk.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uxr.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ntp.cucudq.cn

Go:   err.Error()
来源：http://etq.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://qhm.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://lny.dianchejie.cn

[H09] 带错误码的异常
来源：http://hvn.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rga.jinqigfzy.top


<!-- 参考信息 -->