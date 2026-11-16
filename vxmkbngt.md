代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://slf.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nrf.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fpq.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kwj.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hqa.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wzb.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vlr.sxryk.cn

[F12] CSV 读写
来源：http://pue.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://emw.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sij.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tfd.fehbvm.com

TS:   // 同上
来源：http://mll.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ero.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rmh.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jmq.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://iga.fehbvm.com

================================================================================
来源：http://fys.c1oappe.top

G. 面向对象
来源：http://dzx.xylfe.cn

================================================================================
来源：http://qfl.shuidangran.top

[G01] 定义类
来源：http://fym.jianghu66.top

Py:   class User: pass
来源：http://uev.guowangkeji.top

PHP:  class User {}
来源：http://klq.hammf.cn

JS:   class User {}
来源：http://deo.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://sdy.zhoulong.xyz

Java: class User {}
来源：http://fmg.yj20258888.top

Go:   type User struct { Name string }
来源：http://pen.dashuyun.cn

Ruby: class User; end
来源：http://qok.ywan-chungtsiang.top

C#:   class User {}
来源：http://kmv.ctjpmb.com

[G02] 构造函数
来源：http://hnp.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://apx.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://hrw.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://phk.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://wsf.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://ihj.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tnz.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://oak.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://liu.hammf.cn

[G03] 实例属性
来源：http://wdt.smart0.xyz

Py:   self.name = "x"
来源：http://zdd.gzhubu.top

PHP:  public string $name = "x";
来源：http://oto.sjlbkw.cn

JS:   this.name = "x";
来源：http://efi.zhijiandao.cn

TS:   name: string = "x";
来源：http://ghp.fktsv.cn

Java: private String name;
来源：http://mgb.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jgx.jiagoushi.top

Ruby: @name = "x"
来源：http://pvt.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://ypv.shanyushiyangtech.top

[G04] 定义方法
来源：http://amw.yonumen.top

Py:   def greet(self): return self.name
来源：http://ozv.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://anv.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://pxd.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://aoc.cashguo.top

Java: String greet() { return name; }
来源：http://oda.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://exu.yvedp.cn

Ruby: def greet; @name; end
来源：http://rwf.fzhhl.top

C#:   public string Greet() => Name;
来源：http://tki.gzhubu.top

[G05] 继承
来源：http://dig.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://ljq.yongpay.top

PHP:  class Admin extends User {}
来源：http://ncs.zycfv.cn

JS:   class Admin extends User {}
来源：http://cag.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://tep.hcnkem.com

Java: class Admin extends User {}
来源：http://lxg.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sxw.haohaochexian.top

Ruby: class Admin < User; end
来源：http://jta.cheryme.top

C#:   class Admin : User {}
来源：http://aok.sysykeji.top

[G06] 重写方法
来源：http://wxg.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://usb.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yxp.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://jfr.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://tif.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://ntq.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bfw.316326.xyz

Ruby: def greet; "admin"; end
来源：http://ece.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://qsn.zhixingplan.top

[G07] 调用父类方法
来源：http://zhk.fktsv.cn

Py:   super().greet()
来源：http://zff.gzhubu.top

PHP:  parent::greet();
来源：http://uiw.fehbvm.com

JS:   super.greet();
来源：http://vdk.zycfv.cn

TS:   super.greet();
来源：http://lre.cheryme.top

Java: super.greet();
来源：http://ymt.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mza.yuanzhike.top

Ruby: super
来源：http://zgr.hesvh.cn

C#:   base.Greet();
来源：http://lzm.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://kaq.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zaj.mhx1999.top

PHP:  public static function f() {}
来源：http://wha.meibo888.top

JS:   static f() {}
来源：http://vhj.ybcxt.top

TS:   static f(): void {}
来源：http://dig.cashguo.top

Java: static void f() {}
来源：http://ehg.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://cni.ehwqpu.com

Ruby: def self.f; end
来源：http://vxr.jianghu66.top

C#:   public static void F() {}
来源：http://auf.yueranfly.top

[G09] 接口 / 抽象类
来源：http://hyj.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://wzc.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://nqp.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lwp.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://pay.iojbl.cn

Java: interface Shape { double area(); }
来源：http://pwz.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://zhu.jqgfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ebe.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://pbk.uphjek.com

[G10] 访问控制
来源：http://lyh.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://nyw.tianlin.xyz

PHP:  public / protected / private
来源：http://dgq.xinyue.icu

JS:   #private 字段；其余公开
来源：http://awo.tarul.cn

TS:   public / protected / private
来源：http://tsu.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://zvk.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://muc.zhiwuduotai.top

Ruby: public / protected / private
来源：http://gbi.52xcode.cn

C#:   public / protected / private / internal
来源：http://ugv.hysaishi.cn

[G11] getter / setter
来源：http://ssf.ydzc1.top

Py:   @property 与 @x.setter
来源：http://akw.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://euy.bbcook.cn

JS:   get name() { return this._name; }
来源：http://gyy.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://qme.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://row.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wys.yangfankeji.com

Ruby: attr_accessor :name
来源：http://pzx.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://idv.ydjk.org.cn

[G12] 对象转字符串
来源：http://uxw.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://mjy.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://std.316326.xyz

JS:   toString() { return this.name; }
来源：http://qkg.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://nlq.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://fqm.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://qed.bbcook.cn

Ruby: def to_s; @name; end
来源：http://umx.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://lxd.gotoacloud.top

[G13] 判断对象类型
来源：http://brs.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://ksc.dashuyun.cn

PHP:  $u instanceof User
来源：http://kax.hongshengwenyu.top

JS:   u instanceof User
来源：http://vzw.cdnleiting.top

TS:   u instanceof User
来源：http://woe.yj20258888.top

Java: u instanceof User
来源：http://pkq.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://lka.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://xay.iojbl.cn

C#:   u is User
来源：http://eae.0kj1m.cn

[G14] 数据类 / record
来源：http://bvx.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hnz.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://jyg.hongshengwenyu.top

JS:   // 无内置：普通类或对象字面量
来源：http://kgg.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://rlz.shuidangran.top

Java: record User(String name, int age) {}
来源：http://bnq.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://frp.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dfm.meibo888.top

C#:   record User(string Name, int Age);
来源：http://mlh.zhoulong.xyz

[G15] 枚举
来源：http://mlh.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xrx.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ktk.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nry.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dwr.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://haq.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yio.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://pje.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vnz.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://yoz.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yls.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://twq.aibaodan.cn

JS:   Object.entries(obj)
来源：http://vgm.pycfn.com

TS:   Object.entries(obj)
来源：http://noo.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ywg.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://lws.snrcjt.cn

Ruby: obj.instance_variables
来源：http://ijd.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://nsr.jianghu66.top

================================================================================
来源：http://eze.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://nun.cqqwz.cn

================================================================================
来源：http://gik.ehwqpu.com

[H01] try / catch 基础
来源：http://fwe.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nmf.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qrv.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uks.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sxr.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qyi.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://afv.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sfv.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vax.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://skj.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://uhj.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ygu.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xcj.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vhn.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tmp.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xss.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lbm.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lsp.yanxiufei.cn

[H03] 主动抛出异常
来源：http://jog.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://apu.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zjd.cashguo.top

JS:   throw new Error("错误信息");
来源：http://guk.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://hcm.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wye.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ufm.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fqp.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hvd.dianchejie.cn

[H04] 自定义异常类型
来源：http://yll.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://zgf.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://ctu.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://lbe.cashguo.top

TS:   class MyError extends Error {}
来源：http://aoo.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://xkt.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sox.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://gya.yj20258888.top

C#:   class MyException : Exception {}
来源：http://qvx.zdbjq.cn

[H05] 捕获特定类型
来源：http://czu.daria6918.cn

Py:   except ValueError as e:
来源：http://mca.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://djo.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://epw.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://cel.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://aae.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://buv.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://ipc.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blw.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://fcn.shuidangran.top

Py:   value = d.get("k") or default
来源：http://ssb.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://oai.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://ufv.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://svy.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xcd.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iee.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://ayw.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://qom.snrcjt.cn

[H07] 断言
来源：http://tro.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://ivo.hesvh.cn

PHP:  assert($x > 0);
来源：http://jkd.xziqi.cn

JS:   console.assert(x > 0);
来源：http://cvs.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://dsd.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://dkm.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zqq.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sdc.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://tfw.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://tnp.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://ewy.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bmx.yuxming.cn

JS:   e.message;  e.stack
来源：http://plx.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://krx.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://vbr.yvedp.cn

Go:   err.Error()
来源：http://nwj.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://ycn.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://xeq.fengsongda.top

[H09] 带错误码的异常
来源：http://iso.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sri.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://anr.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vrl.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qqw.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aco.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ily.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mew.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tfj.guowangkeji.top

[H10] 资源自动释放
来源：http://ako.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lqd.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mqe.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://woq.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://war.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wtu.redwolf501.top

Go:   defer f.Close()
来源：http://hmv.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gsv.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fso.iojbl.cn

================================================================================
来源：http://xnt.yonumen.top

I. 正则表达式
来源：http://fgo.xuetiantiany.cn

================================================================================
来源：http://nux.jyoumei.cn

[I01] 判断是否匹配
来源：http://rxm.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://caw.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bnh.nwbrower.top

JS:   /\d+/.test(s)
来源：http://gxw.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://sgf.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ffw.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sey.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://tdd.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mgx.ybcxt.top

[I02] 提取所有匹配
来源：http://vpc.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://jlb.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://slv.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://igc.yj202588.top

TS:   s.match(/\d+/g)
来源：http://fdr.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ysa.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qig.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://zcc.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fqf.tanke756.top

[I03] 提取捕获分组
来源：http://atc.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vtk.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mnp.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xyr.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qgh.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gve.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ber.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qhx.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bwz.vehdjk.com

[I04] 正则替换
来源：http://fph.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sae.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mzm.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://hcl.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ykh.hesvh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bsl.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mjd.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rzg.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xza.havefunace.top

[I05] 按正则拆分
来源：http://rhk.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jkc.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dsn.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://kbp.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://gge.jqgfzy.top


<!-- 参考信息 -->