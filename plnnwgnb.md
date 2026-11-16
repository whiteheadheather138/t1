代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aim.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gsw.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dbn.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nur.fzhhl.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aqg.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fou.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pus.xuanzx.com

[F12] CSV 读写
来源：http://kys.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rfq.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jdc.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zzj.cashguo.top

TS:   // 同上
来源：http://yae.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uxy.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lcn.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xpi.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://utr.pengpengdd.cyou

================================================================================
来源：http://eer.xylfe.cn

G. 面向对象
来源：http://znq.daxiang520.top

================================================================================
来源：http://kfl.ehwqpu.com

[G01] 定义类
来源：http://sty.ydjk.org.cn

Py:   class User: pass
来源：http://mme.yueranfly.top

PHP:  class User {}
来源：http://wli.shangyingyoupin.top

JS:   class User {}
来源：http://xem.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://ycr.jinghuilouyu.cn

Java: class User {}
来源：http://dsy.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://hiv.hywenlv.cn

Ruby: class User; end
来源：http://vha.yueranfly.top

C#:   class User {}
来源：http://tzu.dianchejie.cn

[G02] 构造函数
来源：http://axf.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://cfv.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://wjz.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://uxi.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://txu.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://xoz.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://okq.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://jol.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://gpk.uphjek.com

[G03] 实例属性
来源：http://bid.chenzaomai.com

Py:   self.name = "x"
来源：http://mkn.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://zyj.yanxiufei.cn

JS:   this.name = "x";
来源：http://veb.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://djr.yonumen.top

Java: private String name;
来源：http://bus.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gqh.jlsjyb.cn

Ruby: @name = "x"
来源：http://wmj.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://nlb.zhengqikj.top

[G04] 定义方法
来源：http://umv.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://ldp.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hit.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://gfh.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://hgi.guowangkeji.top

Java: String greet() { return name; }
来源：http://hjo.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jgr.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://fry.cashguo.top

C#:   public string Greet() => Name;
来源：http://fog.zhixingplan.top

[G05] 继承
来源：http://zzj.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://zqo.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://tml.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://twc.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://hem.redwolf501.top

Java: class Admin extends User {}
来源：http://tvt.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tgv.yj20258.top

Ruby: class Admin < User; end
来源：http://tfq.sxryk.cn

C#:   class Admin : User {}
来源：http://abd.aizwys.cn

[G06] 重写方法
来源：http://vdk.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://sgk.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://nyv.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://umj.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://wiq.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://xuy.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wrm.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://isz.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://nuw.cashguo.top

[G07] 调用父类方法
来源：http://cbz.ydjk.org.cn

Py:   super().greet()
来源：http://lpa.gaohongyu789.top

PHP:  parent::greet();
来源：http://wad.tarul.cn

JS:   super.greet();
来源：http://mji.52xcode.cn

TS:   super.greet();
来源：http://dbx.havefunace.top

Java: super.greet();
来源：http://rbt.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fcp.sxryk.cn

Ruby: super
来源：http://jok.c1oappe.top

C#:   base.Greet();
来源：http://djc.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://kxa.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uxl.svipenyu.cn

PHP:  public static function f() {}
来源：http://mar.svipenyu.cn

JS:   static f() {}
来源：http://vdz.jinqigfzy.top

TS:   static f(): void {}
来源：http://snq.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://zdd.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://mhp.xinyue.icu

Ruby: def self.f; end
来源：http://fim.shangyingyoupin.top

C#:   public static void F() {}
来源：http://pak.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://vlg.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ygg.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://rpc.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kvz.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://bnt.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://hsm.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://vpt.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zbk.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://opp.haohaochexian.top

[G10] 访问控制
来源：http://awu.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://ioe.svipenyu.cn

PHP:  public / protected / private
来源：http://ibt.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://ntk.hesvh.cn

TS:   public / protected / private
来源：http://srg.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://bey.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://flg.yanxiufei.cn

Ruby: public / protected / private
来源：http://frw.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://sma.quarkkingdee.top

[G11] getter / setter
来源：http://nhd.epnwcf.com

Py:   @property 与 @x.setter
来源：http://fiz.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jqh.smart0.xyz

JS:   get name() { return this._name; }
来源：http://xse.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://rly.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://fyb.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bfi.yuanzhike.top

Ruby: attr_accessor :name
来源：http://hrp.bjfxy.top

C#:   public string Name { get; set; }
来源：http://qut.cheryme.top

[G12] 对象转字符串
来源：http://sqg.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://bhk.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mjw.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://vhi.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://cwf.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://ybx.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uvb.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://ehb.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://sta.iojbl.cn

[G13] 判断对象类型
来源：http://rux.gzhubu.top

Py:   isinstance(u, User)
来源：http://pgh.epnwcf.com

PHP:  $u instanceof User
来源：http://gka.wangdashe.top

JS:   u instanceof User
来源：http://jbk.yueranfly.top

TS:   u instanceof User
来源：http://gii.zycfv.cn

Java: u instanceof User
来源：http://xfg.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kyq.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://occ.feifeiyinyue.top

C#:   u is User
来源：http://vtg.sufxvd.cn

[G14] 数据类 / record
来源：http://hxt.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lqd.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://sfq.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://gvk.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://nbw.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://pmg.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://kco.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://koz.birdmap.top

C#:   record User(string Name, int Age);
来源：http://nwq.ywan-chungtsiang.top

[G15] 枚举
来源：http://yin.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rgr.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oxy.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://obc.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rjb.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://hkq.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sby.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://evu.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xjg.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://nyq.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jlj.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://lwl.hnxiangtu.top

JS:   Object.entries(obj)
来源：http://rro.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://cwj.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://djv.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://cry.aizwys.cn

Ruby: obj.instance_variables
来源：http://czw.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://pad.aizwys.cn

================================================================================
来源：http://kbv.snrcjt.cn

H. 异常与错误处理
来源：http://cvs.jinyuanbaomall.cn

================================================================================
来源：http://ocq.daxiang520.top

[H01] try / catch 基础
来源：http://zja.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://whs.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kek.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://boc.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lvp.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hfm.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zco.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://doq.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hqd.jianghu66.top

[H02] finally / ensure 收尾
来源：http://ytl.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lad.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yit.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://pjs.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://lhj.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://xrc.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ocy.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hob.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qql.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://tzw.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://dhh.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://azr.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://cqb.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://zfn.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zoe.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aff.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ykh.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wpj.gotoacloud.top

[H04] 自定义异常类型
来源：http://qjq.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://hfh.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nza.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://ctm.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://nss.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://zzu.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rva.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://csh.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://sgo.xinyue.icu

[H05] 捕获特定类型
来源：http://wsa.ivvv.top

Py:   except ValueError as e:
来源：http://kdb.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dac.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://roe.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://uzb.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://bdt.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mst.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://hfw.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zpm.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://ayb.aizwys.cn

Py:   value = d.get("k") or default
来源：http://wze.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://fad.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://tuv.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://xww.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xqm.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ddo.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://wwl.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://vum.jlsjyb.cn

[H07] 断言
来源：http://lsf.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://usx.fehbvm.com

PHP:  assert($x > 0);
来源：http://wvb.meibo888.top

JS:   console.assert(x > 0);
来源：http://ffi.meibo888.top

TS:   console.assert(x > 0);
来源：http://dad.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://yce.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nln.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ypg.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://eqa.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://rwk.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://ljn.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ycv.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://vil.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://afd.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pmo.hnxiangtu.top

Go:   err.Error()
来源：http://jow.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://fgq.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://kut.hywenlv.cn

[H09] 带错误码的异常
来源：http://oey.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://phv.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fot.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://huz.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gju.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nfs.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ctk.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://grh.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oda.aizwys.cn

[H10] 资源自动释放
来源：http://cuf.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xzl.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pdl.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tqe.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://imi.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xvw.sjlbkw.cn

Go:   defer f.Close()
来源：http://usu.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://plw.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uoj.zdbjq.cn

================================================================================
来源：http://pzx.andypj.xyz

I. 正则表达式
来源：http://ocl.ydjk.org.cn

================================================================================
来源：http://shg.yj20258888.top

[I01] 判断是否匹配
来源：http://kol.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cin.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://beb.316326.xyz

JS:   /\d+/.test(s)
来源：http://ecl.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://lxo.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qyt.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://myf.sweek.top

Ruby: s.match?(/\d+/)
来源：http://xvu.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bfx.aizwys.cn

[I02] 提取所有匹配
来源：http://itu.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://ada.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nyt.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ist.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://ipv.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zfn.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vpn.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://bjw.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ijg.dianchejie.cn

[I03] 提取捕获分组
来源：http://piq.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jka.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hmi.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://efv.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kqo.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fkq.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cbm.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nxk.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ihz.jinyuanbaomall.cn

[I04] 正则替换
来源：http://ivw.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lrx.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hzo.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zpc.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://dck.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://coc.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://imu.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://iro.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jxy.daria6918.cn

[I05] 按正则拆分
来源：http://zxc.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://obv.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://maa.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://tmb.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://wuo.tianlin.xyz


<!-- 参考信息 -->