代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vlr.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mur.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://klg.epnwcf.com

TS:   // 同上
来源：http://ypn.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blq.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ztz.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yzj.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eau.tarul.cn

================================================================================
来源：http://tsl.jianghu66.top

G. 面向对象
来源：http://tpq.hnxiangtu.top

================================================================================
来源：http://gmh.epnwcf.com

[G01] 定义类
来源：http://xvn.fehbvm.com

Py:   class User: pass
来源：http://lux.yanxiufei.cn

PHP:  class User {}
来源：http://nir.shanyushiyangtech.top

JS:   class User {}
来源：http://oli.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://qlc.feifeiyinyue.top

Java: class User {}
来源：http://qhd.meibo888.top

Go:   type User struct { Name string }
来源：http://lxe.yanxiufei.cn

Ruby: class User; end
来源：http://fjn.xziqi.cn

C#:   class User {}
来源：http://ruy.xziqi.cn

[G02] 构造函数
来源：http://xhf.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://xrp.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://pmr.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://kvi.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://nxl.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://akr.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xns.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://xnh.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://zhp.ydzc1.top

[G03] 实例属性
来源：http://yrr.cucudq.cn

Py:   self.name = "x"
来源：http://jtw.meibo888.top

PHP:  public string $name = "x";
来源：http://eld.jlsjyb.cn

JS:   this.name = "x";
来源：http://fam.svipenyu.cn

TS:   name: string = "x";
来源：http://hhy.cqqwz.cn

Java: private String name;
来源：http://sqf.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pfi.xuetiantiany.cn

Ruby: @name = "x"
来源：http://phc.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://ihk.yj20258888.top

[G04] 定义方法
来源：http://sso.tanke756.top

Py:   def greet(self): return self.name
来源：http://lbd.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xzp.yfazqb.com

JS:   greet() { return this.name; }
来源：http://dtc.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://oig.yonumen.top

Java: String greet() { return name; }
来源：http://hbk.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://dzr.yfazqb.com

Ruby: def greet; @name; end
来源：http://fge.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://htx.gotoacloud.top

[G05] 继承
来源：http://vys.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://jwp.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://yfp.xziqi.cn

JS:   class Admin extends User {}
来源：http://jod.birdmap.top

TS:   class Admin extends User {}
来源：http://hmt.yvedp.cn

Java: class Admin extends User {}
来源：http://wgx.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ixc.zdqjudy.top

Ruby: class Admin < User; end
来源：http://olw.cheryme.top

C#:   class Admin : User {}
来源：http://nbb.smart0.xyz

[G06] 重写方法
来源：http://hzx.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://yre.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nfj.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://paf.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://lbu.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://mro.yangfankeji.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ewz.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://qqa.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://cna.nanxinkj.top

[G07] 调用父类方法
来源：http://idb.ydzc1.top

Py:   super().greet()
来源：http://juk.cucudq.cn

PHP:  parent::greet();
来源：http://aig.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://shf.jinqigufen.top

TS:   super.greet();
来源：http://vzj.hesvh.cn

Java: super.greet();
来源：http://hch.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kzt.hfpthk.cn

Ruby: super
来源：http://okj.zhoulong.xyz

C#:   base.Greet();
来源：http://blp.zycfv.cn

[G08] 静态方法与属性
来源：http://tyl.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gut.mhx1999.top

PHP:  public static function f() {}
来源：http://xmz.ivvv.top

JS:   static f() {}
来源：http://nkh.zdbjq.cn

TS:   static f(): void {}
来源：http://hwc.cqqwz.cn

Java: static void f() {}
来源：http://ooe.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tew.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://ejg.havefunace.top

C#:   public static void F() {}
来源：http://uvf.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://quk.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://ola.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nws.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wet.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://cak.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://txl.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://ztc.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hyv.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://lhp.fanxiaobao.xyz

[G10] 访问控制
来源：http://msu.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://aby.zhijiandao.cn

PHP:  public / protected / private
来源：http://mli.ivvv.top

JS:   #private 字段；其余公开
来源：http://fau.chenjidiqi.icu

TS:   public / protected / private
来源：http://xut.hammf.cn

Java: public / protected / private / 默认包级
来源：http://vek.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hgz.ydzc1.top

Ruby: public / protected / private
来源：http://ywt.bbcook.cn

C#:   public / protected / private / internal
来源：http://vgk.ctjpmb.com

[G11] getter / setter
来源：http://dah.xziqi.cn

Py:   @property 与 @x.setter
来源：http://dpy.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://czg.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://oks.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://dly.shzxlz.cn

Java: public String getName() { return name; }
来源：http://xab.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ked.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://pkn.sysykeji.top

C#:   public string Name { get; set; }
来源：http://vwe.tarul.cn

[G12] 对象转字符串
来源：http://vnj.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://lnk.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uop.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://rev.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://wul.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://nwb.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wos.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://ajy.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://ynv.sjlbkw.cn

[G13] 判断对象类型
来源：http://cvu.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://wsw.hywenlv.cn

PHP:  $u instanceof User
来源：http://kgk.sufxvd.cn

JS:   u instanceof User
来源：http://egy.havefunace.top

TS:   u instanceof User
来源：http://oid.yj20258.top

Java: u instanceof User
来源：http://rwy.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hbz.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://njz.yonumen.top

C#:   u is User
来源：http://jfb.hammf.cn

[G14] 数据类 / record
来源：http://ugn.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kez.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://fze.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://xlz.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://gzx.mhx1999.top

Java: record User(String name, int age) {}
来源：http://wuk.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://lja.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://spm.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://cjv.shzxlz.cn

[G15] 枚举
来源：http://dwq.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eng.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://yzb.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fgy.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://piv.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://ffg.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tdy.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://vhd.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lxc.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://mzn.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qgs.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://fwi.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://ouc.yvedp.cn

TS:   Object.entries(obj)
来源：http://jjh.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tbw.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cib.iojbl.cn

Ruby: obj.instance_variables
来源：http://tjm.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://kxr.andypj.xyz

================================================================================
来源：http://xtz.xuetiantiany.cn

H. 异常与错误处理
来源：http://mqb.tanke756.top

================================================================================
来源：http://cxr.feifeiyinyue.top

[H01] try / catch 基础
来源：http://dbe.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xzl.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://btv.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ols.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wla.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cnd.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pwf.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gjc.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qxz.cheryme.top

[H02] finally / ensure 收尾
来源：http://dyw.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://yuq.redwolf501.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vzj.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hbo.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mkg.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gjx.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tzp.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://wdx.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rld.xuanzx.com

[H03] 主动抛出异常
来源：http://thp.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://gwz.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dqm.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://zxe.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://ipu.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wqq.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rer.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://zkz.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://bca.kuanghao11.cn

[H04] 自定义异常类型
来源：http://osy.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://trn.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://ooy.yueranfly.top

JS:   class MyError extends Error {}
来源：http://bem.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://fjy.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://pna.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dyu.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://wbj.havefunace.top

C#:   class MyException : Exception {}
来源：http://vgj.tanke756.top

[H05] 捕获特定类型
来源：http://gdn.yongpay.top

Py:   except ValueError as e:
来源：http://jsj.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://apm.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://lts.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://uwl.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://ypa.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zxh.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://nvz.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://upp.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://mti.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://vrb.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ifn.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://hnw.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://btt.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://afw.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://gqc.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://owx.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://cex.hfpthk.cn

[H07] 断言
来源：http://bew.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://qok.xinyue.icu

PHP:  assert($x > 0);
来源：http://xxd.iojbl.cn

JS:   console.assert(x > 0);
来源：http://ydy.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://hzl.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://dbo.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ihh.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jqs.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://sfv.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://won.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://iwd.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ltu.bjfxy.top

JS:   e.message;  e.stack
来源：http://xjn.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oke.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iae.snrcjt.cn

Go:   err.Error()
来源：http://hlw.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://eac.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://wtn.sweek.top

[H09] 带错误码的异常
来源：http://pbf.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vil.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://apf.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qhg.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qyw.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fnv.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dij.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://zgf.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://twl.gogol.net.cn

[H10] 资源自动释放
来源：http://fxc.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vsy.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xvj.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cnz.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bmq.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tbd.daria6918.cn

Go:   defer f.Close()
来源：http://bkd.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vda.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ffg.xylfe.cn

================================================================================
来源：http://nho.fehbvm.com

I. 正则表达式
来源：http://doh.dashuyun.cn

================================================================================
来源：http://nbx.tianlin.xyz

[I01] 判断是否匹配
来源：http://pis.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jwm.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://znc.shuidangran.top

JS:   /\d+/.test(s)
来源：http://tem.hammf.cn

TS:   /\d+/.test(s)
来源：http://sxg.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tij.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eho.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://fkk.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kro.nanxuanxn.top

[I02] 提取所有匹配
来源：http://kdr.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://ugn.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nju.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jcv.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://htz.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aco.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jah.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://sqw.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lfs.c1oappe.top

[I03] 提取捕获分组
来源：http://buq.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bpt.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kzn.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tcd.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cut.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://khr.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uwq.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bni.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://chi.yj20258888.top

[I04] 正则替换
来源：http://hiy.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vgc.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://thf.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uat.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pab.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qnl.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ijd.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rmj.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qwh.jqgfzy.top

[I05] 按正则拆分
来源：http://esp.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rut.xziqi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jwq.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://jiy.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://qvw.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://rmy.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jhw.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eyq.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bcf.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lvt.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rgw.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hes.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksc.daria6918.cn


<!-- 参考信息 -->