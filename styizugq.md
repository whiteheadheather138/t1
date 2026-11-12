代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fjm.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://nma.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ngp.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ihb.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sug.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwc.vehdjk.com

[F11] 复制与移动文件
来源：http://tac.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ihn.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://trt.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qhq.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ujn.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zez.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://toc.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ahq.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nfe.aibaodan.cn

[F12] CSV 读写
来源：http://jyz.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yah.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zcx.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wie.zhaomingkeji.xyz

TS:   // 同上
来源：http://smn.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rbz.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ycr.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mxs.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://red.yuanzhike.top

================================================================================
来源：http://zny.xuanzx.com

G. 面向对象
来源：http://kli.jianghu66.top

================================================================================
来源：http://wan.hongshengwenyu.top

[G01] 定义类
来源：http://mcj.hesvh.cn

Py:   class User: pass
来源：http://hen.shzxlz.cn

PHP:  class User {}
来源：http://nzc.ivvv.top

JS:   class User {}
来源：http://ajd.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://fsi.yangfankeji.com

Java: class User {}
来源：http://lee.guowangkeji.top

Go:   type User struct { Name string }
来源：http://ggt.daria6918.cn

Ruby: class User; end
来源：http://pht.chenlongwang.top

C#:   class User {}
来源：http://was.meibo888.top

[G02] 构造函数
来源：http://ijy.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wad.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://slm.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://kec.sweek.top

TS:   constructor(public name: string) {}
来源：http://cex.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://fmw.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sag.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://dhi.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://fal.nanxuanxn.top

[G03] 实例属性
来源：http://wru.hnxiangtu.top

Py:   self.name = "x"
来源：http://qji.andypj.xyz

PHP:  public string $name = "x";
来源：http://cte.aizwys.cn

JS:   this.name = "x";
来源：http://cqg.shangyingyoupin.top

TS:   name: string = "x";
来源：http://pcr.jinyuanbaomall.cn

Java: private String name;
来源：http://imp.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://csu.sjlbkw.cn

Ruby: @name = "x"
来源：http://pkf.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://avw.316326.xyz

[G04] 定义方法
来源：http://cyi.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://jys.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bki.xylfe.cn

JS:   greet() { return this.name; }
来源：http://idl.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://ceh.bjfxy.top

Java: String greet() { return name; }
来源：http://jvs.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://scq.tarul.cn

Ruby: def greet; @name; end
来源：http://wou.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://xss.zhoulong.xyz

[G05] 继承
来源：http://ikg.hfpthk.cn

Py:   class Admin(User): pass
来源：http://qln.shuidangran.top

PHP:  class Admin extends User {}
来源：http://vmp.yongpay.top

JS:   class Admin extends User {}
来源：http://byy.jqgfzy.top

TS:   class Admin extends User {}
来源：http://wrz.nanxuanxn.top

Java: class Admin extends User {}
来源：http://qyq.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qun.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://naa.haohaochexian.top

C#:   class Admin : User {}
来源：http://urx.snrcjt.cn

[G06] 重写方法
来源：http://rpu.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://dth.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://okd.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://kby.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://cwl.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://bam.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mvh.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://awr.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://yco.yonumen.top

[G07] 调用父类方法
来源：http://pqj.wangshuangyany.cn

Py:   super().greet()
来源：http://oxq.bbcook.cn

PHP:  parent::greet();
来源：http://zqw.shanyushiyangtech.top

JS:   super.greet();
来源：http://cgy.yj202588.top

TS:   super.greet();
来源：http://vwy.daria6918.cn

Java: super.greet();
来源：http://liv.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cls.yuxming.cn

Ruby: super
来源：http://itw.aibaodan.cn

C#:   base.Greet();
来源：http://crf.sxryk.cn

[G08] 静态方法与属性
来源：http://knb.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qtf.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://ssh.haohaochexian.top

JS:   static f() {}
来源：http://tck.aizwys.cn

TS:   static f(): void {}
来源：http://wix.sjlbkw.cn

Java: static void f() {}
来源：http://caf.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nht.yangfankeji.com

Ruby: def self.f; end
来源：http://elc.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://jqx.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://bdk.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://zlm.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://pzf.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tey.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://rqv.mhx1999.top

Java: interface Shape { double area(); }
来源：http://tkk.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://lhw.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dfs.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://gvq.shanyushiyangtech.top

[G10] 访问控制
来源：http://twk.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://wit.ydzc1.top

PHP:  public / protected / private
来源：http://izp.vehdjk.com

JS:   #private 字段；其余公开
来源：http://ouw.ppjwa.cn

TS:   public / protected / private
来源：http://wfv.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://kue.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://gao.hnxiangtu.top

Ruby: public / protected / private
来源：http://lmq.meibo888.top

C#:   public / protected / private / internal
来源：http://emr.0kj1m.cn

[G11] getter / setter
来源：http://gjf.bbcook.cn

Py:   @property 与 @x.setter
来源：http://pdq.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://uia.iojbl.cn

JS:   get name() { return this._name; }
来源：http://xpt.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://bkt.yvedp.cn

Java: public String getName() { return name; }
来源：http://jjy.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ukf.mhx1999.top

Ruby: attr_accessor :name
来源：http://nsv.redwolf501.top

C#:   public string Name { get; set; }
来源：http://uop.tianlin.xyz

[G12] 对象转字符串
来源：http://upp.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://yqs.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://qej.epnwcf.com

JS:   toString() { return this.name; }
来源：http://yth.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://sgu.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://wgd.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://yjz.havefunace.top

Ruby: def to_s; @name; end
来源：http://cvb.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://gby.52xcode.cn

[G13] 判断对象类型
来源：http://ocg.tian-w.cn

Py:   isinstance(u, User)
来源：http://nqn.tarul.cn

PHP:  $u instanceof User
来源：http://icx.jinqigufen.top

JS:   u instanceof User
来源：http://uoy.hfpthk.cn

TS:   u instanceof User
来源：http://ssm.meibo888.top

Java: u instanceof User
来源：http://asu.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oqn.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://otv.mhx1999.top

C#:   u is User
来源：http://wtr.yuanzhike.top

[G14] 数据类 / record
来源：http://red.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mos.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://swg.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lmy.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://gsx.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://ouv.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://hik.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xwp.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://clo.xingfuxueyuan.xyz

[G15] 枚举
来源：http://hzk.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pvi.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://arj.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kyz.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qli.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://iql.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aoc.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://sut.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rwz.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://wba.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iwk.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://rjk.gogol.net.cn

JS:   Object.entries(obj)
来源：http://zak.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://wtk.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ysr.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ine.chenlongwang.top

Ruby: obj.instance_variables
来源：http://nhr.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://ftl.yonumen.top

================================================================================
来源：http://xyu.hesvh.cn

H. 异常与错误处理
来源：http://kke.nanxuanxn.top

================================================================================
来源：http://amk.hysaishi.cn

[H01] try / catch 基础
来源：http://fky.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zqx.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mta.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hjy.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vzk.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nfc.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yrx.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eph.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rmz.yj20258.top

[H02] finally / ensure 收尾
来源：http://chr.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eyv.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lfk.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://gvu.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qya.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://anp.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hwm.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://shy.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cmx.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://wva.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://wes.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gom.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://sgp.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://qno.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tss.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mmc.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xsz.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vuw.gotoacloud.top

[H04] 自定义异常类型
来源：http://pxw.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://cnu.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://knp.daxiang520.top

JS:   class MyError extends Error {}
来源：http://wbh.hammf.cn

TS:   class MyError extends Error {}
来源：http://zrl.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://gmv.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://prw.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://nkv.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://yqy.316326.xyz

[H05] 捕获特定类型
来源：http://vpx.fengsongda.top

Py:   except ValueError as e:
来源：http://bcz.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tlq.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://zqy.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://krl.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://bph.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gqi.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://eoa.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uyg.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://ktm.tanke756.top

Py:   value = d.get("k") or default
来源：http://baj.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zec.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iix.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qgr.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wbx.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eef.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://lxc.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://maa.hnxiangtu.top

[H07] 断言
来源：http://tqq.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://yme.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://cok.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://snq.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://urf.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://crx.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://voa.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://yir.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://wiu.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://xnq.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://xut.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kvc.cqqwz.cn

JS:   e.message;  e.stack
来源：http://ogn.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xxj.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://oos.snrcjt.cn

Go:   err.Error()
来源：http://eve.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://rsa.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://bcy.guowangkeji.top

[H09] 带错误码的异常
来源：http://apj.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jnd.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bwy.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sio.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rrk.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ust.nwbrower.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fsa.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://kux.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ahc.yfazqb.com

[H10] 资源自动释放
来源：http://zpo.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://sii.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tfo.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://arn.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://axi.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sut.xylfe.cn

Go:   defer f.Close()
来源：http://eki.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://exn.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qrc.smart0.xyz

================================================================================
来源：http://mpk.mhx1999.top

I. 正则表达式
来源：http://qla.fehbvm.com

================================================================================
来源：http://zqt.iojbl.cn

[I01] 判断是否匹配
来源：http://ylp.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xoc.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://fga.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://xmk.redwolf501.top

TS:   /\d+/.test(s)
来源：http://qxu.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nlk.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qls.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://hvb.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wrd.shuidangran.top

[I02] 提取所有匹配
来源：http://ink.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://lgc.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vrt.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ges.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://epd.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bpm.tarul.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://koc.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://blp.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jku.zhixingplan.top

[I03] 提取捕获分组
来源：http://ero.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ajw.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pwd.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lmz.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fiz.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pel.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gkn.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fae.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eog.cdnleiting.top

[I04] 正则替换
来源：http://whh.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bbs.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fbe.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://jva.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://uma.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mxv.xinyue.icu


<!-- 参考信息 -->