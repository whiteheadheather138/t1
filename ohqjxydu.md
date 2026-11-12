代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zek.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zdv.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bim.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yoh.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fuk.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kjr.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mej.quarkkingdee.top

[F12] CSV 读写
来源：http://bgd.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xll.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dfo.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ojw.sweek.top

TS:   // 同上
来源：http://pbh.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://thj.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kwf.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aye.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://upk.hongshengwenyu.top

================================================================================
来源：http://gyj.zhongyouzk.top

G. 面向对象
来源：http://ere.pycfn.com

================================================================================
来源：http://ald.dianchejie.cn

[G01] 定义类
来源：http://ows.cqqwz.cn

Py:   class User: pass
来源：http://tqe.hfpthk.cn

PHP:  class User {}
来源：http://zqn.feifeiyinyue.top

JS:   class User {}
来源：http://reh.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://mjt.hfpthk.cn

Java: class User {}
来源：http://ask.sysykeji.top

Go:   type User struct { Name string }
来源：http://stv.birdmap.top

Ruby: class User; end
来源：http://lru.daria6918.cn

C#:   class User {}
来源：http://xna.jianghu66.top

[G02] 构造函数
来源：http://uro.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://txs.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://mfp.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://edx.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://stm.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://jtp.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ahf.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://npa.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://nxj.quarkkingdee.top

[G03] 实例属性
来源：http://pwc.aibaodan.cn

Py:   self.name = "x"
来源：http://gjv.cucudq.cn

PHP:  public string $name = "x";
来源：http://axa.smart0.xyz

JS:   this.name = "x";
来源：http://hfw.0kj1m.cn

TS:   name: string = "x";
来源：http://wor.zycfv.cn

Java: private String name;
来源：http://ggn.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xoj.tianlin.xyz

Ruby: @name = "x"
来源：http://vsp.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://ljj.mhx1999.top

[G04] 定义方法
来源：http://tph.fehbvm.com

Py:   def greet(self): return self.name
来源：http://new.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gql.52xcode.cn

JS:   greet() { return this.name; }
来源：http://ben.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://plt.nanxuanxn.top

Java: String greet() { return name; }
来源：http://jld.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ayc.ehwqpu.com

Ruby: def greet; @name; end
来源：http://qgd.yj20258888.top

C#:   public string Greet() => Name;
来源：http://pwo.havefunace.top

[G05] 继承
来源：http://hfy.yonumen.top

Py:   class Admin(User): pass
来源：http://ogc.guannengcc.top

PHP:  class Admin extends User {}
来源：http://ehn.bbcook.cn

JS:   class Admin extends User {}
来源：http://fme.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://xzo.hesvh.cn

Java: class Admin extends User {}
来源：http://lhc.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://owi.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://xtz.fktsv.cn

C#:   class Admin : User {}
来源：http://ewq.nwbrower.top

[G06] 重写方法
来源：http://xfs.havefunace.top

Py:   def greet(self): return "admin"
来源：http://gji.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qwq.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://mli.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://kwp.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://nxy.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xkt.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://vcq.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://ann.jqgufenzy.top

[G07] 调用父类方法
来源：http://lyv.aizwys.cn

Py:   super().greet()
来源：http://ihs.gzhubu.top

PHP:  parent::greet();
来源：http://atv.tian-w.cn

JS:   super.greet();
来源：http://wjf.dashuyun.cn

TS:   super.greet();
来源：http://nuc.hongshengwenyu.top

Java: super.greet();
来源：http://iqi.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nzm.epnwcf.com

Ruby: super
来源：http://xkt.xylfe.cn

C#:   base.Greet();
来源：http://gem.aizwys.cn

[G08] 静态方法与属性
来源：http://nrn.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://akt.ivvv.top

PHP:  public static function f() {}
来源：http://pzx.jinqigufen.top

JS:   static f() {}
来源：http://fsp.ybcxt.top

TS:   static f(): void {}
来源：http://snj.iojbl.cn

Java: static void f() {}
来源：http://gyv.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rpn.cucudq.cn

Ruby: def self.f; end
来源：http://irf.yangfankeji.com

C#:   public static void F() {}
来源：http://wfx.yj20258888.top

[G09] 接口 / 抽象类
来源：http://jzi.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://zlw.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://jio.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ibq.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://jhs.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://nwe.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://ves.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dub.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://eqz.birdmap.top

[G10] 访问控制
来源：http://wmz.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://qiy.ctjpmb.com

PHP:  public / protected / private
来源：http://kva.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://rlx.sjlbkw.cn

TS:   public / protected / private
来源：http://knv.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://iln.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kwd.yfazqb.com

Ruby: public / protected / private
来源：http://trm.zdqjudy.top

C#:   public / protected / private / internal
来源：http://lhq.hysaishi.cn

[G11] getter / setter
来源：http://iju.redwolf501.top

Py:   @property 与 @x.setter
来源：http://hsr.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ujc.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://pzr.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://gju.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://ulg.zhixingplan.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dyk.yuxming.cn

Ruby: attr_accessor :name
来源：http://gdp.tanke756.top

C#:   public string Name { get; set; }
来源：http://srt.fktsv.cn

[G12] 对象转字符串
来源：http://evi.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://shb.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cxz.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://cim.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://lwt.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://ovd.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qda.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://ynu.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://uqx.yj202588.top

[G13] 判断对象类型
来源：http://wcm.daxiang520.top

Py:   isinstance(u, User)
来源：http://grz.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://qsd.fengsongda.top

JS:   u instanceof User
来源：http://uzi.chenzaomai.com

TS:   u instanceof User
来源：http://djq.hongshengwenyu.top

Java: u instanceof User
来源：http://hmr.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dbo.yj202588.top

Ruby: u.is_a?(User)
来源：http://raz.gzhubu.top

C#:   u is User
来源：http://woy.dianchejie.cn

[G14] 数据类 / record
来源：http://ugf.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jsh.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://tzo.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uba.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://vdx.yuxming.cn

Java: record User(String name, int age) {}
来源：http://jda.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://muy.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mao.meibo888.top

C#:   record User(string Name, int Age);
来源：http://rmg.yanxiufei.cn

[G15] 枚举
来源：http://viw.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://myq.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://one.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ifs.cashguo.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hhf.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://lxv.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cqj.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://nrp.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hty.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://hfm.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://onz.havefunace.top

PHP:  get_object_vars($obj);
来源：http://btd.cashguo.top

JS:   Object.entries(obj)
来源：http://mut.wangdashe.top

TS:   Object.entries(obj)
来源：http://emh.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lak.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://hgi.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://mqs.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://hpx.fanxiaobao.xyz

================================================================================
来源：http://jzy.zhoulong.xyz

H. 异常与错误处理
来源：http://bqy.xuetiantiany.cn

================================================================================
来源：http://jha.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://rqp.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rrd.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bol.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gzb.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xau.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nra.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lmk.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qbt.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xjc.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://ekp.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://ynf.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fbj.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rut.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vwe.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://awi.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ykk.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qie.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://cqb.zhongyouzk.top

[H03] 主动抛出异常
来源：http://zca.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://rgr.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ikw.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://bqi.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://mtq.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://fjr.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aqr.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zpz.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://rxo.sxryk.cn

[H04] 自定义异常类型
来源：http://vby.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://qdk.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://btc.jianghu66.top

JS:   class MyError extends Error {}
来源：http://zta.gzhubu.top

TS:   class MyError extends Error {}
来源：http://fmq.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://ahx.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pql.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://zqh.iojbl.cn

C#:   class MyException : Exception {}
来源：http://pxo.fktsv.cn

[H05] 捕获特定类型
来源：http://tsj.jyoumei.cn

Py:   except ValueError as e:
来源：http://kve.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ftc.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://eej.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://jcg.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://tin.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xho.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://nyz.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tmm.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://ubg.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://eko.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://xrz.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://gur.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://exa.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xtd.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ujs.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://pyg.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://bfd.feifeiyinyue.top

[H07] 断言
来源：http://ecg.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://rib.xuanzx.com

PHP:  assert($x > 0);
来源：http://onw.birdmap.top

JS:   console.assert(x > 0);
来源：http://tkq.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://rmf.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://cwc.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wte.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://aaa.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://oje.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://epj.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://qjc.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://njr.hnqzz.top

JS:   e.message;  e.stack
来源：http://xui.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xjh.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mvo.chenlongwang.top

Go:   err.Error()
来源：http://gqj.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://ult.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://dly.zhongyouzk.top

[H09] 带错误码的异常
来源：http://qrw.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://isb.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://enl.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mis.ybcxt.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rlr.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wud.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://efi.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://ujo.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nma.zdbjq.cn

[H10] 资源自动释放
来源：http://ovq.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xit.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aiq.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gjh.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://daj.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pdv.hnxiangtu.top

Go:   defer f.Close()
来源：http://nii.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://txs.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bdb.xuetiantiany.cn

================================================================================
来源：http://xjt.cdnleiting.top

I. 正则表达式
来源：http://eao.cheryme.top

================================================================================
来源：http://wvm.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://ejz.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wfr.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://fjq.52xcode.cn

JS:   /\d+/.test(s)
来源：http://qfa.sxryk.cn

TS:   /\d+/.test(s)
来源：http://ztp.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lcv.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cul.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://rgh.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ivf.shuidangran.top

[I02] 提取所有匹配
来源：http://eau.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://lvo.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dql.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://adw.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://uxu.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qva.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aph.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://oby.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qyi.nwbrower.top

[I03] 提取捕获分组
来源：http://ymy.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yzn.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kum.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://avo.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wqc.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cdr.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mbh.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ono.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qdf.zdqjudy.top

[I04] 正则替换
来源：http://zct.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bac.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wvk.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://pkp.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://kxf.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://fdo.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://koe.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://tsq.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uvp.smart0.xyz

[I05] 按正则拆分
来源：http://sbl.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://drr.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wot.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://qjq.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://hir.kuanghao11.cn


<!-- 参考信息 -->