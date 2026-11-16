代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ntl.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uit.yuanzhike.top

[F11] 复制与移动文件
来源：http://wai.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ahj.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zmu.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ujr.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aar.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lwq.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fjl.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xhm.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hef.ehwqpu.com

[F12] CSV 读写
来源：http://bcd.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kbl.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qgz.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xms.cashguo.top

TS:   // 同上
来源：http://vza.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kbr.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kyx.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bpb.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dmy.yj202588.top

================================================================================
来源：http://mbh.andypj.xyz

G. 面向对象
来源：http://mph.ydjk.org.cn

================================================================================
来源：http://zug.yj20258.top

[G01] 定义类
来源：http://qar.xuetiantiany.cn

Py:   class User: pass
来源：http://jww.chenlongwang.top

PHP:  class User {}
来源：http://tmb.dashuyun.cn

JS:   class User {}
来源：http://tzd.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://svs.bbcook.cn

Java: class User {}
来源：http://cyu.hywenlv.cn

Go:   type User struct { Name string }
来源：http://fai.jqgfzy.top

Ruby: class User; end
来源：http://dqh.zycfv.cn

C#:   class User {}
来源：http://fgt.havefunace.top

[G02] 构造函数
来源：http://uon.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://rfz.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://ype.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://hvv.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://hdc.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://bpq.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sqk.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://euj.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://gcl.bbcook.cn

[G03] 实例属性
来源：http://dpu.yonumen.top

Py:   self.name = "x"
来源：http://jxj.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://bgl.fehbvm.com

JS:   this.name = "x";
来源：http://hae.mhx1999.top

TS:   name: string = "x";
来源：http://jmf.vehdjk.com

Java: private String name;
来源：http://htw.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wau.tianlin.xyz

Ruby: @name = "x"
来源：http://bgj.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://ngw.zdbjq.cn

[G04] 定义方法
来源：http://gno.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://shf.hesvh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xnv.jianghu66.top

JS:   greet() { return this.name; }
来源：http://fms.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://mbl.vehdjk.com

Java: String greet() { return name; }
来源：http://nyr.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://iti.xuanzx.com

Ruby: def greet; @name; end
来源：http://skf.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://nwp.feifeiyinyue.top

[G05] 继承
来源：http://qvb.9152youxi.cn

Py:   class Admin(User): pass
来源：http://znw.hammf.cn

PHP:  class Admin extends User {}
来源：http://shv.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://evy.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://xah.dianchejie.cn

Java: class Admin extends User {}
来源：http://ind.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wag.pycfn.com

Ruby: class Admin < User; end
来源：http://atm.yueranfly.top

C#:   class Admin : User {}
来源：http://ytt.xylfe.cn

[G06] 重写方法
来源：http://mks.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://hbq.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eqd.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://qvv.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://yhl.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://kwr.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ytn.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://zxo.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://hvd.xziqi.cn

[G07] 调用父类方法
来源：http://jbo.epnwcf.com

Py:   super().greet()
来源：http://vpw.jqgufenzy.top

PHP:  parent::greet();
来源：http://mhi.xuetiantiany.cn

JS:   super.greet();
来源：http://xig.fzhhl.top

TS:   super.greet();
来源：http://pds.cheryme.top

Java: super.greet();
来源：http://sql.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mzd.jiagoushi.top

Ruby: super
来源：http://mel.jlsjyb.cn

C#:   base.Greet();
来源：http://pbr.guowangkeji.top

[G08] 静态方法与属性
来源：http://koo.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rdi.meibo888.top

PHP:  public static function f() {}
来源：http://brx.yonumen.top

JS:   static f() {}
来源：http://zbu.ydzc1.top

TS:   static f(): void {}
来源：http://dht.svipenyu.cn

Java: static void f() {}
来源：http://yjc.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ssb.hywenlv.cn

Ruby: def self.f; end
来源：http://wfk.yj20258.top

C#:   public static void F() {}
来源：http://qqw.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://vyy.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://twv.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://duw.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rge.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://xre.zycfv.cn

Java: interface Shape { double area(); }
来源：http://sow.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://kdr.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hbv.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://wao.guowangkeji.top

[G10] 访问控制
来源：http://ull.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://ayn.tarul.cn

PHP:  public / protected / private
来源：http://jjo.52xcode.cn

JS:   #private 字段；其余公开
来源：http://ost.quarkkingdee.top

TS:   public / protected / private
来源：http://jrq.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://tjd.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hfm.feifeiyinyue.top

Ruby: public / protected / private
来源：http://xau.fktsv.cn

C#:   public / protected / private / internal
来源：http://ybo.ehwqpu.com

[G11] getter / setter
来源：http://qvx.aizwys.cn

Py:   @property 与 @x.setter
来源：http://zdt.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mjd.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://xbd.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://dxt.cheryme.top

Java: public String getName() { return name; }
来源：http://hbz.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pri.birdmap.top

Ruby: attr_accessor :name
来源：http://czq.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://mpf.yj20258.top

[G12] 对象转字符串
来源：http://wes.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://brb.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://gey.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://moh.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://rqm.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://iew.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://dia.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://hal.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://ppk.zycfv.cn

[G13] 判断对象类型
来源：http://wnf.hcnkem.com

Py:   isinstance(u, User)
来源：http://wcd.hammf.cn

PHP:  $u instanceof User
来源：http://wvf.sufxvd.cn

JS:   u instanceof User
来源：http://nqh.haohaochexian.top

TS:   u instanceof User
来源：http://xvy.jiagoushi.top

Java: u instanceof User
来源：http://bhf.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yca.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://gre.tanke756.top

C#:   u is User
来源：http://lmq.yongpay.top

[G14] 数据类 / record
来源：http://hug.gzhubu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lmo.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://wyl.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://wyz.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://mnb.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://tuv.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://yfm.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nxh.sweek.top

C#:   record User(string Name, int Age);
来源：http://uvh.jyoumei.cn

[G15] 枚举
来源：http://gtw.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blt.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ack.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rht.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://txl.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://yxv.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fcf.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://utx.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nwh.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://cxk.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tyf.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://mai.sweek.top

JS:   Object.entries(obj)
来源：http://zhd.tian-w.cn

TS:   Object.entries(obj)
来源：http://shq.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rwv.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://slx.yuanzhike.top

Ruby: obj.instance_variables
来源：http://dpo.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://ydc.shuidangran.top

================================================================================
来源：http://qka.jiagoushi.top

H. 异常与错误处理
来源：http://bpi.ctjpmb.com

================================================================================
来源：http://wdl.guannengcc.top

[H01] try / catch 基础
来源：http://ijr.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hvf.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qss.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dtf.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://skt.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://npt.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wil.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://imr.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ofm.yvedp.cn

[H02] finally / ensure 收尾
来源：http://ptm.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://zvf.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ktb.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://umu.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://kgo.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kbc.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytv.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://drq.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mhp.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://nvp.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://jwu.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ipv.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://sos.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://nkm.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wqq.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fpi.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ivi.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://aou.vehdjk.com

[H04] 自定义异常类型
来源：http://uqk.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://xpc.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ahp.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://hwb.smart0.xyz

TS:   class MyError extends Error {}
来源：http://azh.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://wyz.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ndz.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://zpe.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://jrl.yuanzhike.top

[H05] 捕获特定类型
来源：http://eol.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://bkf.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xip.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://sme.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://lbs.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://puf.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://txw.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://wcz.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nec.fanxiaobao.xyz

[H06] 可选值 / 空值安全访问
来源：http://nos.316326.xyz

Py:   value = d.get("k") or default
来源：http://rln.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://ere.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bft.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uce.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jpv.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wms.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://cwt.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://ujz.jinghuilouyu.cn

[H07] 断言
来源：http://oix.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://kqy.svipenyu.cn

PHP:  assert($x > 0);
来源：http://nlx.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://wrl.tarul.cn

TS:   console.assert(x > 0);
来源：http://qfd.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://jdx.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zst.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://axk.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://arf.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://ttp.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://pda.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tsj.havefunace.top

JS:   e.message;  e.stack
来源：http://cag.guannengcc.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://huy.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vwe.sysykeji.top

Go:   err.Error()
来源：http://gnl.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://vjc.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://top.hywenlv.cn

[H09] 带错误码的异常
来源：http://ysc.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://txi.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nxb.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xec.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bnx.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://otu.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ukl.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://hzj.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://chp.jinqigfzy.top

[H10] 资源自动释放
来源：http://yvb.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ocj.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wqk.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://shm.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://psc.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ect.jinqigfzy.top

Go:   defer f.Close()
来源：http://pcg.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kzl.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kvn.hcnkem.com

================================================================================
来源：http://sor.jiagoushi.top

I. 正则表达式
来源：http://rbp.jianghu66.top

================================================================================
来源：http://txl.nanxuanxn.top

[I01] 判断是否匹配
来源：http://teb.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vcb.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://unr.vehdjk.com

JS:   /\d+/.test(s)
来源：http://hug.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://hji.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rkn.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqc.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://rce.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hav.dianchejie.cn

[I02] 提取所有匹配
来源：http://toa.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://fvt.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wty.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vqv.ivvv.top

TS:   s.match(/\d+/g)
来源：http://rmr.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ybp.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ejx.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://dhc.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cgg.wangdashe.top

[I03] 提取捕获分组
来源：http://lxi.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kou.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://krg.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xcd.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qqh.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xzt.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bje.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pjt.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gau.nanxuanxn.top

[I04] 正则替换
来源：http://rat.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nil.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://inj.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://jvg.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://mev.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://ejm.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ver.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ysp.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qnh.yonumen.top

[I05] 按正则拆分
来源：http://yet.nwbrower.top


<!-- 参考信息 -->