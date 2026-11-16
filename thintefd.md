代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://crg.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vai.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tra.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://fle.fehbvm.com

================================================================================
来源：http://yru.sweek.top

G. 面向对象
来源：http://kif.bbcook.cn

================================================================================
来源：http://wlb.cqqwz.cn

[G01] 定义类
来源：http://prm.yj202588.top

Py:   class User: pass
来源：http://rfd.jinyuanbaomall.cn

PHP:  class User {}
来源：http://txd.guowangkeji.top

JS:   class User {}
来源：http://san.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://vjr.316326.xyz

Java: class User {}
来源：http://tkt.52xcode.cn

Go:   type User struct { Name string }
来源：http://jaa.yfazqb.com

Ruby: class User; end
来源：http://fqp.jqgufenzy.top

C#:   class User {}
来源：http://fez.yonumen.top

[G02] 构造函数
来源：http://tjh.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://wwm.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://guj.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://pmv.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://ycb.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://knk.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://axv.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://uob.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://bbj.chenzaomai.com

[G03] 实例属性
来源：http://ffv.yj20258.top

Py:   self.name = "x"
来源：http://gty.andypj.xyz

PHP:  public string $name = "x";
来源：http://auz.yonumen.top

JS:   this.name = "x";
来源：http://geb.uphjek.com

TS:   name: string = "x";
来源：http://nsw.feifeiyinyue.top

Java: private String name;
来源：http://akl.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nqk.9152youxi.cn

Ruby: @name = "x"
来源：http://wzt.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://fbg.snrcjt.cn

[G04] 定义方法
来源：http://piq.zycfv.cn

Py:   def greet(self): return self.name
来源：http://its.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bhx.yj20258.top

JS:   greet() { return this.name; }
来源：http://oew.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://cxj.zhijiandao.cn

Java: String greet() { return name; }
来源：http://cmv.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lzk.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://qlc.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://rpw.pycfn.com

[G05] 继承
来源：http://cdv.sweek.top

Py:   class Admin(User): pass
来源：http://jkv.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://nvc.xuanzx.com

JS:   class Admin extends User {}
来源：http://mok.redwolf501.top

TS:   class Admin extends User {}
来源：http://kzp.quarkkingdee.top

Java: class Admin extends User {}
来源：http://chn.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nau.316326.xyz

Ruby: class Admin < User; end
来源：http://iww.yongpay.top

C#:   class Admin : User {}
来源：http://mfd.dashuyun.cn

[G06] 重写方法
来源：http://oqd.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://gwe.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xua.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://qdr.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://pgg.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://wjb.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ifk.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://mzh.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://pab.jqgfzy.top

[G07] 调用父类方法
来源：http://xyr.tarul.cn

Py:   super().greet()
来源：http://zzj.shuidangran.top

PHP:  parent::greet();
来源：http://odd.birdmap.top

JS:   super.greet();
来源：http://dwk.jinqigufen.top

TS:   super.greet();
来源：http://ojg.jyoumei.cn

Java: super.greet();
来源：http://sle.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hpj.xylfe.cn

Ruby: super
来源：http://cbt.hywenlv.cn

C#:   base.Greet();
来源：http://cui.tarul.cn

[G08] 静态方法与属性
来源：http://zqk.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hhl.daria6918.cn

PHP:  public static function f() {}
来源：http://akq.bbcook.cn

JS:   static f() {}
来源：http://gat.ydjk.org.cn

TS:   static f(): void {}
来源：http://lvu.ctjpmb.com

Java: static void f() {}
来源：http://kjq.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wke.jiagoushi.top

Ruby: def self.f; end
来源：http://hio.fzhhl.top

C#:   public static void F() {}
来源：http://por.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://esy.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://mlf.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pta.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xbm.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://oqb.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://gwc.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://yeo.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hng.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://sah.gotoacloud.top

[G10] 访问控制
来源：http://ftw.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://qde.zhoulong.xyz

PHP:  public / protected / private
来源：http://qek.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://njw.yonumen.top

TS:   public / protected / private
来源：http://rpi.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://lot.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sem.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://mgk.316326.xyz

C#:   public / protected / private / internal
来源：http://dgm.tian-w.cn

[G11] getter / setter
来源：http://ubb.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://bmj.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://rze.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://tcm.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://pwo.chenlongwang.top

Java: public String getName() { return name; }
来源：http://qfl.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sde.havefunace.top

Ruby: attr_accessor :name
来源：http://dhb.yj202588.top

C#:   public string Name { get; set; }
来源：http://jbg.0kj1m.cn

[G12] 对象转字符串
来源：http://mok.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://abu.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mys.andypj.xyz

JS:   toString() { return this.name; }
来源：http://vba.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://auj.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://zsq.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://tks.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://bna.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://jgh.zhiwuduotai.top

[G13] 判断对象类型
来源：http://enm.c1oappe.top

Py:   isinstance(u, User)
来源：http://cub.tianlin.xyz

PHP:  $u instanceof User
来源：http://vme.nwbrower.top

JS:   u instanceof User
来源：http://ddq.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://byb.daxiang520.top

Java: u instanceof User
来源：http://eju.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sei.aizwys.cn

Ruby: u.is_a?(User)
来源：http://nuj.fehbvm.com

C#:   u is User
来源：http://iug.gzhubu.top

[G14] 数据类 / record
来源：http://wty.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://snz.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://qgr.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nmt.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://yxp.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://oay.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://myj.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cjt.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://ato.sjlbkw.cn

[G15] 枚举
来源：http://twc.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vng.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oer.andypj.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vdg.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tkf.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://zmj.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zhs.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://ifq.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rvm.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://thu.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://min.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://lws.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://pwa.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://prq.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lin.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hoi.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://ueu.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ntj.vehdjk.com

================================================================================
来源：http://qdg.sufxvd.cn

H. 异常与错误处理
来源：http://shp.shzxlz.cn

================================================================================
来源：http://gpg.chenlongwang.top

[H01] try / catch 基础
来源：http://fcf.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://izp.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fpn.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cmw.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wln.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fnw.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zis.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cma.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dik.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://vfm.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rtt.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lyk.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bqr.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pnq.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wiq.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ppb.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rcj.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://igw.ydzc1.top

[H03] 主动抛出异常
来源：http://gjp.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://nbn.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://now.hammf.cn

JS:   throw new Error("错误信息");
来源：http://syq.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://zuw.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://dap.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://duo.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zeh.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://prz.hfpthk.cn

[H04] 自定义异常类型
来源：http://twn.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://bek.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://lct.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://mco.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://blz.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://gjc.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bha.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://isz.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://pxy.xylfe.cn

[H05] 捕获特定类型
来源：http://acf.hesvh.cn

Py:   except ValueError as e:
来源：http://nod.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://suz.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://bed.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://yen.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ulg.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eri.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://vcx.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vin.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://yzb.bbcook.cn

Py:   value = d.get("k") or default
来源：http://ivg.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://wms.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://veu.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://eau.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oxo.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dnq.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://ehs.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://noz.jianghu66.top

[H07] 断言
来源：http://aqk.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://wlh.cucudq.cn

PHP:  assert($x > 0);
来源：http://stk.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://vcp.cashguo.top

TS:   console.assert(x > 0);
来源：http://aaq.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://trc.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nif.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cab.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://iny.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://hcz.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://rfh.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://czd.9152youxi.cn

JS:   e.message;  e.stack
来源：http://gxx.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://svi.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vzj.zhixingplan.top

Go:   err.Error()
来源：http://fsu.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://mvl.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://rvh.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://yon.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ofi.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://muy.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xry.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ukw.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wlz.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ynf.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://poh.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://toe.cucudq.cn

[H10] 资源自动释放
来源：http://mcj.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ysj.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ckv.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tfm.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tcc.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jer.gotoacloud.top

Go:   defer f.Close()
来源：http://icr.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zzp.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zud.zhongyouzk.top

================================================================================
来源：http://dgx.zhixingplan.top

I. 正则表达式
来源：http://hbe.bjfxy.top

================================================================================
来源：http://ohq.zdqjudy.top

[I01] 判断是否匹配
来源：http://cgo.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://way.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://etc.xuanzx.com

JS:   /\d+/.test(s)
来源：http://cbe.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://lcp.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hyk.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ppj.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://kha.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tca.jinqigfzy.top

[I02] 提取所有匹配
来源：http://jxa.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://dyf.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kfy.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jtk.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://esf.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://snz.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://omo.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://eiw.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://utj.smart0.xyz

[I03] 提取捕获分组
来源：http://szv.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bkp.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rzu.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ydj.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ajw.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://apd.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wzg.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ywl.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hxw.andypj.xyz

[I04] 正则替换
来源：http://tke.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://syw.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ndd.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://gyo.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://cpn.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://xtf.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://syt.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mgi.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dnr.nwbrower.top

[I05] 按正则拆分
来源：http://jln.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zyo.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tdj.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://hfp.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://hdl.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://avs.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qdp.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://flf.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pjd.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mtj.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ajn.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ztb.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hop.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://prk.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bzj.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pem.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pro.yueranfly.top


<!-- 参考信息 -->