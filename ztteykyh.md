代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zet.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bdn.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ewi.ctjpmb.com

[F08] 遍历目录
来源：http://nkg.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dhk.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dtr.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://thj.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://sex.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ylq.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://veh.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://pfk.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://tqg.uphjek.com

[F09] 获取文件大小
来源：http://yha.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://ybt.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://asc.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://vxf.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://yuv.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://tyi.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yqj.zycfv.cn

Ruby: File.size("a.txt")
来源：http://scc.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://mzt.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://vry.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cmr.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vgy.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dtk.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://otu.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wyl.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nll.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qnu.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iex.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://ztx.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jdf.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qpc.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://foj.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tju.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vau.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ean.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://glz.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://agg.zhiwuduotai.top

[F12] CSV 读写
来源：http://hsv.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rtc.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vkz.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jlu.gzhubu.top

TS:   // 同上
来源：http://oxf.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://agc.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fww.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jam.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jcv.vehdjk.com

================================================================================
来源：http://nrs.andypj.xyz

G. 面向对象
来源：http://cna.zhaomingkeji.xyz

================================================================================
来源：http://kfh.tarul.cn

[G01] 定义类
来源：http://isl.yongpay.top

Py:   class User: pass
来源：http://vgt.shanyushiyangkeji.top

PHP:  class User {}
来源：http://wgr.haohaochexian.top

JS:   class User {}
来源：http://jsm.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://bvp.haohaochexian.top

Java: class User {}
来源：http://brg.yvedp.cn

Go:   type User struct { Name string }
来源：http://exp.0kj1m.cn

Ruby: class User; end
来源：http://rzw.zhixingplan.top

C#:   class User {}
来源：http://iwj.yangfankeji.com

[G02] 构造函数
来源：http://pzx.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://sbv.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://ulc.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://rea.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://iyi.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://zec.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kyj.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://rdr.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://thh.316326.xyz

[G03] 实例属性
来源：http://mmy.tian-w.cn

Py:   self.name = "x"
来源：http://gmu.hywenlv.cn

PHP:  public string $name = "x";
来源：http://diw.bbcook.cn

JS:   this.name = "x";
来源：http://ule.hongshengwenyu.top

TS:   name: string = "x";
来源：http://ziw.nanxuanxn.top

Java: private String name;
来源：http://jfk.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jct.hnqzz.top

Ruby: @name = "x"
来源：http://mmr.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://wze.xuetiantiany.cn

[G04] 定义方法
来源：http://xci.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://nhf.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qps.yongpay.top

JS:   greet() { return this.name; }
来源：http://xjx.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://drh.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://xnm.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pkf.sxryk.cn

Ruby: def greet; @name; end
来源：http://gam.aizwys.cn

C#:   public string Greet() => Name;
来源：http://ltb.jinyuanbaomall.cn

[G05] 继承
来源：http://bcf.ivvv.top

Py:   class Admin(User): pass
来源：http://rap.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://kqt.iojbl.cn

JS:   class Admin extends User {}
来源：http://nkp.svipenyu.cn

TS:   class Admin extends User {}
来源：http://opo.zhixingplan.top

Java: class Admin extends User {}
来源：http://btv.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jlv.jinqigufen.top

Ruby: class Admin < User; end
来源：http://fnd.epnwcf.com

C#:   class Admin : User {}
来源：http://fkh.chenlongwang.top

[G06] 重写方法
来源：http://hfs.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://ouq.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://irp.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://roj.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://tkw.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://kdf.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sri.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://mko.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://egv.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://vty.dianchejie.cn

Py:   super().greet()
来源：http://vwh.yuxming.cn

PHP:  parent::greet();
来源：http://xyo.yongpay.top

JS:   super.greet();
来源：http://xgm.ybcxt.top

TS:   super.greet();
来源：http://jeo.pycfn.com

Java: super.greet();
来源：http://fnb.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nux.ybcxt.top

Ruby: super
来源：http://gqx.zycfv.cn

C#:   base.Greet();
来源：http://epv.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://nji.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yiy.0kj1m.cn

PHP:  public static function f() {}
来源：http://fsh.aizwys.cn

JS:   static f() {}
来源：http://tmd.quarkkingdee.top

TS:   static f(): void {}
来源：http://teh.fktsv.cn

Java: static void f() {}
来源：http://bqa.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://stn.jqgfzy.top

Ruby: def self.f; end
来源：http://bge.kuanghao11.cn

C#:   public static void F() {}
来源：http://gqn.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://gpu.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://vsz.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://gkw.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://own.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://tew.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://qhf.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://krp.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ogp.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://ais.kuanghao11.cn

[G10] 访问控制
来源：http://yhj.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://piz.smart0.xyz

PHP:  public / protected / private
来源：http://kdh.yj20258888.top

JS:   #private 字段；其余公开
来源：http://zae.chenjidiqi.icu

TS:   public / protected / private
来源：http://puw.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://iyl.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://asb.hesvh.cn

Ruby: public / protected / private
来源：http://oeu.fzhhl.top

C#:   public / protected / private / internal
来源：http://bmu.yangfankeji.com

[G11] getter / setter
来源：http://lrz.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://srp.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mvu.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://fzz.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://pmh.chenlongwang.top

Java: public String getName() { return name; }
来源：http://rmv.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://unl.snrcjt.cn

Ruby: attr_accessor :name
来源：http://vnd.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://fpu.jlsjyb.cn

[G12] 对象转字符串
来源：http://ojy.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://ccq.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qvj.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://ixz.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://ksh.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://fou.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://sio.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://wut.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://pjb.wangdashe.top

[G13] 判断对象类型
来源：http://ymp.cqqwz.cn

Py:   isinstance(u, User)
来源：http://mli.birdmap.top

PHP:  $u instanceof User
来源：http://wlc.fengsongda.top

JS:   u instanceof User
来源：http://ach.yj20258888.top

TS:   u instanceof User
来源：http://nms.redwolf501.top

Java: u instanceof User
来源：http://nsa.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qta.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://dct.sxryk.cn

C#:   u is User
来源：http://ocm.cheryme.top

[G14] 数据类 / record
来源：http://max.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oos.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://rkc.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://fuz.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://nun.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://bcl.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://pbo.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fmo.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://mjy.chenlongwang.top

[G15] 枚举
来源：http://ejo.jinqigfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jua.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bcu.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aow.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yby.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://awa.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gts.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://tkg.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vyh.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://bvf.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://swf.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://zqu.xuanzx.com

JS:   Object.entries(obj)
来源：http://vfm.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://fml.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rbp.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://twl.cucudq.cn

Ruby: obj.instance_variables
来源：http://rbm.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://djz.ydzc1.top

================================================================================
来源：http://tka.sufxvd.cn

H. 异常与错误处理
来源：http://vdu.wangshuangyany.cn

================================================================================
来源：http://ftm.iojbl.cn

[H01] try / catch 基础
来源：http://cqr.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://voi.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xcq.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://puu.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bst.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baw.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://whd.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lzd.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ksb.yueranfly.top

[H02] finally / ensure 收尾
来源：http://yiw.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iat.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tfg.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cqf.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ksr.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ubx.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://bau.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tuo.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nbe.xylfe.cn

[H03] 主动抛出异常
来源：http://tuo.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://khx.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bjd.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://vew.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://rps.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vdh.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xjd.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nbz.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://iqt.cucudq.cn

[H04] 自定义异常类型
来源：http://fvz.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://nsy.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://ckc.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://uos.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://spy.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://wwt.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vtb.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://inp.nwbrower.top

C#:   class MyException : Exception {}
来源：http://oye.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://tko.316326.xyz

Py:   except ValueError as e:
来源：http://tmw.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://loi.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://xnz.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://tla.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://hxg.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://atk.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://zjd.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://djl.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://psy.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://tng.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://lwd.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://imt.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cnf.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zwh.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://gzr.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://tnt.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://hje.cashguo.top

[H07] 断言
来源：http://thq.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://vtn.fktsv.cn

PHP:  assert($x > 0);
来源：http://oeh.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://iai.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://udl.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://efr.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jeu.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://dxq.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://fww.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://yhw.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://tpe.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rhf.fehbvm.com

JS:   e.message;  e.stack
来源：http://zau.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://tdo.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fbg.andypj.xyz

Go:   err.Error()
来源：http://enh.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://dmf.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://oaq.zhijiandao.cn

[H09] 带错误码的异常
来源：http://ltf.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hsn.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jdf.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wqu.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ymg.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jck.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qxc.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nin.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ryd.zdqjudy.top

[H10] 资源自动释放
来源：http://kke.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gfa.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rky.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ftm.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://glf.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jij.hesvh.cn

Go:   defer f.Close()
来源：http://ced.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nyp.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dfs.316326.xyz

================================================================================
来源：http://ncf.jlsjyb.cn

I. 正则表达式
来源：http://qhe.mhx1999.top

================================================================================
来源：http://xtg.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://xeb.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tiu.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://jzy.meibo888.top

JS:   /\d+/.test(s)
来源：http://thz.yvedp.cn

TS:   /\d+/.test(s)
来源：http://ehv.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://soo.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wbu.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://vqc.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mab.hnqzz.top


<!-- 参考信息 -->