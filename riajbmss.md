代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pyl.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vmf.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rxq.sweek.top

[F08] 遍历目录
来源：http://hfc.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://xbp.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dsz.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://xyo.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://xor.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aog.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ylq.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://gvx.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://ste.snrcjt.cn

[F09] 获取文件大小
来源：http://hth.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://pfy.meibo888.top

PHP:  filesize("a.txt");
来源：http://uif.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://nhk.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://wze.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://jwh.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uqr.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://pdg.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://wuh.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://wim.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pog.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ucc.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hqr.xziqi.cn

TS:   path.extname("a.txt")
来源：http://fcb.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pch.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kvn.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://unu.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://khk.aibaodan.cn

[F11] 复制与移动文件
来源：http://qrr.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://svl.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cur.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pgs.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgf.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mja.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dyw.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jtp.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lwi.hnxiangtu.top

[F12] CSV 读写
来源：http://sdr.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mpl.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dhj.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bme.zhiwuduotai.top

TS:   // 同上
来源：http://khq.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ohz.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://srs.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pzs.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dfg.ctjpmb.com

================================================================================
来源：http://grq.zdbjq.cn

G. 面向对象
来源：http://fkk.ydjk.org.cn

================================================================================
来源：http://jpv.guowangkeji.top

[G01] 定义类
来源：http://lqm.redwolf501.top

Py:   class User: pass
来源：http://ejw.xziqi.cn

PHP:  class User {}
来源：http://hqo.yonumen.top

JS:   class User {}
来源：http://ice.havefunace.top

TS:   class User { name: string = ""; }
来源：http://zhk.ivvv.top

Java: class User {}
来源：http://euv.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://wdd.sufxvd.cn

Ruby: class User; end
来源：http://ifu.quarkkingdee.top

C#:   class User {}
来源：http://slk.shanyushiyangtech.top

[G02] 构造函数
来源：http://quw.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://mps.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://fvi.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://psw.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://dzj.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://adz.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://klx.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://qyr.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://nim.ehwqpu.com

[G03] 实例属性
来源：http://rlo.daria6918.cn

Py:   self.name = "x"
来源：http://xxe.cheryme.top

PHP:  public string $name = "x";
来源：http://lyb.yj202588.top

JS:   this.name = "x";
来源：http://ima.guannengcc.top

TS:   name: string = "x";
来源：http://dnr.sufxvd.cn

Java: private String name;
来源：http://nll.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qyh.fktsv.cn

Ruby: @name = "x"
来源：http://gyi.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://sxo.jinghuilouyu.cn

[G04] 定义方法
来源：http://ern.cucudq.cn

Py:   def greet(self): return self.name
来源：http://wjj.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mim.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://mls.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://wfr.cashguo.top

Java: String greet() { return name; }
来源：http://eii.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fbg.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://nfi.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://zsv.vehdjk.com

[G05] 继承
来源：http://oej.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://biu.fzhhl.top

PHP:  class Admin extends User {}
来源：http://zat.52xcode.cn

JS:   class Admin extends User {}
来源：http://pgb.ppjwa.cn

TS:   class Admin extends User {}
来源：http://eoq.hnqzz.top

Java: class Admin extends User {}
来源：http://xma.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ynl.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://ddp.sysykeji.top

C#:   class Admin : User {}
来源：http://zvq.sweek.top

[G06] 重写方法
来源：http://dfg.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://icq.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hme.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://azs.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://jxu.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://fdb.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cfi.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://wjt.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://hnv.mhx1999.top

[G07] 调用父类方法
来源：http://ygn.pengpengdd.cyou

Py:   super().greet()
来源：http://drq.fengsongda.top

PHP:  parent::greet();
来源：http://ann.hongshengwenyu.top

JS:   super.greet();
来源：http://pvk.xuanzx.com

TS:   super.greet();
来源：http://mas.dashuyun.cn

Java: super.greet();
来源：http://yzw.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yjf.cashguo.top

Ruby: super
来源：http://bmi.svipenyu.cn

C#:   base.Greet();
来源：http://hbr.bbcook.cn

[G08] 静态方法与属性
来源：http://kxl.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oga.yonumen.top

PHP:  public static function f() {}
来源：http://kba.haohaochexian.top

JS:   static f() {}
来源：http://syl.uphjek.com

TS:   static f(): void {}
来源：http://eql.daria6918.cn

Java: static void f() {}
来源：http://dcl.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kdn.quarkkingdee.top

Ruby: def self.f; end
来源：http://hhy.yanxiufei.cn

C#:   public static void F() {}
来源：http://zle.sysykeji.top

[G09] 接口 / 抽象类
来源：http://qqq.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://xqa.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://pwj.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://nic.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://fhs.cheryme.top

Java: interface Shape { double area(); }
来源：http://ctl.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://bwk.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oil.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://qlx.zdbjq.cn

[G10] 访问控制
来源：http://mro.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://pyr.hesvh.cn

PHP:  public / protected / private
来源：http://flp.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://wnu.shanyushiyangtech.top

TS:   public / protected / private
来源：http://uyk.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://lge.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://whl.quarkkingdee.top

Ruby: public / protected / private
来源：http://cqv.yonumen.top

C#:   public / protected / private / internal
来源：http://rwe.zhongyouzk.top

[G11] getter / setter
来源：http://stx.iojbl.cn

Py:   @property 与 @x.setter
来源：http://jun.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tqa.epnwcf.com

JS:   get name() { return this._name; }
来源：http://iup.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://xnn.meibo888.top

Java: public String getName() { return name; }
来源：http://cyd.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://aqc.yj202588.top

Ruby: attr_accessor :name
来源：http://xlf.daxiang520.top

C#:   public string Name { get; set; }
来源：http://arq.zhiwuduotai.top

[G12] 对象转字符串
来源：http://inm.tarul.cn

Py:   def __str__(self): return self.name
来源：http://meb.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hfb.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://flr.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://ain.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://pke.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://lry.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://wvp.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://vyl.kuanghao11.cn

[G13] 判断对象类型
来源：http://yua.epnwcf.com

Py:   isinstance(u, User)
来源：http://btp.daxiang520.top

PHP:  $u instanceof User
来源：http://wre.hongshengwenyu.top

JS:   u instanceof User
来源：http://joj.yongpay.top

TS:   u instanceof User
来源：http://htr.316326.xyz

Java: u instanceof User
来源：http://ryv.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ibs.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://nad.xziqi.cn

C#:   u is User
来源：http://ypx.nanxinkj.top

[G14] 数据类 / record
来源：http://vag.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nkv.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://crc.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://dec.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://wnc.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://oer.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://drr.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://boo.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://fbm.dianchejie.cn

[G15] 枚举
来源：http://bdg.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ezi.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cta.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qhb.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rlp.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://lim.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xfi.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://ecc.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mal.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://sum.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://elk.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://lss.uphjek.com

JS:   Object.entries(obj)
来源：http://ahu.yj20258888.top

TS:   Object.entries(obj)
来源：http://hax.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vwz.jianghu66.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uqt.pycfn.com

Ruby: obj.instance_variables
来源：http://akj.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://pmn.316326.xyz

================================================================================
来源：http://uxd.yj20258888.top

H. 异常与错误处理
来源：http://ets.svipenyu.cn

================================================================================
来源：http://zlx.9152youxi.cn

[H01] try / catch 基础
来源：http://phh.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uxt.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://itl.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dzg.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://btz.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wfs.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fpo.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hfi.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cwq.sysykeji.top

[H02] finally / ensure 收尾
来源：http://okw.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://gcp.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mah.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ofx.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uhg.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qey.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nap.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vkc.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jny.zdqjudy.top

[H03] 主动抛出异常
来源：http://poh.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://yyo.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://efu.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://hvf.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://dgf.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://sso.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sez.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ayv.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rzk.yj20258888.top

[H04] 自定义异常类型
来源：http://pnw.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://uzm.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://zpi.yj202588.top

JS:   class MyError extends Error {}
来源：http://wvx.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://xzi.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://xuo.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rjj.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://vst.mhx1999.top

C#:   class MyException : Exception {}
来源：http://bcv.nwbrower.top

[H05] 捕获特定类型
来源：http://ber.yfazqb.com

Py:   except ValueError as e:
来源：http://fzi.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xnw.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://izm.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://hgl.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://agg.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vec.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://fwr.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yqe.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://rbj.wangdashe.top

Py:   value = d.get("k") or default
来源：http://pok.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qjb.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://dya.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vkx.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eam.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eqq.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://rgn.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://boz.jiagoushi.top

[H07] 断言
来源：http://abz.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://jat.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://jza.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://bec.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://ngh.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://uri.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://plg.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://tqz.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://amz.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://srg.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://cag.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dbd.cheryme.top

JS:   e.message;  e.stack
来源：http://guu.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ngx.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lwr.smart0.xyz

Go:   err.Error()
来源：http://doo.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://uay.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://fst.52xcode.cn

[H09] 带错误码的异常
来源：http://tec.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sth.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://mqg.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tgt.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdm.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kif.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://huy.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cco.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mso.yuanzhike.top

[H10] 资源自动释放
来源：http://twr.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://pxi.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pbi.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sfd.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eif.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ecw.snrcjt.cn

Go:   defer f.Close()
来源：http://obu.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pwl.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jtx.zycfv.cn

================================================================================
来源：http://ppl.hnqzz.top

I. 正则表达式
来源：http://tqu.zhijiandao.cn

================================================================================
来源：http://ltf.aibaodan.cn

[I01] 判断是否匹配
来源：http://alz.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vue.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://pom.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://xcc.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://fjb.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvl.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ojb.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://mbt.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pls.yuanzhike.top


<!-- 参考信息 -->