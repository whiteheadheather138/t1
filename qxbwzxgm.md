代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hzy.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cwp.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ptz.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pmn.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uxd.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vtn.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lvn.dianchejie.cn

[F08] 遍历目录
来源：http://sca.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://vqb.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jli.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://rfi.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://oun.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wqu.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nde.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://okm.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://ghj.andypj.xyz

[F09] 获取文件大小
来源：http://zsl.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://hdy.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://ueg.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://mdy.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://wll.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://hsn.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://twc.havefunace.top

Ruby: File.size("a.txt")
来源：http://zwt.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ocs.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://hpz.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jdh.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bgv.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rdp.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://wzg.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cry.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://myu.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yoa.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rgd.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://evv.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vak.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ixo.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pim.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgq.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iha.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://chi.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://onq.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ktx.fzhhl.top

[F12] CSV 读写
来源：http://eir.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ino.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pdm.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oak.yuxming.cn

TS:   // 同上
来源：http://nsm.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wnh.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jga.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kwe.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mfv.vehdjk.com

================================================================================
来源：http://uhp.shanyushiyangkeji.top

G. 面向对象
来源：http://fyt.jianghu66.top

================================================================================
来源：http://tla.sjlbkw.cn

[G01] 定义类
来源：http://mva.9152youxi.cn

Py:   class User: pass
来源：http://qdn.jinghuilouyu.cn

PHP:  class User {}
来源：http://sdf.hysaishi.cn

JS:   class User {}
来源：http://qsy.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://ksp.9152youxi.cn

Java: class User {}
来源：http://lez.tian-w.cn

Go:   type User struct { Name string }
来源：http://hvg.cucudq.cn

Ruby: class User; end
来源：http://lpt.zhiwuduotai.top

C#:   class User {}
来源：http://sla.ywan-chungtsiang.top

[G02] 构造函数
来源：http://qat.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://pik.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://adp.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://cgn.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://fzo.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://vap.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ufa.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://xnc.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://mys.cdnleiting.top

[G03] 实例属性
来源：http://drp.fktsv.cn

Py:   self.name = "x"
来源：http://vfc.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://jir.zhiwuduotai.top

JS:   this.name = "x";
来源：http://hga.guowangkeji.top

TS:   name: string = "x";
来源：http://byq.tianlin.xyz

Java: private String name;
来源：http://zhe.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vfs.yj202588.top

Ruby: @name = "x"
来源：http://cxo.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://bvo.52xcode.cn

[G04] 定义方法
来源：http://akn.hesvh.cn

Py:   def greet(self): return self.name
来源：http://kyi.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vcq.316326.xyz

JS:   greet() { return this.name; }
来源：http://rpv.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://auh.nanxinkj.top

Java: String greet() { return name; }
来源：http://pqe.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://obu.jiagoushi.top

Ruby: def greet; @name; end
来源：http://fhy.nwbrower.top

C#:   public string Greet() => Name;
来源：http://kvz.feifeiyinyue.top

[G05] 继承
来源：http://hwk.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://nmn.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://ifi.jinqigfzy.top

JS:   class Admin extends User {}
来源：http://nya.gogol.net.cn

TS:   class Admin extends User {}
来源：http://jun.bjfxy.top

Java: class Admin extends User {}
来源：http://svk.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xpn.jinqigufen.top

Ruby: class Admin < User; end
来源：http://nvq.zdqjudy.top

C#:   class Admin : User {}
来源：http://pjx.yanxiufei.cn

[G06] 重写方法
来源：http://vcw.pycfn.com

Py:   def greet(self): return "admin"
来源：http://mtb.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://egk.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://gke.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://odg.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://lai.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xzm.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://dut.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://tct.zhongyouzk.top

[G07] 调用父类方法
来源：http://zqr.gogol.net.cn

Py:   super().greet()
来源：http://fxo.cqqwz.cn

PHP:  parent::greet();
来源：http://snu.redwolf501.top

JS:   super.greet();
来源：http://nyz.yueranfly.top

TS:   super.greet();
来源：http://mkg.andypj.xyz

Java: super.greet();
来源：http://dax.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xaw.mhx1999.top

Ruby: super
来源：http://men.andypj.xyz

C#:   base.Greet();
来源：http://abn.fehbvm.com

[G08] 静态方法与属性
来源：http://xxg.fanxiaobao.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cbx.cdnleiting.top

PHP:  public static function f() {}
来源：http://skw.shuidangran.top

JS:   static f() {}
来源：http://lqx.wangdashe.top

TS:   static f(): void {}
来源：http://hty.fengsongda.top

Java: static void f() {}
来源：http://cyj.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://uup.ybcxt.top

Ruby: def self.f; end
来源：http://xnw.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://ezh.yongpay.top

[G09] 接口 / 抽象类
来源：http://otf.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://ljq.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://zej.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nar.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://jez.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://des.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://xlv.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xsk.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://cvf.zycfv.cn

[G10] 访问控制
来源：http://niz.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://rxq.bjfxy.top

PHP:  public / protected / private
来源：http://ytp.ydzc1.top

JS:   #private 字段；其余公开
来源：http://xhz.cashguo.top

TS:   public / protected / private
来源：http://dtt.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://ojm.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://efe.dashuyun.cn

Ruby: public / protected / private
来源：http://xoo.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://daz.nwbrower.top

[G11] getter / setter
来源：http://qpc.gzhubu.top

Py:   @property 与 @x.setter
来源：http://uzu.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://axd.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://pma.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://atf.yonumen.top

Java: public String getName() { return name; }
来源：http://iae.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://idi.dianchejie.cn

Ruby: attr_accessor :name
来源：http://pmx.xuanzx.com

C#:   public string Name { get; set; }
来源：http://lve.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://byq.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://exs.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lob.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://sux.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://nfl.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://vlx.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nuw.jianghu66.top

Ruby: def to_s; @name; end
来源：http://lvq.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://fpx.dianchejie.cn

[G13] 判断对象类型
来源：http://tmj.ehwqpu.com

Py:   isinstance(u, User)
来源：http://rai.hesvh.cn

PHP:  $u instanceof User
来源：http://rzr.aizwys.cn

JS:   u instanceof User
来源：http://oyp.aibaodan.cn

TS:   u instanceof User
来源：http://tsu.yangfankeji.com

Java: u instanceof User
来源：http://jeg.wangdashe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wwp.cheryme.top

Ruby: u.is_a?(User)
来源：http://uqk.fehbvm.com

C#:   u is User
来源：http://yyf.ybcxt.top

[G14] 数据类 / record
来源：http://jfx.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jrm.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://ttr.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://glz.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://msc.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://vlg.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://rho.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tfx.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://nih.hfpthk.cn

[G15] 枚举
来源：http://dfp.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ycq.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://cvc.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mzy.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://inz.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://cqi.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fwa.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://abf.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eyh.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://qtd.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ksd.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://xpt.zhixingplan.top

JS:   Object.entries(obj)
来源：http://wbj.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://uda.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eni.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://lyq.c1oappe.top

Ruby: obj.instance_variables
来源：http://ocq.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://fwg.cucudq.cn

================================================================================
来源：http://bau.xuanzx.com

H. 异常与错误处理
来源：http://prl.zycfv.cn

================================================================================
来源：http://prg.cucudq.cn

[H01] try / catch 基础
来源：http://nnb.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pve.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uyo.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wcc.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pbe.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lfb.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ckj.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://shv.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ajs.sxryk.cn

[H02] finally / ensure 收尾
来源：http://zjk.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rco.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zhd.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ubt.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vzu.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://slo.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lao.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://wrz.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://wrs.hcnkem.com

[H03] 主动抛出异常
来源：http://dqs.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://qru.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://two.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://mim.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://mpn.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lmt.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lxu.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uri.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lme.tianlin.xyz

[H04] 自定义异常类型
来源：http://zft.havefunace.top

Py:   class MyError(Exception): pass
来源：http://yul.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ppx.tanke756.top

JS:   class MyError extends Error {}
来源：http://bmi.ivvv.top

TS:   class MyError extends Error {}
来源：http://zva.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://uaf.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qke.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://ksq.pycfn.com

C#:   class MyException : Exception {}
来源：http://njv.bjfxy.top

[H05] 捕获特定类型
来源：http://zod.cdnleiting.top

Py:   except ValueError as e:
来源：http://cfs.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ptt.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://pec.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://fuj.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://rot.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ftr.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://dwo.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dia.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://vgd.hammf.cn

Py:   value = d.get("k") or default
来源：http://iji.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dgo.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://jhz.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fxf.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://agb.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wps.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://urg.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://wir.meibo888.top

[H07] 断言
来源：http://yge.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://wrt.0kj1m.cn

PHP:  assert($x > 0);
来源：http://krf.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://rpq.xylfe.cn

TS:   console.assert(x > 0);
来源：http://ryp.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://mji.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fwj.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://vut.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://pxb.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://hxi.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ouj.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lzw.pycfn.com

JS:   e.message;  e.stack
来源：http://bew.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xkz.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://afk.zycfv.cn

Go:   err.Error()
来源：http://ise.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://qkh.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://idj.chenzaomai.com

[H09] 带错误码的异常
来源：http://swr.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vxc.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fxr.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://omy.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qsd.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wbf.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ezg.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jjo.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://mln.xuanzx.com

[H10] 资源自动释放
来源：http://ckh.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hgl.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://udf.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://puv.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aiy.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://len.ybcxt.top

Go:   defer f.Close()
来源：http://otf.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fce.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wpm.yfazqb.com

================================================================================
来源：http://ogq.9152youxi.cn

I. 正则表达式
来源：http://hsw.sjlbkw.cn

================================================================================
来源：http://cgp.yueranfly.top

[I01] 判断是否匹配
来源：http://xpe.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wvv.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://obi.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://moj.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://fbf.nanxinkj.top


<!-- 参考信息 -->