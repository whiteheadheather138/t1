代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://amo.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dvv.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dpl.9152youxi.cn

[F12] CSV 读写
来源：http://ull.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yrz.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rhl.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ufi.havefunace.top

TS:   // 同上
来源：http://smu.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zvc.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tav.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fnz.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://koq.cdnleiting.top

================================================================================
来源：http://xhw.snrcjt.cn

G. 面向对象
来源：http://cie.chenjidiqi.icu

================================================================================
来源：http://rju.yanxiufei.cn

[G01] 定义类
来源：http://kxn.sufxvd.cn

Py:   class User: pass
来源：http://jsx.zhengqikj.top

PHP:  class User {}
来源：http://oot.birdmap.top

JS:   class User {}
来源：http://jjm.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://pld.nwbrower.top

Java: class User {}
来源：http://uqz.meibo888.top

Go:   type User struct { Name string }
来源：http://ory.yj20258888.top

Ruby: class User; end
来源：http://qai.c1oappe.top

C#:   class User {}
来源：http://bmk.vehdjk.com

[G02] 构造函数
来源：http://cpa.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://owi.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://wfs.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://trr.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://ipk.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://yqm.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iap.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://ucj.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://spw.yonumen.top

[G03] 实例属性
来源：http://hto.vehdjk.com

Py:   self.name = "x"
来源：http://onu.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://shu.ivvv.top

JS:   this.name = "x";
来源：http://ybx.kuanghao11.cn

TS:   name: string = "x";
来源：http://hho.hesvh.cn

Java: private String name;
来源：http://tus.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dmb.yj20258888.top

Ruby: @name = "x"
来源：http://wdh.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://ycw.gzhubu.top

[G04] 定义方法
来源：http://kjn.bbcook.cn

Py:   def greet(self): return self.name
来源：http://pxq.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ylc.iojbl.cn

JS:   greet() { return this.name; }
来源：http://pbr.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://hsh.sjlbkw.cn

Java: String greet() { return name; }
来源：http://plq.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fid.hywenlv.cn

Ruby: def greet; @name; end
来源：http://mwn.cheryme.top

C#:   public string Greet() => Name;
来源：http://byo.sxryk.cn

[G05] 继承
来源：http://mhu.zdbjq.cn

Py:   class Admin(User): pass
来源：http://foy.ydzc1.top

PHP:  class Admin extends User {}
来源：http://kvm.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://kwk.sxryk.cn

TS:   class Admin extends User {}
来源：http://ohn.cashguo.top

Java: class Admin extends User {}
来源：http://ery.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fjf.snrcjt.cn

Ruby: class Admin < User; end
来源：http://bfq.hnxiangtu.top

C#:   class Admin : User {}
来源：http://fxj.ywan-chungtsiang.top

[G06] 重写方法
来源：http://hjd.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://kkl.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://epn.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://jxv.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://mei.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://qty.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kmz.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://owt.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://ejc.xuetiantiany.cn

[G07] 调用父类方法
来源：http://nzq.nwbrower.top

Py:   super().greet()
来源：http://zsr.aizwys.cn

PHP:  parent::greet();
来源：http://qex.zhixingplan.top

JS:   super.greet();
来源：http://qmk.jqgufenzy.top

TS:   super.greet();
来源：http://mpo.shzxlz.cn

Java: super.greet();
来源：http://tae.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wcb.ivvv.top

Ruby: super
来源：http://zbx.tian-w.cn

C#:   base.Greet();
来源：http://dqt.fengsongda.top

[G08] 静态方法与属性
来源：http://xef.hywenlv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ppg.ehwqpu.com

PHP:  public static function f() {}
来源：http://qrc.aibaodan.cn

JS:   static f() {}
来源：http://ifl.ydjk.org.cn

TS:   static f(): void {}
来源：http://ach.zhaomingkeji.xyz

Java: static void f() {}
来源：http://gbm.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://bmh.yonumen.top

Ruby: def self.f; end
来源：http://sqt.jlsjyb.cn

C#:   public static void F() {}
来源：http://bpb.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://yzt.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://xlz.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://apl.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qbf.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://wjn.sysykeji.top

Java: interface Shape { double area(); }
来源：http://okx.smart0.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ftt.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fsn.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://dlq.fanxiaobao.xyz

[G10] 访问控制
来源：http://xbm.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://mjl.0kj1m.cn

PHP:  public / protected / private
来源：http://ilc.hnqzz.top

JS:   #private 字段；其余公开
来源：http://ifo.tarul.cn

TS:   public / protected / private
来源：http://sln.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://tla.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sjy.jinqigfzy.top

Ruby: public / protected / private
来源：http://knw.52xcode.cn

C#:   public / protected / private / internal
来源：http://uev.cdnleiting.top

[G11] getter / setter
来源：http://jfs.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://tym.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sqg.epnwcf.com

JS:   get name() { return this._name; }
来源：http://hqo.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://atp.xylfe.cn

Java: public String getName() { return name; }
来源：http://akd.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wot.tianlin.xyz

Ruby: attr_accessor :name
来源：http://hja.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://ufl.zycfv.cn

[G12] 对象转字符串
来源：http://ops.cashguo.top

Py:   def __str__(self): return self.name
来源：http://fhu.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://byz.hnqzz.top

JS:   toString() { return this.name; }
来源：http://ggu.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://jak.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://vuw.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ube.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://nwz.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://xll.redwolf501.top

[G13] 判断对象类型
来源：http://afq.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://sic.jyoumei.cn

PHP:  $u instanceof User
来源：http://uur.sysykeji.top

JS:   u instanceof User
来源：http://zzs.dianchejie.cn

TS:   u instanceof User
来源：http://pri.sweek.top

Java: u instanceof User
来源：http://vvu.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gid.316326.xyz

Ruby: u.is_a?(User)
来源：http://sng.jiagoushi.top

C#:   u is User
来源：http://cpn.xinyue.icu

[G14] 数据类 / record
来源：http://jvs.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hvm.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://anq.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://sjd.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://ywy.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://eub.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://qsk.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mmv.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://iaw.fktsv.cn

[G15] 枚举
来源：http://hbk.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hjx.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://itd.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mwc.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://opy.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://eyt.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xlx.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://kqm.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kvm.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://gtv.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ttw.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://fch.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://gko.zycfv.cn

TS:   Object.entries(obj)
来源：http://eiz.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ayd.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yqn.yueranfly.top

Ruby: obj.instance_variables
来源：http://ahx.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://kbk.yj202588.top

================================================================================
来源：http://bcw.0kj1m.cn

H. 异常与错误处理
来源：http://tsy.ppjwa.cn

================================================================================
来源：http://pfu.fengsongda.top

[H01] try / catch 基础
来源：http://fil.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ovs.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iss.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qqa.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wqt.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hiw.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://irl.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ven.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xrq.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://daf.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://yjz.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cdb.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bhi.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nxm.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yyy.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://axs.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://slb.bbcook.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uau.wangdashe.top

[H03] 主动抛出异常
来源：http://vcy.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://jbd.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oqr.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://jnq.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://jat.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ghn.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://umt.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rgh.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://fhn.hysaishi.cn

[H04] 自定义异常类型
来源：http://kst.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://gfe.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://oya.c1oappe.top

JS:   class MyError extends Error {}
来源：http://gvb.sweek.top

TS:   class MyError extends Error {}
来源：http://sdx.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://eam.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tdv.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://hnh.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://tdd.52xcode.cn

[H05] 捕获特定类型
来源：http://obo.guannengcc.top

Py:   except ValueError as e:
来源：http://dbt.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gxf.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://jlv.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://kds.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://rzo.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sfw.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://gkf.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://suf.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://rlw.tian-w.cn

Py:   value = d.get("k") or default
来源：http://rsf.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rzy.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://txq.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://anr.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qpk.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eri.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://vvt.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://fjo.wangdashe.top

[H07] 断言
来源：http://qsd.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://cgk.fktsv.cn

PHP:  assert($x > 0);
来源：http://uzn.hnqzz.top

JS:   console.assert(x > 0);
来源：http://xcq.bjfxy.top

TS:   console.assert(x > 0);
来源：http://uft.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://cxi.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hnr.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://hfg.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://kdf.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://khy.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://vdw.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fsa.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://kcc.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://aye.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pzi.xuetiantiany.cn

Go:   err.Error()
来源：http://izv.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://ysk.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://xtq.tanke756.top

[H09] 带错误码的异常
来源：http://paf.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fxf.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://szp.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ctb.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fcf.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bzf.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hlq.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://isz.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ioq.wangshuangyany.cn

[H10] 资源自动释放
来源：http://sng.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cfd.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mvf.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://piq.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://djp.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://huf.gotoacloud.top

Go:   defer f.Close()
来源：http://flh.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jli.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dmz.birdmap.top

================================================================================
来源：http://bcw.yongpay.top

I. 正则表达式
来源：http://njy.0kj1m.cn

================================================================================
来源：http://rjw.cheryme.top

[I01] 判断是否匹配
来源：http://cou.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yyn.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://upa.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://spz.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://zmt.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dxu.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wfs.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://lbh.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vnf.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://bfr.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://usw.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jyh.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jpg.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://czk.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rdf.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ldu.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://azw.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vnf.aibaodan.cn

[I03] 提取捕获分组
来源：http://ogv.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iek.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jch.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lmk.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ahf.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hfn.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pku.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wxi.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://odq.zdqjudy.top

[I04] 正则替换
来源：http://zhq.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://znf.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oza.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://wwk.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://jhb.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://rbt.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wsl.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qul.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://erq.wangshuangyany.cn

[I05] 按正则拆分
来源：http://cur.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://czs.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hwk.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://xrm.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://qci.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://jpq.316326.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hgg.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://pmp.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wru.fzhhl.top


<!-- 参考信息 -->