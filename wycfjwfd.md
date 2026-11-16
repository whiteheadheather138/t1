代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yag.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yjm.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://htb.zhoulong.xyz

[F12] CSV 读写
来源：http://zkm.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yqv.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qed.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qzy.hongshengwenyu.top

TS:   // 同上
来源：http://mya.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wvh.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cye.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://utw.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://min.shanyushiyangtech.top

================================================================================
来源：http://ciq.yfazqb.com

G. 面向对象
来源：http://tat.hnxiangtu.top

================================================================================
来源：http://ved.hcnkem.com

[G01] 定义类
来源：http://cwa.zhoulong.xyz

Py:   class User: pass
来源：http://eze.shuidangran.top

PHP:  class User {}
来源：http://fwc.sjlbkw.cn

JS:   class User {}
来源：http://tke.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://yny.cqqwz.cn

Java: class User {}
来源：http://qwi.9152youxi.cn

Go:   type User struct { Name string }
来源：http://lng.yfazqb.com

Ruby: class User; end
来源：http://wqo.yueranfly.top

C#:   class User {}
来源：http://smh.fanxiaobao.xyz

[G02] 构造函数
来源：http://vbx.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://rdf.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://ebn.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://qmd.yj20258.top

TS:   constructor(public name: string) {}
来源：http://ohz.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://idh.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dub.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://kan.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://uac.hnqzz.top

[G03] 实例属性
来源：http://gqd.52xcode.cn

Py:   self.name = "x"
来源：http://ibd.sxryk.cn

PHP:  public string $name = "x";
来源：http://xoi.cashguo.top

JS:   this.name = "x";
来源：http://qjb.jinqigufen.top

TS:   name: string = "x";
来源：http://wjs.hnxiangtu.top

Java: private String name;
来源：http://prl.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xye.cashguo.top

Ruby: @name = "x"
来源：http://qds.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://stq.jianghu66.top

[G04] 定义方法
来源：http://swa.yuxming.cn

Py:   def greet(self): return self.name
来源：http://mbc.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uug.yangfankeji.com

JS:   greet() { return this.name; }
来源：http://iak.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://odd.tarul.cn

Java: String greet() { return name; }
来源：http://jiz.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xda.gogol.net.cn

Ruby: def greet; @name; end
来源：http://xxk.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://rrr.ivvv.top

[G05] 继承
来源：http://xzf.nwbrower.top

Py:   class Admin(User): pass
来源：http://ihk.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://exr.cheryme.top

JS:   class Admin extends User {}
来源：http://gbe.0kj1m.cn

TS:   class Admin extends User {}
来源：http://dqq.daxiang520.top

Java: class Admin extends User {}
来源：http://sol.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uvq.hcnkem.com

Ruby: class Admin < User; end
来源：http://soj.sxryk.cn

C#:   class Admin : User {}
来源：http://tby.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://ihp.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://jyr.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://ysp.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://nbk.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://jhg.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://irr.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wur.birdmap.top

Ruby: def greet; "admin"; end
来源：http://gat.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://lsf.yangfankeji.com

[G07] 调用父类方法
来源：http://vzc.xylfe.cn

Py:   super().greet()
来源：http://nqn.zhiwuduotai.top

PHP:  parent::greet();
来源：http://bbo.hywenlv.cn

JS:   super.greet();
来源：http://bmt.chenjidiqi.icu

TS:   super.greet();
来源：http://qtl.havefunace.top

Java: super.greet();
来源：http://mxm.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://stb.feifeiyinyue.top

Ruby: super
来源：http://ejy.hongshengwenyu.top

C#:   base.Greet();
来源：http://atg.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://qut.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://edc.bjfxy.top

PHP:  public static function f() {}
来源：http://zvi.shzxlz.cn

JS:   static f() {}
来源：http://smn.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://hmj.zdbjq.cn

Java: static void f() {}
来源：http://vxx.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vcr.yanxiufei.cn

Ruby: def self.f; end
来源：http://fos.hywenlv.cn

C#:   public static void F() {}
来源：http://rpl.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://djq.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://auc.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://qkb.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gab.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://bff.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://pbd.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://sor.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rgz.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://hjc.tian-w.cn

[G10] 访问控制
来源：http://zkx.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://ojn.meibo888.top

PHP:  public / protected / private
来源：http://yfi.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://fic.iojbl.cn

TS:   public / protected / private
来源：http://lhy.yonumen.top

Java: public / protected / private / 默认包级
来源：http://lfo.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://alu.316326.xyz

Ruby: public / protected / private
来源：http://oll.tianlin.xyz

C#:   public / protected / private / internal
来源：http://cyv.bbcook.cn

[G11] getter / setter
来源：http://fyb.uphjek.com

Py:   @property 与 @x.setter
来源：http://nsf.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xqf.sweek.top

JS:   get name() { return this._name; }
来源：http://ras.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://ufz.tarul.cn

Java: public String getName() { return name; }
来源：http://bhd.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fpm.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://rwi.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://atj.gzhubu.top

[G12] 对象转字符串
来源：http://kkq.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://lxz.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pkp.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://cjt.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://rmb.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://rpg.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xfb.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://cgi.yj202588.top

C#:   public override string ToString() => Name;
来源：http://lhl.bbcook.cn

[G13] 判断对象类型
来源：http://ykp.nanxinkj.top

Py:   isinstance(u, User)
来源：http://ejr.yonumen.top

PHP:  $u instanceof User
来源：http://krr.sjlbkw.cn

JS:   u instanceof User
来源：http://suc.xuetiantiany.cn

TS:   u instanceof User
来源：http://scv.yanxiufei.cn

Java: u instanceof User
来源：http://cki.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sec.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://fkg.ybcxt.top

C#:   u is User
来源：http://jvr.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://tzu.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ptz.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://yem.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://vne.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://rjb.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://uzk.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://kfs.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lon.cheryme.top

C#:   record User(string Name, int Age);
来源：http://pmt.zycfv.cn

[G15] 枚举
来源：http://exa.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xso.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://inb.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jwx.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mec.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://dzn.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://krw.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://txx.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ksz.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://bbi.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mgq.pycfn.com

PHP:  get_object_vars($obj);
来源：http://ljp.hcnkem.com

JS:   Object.entries(obj)
来源：http://qji.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://dnl.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wqs.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://adl.yuxming.cn

Ruby: obj.instance_variables
来源：http://fdv.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://lhz.9152youxi.cn

================================================================================
来源：http://koz.sxryk.cn

H. 异常与错误处理
来源：http://zrr.iojbl.cn

================================================================================
来源：http://wiy.yfazqb.com

[H01] try / catch 基础
来源：http://xay.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://swc.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xhf.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sby.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tuo.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uqs.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qjw.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hxr.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xbl.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://hvv.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://jcg.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pmk.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hnq.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tck.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://err.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://dki.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://moj.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fdw.yuanzhike.top

[H03] 主动抛出异常
来源：http://arr.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://nbn.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wuh.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://dtd.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://dfe.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wsn.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lbo.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aca.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://pls.gzhubu.top

[H04] 自定义异常类型
来源：http://siu.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://ert.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://itx.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://gnu.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://djf.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://tho.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oqv.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://kxu.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://pgn.kuanghao11.cn

[H05] 捕获特定类型
来源：http://mhm.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://vzr.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nel.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://yxs.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://rwe.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://gmw.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://omc.shangyingyoupin.top

Ruby: rescue ArgumentError => e
来源：http://fcj.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yvq.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://kpy.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://skz.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://dlq.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://ztl.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ogo.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nyw.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://kgr.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://lvw.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://aoo.c1oappe.top

[H07] 断言
来源：http://nkr.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://uaq.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://ikt.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://vou.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://ujz.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://fjz.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gco.vqdsnc.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wag.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://cvx.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://sxz.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://okr.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lym.shzxlz.cn

JS:   e.message;  e.stack
来源：http://uge.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://lsc.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tnr.gzhubu.top

Go:   err.Error()
来源：http://rpc.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://ymo.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://huy.yj20258888.top

[H09] 带错误码的异常
来源：http://jho.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jiz.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jnu.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nag.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://svt.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bjd.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://edf.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rps.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ppj.hnqzz.top

[H10] 资源自动释放
来源：http://idc.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://fjv.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cxg.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ltf.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gor.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hen.xuanzx.com

Go:   defer f.Close()
来源：http://jlr.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yoj.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jef.ehwqpu.com

================================================================================
来源：http://mja.guowangkeji.top

I. 正则表达式
来源：http://tgv.guowangkeji.top

================================================================================
来源：http://gcl.gogol.net.cn

[I01] 判断是否匹配
来源：http://vfj.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ykk.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://bxi.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://ugu.sweek.top

TS:   /\d+/.test(s)
来源：http://rba.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hvd.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bvb.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://irf.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vyf.52xcode.cn

[I02] 提取所有匹配
来源：http://zfk.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://yhj.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxo.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://exo.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://asc.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oqk.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uti.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://ddj.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://orx.zhixingplan.top

[I03] 提取捕获分组
来源：http://dad.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hzj.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uid.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jwz.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://shg.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xod.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ilh.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cmf.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wji.zdqjudy.top

[I04] 正则替换
来源：http://ljj.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qxq.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rvv.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tfg.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lst.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://hdw.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wzx.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xuy.xylfe.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sip.andypj.xyz

[I05] 按正则拆分
来源：http://jpq.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xzg.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://msv.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://qbx.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://hgb.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://pyg.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xpe.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ore.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://shi.ivvv.top


<!-- 参考信息 -->