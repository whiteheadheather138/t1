代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tit.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://wdp.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pmo.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sdr.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mlp.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ahz.mhx1999.top

[F11] 复制与移动文件
来源：http://xhx.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jus.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xji.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sda.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdv.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gnc.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ldw.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gul.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zco.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://fhj.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vim.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ymu.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fzq.hysaishi.cn

TS:   // 同上
来源：http://csh.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xrp.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://npr.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fkf.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sdb.yangfankeji.com

================================================================================
来源：http://zsv.zhaomingkeji.xyz

G. 面向对象
来源：http://ewl.chenjidiqi.icu

================================================================================
来源：http://pss.daria6918.cn

[G01] 定义类
来源：http://xzu.havefunace.top

Py:   class User: pass
来源：http://xfg.0kj1m.cn

PHP:  class User {}
来源：http://yiz.shzxlz.cn

JS:   class User {}
来源：http://obr.hammf.cn

TS:   class User { name: string = ""; }
来源：http://oel.tianlin.xyz

Java: class User {}
来源：http://zpq.fengsongda.top

Go:   type User struct { Name string }
来源：http://ifd.shangyingyoupin.top

Ruby: class User; end
来源：http://uiy.yuanzhike.top

C#:   class User {}
来源：http://phu.birdmap.top

[G02] 构造函数
来源：http://aws.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://osf.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://xos.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://loa.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://lhc.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://qja.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tip.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://old.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://zox.redwolf501.top

[G03] 实例属性
来源：http://nnu.cdnleiting.top

Py:   self.name = "x"
来源：http://cjd.chenzaomai.com

PHP:  public string $name = "x";
来源：http://wuw.feifeiyinyue.top

JS:   this.name = "x";
来源：http://mui.redwolf501.top

TS:   name: string = "x";
来源：http://ulg.jlsjyb.cn

Java: private String name;
来源：http://kxt.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dzi.hywenlv.cn

Ruby: @name = "x"
来源：http://isu.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://cjm.shanyushiyangkeji.top

[G04] 定义方法
来源：http://rtc.jianghu66.top

Py:   def greet(self): return self.name
来源：http://uru.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://sxg.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://suj.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://sqp.ehwqpu.com

Java: String greet() { return name; }
来源：http://tal.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://voe.0kj1m.cn

Ruby: def greet; @name; end
来源：http://kqn.daxiang520.top

C#:   public string Greet() => Name;
来源：http://gzw.chenjidiqi.icu

[G05] 继承
来源：http://hmr.yongpay.top

Py:   class Admin(User): pass
来源：http://uwq.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://ggx.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://xnr.gotoacloud.top

TS:   class Admin extends User {}
来源：http://dyf.chenlongwang.top

Java: class Admin extends User {}
来源：http://dvi.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://imw.jqgfzy.top

Ruby: class Admin < User; end
来源：http://crq.yuanzhike.top

C#:   class Admin : User {}
来源：http://nec.cucudq.cn

[G06] 重写方法
来源：http://jjy.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://svc.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ltp.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://ocj.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://xjs.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://cwz.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pxl.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://mtx.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://ixp.yj20258888.top

[G07] 调用父类方法
来源：http://czy.guowangkeji.top

Py:   super().greet()
来源：http://zks.chenlongwang.top

PHP:  parent::greet();
来源：http://tbb.shzxlz.cn

JS:   super.greet();
来源：http://dsg.hnxiangtu.top

TS:   super.greet();
来源：http://qdg.hongshengwenyu.top

Java: super.greet();
来源：http://ekv.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kpo.svipenyu.cn

Ruby: super
来源：http://cre.sysykeji.top

C#:   base.Greet();
来源：http://djl.aibaodan.cn

[G08] 静态方法与属性
来源：http://mvw.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dzt.hnxiangtu.top

PHP:  public static function f() {}
来源：http://oiu.yj20258888.top

JS:   static f() {}
来源：http://cqw.sweek.top

TS:   static f(): void {}
来源：http://izm.yuanzhike.top

Java: static void f() {}
来源：http://avq.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jos.nanxinkj.top

Ruby: def self.f; end
来源：http://uzh.snrcjt.cn

C#:   public static void F() {}
来源：http://vuv.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://xch.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://fau.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://nbs.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://zkk.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://qda.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://nge.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://hiv.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mnc.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://pxq.xinyue.icu

[G10] 访问控制
来源：http://pee.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://owk.bjfxy.top

PHP:  public / protected / private
来源：http://nos.hesvh.cn

JS:   #private 字段；其余公开
来源：http://kep.jqgfzy.top

TS:   public / protected / private
来源：http://dzy.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://qtg.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jdp.dianchejie.cn

Ruby: public / protected / private
来源：http://pmy.fengsongda.top

C#:   public / protected / private / internal
来源：http://tbe.yueranfly.top

[G11] getter / setter
来源：http://igt.sxryk.cn

Py:   @property 与 @x.setter
来源：http://ehz.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dog.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://zzc.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://dqp.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://ahg.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fme.yueranfly.top

Ruby: attr_accessor :name
来源：http://taw.epnwcf.com

C#:   public string Name { get; set; }
来源：http://rwj.fzhhl.top

[G12] 对象转字符串
来源：http://qqx.meibo888.top

Py:   def __str__(self): return self.name
来源：http://fzy.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dyv.havefunace.top

JS:   toString() { return this.name; }
来源：http://tae.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://mbl.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://mjp.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nrz.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://hzq.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://qla.uphjek.com

[G13] 判断对象类型
来源：http://ibp.sweek.top

Py:   isinstance(u, User)
来源：http://ajv.yanxiufei.cn

PHP:  $u instanceof User
来源：http://wkz.fanxiaobao.xyz

JS:   u instanceof User
来源：http://dvs.zdbjq.cn

TS:   u instanceof User
来源：http://peh.ydzc1.top

Java: u instanceof User
来源：http://mgm.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pfh.wangdashe.top

Ruby: u.is_a?(User)
来源：http://yim.xinyue.icu

C#:   u is User
来源：http://xxa.chenlongwang.top

[G14] 数据类 / record
来源：http://hoh.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lfs.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://xph.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qyx.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://txj.haohaochexian.top

Java: record User(String name, int age) {}
来源：http://oqa.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://ekh.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dqo.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://zjq.epnwcf.com

[G15] 枚举
来源：http://cjl.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wah.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jgv.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tcv.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fek.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://hfh.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mgq.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://ekd.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rbp.cheryme.top

[G16] 对象转数组 / 字典
来源：http://eew.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iid.hammf.cn

PHP:  get_object_vars($obj);
来源：http://uot.hysaishi.cn

JS:   Object.entries(obj)
来源：http://rxz.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://mss.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ssb.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zbd.xylfe.cn

Ruby: obj.instance_variables
来源：http://brz.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://icw.zhongyouzk.top

================================================================================
来源：http://ysm.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://wsr.sweek.top

================================================================================
来源：http://trc.yueranfly.top

[H01] try / catch 基础
来源：http://oca.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://juu.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qig.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xpp.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mvh.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bwt.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lcv.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vyc.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qjj.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://nbe.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://llg.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rlq.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://vnm.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vao.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tow.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ren.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ayy.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fiu.kuanghao11.cn

[H03] 主动抛出异常
来源：http://ols.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://zpk.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oze.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://uvm.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://rzc.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tcf.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://byw.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nuh.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://xhl.yuanzhike.top

[H04] 自定义异常类型
来源：http://nxl.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://gyi.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://dby.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://jbr.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://wvs.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://anl.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cpu.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://uaa.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://ptx.jianghu66.top

[H05] 捕获特定类型
来源：http://hqu.daria6918.cn

Py:   except ValueError as e:
来源：http://wso.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bti.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://jng.shzxlz.cn

TS:   if (e instanceof TypeError) {}
来源：http://dlt.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://ume.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cxo.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://xsl.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zrn.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://deu.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://anc.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://npu.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://xdz.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://rad.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xkl.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zdo.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://bbt.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://bab.wangdashe.top

[H07] 断言
来源：http://idk.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://tfe.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://oxw.yj202588.top

JS:   console.assert(x > 0);
来源：http://fyp.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://fba.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://ynm.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://noh.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://vin.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://qxt.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://bhq.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://tnx.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rbr.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://qpm.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ghc.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uqh.meibo888.top

Go:   err.Error()
来源：http://bow.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://uze.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://mcq.dianchejie.cn

[H09] 带错误码的异常
来源：http://vvg.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ihs.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ykg.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bjx.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vnp.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tvh.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vag.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://lii.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gjp.jlsjyb.cn

[H10] 资源自动释放
来源：http://qbx.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kyl.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fsx.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://duh.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://plo.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zuj.zhongyouzk.top

Go:   defer f.Close()
来源：http://rdk.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wve.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://imu.daxiang520.top

================================================================================
来源：http://rxd.xuanzx.com

I. 正则表达式
来源：http://fhw.jlsjyb.cn

================================================================================
来源：http://iao.gaohongyu789.top

[I01] 判断是否匹配
来源：http://ztm.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nfd.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://suz.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://nqe.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://dzv.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hha.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dfd.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://ugk.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://esh.epnwcf.com

[I02] 提取所有匹配
来源：http://cyf.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://yim.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ckl.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xky.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://vme.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rms.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://als.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://fuu.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vjy.hywenlv.cn

[I03] 提取捕获分组
来源：http://ljy.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vgg.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qzw.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jny.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ltu.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gia.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xrv.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hor.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xxm.gogol.net.cn

[I04] 正则替换
来源：http://qql.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lps.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qma.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://amh.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lfi.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uej.zhijiandao.cn


<!-- 参考信息 -->